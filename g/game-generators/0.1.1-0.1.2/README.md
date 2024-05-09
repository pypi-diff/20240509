# Comparing `tmp/game_generators-0.1.1.tar.gz` & `tmp/game_generators-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_generators-0.1.1.tar", max compression
+gzip compressed data, was "game_generators-0.1.2.tar", max compression
```

## Comparing `game_generators-0.1.1.tar` & `game_generators-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.1/LICENSE
--rw-r--r--   0        0        0     2664 2023-11-15 12:41:44.087214 game_generators-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-05 12:41:11.281873 game_generators-0.1.1/game_generators/__init__.py
--rw-r--r--   0        0        0      425 2023-11-15 12:34:36.108713 game_generators-0.1.1/game_generators/functions/__init__.py
--rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.1/game_generators/functions/ces.py
--rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.1/game_generators/functions/cobb_douglas.py
--rw-r--r--   0        0        0     4562 2023-11-15 12:34:36.113509 game_generators-0.1.1/game_generators/functions/concave.py
--rw-r--r--   0        0        0      907 2023-11-15 09:37:28.877926 game_generators-0.1.1/game_generators/functions/interpolate.py
--rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.1/game_generators/functions/leontief.py
--rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.1/game_generators/functions/linear.py
--rw-r--r--   0        0        0     4540 2023-11-15 12:34:36.118874 game_generators-0.1.1/game_generators/functions/monotonic.py
--rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.1/game_generators/functions/polynomial.py
--rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.1/game_generators/multi_objective/__init__.py
--rw-r--r--   0        0        0     1070 2023-11-15 09:25:46.503128 game_generators-0.1.1/game_generators/multi_objective/from_nfg.py
--rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.1/game_generators/multi_objective/identity.py
--rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.1/game_generators/nfg/__init__.py
--rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.1/game_generators/nfg/bach_stravinsky.py
--rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.1/game_generators/nfg/bertrand_oligopoly.py
--rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.1/game_generators/nfg/chicken.py
--rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.1/game_generators/nfg/congestion.py
--rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.1/game_generators/nfg/covariant.py
--rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.1/game_generators/nfg/discrete_uniform.py
--rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.1/game_generators/nfg/grab_the_dollar.py
--rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.1/game_generators/nfg/hawk_dove.py
--rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.1/game_generators/nfg/majority_voting.py
--rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.1/game_generators/nfg/potential.py
--rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.1/game_generators/nfg/random_uniform.py
--rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.1/game_generators/nfg/war_of_attrition.py
--rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.1/game_generators/nfg/zero_sum.py
--rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.1/game_generators/utils/__init__.py
--rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.1/game_generators/utils/data.py
--rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.1/game_generators/utils/generators.py
--rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.1/game_generators/utils/transforms.py
--rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.1/game_generators/utils/visualisation.py
--rw-r--r--   0        0        0      490 2023-11-15 12:53:18.409963 game_generators-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 game_generators-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2776 2024-02-12 15:39:26.386891 game_generators-0.1.2/README.md
+-rw-r--r--   0        0        0      268 2024-02-12 15:39:48.773435 game_generators-0.1.2/game_generators/__init__.py
+-rw-r--r--   0        0        0     1308 2024-02-12 15:38:16.190643 game_generators-0.1.2/game_generators/functions/__init__.py
+-rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.2/game_generators/functions/ces.py
+-rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.2/game_generators/functions/cobb_douglas.py
+-rw-r--r--   0        0        0     4562 2023-11-15 12:34:36.113509 game_generators-0.1.2/game_generators/functions/concave.py
+-rw-r--r--   0        0        0      907 2023-11-15 09:37:28.877926 game_generators-0.1.2/game_generators/functions/interpolate.py
+-rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.2/game_generators/functions/leontief.py
+-rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.2/game_generators/functions/linear.py
+-rw-r--r--   0        0        0     8661 2024-05-09 08:44:32.236987 game_generators-0.1.2/game_generators/functions/monotonic.py
+-rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.2/game_generators/functions/polynomial.py
+-rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.2/game_generators/multi_objective/__init__.py
+-rw-r--r--   0        0        0     1068 2024-02-12 15:34:16.243350 game_generators-0.1.2/game_generators/multi_objective/from_nfg.py
+-rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.2/game_generators/multi_objective/identity.py
+-rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.2/game_generators/nfg/__init__.py
+-rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.2/game_generators/nfg/bach_stravinsky.py
+-rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.2/game_generators/nfg/bertrand_oligopoly.py
+-rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.2/game_generators/nfg/chicken.py
+-rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.2/game_generators/nfg/congestion.py
+-rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.2/game_generators/nfg/covariant.py
+-rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.2/game_generators/nfg/discrete_uniform.py
+-rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.2/game_generators/nfg/grab_the_dollar.py
+-rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.2/game_generators/nfg/hawk_dove.py
+-rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.2/game_generators/nfg/majority_voting.py
+-rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.2/game_generators/nfg/potential.py
+-rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.2/game_generators/nfg/random_uniform.py
+-rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.2/game_generators/nfg/war_of_attrition.py
+-rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.2/game_generators/nfg/zero_sum.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.2/game_generators/utils/__init__.py
+-rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.2/game_generators/utils/data.py
+-rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.2/game_generators/utils/generators.py
+-rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.2/game_generators/utils/transforms.py
+-rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.2/game_generators/utils/visualisation.py
+-rw-r--r--   0        0        0      490 2024-05-09 10:58:04.349617 game_generators-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 game_generators-0.1.2/PKG-INFO
```

### Comparing `game_generators-0.1.1/LICENSE` & `game_generators-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/README.md` & `game_generators-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 # Game Generators
 
