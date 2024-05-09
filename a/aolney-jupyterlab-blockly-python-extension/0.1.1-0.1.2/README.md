# Comparing `tmp/aolney_jupyterlab_blockly_python_extension-0.1.1.tar.gz` & `tmp/aolney_jupyterlab_blockly_python_extension-0.1.2.tar.gz`

## Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1.tar` & `aolney_jupyterlab_blockly_python_extension-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/babel.config.js
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/environment.yml
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/jest.config.js
--rw-r--r--   0        0        0   634891 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/package-lock.json
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/package.json
--rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/python-test.ipynb
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.test.json
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/watch.sh
--rw-r--r--   0        0        0   378847 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/yarn.lock
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/_version.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/package.json
--rw-r--r--   0        0        0    29983 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js.LICENSE.txt
--rw-r--r--   0        0        0    31898 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js.LICENSE.txt
--rw-r--r--   0        0        0    46479 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js.LICENSE.txt
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js
--rw-r--r--   0        0        0   666972 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js.LICENSE.txt
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.49e44ba8d7266e1def33.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/SearchDropdown.ts
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_minus.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_plus.ts
--rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/index.ts
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/logging.ts
--rw-r--r--   0        0        0    54321 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/toolbox.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/__tests__/aolney_jupyterlab_blockly_python_extension.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/package.json
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/LICENSE
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/README.md
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/.copier-answers.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/babel.config.js
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/environment.yml
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/jest.config.js
+-rw-r--r--   0        0        0   634891 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/package-lock.json
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/package.json
+-rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/python-test.ipynb
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/tsconfig.test.json
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/watch.sh
+-rw-r--r--   0        0        0   378847 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/yarn.lock
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/_version.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/package.json
+-rw-r--r--   0        0        0    29983 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js.LICENSE.txt
+-rw-r--r--   0        0        0    31898 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js.LICENSE.txt
+-rw-r--r--   0        0        0    46657 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/603.1ed66e959bf847ade7c1.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/603.1ed66e959bf847ade7c1.js.LICENSE.txt
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js
+-rw-r--r--   0        0        0   666972 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js.LICENSE.txt
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.bb156bd35e8fad0c52bf.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/SearchDropdown.ts
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/field_minus.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/field_plus.ts
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/index.ts
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/logging.ts
+-rw-r--r--   0        0        0    56985 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/toolbox.ts
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/src/__tests__/aolney_jupyterlab_blockly_python_extension.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/package.json
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/README.md
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    19029 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.2/PKG-INFO
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/.copier-answers.yml` & `aolney_jupyterlab_blockly_python_extension-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/RELEASE.md` & `aolney_jupyterlab_blockly_python_extension-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/jest.config.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/package-lock.json` & `aolney_jupyterlab_blockly_python_extension-0.1.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/package.json` & `aolney_jupyterlab_blockly_python_extension-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -189,9 +189,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/python-test.ipynb` & `aolney_jupyterlab_blockly_python_extension-0.1.2/python-test.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'cells'": "{0: {'execution_count': 4}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "id": "dd261eb5-bfe5-44f8-b337-18f4b3961061",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "\n",
                 "#<xml xmlns=\"https://developers.google.com/blockly/xml\"><variables><variable id=\"R*KYgfF%1g]kBJ!#(J5/\">pd</variable></variables><block type=\"importAs_Python\" id=\"zjFO8#zT,LpMBz=~;Is3\" x=\"16\" y=\"8\"><field name=\"libraryName\">pandas</field><field name=\"libraryAlias\" id=\"R*KYgfF%1g]kBJ!#(J5/\">pd</field></block></xml>"
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.json` & `aolney_jupyterlab_blockly_python_extension-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/yarn.lock` & `aolney_jupyterlab_blockly_python_extension-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/__init__.py` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/package.json` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.bb156bd35e8fad0c52bf.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -108,15 +108,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aolney/jupyterlab-blockly-python-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.49e44ba8d7266e1def33.js",
+            "load": "static/remoteEntry.bb156bd35e8fad0c52bf.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "aolney_jupyterlab_blockly_python_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -194,9 +194,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/603.1ed66e959bf847ade7c1.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,36 @@
-/*! For license information please see 603.4a974815d784d1ce9ced.js.LICENSE.txt */
+/*! For license information please see 603.1ed66e959bf847ade7c1.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_aolney_jupyterlab_blockly_python_extension = self.webpackChunk_aolney_jupyterlab_blockly_python_extension || []).push([
     [603], {
         603: (e, t, n) => {
             n.r(t), n.d(t, {
-                BlocklyWidget_$ctor_A44FDC6: () => K,
-                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => oe,
-                BlocklyWidget__RenderBlocks: () => ie,
-                BlocklyWidget__RenderCode: () => le,
-                BlocklyWidget__RenderCodeToLastCell: () => ae,
-                BlocklyWidget__clearBlocks: () => se,
-                BlocklyWidget__get_Notebooks: () => z,
-                BlocklyWidget__get_blocksRendered: () => J,
-                BlocklyWidget__get_lastCell: () => $,
-                BlocklyWidget__get_notHooked: () => q,
-                BlocklyWidget__get_onActiveCellChanged: () => ne,
-                BlocklyWidget__get_onKernelExecuted: () => te,
-                BlocklyWidget__get_workspace: () => Y,
-                BlocklyWidget__set_blocksRendered_Z1FBCCD16: () => Z,
-                BlocklyWidget__set_lastCell_Z4422E5A0: () => ee,
-                BlocklyWidget__set_notHooked_Z1FBCCD16: () => Q,
-                BlocklyWidget__set_workspace_Z1D3C0780: () => X,
-                attachWidget: () => re,
-                createMainAreaWidget: () => ce,
-                default: () => pe,
-                onKernelChanged: () => ue,
-                onNotebookChanged: () => de,
-                runCommandOnNotebookChanged: () => he
+                BlocklyWidget_$ctor_A44FDC6: () => Z,
+                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => le,
+                BlocklyWidget__RenderBlocks: () => ae,
+                BlocklyWidget__RenderCode: () => ie,
+                BlocklyWidget__RenderCodeToLastCell: () => se,
+                BlocklyWidget__clearBlocks: () => re,
+                BlocklyWidget__get_Notebooks: () => K,
+                BlocklyWidget__get_blocksRendered: () => q,
+                BlocklyWidget__get_lastCell: () => ee,
+                BlocklyWidget__get_notHooked: () => Q,
+                BlocklyWidget__get_onActiveCellChanged: () => oe,
+                BlocklyWidget__get_onKernelExecuted: () => ne,
+                BlocklyWidget__get_workspace: () => z,
+                BlocklyWidget__set_blocksRendered_Z1FBCCD16: () => J,
+                BlocklyWidget__set_lastCell_Z4422E5A0: () => te,
+                BlocklyWidget__set_notHooked_Z1FBCCD16: () => $,
+                BlocklyWidget__set_workspace_Z1D3C0780: () => Y,
+                attachWidget: () => ce,
+                createMainAreaWidget: () => ue,
+                default: () => me,
+                onKernelChanged: () => de,
+                onNotebookChanged: () => he,
+                runCommandOnNotebookChanged: () => pe
             });
             var o = n(626),
                 l = n(923),
                 i = n(206),
                 a = n(256),
                 s = n(291),
                 r = n(983),
@@ -197,15 +197,15 @@
                 r.Blocks[e] = {
                     init: function() {
                         this.appendDummyInput().appendField(t).appendField(new r.FieldTextInput("some library"), "libraryName").appendField(n).appendField(new r.FieldVariable("variable name"), "libraryAlias"), this.setNextStatement(!0), this.setPreviousStatement(!0), this.setColour(230), this.setTooltip("Import a python package to access functions in that package"), this.setHelpUrl("https://docs.python.org/3/reference/import.html")
                     }
                 }, c.pythonGenerator[e] = e => t + " " + e.getFieldValue("libraryName") + " " + n + " " + c.pythonGenerator.getVariableName(e.getFieldValue("libraryAlias")) + "\n"
             }
 
-            function w(e, t, n, o, l, i) {
+            function I(e, t, n, o, l, i) {
                 r.Blocks[e] = {
                     init: function() {
                         console.log(e + " init"), this.appendValueInput("x").setCheck(null).appendField(t), this.setInputsInline(!0), this.setOutput(!0, n), this.setColour(230), this.setTooltip(o), this.setHelpUrl(l)
                     }
                 }, c.pythonGenerator[e] = e => [i + "(" + c.pythonGenerator.valueToCode(e, "x", c.pythonGenerator.ORDER_MEMBER).replace("^\\[|\\]$", "") + ")", c.pythonGenerator.ORDER_FUNCTION_CALL]
             }
             c.pythonGenerator.finish = e => {
@@ -244,20 +244,20 @@
                 init: function() {
                     console.log("openWriteFile_Python init"), this.appendValueInput("FILENAME").setCheck("String").appendField("open file for writing"), this.setOutput(!0, null), this.setColour(230), this.setTooltip("Use this to write to a file. It will output a file, not a string."), this.setHelpUrl("https://docs.python.org/3/tutorial/inputoutput.html")
                 }
             }, c.pythonGenerator.openWriteFile_Python = e => ["open(" + c.pythonGenerator.valueToCode(e, "FILENAME", c.pythonGenerator.ORDER_ATOMIC) + ",'w',encoding='utf-8')", c.pythonGenerator.ORDER_FUNCTION_CALL], v("dummyOutputCodeBlock_Python", !1, !0), v("dummyNoOutputCodeBlock_Python", !1, !1), v("valueOutputCodeBlock_Python", !0, !0), v("valueNoOutputCodeBlock_Python", !0, !1), E("dummyOutputCommentBlock_Python", !1, !0), E("dummyNoOutputCommentBlock_Python", !1, !1), E("valueOutputCommentBlock_Python", !0, !0), E("valueNoOutputCommentBlock_Python", !0, !1), C("importAs_Python", "import", "as"), C("importFrom_Python", "from", "import"), r.Blocks.indexer_Python = {
                 init: function() {
                     this.appendValueInput("INDEX").appendField(new r.FieldVariable("{dictVariable}"), "VAR").appendField("["), this.appendDummyInput().appendField("]"), this.setInputsInline(!0), this.setOutput(!0), this.setColour(230), this.setTooltip("Gets an item from the variable at a given index. Not supported for all variables."), this.setHelpUrl("https://docs.python.org/3/reference/datamodel.html#object.__getitem__")
                 }
-            }, c.pythonGenerator.indexer_Python = e => [c.pythonGenerator.getVariableName(e.getFieldValue("VAR")) + "[" + c.pythonGenerator.valueToCode(e, "INDEX", c.pythonGenerator.ORDER_ATOMIC) + "]", c.pythonGenerator.ORDER_ATOMIC], w("reversedBlock_Python", "reversed", "None", "Create a reversed iterator to reverse a list or a tuple; wrap it in a new list or tuple.", "https://docs.python.org/3/library/functions.html#reversed", "reversed"), w("tupleConstructorBlock_Python", "tuple", "None", "Create a tuple from a list, e.g. ['a','b'] becomes ('a','b')", "https://docs.python.org/3/library/stdtypes.html#tuple", "tuple"), w("dictBlock_Python", "dict", "None", "Create a dictionary from a list of tuples, e.g. [('a',1),('b',2)...]", "https://docs.python.org/3/tutorial/datastructures.html#dictionaries", "dict"), w("listBlock_Python", "list", "None", "Create a list from an iterable, e.g. list(zip(...))", "https://docs.python.org/3/library/stdtypes.html#typesseq-list", "list"), w("zipBlock_Python", "zip", "Array", "Zip together two or more lists", "https://docs.python.org/3.3/library/functions.html#zip", "zip"), w("sortedBlock_Python", "as sorted", "Array", "Sort lists of stuff", "https://docs.python.org/3.3/library/functions.html#sorted", "sorted"), w("setBlock_Python", "set", "Array", "Make a set with unique members of a list.", "https://docs.python.org/2/library/sets.html", "set"), w("boolConversion_Python", "as bool", "Boolean", "Convert something to Boolean.", "https://docs.python.org/3/library/stdtypes.html#boolean-values", "bool"), w("strConversion_Python", "as str", "String", "Convert something to String.", "https://docs.python.org/3/library/stdtypes.html#str", "str"), w("floatConversion_Python", "as float", "Number", "Convert something to Float.", "https://docs.python.org/3/library/functions.html#float", "float"), w("intConversion_Python", "as int", "Number", "Convert something to Int.", "https://docs.python.org/3/library/functions.html#int", "int"), w("getInput_Python", "input", "String", "Present the given prompt to the user and wait for their typed input response.", "https://docs.python.org/3/library/functions.html#input", "input"), r.Blocks.tupleBlock_Python = {
+            }, c.pythonGenerator.indexer_Python = e => [c.pythonGenerator.getVariableName(e.getFieldValue("VAR")) + "[" + c.pythonGenerator.valueToCode(e, "INDEX", c.pythonGenerator.ORDER_ATOMIC) + "]", c.pythonGenerator.ORDER_ATOMIC], I("reversedBlock_Python", "reversed", "None", "Create a reversed iterator to reverse a list or a tuple; wrap it in a new list or tuple.", "https://docs.python.org/3/library/functions.html#reversed", "reversed"), I("tupleConstructorBlock_Python", "tuple", "None", "Create a tuple from a list, e.g. ['a','b'] becomes ('a','b')", "https://docs.python.org/3/library/stdtypes.html#tuple", "tuple"), I("dictBlock_Python", "dict", "None", "Create a dictionary from a list of tuples, e.g. [('a',1),('b',2)...]", "https://docs.python.org/3/tutorial/datastructures.html#dictionaries", "dict"), I("listBlock_Python", "list", "None", "Create a list from an iterable, e.g. list(zip(...))", "https://docs.python.org/3/library/stdtypes.html#typesseq-list", "list"), I("zipBlock_Python", "zip", "Array", "Zip together two or more lists", "https://docs.python.org/3.3/library/functions.html#zip", "zip"), I("sortedBlock_Python", "as sorted", "Array", "Sort lists of stuff", "https://docs.python.org/3.3/library/functions.html#sorted", "sorted"), I("setBlock_Python", "set", "Array", "Make a set with unique members of a list.", "https://docs.python.org/2/library/sets.html", "set"), I("boolConversion_Python", "as bool", "Boolean", "Convert something to Boolean.", "https://docs.python.org/3/library/stdtypes.html#boolean-values", "bool"), I("strConversion_Python", "as str", "String", "Convert something to String.", "https://docs.python.org/3/library/stdtypes.html#str", "str"), I("floatConversion_Python", "as float", "Number", "Convert something to Float.", "https://docs.python.org/3/library/functions.html#float", "float"), I("intConversion_Python", "as int", "Number", "Convert something to Int.", "https://docs.python.org/3/library/functions.html#int", "int"), I("getInput_Python", "input", "String", "Present the given prompt to the user and wait for their typed input response.", "https://docs.python.org/3/library/functions.html#input", "input"), r.Blocks.tupleBlock_Python = {
                 init: function() {
                     this.appendValueInput("FIRST").setCheck(null).appendField("("), this.appendValueInput("SECOND").setCheck(null).appendField(","), this.appendDummyInput().appendField(")"), this.setInputsInline(!0), this.setOutput(!0, null), this.setColour(230), this.setTooltip("Use this to create a two-element tuple"), this.setHelpUrl("https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences")
                 }
             }, c.pythonGenerator.tupleBlock_Python = e => ["(" + c.pythonGenerator.valueToCode(e, "FIRST", c.pythonGenerator.ORDER_ATOMIC) + "," + c.pythonGenerator.valueToCode(e, "SECOND", c.pythonGenerator.ORDER_ATOMIC) + ")", c.pythonGenerator.ORDER_NONE];
-            class I {
+            class w {
                 constructor(e, t, n, o) {
                     this.Name = e, this.Info = t, this.isFunction = n, this.isClass = o
                 }
             }
             class T {
                 constructor(e, t) {
                     this.VariableEntry = e, this.ChildEntries = t
@@ -320,25 +320,30 @@
                 return e.includes("Signature:") && e.includes("function")
             }
 
             function R(e) {
                 return e.includes("signature:") && e.includes("class")
             }
 
-            function A(e, t) {
+            function A(e) {
+                try {
+                    const t = new r.Events.BlockChange(e, "field", "VAR", 0, 1);
+                    t.group = "INTELLISENSE", console.log("event status is " + r.Events.disabled_), r.Events.disabled_ = 0, r.Events.fire(t)
+                } catch (e) {
+                    e instanceof Error && console.log("Intellisense event failed to fire; " + e.message)
+                }
+            }
+
+            function P(e, t) {
                 return "" === t || e.isInFlyout || function(e, t) {
                     N(t).then((n => {
-                        const o = new I(t, n, D(n), R(n));
-                        let l, i = new T(o, []);
-                        const a = [O.has(o.Name), i];
-                        if (a[0]) {
-                            const e = a[1];
-                            l = e.VariableEntry.Info !== o.Info || 0 === e.ChildEntries.length
-                        } else l = !0;
-                        l ? function(e) {
+                        const o = new w(t, n, D(n), R(n));
+                        let l = !0,
+                            i = O.get(o.Name);
+                        i && (l = i.VariableEntry.Info !== o.Info || i.ChildEntries.length <= 1), l ? function(e) {
                             const t = M();
                             if (null == t) return Promise.reject((() => {
                                 throw 1
                             })());
                             {
                                 const n = t[1];
                                 return new Promise(((t, o) => {
@@ -351,68 +356,70 @@
                                             "matches" in n && t(n.matches.slice())
                                         })).catch((t => {
                                             o([e + " is unavailable"])
                                         }))
                                     }), 100)
                                 }))
                             }
-                        }(t + ".").then((e => {
-                            const n = e.filter((e => 0 !== o.Info.indexOf("Signature: DataFrame") || !(0 === e.indexOf("_") || 0 === e.indexOf("style")))),
-                                l = n.map((e => N(t + "." + e)));
-                            return Promise.all(l).then((e => {
-                                const l = new T(o, n.map(((t, n) => new I(t, e[n], D(e[n]), R(e[n])))));
-                                O.has(t) ? O.set(t, l) : function(e, t, n) {
-                                    if (e.has(t)) throw new Error("An item with the same key has already been added. Key: " + t);
-                                    e.set(t, n)
-                                }(O, t, l)
+                        }(t + ".").then((n => {
+                            let l = n.filter((e => !o.Info.startsWith("Signature: DataFrame") || !e.startsWith("_") && !e.startsWith("style")));
+                            const i = l.map(((e, n) => N(t + "." + e)));
+                            Promise.allSettled(i).then((n => {
+                                let i = l.map(((e, t) => {
+                                        let o = "",
+                                            l = !0,
+                                            i = !1;
+                                        return "fulfilled" === n[t].status && (o = n[t].value, l = D(o), i = R(o)), new w(e, o, l, i)
+                                    })).sort(((e, t) => e.Name < t.Name ? -1 : 1)),
+                                    a = new T(o, i);
+                                O.set(t, a), A(e)
+                            })).catch((e => {
+                                console.log("Intellisense error getting inspections for children of " + t, e)
                             }))
-                        })).then((function() {
-                            const t = new r.Events.BlockChange(e, "field", "VAR", 0, 1);
-                            t.group = "INTELLISENSE", console.log("event status is " + r.Events.disabled_), r.Events.disabled_ = 0, r.Events.fire(t)
                         })).catch((e => {
-                            console.log("Intellisense event failed to fire; " + e.message)
-                        })) : console.log("Not refreshing intellisense for " + o.Name)
+                            console.log("Intellisense error getting child completions of " + t, e)
+                        })) : (console.log("Not refreshing intellisense for " + o.Name), A(e))
                     })).catch((e => {
-                        console.log("Intellisense event failed to fire; " + e.message)
+                        console.log("Intellisense error getting inspection of intellisense variable candidate (parent) " + t, e)
                     }))
                 }(e, t), e.isInFlyout ? [
                     [" ", " "]
                 ] : "" !== t && O.has(t) ? [
                     ["!Waiting for kernel to respond with options.", "!Waiting for kernel to respond with options."]
                 ] : [
                     ["!Not defined until you execute code.", "!Not defined until you execute code."]
                 ]
             }
 
-            function P(e, t) {
+            function B(e, t) {
                 var n;
                 const o = (i = e, null, (l = O).has(i) ? [!0, l.get(i)] : [!1, null]);
                 var l, i;
                 if (o[0]) {
                     const e = null === (n = o[1]) || void 0 === n ? void 0 : n.ChildEntries.find((e => e.Name === t));
                     return null == e ? "!Not defined until you execute code." : e.Info
                 }
                 return "!Not defined until you execute code."
             }
 
-            function B() {
+            function F() {
                 const e = r.getMainWorkspace(),
                     t = e.getBlocksByType("varGetProperty_Python", !1);
                 e.getBlocksByType("varDoMethod_Python", !1).forEach((e => t.push(e))), t.forEach((e => {
-                    e.updateIntellisense(e, null, (t => A(e, t)))
+                    e.updateIntellisense(e, null, (t => P(e, t)))
                 })), e.registerToolboxCategoryCallback("VARIABLE", r.Variables.flyoutCategoryBlocks)
             }
 
-            function F(e, t, n) {
+            function S(e, t, n) {
                 const o = e.getField(t),
                     l = e.getInput(n);
                 o && (l ? l.removeField(t) : console.log("error removing (" + t + ") from block; input (" + n + ") does not exist"))
             }
 
-            function S(e, t, n, o, l, i) {
+            function U(e, t, n, o, l, i) {
                 r.Blocks[e] = {
                     varSelectionUserName(e, t) {
                         const n = e.getField("VAR"),
                             o = e.workspace.getAllVariables().slice(-1)[0],
                             l = e.data,
                             i = l && l.indexOf(":") >= 0 ? l.split(":") : [""];
                         if (null == t) {
@@ -424,33 +431,33 @@
                             const e = n.getOptions().find((e => e[1] === t));
                             return e && "string" == typeof e[0] ? e[0] : ""
                         }
                     },
                     selectedMember: "",
                     updateIntellisense(e, t, n) {
                         const o = e.getInput("INPUT");
-                        F(e, "MEMBER", "INPUT"), F(e, "USING", "INPUT");
+                        S(e, "MEMBER", "INPUT"), S(e, "USING", "INPUT");
                         const l = e.varSelectionUserName(e, t),
                             i = n(l).map((e => e[0])),
                             a = e.data ? e.data : "",
                             s = a.indexOf(":") >= 0 ? a.split(":")[1] : "";
                         if (o) {
                             let t = new g.FieldFilter(s, i, (function(t) {
                                 const n = "" === t ? s : this.WORDS[t];
                                 let o;
-                                return this.setTooltip(P(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = l + ":" + e.selectedMember), n
+                                return this.setTooltip(B(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = l + ":" + e.selectedMember), n
                             }));
                             o.appendField(t, "MEMBER")
                         }
                         void 0 !== e.data && null !== e.data || (e.data = l + ":" + e.selectedMember);
                         const r = e.getField("MEMBER");
-                        r && r.setTooltip(P(l, r.getText()))
+                        r && r.setTooltip(B(l, r.getText()))
                     },
                     init: function() {
-                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new r.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => A(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => A(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), r.Extensions.apply("intelliblockMutator_Python", this, !0))
+                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new r.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => P(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => P(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), r.Extensions.apply("intelliblockMutator_Python", this, !0))
                     },
                     onchange: function(e) {
                         if (this.workspace && !this.isInFlyout && "INTELLISENSE" === e.group) {
                             const e = this.data ? this.data.toString().split(":") : "";
                             this.updateIntellisense(this, null, (e => function(e, t) {
                                 const n = O.get(t);
                                 return n ? !n.VariableEntry.isFunction && n.ChildEntries.length > 0 ? n.ChildEntries.filter(e).map((e => [e.Name, e.Name])) : "UNDEFINED" === n.VariableEntry.Info ? [
@@ -516,28 +523,28 @@
                         const e = this.getField("MINUS");
                         !e && this.itemCount_ > 0 ? this.topInput_.insertFieldAt(1, new r.FieldImage("data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEuMSIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48cGF0aCBkPSJNMTggMTFoLTEyYy0xLjEwNCAwLTIgLjg5Ni0yIDJzLjg5NiAyIDIgMmgxMmMxLjEwNCAwIDItLjg5NiAyLTJzLS44OTYtMi0yLTJ6IiBmaWxsPSJ3aGl0ZSIgLz48L3N2Zz4K", 15, 15, void 0, d), "MINUS") : e && this.itemCount_ < 1 && this.topInput_.removeField("MINUS")
                     }
                 };
                 r.Extensions.registerMutator("intelliblockMutator_Python", i, (function() {
                     return this.getInput("EMPTY").insertFieldAt(0, h(), "PLUS"), this.updateShape_(1)
                 }))
-            }(), S("varGetProperty_Python", "from", "get", (e => !e.isFunction), !1, !0), S("varDoMethod_Python", "with", "do", (e => e.isFunction), !0, !0), S("varCreateObject_Python", "with", "create", (e => e.isClass), !0, !0);
-            const U = [];
+            }(), U("varGetProperty_Python", "from", "get", (e => !e.isFunction), !1, !0), U("varDoMethod_Python", "with", "do", (e => e.isFunction), !0, !0), U("varCreateObject_Python", "with", "create", (e => e.isClass), !0, !0);
+            const L = [];
             r.Variables.flyoutCategoryBlocks = e => {
-                if (U) {
+                if (L) {
                     const t = M();
                     if (t) {
                         const n = t[1],
-                            o = U.find((e => e.KernelCheckFunction(n.name)));
+                            o = L.find((e => e.KernelCheckFunction(n.name)));
                         return o ? o.FlyoutFunction(e) : []
                     }
                     return []
                 }
                 return []
-            }, U.push(new class {
+            }, L.push(new class {
                 constructor(e, t, n) {
                     this.LanguageName = e, this.KernelCheckFunction = t, this.FlyoutFunction = n
                 }
             }("Python", (e => e.toLocaleLowerCase().indexOf("python") >= 0), (function(e) {
                 const t = e.getVariablesOfType(""),
                     n = [],
                     o = document.createElement("button");
@@ -574,226 +581,226 @@
                                 l = r.utils.xml.createElement("block");
                             l.setAttribute("type", "variables_get"), l.setAttribute("gap", "8"), l.appendChild(r.Variables.generateVariableFieldDom(o)), n.push(l), e++
                         }
                     }
                 }
                 return n
             }))), n(499);
-            var L = n(808);
+            var V = n(808);
 
-            function V(e, t) {
+            function W(e, t) {
                 return {
                     schema: "jle050824",
                     name: e,
                     payload: t
                 }
             }
-            let G, W;
+            let G, j;
 
-            function j(e) {
+            function H(e) {
                 if (G) {
                     let l = window.location.href;
-                    W && (l = W), window.fetch(G, {
+                    j && (l = j), window.fetch(G, {
                         method: "POST",
                         headers: {
                             "Content-Type": "application/json"
                         },
                         body: JSON.stringify({
                             username: l,
-                            json: (t = e, 0 === (null === (o = null === (n = null == t ? void 0 : t.object) || void 0 === n ? void 0 : n.element) || void 0 === o ? void 0 : o.toString().indexOf("drag")) && (t.object.newValue = void 0, t.object.oldValue = void 0), t)
+                            json: btoa((t = e, 0 === (null === (o = null === (n = null == t ? void 0 : t.object) || void 0 === n ? void 0 : n.element) || void 0 === o ? void 0 : o.toString().indexOf("drag")) && (t.object.newValue = void 0, t.object.oldValue = void 0), t))
                         })
                     }).then((e => {
                         e.ok || console.log(e.statusText)
                     }))
                 }
                 var t, n, o
             }
-            r.setLocale(L);
-            class H extends a.Widget {
+            r.setLocale(V);
+            class X extends a.Widget {
                 constructor(e) {
                     super(), this.onResize = e => {
                             let t = e.width,
                                 n = e.width;
                             const o = document.getElementById("blocklyDivPython"),
                                 l = document.getElementById("buttonDivPython"),
                                 i = e.height - 30;
-                            o.setAttribute("style", "width: " + (t = e.width, t.toString() + "px; height: ") + i.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + i.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), r.svgResize(Y(this))
-                        }, this.notebooks = e, this.generator = c.pythonGenerator, this.notebooks.activeCellChanged.connect(ne(this), this),
+                            o.setAttribute("style", "width: " + (t = e.width, t.toString() + "px; height: ") + i.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + i.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), r.svgResize(z(this))
+                        }, this.notebooks = e, this.generator = c.pythonGenerator, this.notebooks.activeCellChanged.connect(oe(this), this),
                         function(e) {
                             x = e
                         }(this.notebooks), this.div = document.createElement("div"), this.div.id = "blocklyDivPython", this.node.appendChild(this.div);
                     const t = document.createElement("div");
                     t.id = "buttonDivPython";
                     const n = document.createElement("button");
                     n.innerText = "Blocks to Code", t.appendChild(n), n.addEventListener("click", (e => {
-                        le(this)
+                        ie(this)
                     }));
                     const o = document.createElement("button");
                     o.innerText = "Code to Blocks", o.addEventListener("click", (e => {
-                        ie(this)
+                        ae(this)
                     })), t.appendChild(o);
                     const l = document.createElement("button");
                     l.innerText = "Report Bug", l.addEventListener("click", (e => {
                         const t = window.open("https://github.com/aolney/jupyterlab-blockly-python-extension/issues", "_blank");
                         t && t.focus()
                     })), t.appendChild(l);
                     const i = document.createElement("input");
                     i.setAttribute("type", "checkbox"), i.checked = !0, i.id = "syncCheckboxPython";
                     const a = document.createElement("label");
                     a.innerText = "Notebook Sync", a.setAttribute("for", "syncCheckboxPython"), t.appendChild(i), t.appendChild(a), this.node.appendChild(t), this["blocksRendered@"] = !1, this["notHooked@"] = !0, this["init@34"] = 1
                 }
                 onAfterAttach() {
                     const e = this;
-                    X(e, r.inject("blocklyDivPython", {
+                    Y(e, r.inject("blocklyDivPython", {
                         toolbox: '<xml xmlns="https://developers.google.com/blockly/xml" id="toolbox" style="display: none">\n    <category name="IMPORT" colour="255">\n      <block type="importAs_Python"></block>\n      <block type="importFrom_Python"></block>\n    </category>\n    <category name="FREESTYLE" colour="290">\n      <block type="dummyOutputCodeBlock_Python"></block>\n      <block type="dummyNoOutputCodeBlock_Python"></block>\n      <block type="valueOutputCodeBlock_Python"></block>\n      <block type="valueNoOutputCodeBlock_Python"></block>\n    </category>\n    <category name="COMMENT" colour="%{BKY_COLOUR_HUE}">\n      <block type="dummyOutputCommentBlock_Python"></block>\n      <block type="dummyNoOutputCommentBlock_Python"></block>\n      <block type="valueOutputCommentBlock_Python"></block>\n      <block type="valueNoOutputCommentBlock_Python"></block>\n    </category>\n    <category name="LOGIC" colour="%{BKY_LOGIC_HUE}">\n      <block type="controls_if"></block>\n      <block type="logic_compare"></block>\n      <block type="logic_operation"></block>\n      <block type="logic_negate"></block>\n      <block type="logic_boolean"></block>\n      <block type="logic_null"></block>\n      <block type="logic_ternary"></block>\n    </category>\n    <category name="LOOPS" colour="%{BKY_LOOPS_HUE}">\n      <block type="controls_repeat_ext">\n        <value name="TIMES">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="controls_whileUntil"></block>\n      <block type="controls_for">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n        <value name="BY">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="comprehensionForEach_Python"></block>\n      <block type="controls_forEach"></block>\n      <block type="controls_flow_statements"></block>\n    </category>\n    <category name="MATH" colour="%{BKY_MATH_HUE}">\n      <block type="math_number">\n        <field name="NUM">123</field>\n      </block>\n      <block type="math_arithmetic">\n        <value name="A">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="B">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_single">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">9</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_trig">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">45</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constant"></block>\n      <block type="math_number_property">\n        <value name="NUMBER_TO_CHECK">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_round">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">3.1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_on_list"></block>\n      <block type="math_modulo">\n        <value name="DIVIDEND">\n          <shadow type="math_number">\n            <field name="NUM">64</field>\n          </shadow>\n        </value>\n        <value name="DIVISOR">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constrain">\n        <value name="VALUE">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="LOW">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="HIGH">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_int">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_float"></block>\n      <block type="math_atan2">\n        <value name="X">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="Y">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <category name="TEXT" colour="%{BKY_TEXTS_HUE}">\n      <block type="text"></block>\n      <block type="text_join"></block>\n      <block type="text_append">\n        <value name="TEXT">\n          <shadow type="text"></shadow>\n        </value>\n      </block>\n      <block type="text_length">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_isEmpty">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT"></field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n        <value name="FIND">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_charAt">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_getSubstring">\n        <value name="STRING">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_changeCase">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_trim">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_print">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_prompt_ext">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      \x3c!-- <block type="getInput">\n        <value name="x">\n          <shadow type="text">\n            <field name="TEXT">The prompt shown to the user</field>\n          </shadow>\n        </value>\n      </block> --\x3e\n    </category>\n    <category name="LISTS" colour="%{BKY_LISTS_HUE}">\n      <block type="lists_create_with">\n        <mutation items="0"></mutation>\n      </block>\n      <block type="lists_create_with"></block>\n      <block type="lists_repeat">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">5</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_length"></block>\n      <block type="lists_isEmpty"></block>\n      <block type="lists_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getIndex">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_setIndex">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getSublist">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="indexer_Python"></block>\n      <block type="lists_split">\n        <value name="DELIM">\n          <shadow type="text">\n            <field name="TEXT">,</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_sort"></block>\n      <block type="setBlock_Python"></block>\n      <block type="sortedBlock_Python"></block>\n      <block type="zipBlock_Python"></block>\n      <block type="dictBlock_Python"></block>\n      <block type="listBlock_Python"></block>\n      <block type="tupleBlock_Python"></block>\n      <block type="tupleConstructorBlock_Python"></block>\n      <block type="reversedBlock_Python"></block>\n    </category>\n    <category name="COLOUR" colour="%{BKY_COLOUR_HUE}">\n      <block type="colour_picker"></block>\n      <block type="colour_random"></block>\n      <block type="colour_rgb">\n        <value name="RED">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n        <value name="GREEN">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="BLUE">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="colour_blend">\n        <value name="COLOUR1">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#ff0000</field>\n          </shadow>\n        </value>\n        <value name="COLOUR2">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#3333ff</field>\n          </shadow>\n        </value>\n        <value name="RATIO">\n          <shadow type="math_number">\n            <field name="NUM">0.5</field>\n          </shadow>\n        </value>\n      </block>Conversion\n    </category>\n    <category name="CONVERSION" colour="120">\n      <block type="boolConversion_Python">\n      </block>\n      <block type="intConversion_Python">\n      </block>\n      <block type="floatConversion_Python">\n      </block>\n      <block type="strConversion_Python">\n      </block>\n    </category>\n    <category name="I/O" colour="190">\n      <block type="withAs_Python">\n      </block>\n      <block type="textFromFile_Python">\n        <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="openReadFile_Python">\n              <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="openWriteFile_Python">\n              <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <sep></sep>\n    <category name="VARIABLES" colour="%{BKY_VARIABLES_HUE}" custom="VARIABLE"></category>\n    <category name="FUNCTIONS" colour="%{BKY_PROCEDURES_HUE}" custom="PROCEDURE"></category>\n  </xml>'
                     })), console.log("jupyterlab_blockly_extension_python: blockly palette initialized");
                     const t = t => {
-                        "create" === t.type && Z(e, !1), "finished_loading" === t.type && Z(e, !0), j({
+                        "create" === t.type && J(e, !1), "finished_loading" === t.type && J(e, !0), H({
                             schema: "ble050824",
                             name: t.type,
                             object: t.toJson()
                         })
                     };
-                    Y(e).removeChangeListener(t), Y(e).addChangeListener(t)
+                    z(e).removeChangeListener(t), z(e).addChangeListener(t)
                 }
             }
 
-            function X(e, t) {
+            function Y(e, t) {
                 e["workspace@"] = t
             }
 
-            function Y(e) {
+            function z(e) {
                 return e["workspace@"]
             }
 
-            function z(e) {
+            function K(e) {
                 return e.notebooks
             }
 
-            function K(e) {
-                return new H(e)
+            function Z(e) {
+                return new X(e)
             }
 
-            function Z(e, t) {
+            function J(e, t) {
                 e["blocksRendered@"] = t
             }
 
-            function J(e) {
+            function q(e) {
                 return e["blocksRendered@"]
             }
 
-            function q(e) {
+            function Q(e) {
                 return e["notHooked@"]
             }
 
-            function Q(e, t) {
+            function $(e, t) {
                 e["notHooked@"] = t
             }
 
-            function $(e) {
+            function ee(e) {
                 return e["lastCell@"]
             }
 
-            function ee(e, t) {
+            function te(e, t) {
                 e["lastCell@"] = t
             }
 
-            function te(e) {
+            function ne(e) {
                 return (e, t) => {
                     if (e.name.indexOf("python") >= 0) switch (t.header.msg_type.toString()) {
                         case "execute_input":
-                            console.log("jupyterlab_blockly_extension_python: kernel executed code, updating intellisense"), j(V("execute-code", t.content)), B();
+                            console.log("jupyterlab_blockly_extension_python: kernel executed code, updating intellisense"), H(W("execute-code", t.content)), F();
                             break;
                         case "error":
-                            j(V("execute-code-error", t.content))
+                            H(W("execute-code-error", t.content))
                     }
                     return !0
                 }
             }
 
-            function ne(e) {
+            function oe(e) {
                 return (t, n) => {
                     if (n) {
-                        j(V("active-cell-change", {
+                        H(W("active-cell-change", {
                             cell_text: n.node.outerText
                         }));
                         const t = document.getElementById("syncCheckboxPython"),
                             o = document.getElementById("autosaveCheckboxPython"),
                             l = e => !!e && e.checked;
-                        l(t) && e.notebooks.activeCell && (J(e) && null == oe(e) ? se() : ie(e), B()), l(o) && e.notebooks.activeCell && (ae(e), ee(e, n))
+                        l(t) && e.notebooks.activeCell && (q(e) && null == le(e) ? re() : ae(e), F()), l(o) && e.notebooks.activeCell && (se(e), te(e, n))
                     }
                     return !0
                 }
             }
 
-            function oe(e) {
+            function le(e) {
                 if (e.notebooks.activeCell) {
                     const t = e.notebooks.activeCell.model.sharedModel.getSource();
                     if (!(t.indexOf("xmlns") >= 0)) return null;
                     {
                         const e = /(<xml[\s\S]+<\/xml>)/;
                         let n = t.match(e);
                         if (n && n[0]) return n[0]
                     }
                 }
                 return null
             }
 
-            function le(e) {
+            function ie(e) {
                 let t;
-                const n = e.generator.workspaceToCode(Y(e));
-                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, i.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), j(V("blocks-to-code", {
+                const n = e.generator.workspaceToCode(z(e));
+                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, i.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), H(W("blocks-to-code", {
                     code: e.notebooks.activeCell.model.toJSON().source.toString()
-                })), Z(e, !0))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed\n" + n + "\n")
+                })), J(e, !0))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed\n" + n + "\n")
             }
 
-            function ie(e) {
+            function ae(e) {
                 if (e.notebooks.activeCell) {
                     const t = /(<xml[\s\S]+<\/xml>)/;
                     let n = e.notebooks.activeCell.model.sharedModel.getSource().match(t);
                     try {
                         if (n && n[1]) {
                             const e = n[1];
-                            se(),
+                            re(),
                                 function(e) {
                                     const t = (new DOMParser).parseFromString(e, "application/xml").documentElement;
                                     r.Xml.domToWorkspace(t, r.getMainWorkspace())
-                                }(e), j(V("xml-to-blocks", {
+                                }(e), H(W("xml-to-blocks", {
                                     xml: e
                                 }))
                         }
                     } catch (e) {
                         window.alert("Unable to perform 'Code to Blocks': XML is either invald or renames existing variables. Specific error message is: " + e.message), console.log("jupyterlab_blockly_extension_python: unable to decode blocks, last line is invald xml")
                     }
                 } else console.log("jupyterlab_blockly_extension_python: unable to decode blocks, active cell is null")
             }
 
-            function ae(e) {
+            function se(e) {
                 let t;
-                const n = e.generator.workspaceToCode(Y(e));
-                $(e) ? $(e).model && (t = $(e).model, i.isCodeCellModel(t) && (() => {
+                const n = e.generator.workspaceToCode(z(e));
+                ee(e) ? ee(e).model && (t = ee(e).model, i.isCodeCellModel(t) && (() => {
                     try {
-                        const t = $(e).model.sharedModel.getSource();
+                        const t = ee(e).model.sharedModel.getSource();
                         if (t.indexOf("xmlns") >= 0) {
                             const e = /(<xml[\s\S]+<\/xml>)/;
                             let n = t.match(e);
                             if (n && n[0]) return n[0]
                         }
                     } catch (e) {
                         return !1
                     }
-                })()) && Y(e).getAllBlocks(!1).length > 0 && ($(e).model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), e.notebooks.activeCell && j(V("blocks-to-code-autosave", e.notebooks.activeCell.model.toJSON()))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed instead of autosave\n" + n + "\n")
+                })()) && z(e).getAllBlocks(!1).length > 0 && (ee(e).model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), e.notebooks.activeCell && H(W("blocks-to-code-autosave", e.notebooks.activeCell.model.toJSON()))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed instead of autosave\n" + n + "\n")
             }
 
-            function se(e) {
+            function re(e) {
                 const t = r.getMainWorkspace().getAllBlocks(!1);
                 for (let e = 0; e < t.length; e++) t[e].dispose(!1)
             }
 
-            function re(e, t, n) {
+            function ce(e, t, n) {
                 if (!n.isAttached) {
                     const o = t.currentWidget;
                     if (null == o) e.shell.add(n, "main");
                     else {
                         const e = o,
                             t = {
                                 ref: e.id,
@@ -801,83 +808,83 @@
                             };
                         e.context.addSibling(n, t)
                     }
                 }
                 e.shell.activateById(n.id)
             }
 
-            function ce(e) {
+            function ue(e) {
                 const t = new l.MainAreaWidget({
                     content: e
                 });
                 return t.id = "blockly-jupyterlab-python", t.title.label = "Blockly Python", t.title.closable = !0, t
             }
 
-            function ue(e, t) {
+            function de(e, t) {
                 var n;
                 const o = this;
-                if (q(o)) {
+                if (Q(o)) {
                     const t = null === (n = e.session) || void 0 === n ? void 0 : n.kernel;
                     if (null == t || null == t);
                     else {
                         const e = t;
-                        e.name.indexOf("python") >= 0 && (e.iopubMessage.connect(te(), o), console.log("jupyterlab_blockly_extension_python: Listening for kernel messages"), Q(o, !1))
+                        e.name.indexOf("python") >= 0 && (e.iopubMessage.connect(ne(), o), console.log("jupyterlab_blockly_extension_python: Listening for kernel messages"), $(o, !1))
                     }
                     return !0
                 }
                 return !1
             }
 
-            function de(e, t) {
+            function he(e, t) {
                 const n = this,
                     o = e.currentWidget;
                 if (null == o);
                 else {
                     const e = o;
-                    console.log("jupyterlab_blockly_extension_python: notebook changed to " + e.context.path), j(V("notebook-changed", {
+                    console.log("jupyterlab_blockly_extension_python: notebook changed to " + e.context.path), H(W("notebook-changed", {
                         path: e.context.path
-                    })), e.sessionContext.kernelChanged.connect(ue, n)
+                    })), e.sessionContext.kernelChanged.connect(de, n)
                 }
                 return !0
             }
 
-            function he(e, t) {
+            function pe(e, t) {
                 return null == e.currentWidget || (console.log("jupyterlab_blockly_extension_python: notebook changed, autorunning blockly python command"), this.commands.execute("blockly_python:open")), !0
             }
-            const pe = {
+            const me = {
                 id: "jupyterlab-apod",
                 description: "blockly python extension for jupyter lab.",
                 autoStart: !0,
                 requires: [l.ICommandPalette, s.INotebookTracker, o.ILayoutRestorer],
                 activate: async function(e, t, n, o, i) {
                     console.log("jupyterlab_blockly_extension_python: extension is activated!");
-                    const a = K(n);
-                    let s = ce(a);
+                    const a = Z(n);
+                    let s = ue(a);
                     const r = new l.WidgetTracker({
                         namespace: "blockly_python"
                     });
                     o && o.restore(r, {
                         command: "blockly_python:open",
                         name: () => "blockly_python"
-                    }), n.currentChanged.connect(de, a), e.commands.addCommand("blockly_python:open", {
+                    }), n.currentChanged.connect(he, a), e.commands.addCommand("blockly_python:open", {
                         label: "Blockly Python",
                         execute: () => {
-                            s && !s.isDisposed || (s = ce(a)), re(e, n, s), r.has(s) || r.add(s)
+                            s && !s.isDisposed || (s = ue(a)), ce(e, n, s), r.has(s) || r.add(s)
                         }
                     }), t.addItem({
                         command: "blockly_python:open",
                         category: "Blockly"
                     });
                     const c = new URLSearchParams(window.location.search);
                     "py" === c.get("bl") && (console.log("jupyterlab_blockly_extension_python: openning blockly, bl=py"), e.restored.then((() => {
-                        n.currentChanged.connect(he, e), s.title.closable = !1
+                        n.currentChanged.connect(pe, e), s.title.closable = !1
                     })));
                     let u = c.get("id");
                     u && (function(e) {
-                        W = e
+                        j = e
                     }(u), console.log("jupyterlab_blockly_extension_py: using id=" + u + " for logging"));
                     let d = c.get("log");
                     d && (G = d, console.log("jupyterlab_blockly_extension_py: using log=" + d + " for logging"))
                 }
             }
         }
     }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.49e44ba8d7266e1def33.js` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.bb156bd35e8fad0c52bf.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, f, d, p, c, h, b, v, y, m, g, w, j, k, S, x = {
+    var e, r, t, n, o, a, i, l, u, s, f, d, c, p, h, v, b, y, m, g, w, j, k, S, x = {
             459: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(88), t.e(203), t.e(603)]).then((() => () => t(603))),
                         "./extension": () => Promise.all([t.e(88), t.e(203), t.e(603)]).then((() => () => t(603))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -46,21 +46,21 @@
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         88: "f12ddff976fd53bc3a6c",
         203: "1521356dd3eabef73aae",
         369: "5f4ab4479184dd6b56b7",
-        603: "4a974815d784d1ce9ced",
+        603: "1ed66e959bf847ade7c1",
         728: "ea6e1ffef3f6bcb3b003"
     } [e] + ".js?v=" + {
         88: "f12ddff976fd53bc3a6c",
         203: "1521356dd3eabef73aae",
         369: "5f4ab4479184dd6b56b7",
-        603: "4a974815d784d1ce9ced",
+        603: "1ed66e959bf847ade7c1",
         728: "ea6e1ffef3f6bcb3b003"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -75,19 +75,19 @@
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@aolney/jupyterlab-blockly-python-extension", "0.1.1", (() => Promise.all([P.e(88), P.e(203), P.e(603)]).then((() => () => P(603))))), l("blockly", "10.4.3", (() => Promise.all([P.e(88), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@aolney/jupyterlab-blockly-python-extension", "0.1.2", (() => Promise.all([P.e(88), P.e(203), P.e(603)]).then((() => () => P(603))))), l("blockly", "10.4.3", (() => Promise.all([P.e(88), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -192,50 +192,50 @@
                     u = !1, l--
                 } else {
                     if (l <= n || f < d != o) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || c(s(e, t, o, n)), b(e[t][o])
+        return a(n, o) || p(s(e, t, o, n)), v(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, p = (e, r, t, n) => {
+    }, c = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, c = e => {
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
-        c(p(e, r, t, n))
-    }, b = e => (e.loaded = 1, e.get()), y = (v = e => function(r, t, n, o) {
+        p(c(e, r, t, n))
+    }, v = e => (e.loaded = 1, e.get()), y = (b = e => function(r, t, n, o) {
         var a = P.I(r);
         return a && a.then ? a.then(e.bind(e, r, P.S[r], t, n, o)) : e(r, P.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), b(d(r, t, n) || h(r, e, t, n) || l(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = v(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || h(r, e, t, n) || l(r, t))))), m = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
         var a = r && P.o(r, t) && d(r, t, n);
-        return a ? b(a) : o()
+        return a ? v(a) : o()
     })), w = {}, j = {
         206: () => y("default", "@jupyterlab/cells", [1, 4, 2, 0]),
         236: () => m("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
         256: () => m("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         291: () => m("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
         569: () => g("default", "blockly", [1, 10, 4, 3], (() => P.e(369).then((() => () => P(369))))),
         626: () => m("default", "@jupyterlab/application", [1, 4, 2, 0]),
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json` & `aolney_jupyterlab_blockly_python_extension-0.1.2/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/SearchDropdown.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/SearchDropdown.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_minus.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/field_minus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_plus.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/field_plus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/index.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/logging.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/logging.ts`

 * *Files 26% similar despite different names*

```diff
@@ -13,30 +13,22 @@
     schema: string;
     name: string;
     // payload?: string | null;
     payload: object;
   }
   
   export function createBlocklyLogEntry(name: string, object: any): BlocklyLogEntry050824 {
-    // let encoded_object = btoa(object);
-    // // DEBUG
-    // encoded_object = (object);
     return {
       schema: "ble050824",
       name: name,
       object: object
     };
   }
   
   export function createJupyterLogEntry(name: string, payload: object): JupyterLogEntry050824 {
-    // let encoded_payload = "";
-    // if( payload ) { 
-    //   // DEBUG
-    //   encoded_payload = payload; //btoa(payload); 
-    // }
     return {
       schema: "jle050824",
       name: name,
       payload: payload
     };
   }
   
@@ -65,16 +57,16 @@
       window.fetch(logUrl, {
         method: "POST",
         headers: {
           "Content-Type": "application/json",
         },
         body: JSON.stringify({
           username:id,
-          //TODO btoa(json)
-          json:filterJson(logObject) 
+          //base64 encode the payload because it can have all kinds of craziness inside it
+          json:btoa(filterJson(logObject))
           
         })
       }).then(response => {
         if (!response.ok) {
           console.log(response.statusText);
         }
       })
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/src/toolbox.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/src/toolbox.ts`

 * *Files 5% similar despite different names*

```diff
@@ -508,84 +508,139 @@
 export function addToDict(dict: any, k: any, v: any) {
   if (dict.has(k)) {
     throw new Error("An item with the same key has already been added. Key: " + k);
   }
   dict.set(k, v);
 }
 
+
+/**
+ * Fire intellisense event that causes Blockly to refresh intellisense-driven options
+ * Typically called by RequestIntellisenseVariable 
+ * @param block 
+ */
+export function fireIntellisenseEvent(block: Blockly.Block) {
+  try {
+  // Create event on this block
+  const intellisenseUpdateEvent = new Blockly.Events.BlockChange(block, "field", "VAR", 0, 1);
+  // Set the event group; this allows event listners to focus on only relevant messages
+  intellisenseUpdateEvent.group = "INTELLISENSE";
+  // Do some state tracking; this helps with debugging events
+  // @ts-ignore
+  console.log("event status is " + Blockly.Events.disabled_); //disabled_ existed in old version but not new version?
+  // @ts-ignore
+  Blockly.Events.disabled_ = 0;
+  Blockly.Events.fire(intellisenseUpdateEvent);
+  } 
+  catch(e){
+    if (e instanceof Error) {
+      console.log("Intellisense event failed to fire; " + e.message);
+    }
+  }
+}
+
+/**
+ * Wrap a promise inside another with a timeout in milliseconds
+ * https://github.com/JakeChampion/fetch/issues/175#issuecomment-216791333
+ * @param ms 
+ * @param promise 
+ * @returns 
+ */
+export function timeoutPromise<T>(ms: number, promise: Promise<T>) {
+  return new Promise<T>((resolve, reject) => {
+    const timeoutId = setTimeout(() => {
+      reject(new Error("promise timeout"))
+    }, ms);
+    promise.then(
+      (res) => {
+        clearTimeout(timeoutId);
+        resolve(res);
+      },
+      (err) => {
+        clearTimeout(timeoutId);
+        reject(err);
+      }
+    );
+  })
+}
+
 /**
  * Request an IntellisenseVariable. If the type does not descend from object, the children will be empty.
  * Sometimes we will create a variable but it will have no type until we make an assignment.
  * We might also create a variable and then change its type.
  * So we need to check for introspections/completions repeatedly (no caching right now).
  */
-
-
 export function RequestIntellisenseVariable_Python(block: Blockly.Block, parentName: string): void {
   GetKernalInspection(parentName).then((parentInspection: string) => {
     const parent: IntellisenseEntry = new IntellisenseEntry(parentName, parentInspection, isFunction_Python(parentInspection), isClass_Python(parentInspection));
-    let shouldGetChildren: boolean;
-    let outArg: IntellisenseVariable = new IntellisenseVariable(parent, []);
-    
-    const matchValue: [boolean, IntellisenseVariable] = [
-      intellisenseLookup.has(parent.Name),
-      outArg
-    ];
-    if (matchValue[0]) {
-      const cached: IntellisenseVariable = matchValue[1];
-      if (cached.VariableEntry.Info !== parent.Info || cached.ChildEntries.length === 0) {
+    // Assume we need to get children
+    let shouldGetChildren: boolean = true;
+    // Check the cache to see if we have found children before
+    let cached: IntellisenseVariable | undefined = intellisenseLookup.get(parent.Name);
+    if( cached ) {
+      // Even if we have a cached variable, update it if the parent Info does not match or if child entries is short
+      if (cached.VariableEntry.Info !== parent.Info || cached.ChildEntries.length <= 1) {
         shouldGetChildren = true;
+      // Only avoid getting children if the cached variable looks good
       } else {
         shouldGetChildren = false;
       }
-    } else {
-      shouldGetChildren = true;
     }
   
-
-    if (shouldGetChildren) {
-      GetKernelCompletion(parentName + ".").then((completions: string[]) => {
-        const safeCompletions: string[] = completions.filter((s: string) => {
-          if (parent.Info.indexOf("Signature: DataFrame") === 0) {
-            return !(s.indexOf("_") === 0) && !(s.indexOf("style") === 0);
+    if (!shouldGetChildren) {
+      console.log("Not refreshing intellisense for " + parent.Name);
+      // Trigger update intellisense even if we are cached (this could be reconsidered, but original code does this)
+      fireIntellisenseEvent(block);
+    } else {
+      // Get children by prefixing on parent's name (package completions)
+      GetKernelCompletion(parentName + ".").then((childCompletions: string[]) => {
+        // Filter out bad completions (Python specific)
+        let safeCompletions: string[] = childCompletions.filter((s: string) => {
+          if (parent.Info.startsWith("Signature: DataFrame") ) {
+            return !(s.startsWith("_") ) && !(s.startsWith("style"));
           }
           return true;
         });
-        const pr: Promise<string>[] = safeCompletions.map((completion: string) => GetKernalInspection(parentName + "." + completion));
-        return Promise.all(pr).then((inspections: string[]) => {
-          const intellisenseVariable: IntellisenseVariable = new IntellisenseVariable(parent, safeCompletions.map((completion: string, index: number) => {
-            return new IntellisenseEntry(completion, inspections[index], isFunction_Python(inspections[index]), isClass_Python(inspections[index]));
-          }));
-          if (intellisenseLookup.has(parentName)) {
-            intellisenseLookup.set(parentName, intellisenseVariable);
-          } else {
-            addToDict(intellisenseLookup, parentName, intellisenseVariable);
-          }
+        // Set up inspections for filtered children; use a timeout promise so we don't wait forever; make timeout dynamic based on which child this is (assumes serial bottleneck at kernel)
+        // const pr: Promise<string>[] = safeCompletions.map((childCompletion: string, index: number) => timeoutPromise<string>( 100 * (index+1) , GetKernalInspection(childCompletion)) );
+        // For Python we don't currently seem to have a problem with promises not returning
+        const pr: Promise<string>[] = safeCompletions.map((childCompletion: string, index: number) =>  GetKernalInspection(parentName + "." + childCompletion));
+        // Synchronize on inspections to yield the final result
+        Promise.allSettled(pr).then((results : PromiseSettledResult<string>[]) => {
+          // Create an intellisense entries for children, sorted alphabetically
+          let children: IntellisenseEntry[] = safeCompletions.map((childCompletion: string, index: number) => {
+            let info = "";
+            let isFunction = true;
+            let isClass = false;
+            if( results[index].status === "fulfilled") {
+              info = (results[index] as PromiseFulfilledResult<string>).value;
+              isFunction = isFunction_Python(info);
+              isClass = isClass_Python(info);
+            } 
+            return new IntellisenseEntry(childCompletion, info, isFunction, isClass)}).sort((a, b) => (a.Name < b.Name ? -1 : 1));
+          // Package up IntellisenseVariable (parent + children)
+          let intellisenseVariable: IntellisenseVariable = new IntellisenseVariable(parent, children);
+          // Add to cache
+          intellisenseLookup.set(parentName, intellisenseVariable);
+
+          // Fire event; this causes Blockly to refresh
+          fireIntellisenseEvent(block);
+        }).catch(error => {
+          console.log("Intellisense error getting inspections for children of " + parentName, error);
         });
-      }).then(function() {
-        const intellisenseUpdateEvent = new Blockly.Events.BlockChange(block, "field", "VAR", 0, 1);
-        intellisenseUpdateEvent.group = "INTELLISENSE";
-        // @ts-ignore
-        console.log("event status is " + Blockly.Events.disabled_); //disabled_ existed in old version but not new version?
-        // @ts-ignore
-        Blockly.Events.disabled_ = 0;
-        Blockly.Events.fire(intellisenseUpdateEvent);
-      }).catch((error: Error) => {
-        console.log("Intellisense event failed to fire; " + error.message);
+      }).catch(error => {
+        console.log("Intellisense error getting child completions of " + parentName, error);
       });
-    } else {
-      console.log("Not refreshing intellisense for " + parent.Name);
     }
-  }).catch((error: Error) => {
-    console.log("Intellisense event failed to fire; " + error.message);
+  }).catch((error) => {
+    console.log("Intellisense error getting inspection of intellisense variable candidate (parent) " + parentName, error);
   });
 }
 
 
-
 export function requestAndStubOptions_Python(block: Blockly.Block, varName: string): string[][] {
   if ((varName !== "") && !block.isInFlyout) {
     RequestIntellisenseVariable_Python(block, varName);
   }
   if (block.isInFlyout) {
     return [[" ", " "]];
   }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/README.md` & `aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.2/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/.gitignore` & `aolney_jupyterlab_blockly_python_extension-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/LICENSE` & `aolney_jupyterlab_blockly_python_extension-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/README.md` & `aolney_jupyterlab_blockly_python_extension-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 - bl=py forces the extension to display on load (it is already active)
 - log=xxx specifies a url for a logging endpoint (e.g. https://yourdomain.com/log)
 - id=xxx adds an identifier for logging
 
 
 > [!WARNING]  
 > Currently there appears to be a conflict between the Python and R extensions, so we recommend that only one be installed at a time.
-> Additionally the current version of nbgitpuller is removing the query strings above before they can be processed.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 *An earlier version targets JupyterLab 1.2x. You can find that version on [npm](https://www.npmjs.com/package/@aolney/jupyterlab-blockly-python-extension) and in the commit history of this repository ([final tag](https://github.com/aolney/jupyterlab-blockly-python-extension/releases/tag/0.5.6))*
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/pyproject.toml` & `aolney_jupyterlab_blockly_python_extension-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.1/PKG-INFO` & `aolney_jupyterlab_blockly_python_extension-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aolney_jupyterlab_blockly_python_extension
-Version: 0.1.1
+Version: 0.1.2
 Dynamic: Keywords
 Summary: A JupyterLab extension that creates a Blockly palette for Python.
 Project-URL: Homepage, https://github.com/aolney/jupyterlab-blockly-python-extension
 Project-URL: Bug Tracker, https://github.com/aolney/jupyterlab-blockly-python-extension/issues
 Project-URL: Repository, https://github.com/aolney/jupyterlab-blockly-python-extension.git
 Author-email: "Andrew M. Olney" <aolney@memphis.edu>
 License:                                  Apache License
@@ -237,15 +237,14 @@
 - bl=py forces the extension to display on load (it is already active)
 - log=xxx specifies a url for a logging endpoint (e.g. https://yourdomain.com/log)
 - id=xxx adds an identifier for logging
 
 
 > [!WARNING]  
 > Currently there appears to be a conflict between the Python and R extensions, so we recommend that only one be installed at a time.
-> Additionally the current version of nbgitpuller is removing the query strings above before they can be processed.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 *An earlier version targets JupyterLab 1.2x. You can find that version on [npm](https://www.npmjs.com/package/@aolney/jupyterlab-blockly-python-extension) and in the commit history of this repository ([final tag](https://github.com/aolney/jupyterlab-blockly-python-extension/releases/tag/0.5.6))*
```