-Game Generators (gage) is a package for efficiently generating games for research and experimentation. It is loosely based
+Game Generators (gage) is a package for efficiently generating games for research and experimentation. It is loosely
+based
 on [GAMUT](http://gamut.stanford.edu/). Its main features are:
 
-1. Efficiently generate batches of games from a wide range of available game structures that can be used for deep learning purposes.
-2. Sample random utility functions of widely used classes, such as concave functions, monotonically increasing/decreasing functions and more.
+1. Efficiently generate batches of games from a wide range of available game structures that can be used for deep
+   learning purposes.
+2. Sample random utility functions of widely used classes, such as concave functions, monotonically
+   increasing/decreasing functions and more.
 3. In-depth documentation that provides references to the literature.
 4. Extensive test suite to verify the correctness of the generated games.
 
 ## Installation
 
-For now, Gage is only available for installation from source. To install, clone the repository and pip install the necessary packages.
+You can install the package using pip:
+
+```bash
+pip install game-generators
+```
 
 ## Quickstart
-To start generating games, simply import the package and use the game generator that you desire. For example, to generate a batch of 10 Bach-Stravinsky games, use the following code:
+
+To start generating games, simply import the package and use the game generator that you desire. For example, to
+generate a batch of 10 Bach-Stravinsky games, use the following code:
 
 ```python
-import gage
+import game_generators as gage
 
+# Generate a batch of Bach-Stravinsky games directly.
 batch_size = 10
 payoff_matrices = gage.nfg.bach_stravinsky(batch_size)
+print(payoff_matrices.shape)
+
+# Or alternatively through the generic interface.
+payoff_matrices = gage.generate_nfg("bach_stravinsky", batch_size)
+print(payoff_matrices.shape)
 
-# Or alternatively
-payoff_matrices = gage.generate_game("bach_stravinsky", batch_size)
 ```
 
-To see all available game generators, see the [documentation](https://wilrop.github.io/gage/) or check ``gage.available_games``.
+To see all available game generators, see the [documentation](https://wilrop.github.io/gage/) or
+check ``gage.available_games``.
 
 ## Format
 
-Every game is returned with separate payoff tensors per player. For example, when generating a batch of 10 games with 2  players and 3 actions per player, we return a (10, 2, 3, 3) tensor where the first dimension contains the batch, the second dimension contains a payoff tensor for an individual player, and the remainder is the joint action dimension.
+Every game is returned with separate payoff tensors per player. For example, when generating a batch of 10 games with 2
+players and 3 actions per player, we return a (10, 2, 3, 3) tensor where the first dimension contains the batch, the
+second dimension contains a payoff tensor for an individual player, and the remainder is the joint action dimension.
 
-It is common in game theoretic research to present joint payoff tensors. We provide a function to convert the separate payoff tensors to a joint payoff tensor. This function is called `to_joint_payoff` and is available in
+It is common in game theoretic research to present joint payoff tensors. We provide a function to convert the separate
+payoff tensors to a joint payoff tensor. This function is called `to_joint_payoff` and is available in
 the `utils.transforms` module. In the example above, it would return a (10, 3, 3, 2) tensor.
 
-
 ## Contributing
 
 We are building a suite of game generators that can be used in modern game theoretic research. If you are working in
 this area and want to get involved, contributions are very welcome! For major changes, please open an issue first to
 discuss what you would like to change.
 
 ## Citation
```

### Comparing `game_generators-0.1.1/game_generators/functions/ces.py` & `game_generators-0.1.2/game_generators/functions/ces.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/cobb_douglas.py` & `game_generators-0.1.2/game_generators/functions/cobb_douglas.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/concave.py` & `game_generators-0.1.2/game_generators/functions/concave.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/interpolate.py` & `game_generators-0.1.2/game_generators/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/leontief.py` & `game_generators-0.1.2/game_generators/functions/leontief.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/linear.py` & `game_generators-0.1.2/game_generators/functions/linear.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/functions/polynomial.py` & `game_generators-0.1.2/game_generators/functions/polynomial.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/multi_objective/from_nfg.py` & `game_generators-0.1.2/game_generators/multi_objective/from_nfg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from gage.nfg.generate_nfg import generate_nfg
+from game_generators.nfg import generate_nfg
 
 
 def from_nfg(game, num_players, num_actions, num_objectives, batch_size=1, **kwargs):
     """Generate a multi-objective normal form game.
 
     The function generates multi-objective versions of the NFGs in the main library. These are generated by adding a new
     dimension to the payoff matrices. Multi-objective versions of these games ensure that the payoffs for each objective
```

### Comparing `game_generators-0.1.1/game_generators/multi_objective/identity.py` & `game_generators-0.1.2/game_generators/multi_objective/identity.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/__init__.py` & `game_generators-0.1.2/game_generators/nfg/__init__.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/bach_stravinsky.py` & `game_generators-0.1.2/game_generators/nfg/bach_stravinsky.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/bertrand_oligopoly.py` & `game_generators-0.1.2/game_generators/nfg/bertrand_oligopoly.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/chicken.py` & `game_generators-0.1.2/game_generators/nfg/chicken.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/congestion.py` & `game_generators-0.1.2/game_generators/nfg/congestion.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/covariant.py` & `game_generators-0.1.2/game_generators/nfg/covariant.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/discrete_uniform.py` & `game_generators-0.1.2/game_generators/nfg/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/grab_the_dollar.py` & `game_generators-0.1.2/game_generators/nfg/grab_the_dollar.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/hawk_dove.py` & `game_generators-0.1.2/game_generators/nfg/hawk_dove.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/majority_voting.py` & `game_generators-0.1.2/game_generators/nfg/majority_voting.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/potential.py` & `game_generators-0.1.2/game_generators/nfg/potential.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/random_uniform.py` & `game_generators-0.1.2/game_generators/nfg/random_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/war_of_attrition.py` & `game_generators-0.1.2/game_generators/nfg/war_of_attrition.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/nfg/zero_sum.py` & `game_generators-0.1.2/game_generators/nfg/zero_sum.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/utils/data.py` & `game_generators-0.1.2/game_generators/utils/data.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/utils/generators.py` & `game_generators-0.1.2/game_generators/utils/generators.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/utils/transforms.py` & `game_generators-0.1.2/game_generators/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/game_generators/utils/visualisation.py` & `game_generators-0.1.2/game_generators/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.1/PKG-INFO` & `game_generators-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-generators
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficiently generate games for research and experimentation
 Home-page: https://github.com/wilrop/game-generators
 License: MIT
 Author: Willem Röpke
 Author-email: willem.ropke@vub.be
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,49 +16,65 @@
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: scipy (==1.11.3) ; python_version < "3.13"
 Project-URL: Repository, https://github.com/wilrop/game-generators
 Description-Content-Type: text/markdown
 
 # Game Generators
 
-Game Generators (gage) is a package for efficiently generating games for research and experimentation. It is loosely based
+Game Generators (gage) is a package for efficiently generating games for research and experimentation. It is loosely
+based
 on [GAMUT](http://gamut.stanford.edu/). Its main features are:
 
-1. Efficiently generate batches of games from a wide range of available game structures that can be used for deep learning purposes.
-2. Sample random utility functions of widely used classes, such as concave functions, monotonically increasing/decreasing functions and more.
+1. Efficiently generate batches of games from a wide range of available game structures that can be used for deep
+   learning purposes.
+2. Sample random utility functions of widely used classes, such as concave functions, monotonically
+   increasing/decreasing functions and more.
 3. In-depth documentation that provides references to the literature.
 4. Extensive test suite to verify the correctness of the generated games.
 
 ## Installation
 
-For now, Gage is only available for installation from source. To install, clone the repository and pip install the necessary packages.
+You can install the package using pip:
+
+```bash
+pip install game-generators
+```
 
 ## Quickstart
-To start generating games, simply import the package and use the game generator that you desire. For example, to generate a batch of 10 Bach-Stravinsky games, use the following code:
+
+To start generating games, simply import the package and use the game generator that you desire. For example, to
+generate a batch of 10 Bach-Stravinsky games, use the following code:
 
 ```python
-import gage
+import game_generators as gage
 
+# Generate a batch of Bach-Stravinsky games directly.
 batch_size = 10
 payoff_matrices = gage.nfg.bach_stravinsky(batch_size)
+print(payoff_matrices.shape)
+
+# Or alternatively through the generic interface.
+payoff_matrices = gage.generate_nfg("bach_stravinsky", batch_size)
+print(payoff_matrices.shape)
 
-# Or alternatively
-payoff_matrices = gage.generate_game("bach_stravinsky", batch_size)
 ```
 
-To see all available game generators, see the [documentation](https://wilrop.github.io/gage/) or check ``gage.available_games``.
+To see all available game generators, see the [documentation](https://wilrop.github.io/gage/) or
+check ``gage.available_games``.
 
 ## Format
 
-Every game is returned with separate payoff tensors per player. For example, when generating a batch of 10 games with 2  players and 3 actions per player, we return a (10, 2, 3, 3) tensor where the first dimension contains the batch, the second dimension contains a payoff tensor for an individual player, and the remainder is the joint action dimension.
+Every game is returned with separate payoff tensors per player. For example, when generating a batch of 10 games with 2
+players and 3 actions per player, we return a (10, 2, 3, 3) tensor where the first dimension contains the batch, the
+second dimension contains a payoff tensor for an individual player, and the remainder is the joint action dimension.
 
-It is common in game theoretic research to present joint payoff tensors. We provide a function to convert the separate payoff tensors to a joint payoff tensor. This function is called `to_joint_payoff` and is available in
+It is common in game theoretic research to present joint payoff tensors. We provide a function to convert the separate
+payoff tensors to a joint payoff tensor. This function is called `to_joint_payoff` and is available in
 the `utils.transforms` module. In the example above, it would return a (10, 3, 3, 2) tensor.
 
-
 ## Contributing
 
 We are building a suite of game generators that can be used in modern game theoretic research. If you are working in
 this area and want to get involved, contributions are very welcome! For major changes, please open an issue first to
 discuss what you would like to change.
 
 ## Citation
```

