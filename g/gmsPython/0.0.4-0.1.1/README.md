# Comparing `tmp/gmsPython-0.0.4.tar.gz` & `tmp/gmspython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmsPython-0.0.4.tar", last modified: Thu Jun 22 12:30:16 2023, max compression
+gzip compressed data, was "gmspython-0.1.1.tar", last modified: Thu May  9 12:27:11 2024, max compression
```

## Comparing `gmsPython-0.0.4.tar` & `gmspython-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.913842 gmsPython-0.0.4/
--rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmsPython-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      496 2023-06-22 12:30:16.912848 gmsPython-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       53 2022-11-25 13:02:43.000000 gmsPython-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.874406 gmsPython-0.0.4/gmsPython/
--rw-rw-rw-   0        0        0      113 2022-11-25 08:53:54.000000 gmsPython-0.0.4/gmsPython/__init__.py
--rw-rw-rw-   0        0        0     2850 2023-06-08 21:34:06.000000 gmsPython-0.0.4/gmsPython/_mixedTools.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.895563 gmsPython-0.0.4/gmsPython/gmsPy/
--rw-rw-rw-   0        0        0       56 2022-11-24 16:06:45.000000 gmsPython-0.0.4/gmsPython/gmsPy/__init__.py
--rw-rw-rw-   0        0        0     5517 2023-05-22 09:12:42.000000 gmsPython-0.0.4/gmsPython/gmsPy/_gmsPy.py
--rw-rw-rw-   0        0        0    10392 2023-06-09 12:23:34.000000 gmsPython-0.0.4/gmsPython/gmsPy/gmsPy.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.895563 gmsPython-0.0.4/gmsPython/gmsPyModels/
--rw-rw-rw-   0        0        0       62 2022-11-25 08:55:10.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/__init__.py
--rw-rw-rw-   0        0        0     1484 2022-11-29 12:14:47.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyGlobals.py
--rw-rw-rw-   0        0        0     8892 2023-06-20 20:57:09.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyModels.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.907842 gmsPython-0.0.4/gmsPython/gmsWrite/
--rw-rw-rw-   0        0        0     1402 2023-01-05 13:30:25.000000 gmsPython-0.0.4/gmsPython/gmsWrite/__init__.py
--rw-rw-rw-   0        0        0     9269 2023-06-16 11:20:09.000000 gmsPython-0.0.4/gmsPython/gmsWrite/_gmsWrite.py
--rw-rw-rw-   0        0        0     1423 2023-06-20 11:09:48.000000 gmsPython-0.0.4/gmsPython/gmsWrite/gmsWrite.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.910856 gmsPython-0.0.4/gmsPython/nestingTree/
--rw-rw-rw-   0        0        0       73 2022-11-24 16:05:43.000000 gmsPython-0.0.4/gmsPython/nestingTree/__init__.py
--rw-rw-rw-   0        0        0     9731 2023-06-22 12:28:19.000000 gmsPython-0.0.4/gmsPython/nestingTree/nestingTree.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.885920 gmsPython-0.0.4/gmsPython.egg-info/
--rw-rw-rw-   0        0        0      496 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 12:30:16.913842 gmsPython-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-06-22 12:28:13.000000 gmsPython-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmspython-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      726 2024-05-09 12:27:11.929472 gmspython-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-05-09 09:22:27.000000 gmspython-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.782232 gmspython-0.1.1/gmsPython/
+-rw-rw-rw-   0        0        0      201 2024-05-08 09:08:49.000000 gmspython-0.1.1/gmsPython/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-06 08:19:01.000000 gmspython-0.1.1/gmsPython/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.851294 gmspython-0.1.1/gmsPython/gamY/
+-rw-rw-rw-   0        0        0       29 2024-04-24 17:03:44.000000 gmspython-0.1.1/gmsPython/gamY/__init__.py
+-rw-rw-rw-   0        0        0     3865 2024-05-06 12:20:51.000000 gmspython-0.1.1/gmsPython/gamY/classes.py
+-rw-rw-rw-   0        0        0    51981 2024-05-09 11:27:58.000000 gmspython-0.1.1/gmsPython/gamY/gamY.py
+-rw-rw-rw-   0        0        0     4532 2024-04-24 16:52:32.000000 gmspython-0.1.1/gmsPython/gamY/patterns.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.866959 gmspython-0.1.1/gmsPython/gmsPy/
+-rw-rw-rw-   0        0        0       32 2024-05-07 08:59:34.000000 gmspython-0.1.1/gmsPython/gmsPy/__init__.py
+-rw-rw-rw-   0        0        0     9492 2024-05-09 11:27:59.000000 gmspython-0.1.1/gmsPython/gmsPy/gmsPy.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.882601 gmspython-0.1.1/gmsPython/gmsPyModels/
+-rw-rw-rw-   0        0        0       38 2024-05-07 11:48:39.000000 gmspython-0.1.1/gmsPython/gmsPyModels/__init__.py
+-rw-rw-rw-   0        0        0     1898 2024-05-09 11:28:00.000000 gmspython-0.1.1/gmsPython/gmsPyModels/gmsPyModels.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.913846 gmspython-0.1.1/gmsPython/gmsWrite/
+-rw-rw-rw-   0        0        0       89 2024-04-26 07:40:14.000000 gmspython-0.1.1/gmsPython/gmsWrite/__init__.py
+-rw-rw-rw-   0        0        0     5973 2024-05-09 09:25:04.000000 gmspython-0.1.1/gmsPython/gmsWrite/gmsWrite.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/gmsPython/nestingTree/
+-rw-rw-rw-   0        0        0       91 2024-05-02 08:44:45.000000 gmspython-0.1.1/gmsPython/nestingTree/__init__.py
+-rw-rw-rw-   0        0        0    10078 2024-05-08 08:58:29.000000 gmspython-0.1.1/gmsPython/nestingTree/nestingTree.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/gmsPython.egg-info/
+-rw-rw-rw-   0        0        0      726 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:27:11.929472 gmspython-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      706 2024-05-09 12:26:58.000000 gmspython-0.1.1/setup.py
```

### Comparing `gmsPython-0.0.4/LICENSE` & `gmspython-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.4/gmsPython/nestingTree/nestingTree.py` & `gmspython-0.1.1/gmsPython/nestingTree/nestingTree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,32 @@
-import pandas as pd, pyDatabases
-from pyDatabases import gpyDB, gpyDB_wheels, adj, adjMultiIndex
-from gmsPython._mixedTools import concatMultiIndices
-
+from gmsPython.auxfuncs import *
 _ftype_inputs, _ftype_outputs = ('CES','CES_norm','MNL'), ('CET','CET_norm','MNL_out')
 _scalePreserving = ('CES_norm','CET_norm','MNL','MNL_out')
 
 def checkOrIgnore(d,k):
 	return d[k] if k in d else k
 def reverseDict(d):
 	return {v:k for k,v in d.items()}
 
-def trimNestingStructure(m, sparsity, maxIter = 10):
-	""" Trim nesting structure in pandas multiindex 'm' with a 'sparsity' pattern on the inputs. NB: Only works on pure input-like trees """
-	t = tree(name = 'test', tree = m.tolist())
-	t.attrs_from_trees()
-	nInputs = sparsity.to_frame(index=False).groupby('s').count().n
-	oneInputSectors = nInputs[nInputs == 1]
-	# Define new mapping for relevant sectors:
-	mapOneInput = adjMultiIndex.applyMult(adj.rc_pd(t.get('output'), oneInputSectors), 
-										  adj.rc_pd(sparsity, oneInputSectors).rename(['s','nn']))
-	mMultipleGoods = adj.rc_pd(m, ('not', oneInputSectors))
-	t = tree(name = 'test', tree = mMultipleGoods.to_list())
-	t.attrs_from_tree()
-
-	# 2. Remove inputs that are not used:
-	noUse = adj.rc_pd(t.get('input'), ('not', sparsity))
-	mMultipleGoods = adj.rc_pd(t.get('map'), ('not', adj.rc_pd(noUse, alias = {'n':'nn'})))
-
-	# 2.A: Number of nodes for each parent node in the system:
-	nNodes = mMultipleGoods.to_frame(index=False).groupby(['s','n']).count()
-	i = 0
-	while min(nNodes['nn'])<=1:
-		i = i+1
-		mMultipleGoods, nNodes = trim_ite(mMultipleGoods, nNodes)
-		if i==maxIter:
-			raise StopIteration("Tree trimming did not converge")
-	return mMultipleGoods.union(mapOneInput)
-
-def trim_ite(m, nNodes):
-	# 2B: Define mapping where knots have a single node:
-	nodesOneChild = nNodes[nNodes['nn'] == 1].index
-	mapOneNode = adj.rc_pd(m, nodesOneChild)
-	# We make an exception if a combination (s, x) enters as both a knot and a branch. In this case, we cannot remove the parent node of 'x' (as we need this to maintain the tree structure)
-	keepKnots = adj.rc_pd(mapOneNode.droplevel('nn').unique(), mapOneNode.droplevel('n').rename(['s','n']))
-	nodesOneChild = nodesOneChild.difference(keepKnots)
-	mapOneNode = adj.rc_pd(m, nodesOneChild)
-	m = adj.rc_pd(m, ('not', nodesOneChild))
-	# Apply map to change parent nodes
-	mapNewNodes = adjMultiIndex.applyMult(m, mapOneNode.rename(['s','nn','new'])).droplevel('nn').rename(['s','n','nn'])
-	m = adj.rc_pd(m, ('not', nodesOneChild.rename(['s','nn']))).union(mapNewNodes)
-	# 2A: Return number of nodes for each one now:
-	nNodes = m.to_frame(index = False).groupby(['s','n']).count()
-	return m, nNodes
-
-class tree:
-	def __init__(self, name, tree = None, io = None, db = None, f = None,**ns):
+class Tree:
+	def __init__(self, name, tree = None, db = None, f = None,**ns):
 		self.name = name
-		self.db = pyDatabases.noneInit(db,{})
-		self.addFunctionandIO(f,io)
+		self.db = noneInit(db,{})
+		self.addFunctionandIO(f)
 		self.scalePreserving = True if self.f in _scalePreserving else False
-		self.ns = {k:v if k not in ns else ns[k] for k,v in self.standardNamespace.items()}
-		self.tree = pyDatabases.noneInit(tree,[])
+		self.ns = self.standardNamespace | ns
+		self.tree = noneInit(tree,[])
 
 	@property
 	def standardNamespace(self):
-		return {k: k+'_'+self.name for k in ('map','knot','branch','input','output','int')}
+		return {k: f'{self.name}_{k}' for k in ('map','knot','branch','input','output','int')}
 
-	def addFunctionandIO(self,f,io):
-		if f:
-			self.f = f
-			if io is None:
-				self.io = 'input' if self.f in _ftype_inputs else 'output'
-			else:
-				self.io = io
-		else:
-			self.io = 'input' if io is None else io
-			self.f = 'CES' if self.io == 'input' else 'CET'
+	def addFunctionandIO(self,f):
+		self.f = 'CES' if f is None else f
+		self.io = 'input' if self.f in _ftype_inputs else 'output' 
 
 	def __getitem__(self,item):
 		try:
 			return self.db[self.ns[item]]
 		except KeyError:
 			return self.db[item]
 
@@ -88,102 +35,161 @@
 			self.db[self.ns[item]] = gpyDB.gpy(value,**{'name': self.ns[item]})
 		except KeyError:
 			self.db[item] = gpyDB.gpy(value,**{'name': item})
 
 	def get(self,item):
 		return self[item].vals
 
-	def attrs_from_tree(self):
+	def attrsFromTree_input(self):
+		self['map'] = pd.MultiIndex.from_tuples(self.tree, names = ['s', 'n','nn'])
+		self['knot'] = self.get('map').droplevel('nn').unique()
+		self['branch'] = self.get('map').droplevel('n').unique().rename(['s','n'])
+		self['n'] = self.get('knot').union(self.get('branch')).droplevel('s').unique()
+		self['s'] = self.get('map').get_level_values('s').unique()
+		self['input'] = self.get('branch').difference(self.get('knot'))
+		self['output'] = self.get('knot').difference(self.get('branch'))
+		self['int'] = (self.get('branch').union(self.get('knot'))).difference(self.get('input').union(self.get('output')))
+
+	def attrsFromTree_output(self):
 		self['map'] = pd.MultiIndex.from_tuples(self.tree, names = ['s', 'n','nn'])
-		self['knot'] = self.get('map').droplevel('nn').unique() if self.io == 'input' else self.get('map').droplevel('n').rename(['s','n']).unique()
-		self['branch'] = self.get('map').droplevel('n').unique().rename(['s','n']) if self.io == 'input' else self.get('map').droplevel('nn').unique()
+		self['knot'] = self.get('map').droplevel('n').rename(['s','n']).unique()
+		self['branch'] = self.get('map').droplevel('nn').unique()
 		self['n'] = self.get('knot').union(self.get('branch')).droplevel('s').unique()
 		self['s'] = self.get('map').get_level_values('s').unique()
-		self['input'] = self.get('branch').difference(self.get('knot')) if self.io == 'input' else self.get('knot').difference(self.get('branch'))
-		self['output'] = self.get('branch').difference(self.get('knot')) if self.io == 'output' else self.get('knot').difference(self.get('branch'))
+		self['input'] = self.get('knot').difference(self.get('branch'))
+		self['output'] = self.get('branch').difference(self.get('knot'))
 		self['int'] = (self.get('branch').union(self.get('knot'))).difference(self.get('input').union(self.get('output')))
 
-class tree_from_data(tree):
-	def __init__(self,workbook,sheet,name=None,io=None,f=None,**ns):
-		""" Workbook has to be supplied"""
-		super().__init__(sheet if name is None else name, db = gpyDB_wheels.read.variables(workbook[sheet]),io=io,f=f,**ns)
+	def __call__(self):
+		getattr(self, f'attrsFromTree_{self.io}')()
+		return self
+
+class TreeFromData(Tree):
+	def __init__(self,workbook,sheet,name=None,f=None,**ns):
+		""" Workbook, sheet has to be supplied"""
+		if type(workbook) is str:
+			workbook = gpyDB.DbFromExcel.simpleLoad(workbook)
+		super().__init__(sheet if name is None else name, db = gpyDB.DbFromExcel.var(workbook[sheet]),f=f,**ns)
 		self.tree = self['mu'].index.to_list()
 
-class aggTree:
-	def __init__(self,name="",trees=None,**ns):
+class AggTree:
+	def __init__(self,name="",trees=None, ws = None, **ns):
 		self.name=name
-		self.ns = {k:v if k not in ns else ns[k] for k,v in self.standardNamespace.items()}
-		self.trees = pyDatabases.noneInit(trees,{})
+		self.ns = self.standardNamespace | ns
+		self.trees = noneInit(trees,{})
 		self.prune = ('n','nn','nnn','s','input','output','int')
-		self.db = gpyDB.GpyDB(alias=pd.MultiIndex.from_tuples([(self.n('n'),self.n('nn')), (self.n('n'),self.n('nnn'))]),**{'name':self.name})
+		self.db = gpyDB.GpyDB(ws = ws, alias=[(self.n('n'),self.n('nn')), (self.n('n'),self.n('nnn'))], name = self.name)
 
 	@property
 	def standardNamespace(self):
-		return {k:k for k in ('n','nn','nnn','s')} | {k: k+'_'+self.name for k in ('map','int','input','output','map_spinp','map_spout','knout','kninp','spinp','spout')}
+		return {k:k for k in ('n','nn','nnn','s')} | {k: f'{self.name}_{k}' for k in ('map','int','input','output','map_spinp','map_spout','knout','kninp','spinp','spout')}
 
 	def n(self,item,local=None):
 		return self.ns[item] if local is None else self.trees[local].ns[item]
 
 	def get(self,item,local=None):
 		return self.db[self.n(item,local=local)].vals
 
 	def __setitem__(self,item,value):
 		self.db[self.n(item)] = value
 
 	def __call__(self,namespace=None):
-		[tree.attrs_from_tree() for tree in self.trees.values()];
-		self.attrs_from_trees()
-		self.adjust_trees()
-		[self.add_db_prune(tree) for tree in self.trees.values()];
+		[tree() for tree in self.trees.values()]; 
+		self.attrsFromTrees()
+		self.adjustTrees()
+		[self.addDbAndPrune(tree) for tree in self.trees.values()];
 		self.namespace = namespace
 		if namespace:
-			gpyDB_wheels.aggregateDB.updateSetValues(self.db,self.n('n'),namespace)
+			gpyDB.AggDB.updSetElements(self.db,self.n('n'),namespace)
 		return self
 
-	def add_db_prune(self,tree):
-		[gpyDB.GpyDBs_AOM_Second(self.db,s) for name,s in tree.db.items() if checkOrIgnore(reverseDict(tree.ns),name) not in self.prune];
+	def addDbAndPrune(self,tree):
+		[self.db.aom_gpy(s) for name,s in tree.db.items() if checkOrIgnore(reverseDict(tree.ns), name) not in self.prune];
 
-	def attrs_from_trees(self):
+	def attrsFromTrees(self):
 		self['n'] = pd.Index(set.union(*[set(tree.get('n')) for tree in self.trees.values()]), name = self.n('n'))
 		self['s'] = pd.Index(set.union(*[set(tree.get('s')) for tree in self.trees.values()]), name = self.n('s'))
 		self['map'] = concatMultiIndices([tree.get('map') for tree in self.trees.values()])
 		self['map_spinp'] = concatMultiIndices([tree.get('map') for tree in self.trees.values() if tree.scalePreserving and tree.io == 'input'], names = self.get('map').names)
 		self['map_spout'] = concatMultiIndices([tree.get('map') for tree in self.trees.values() if tree.scalePreserving and tree.io == 'output'], names = self.get('map').names)
 		self['knout'] = concatMultiIndices([tree.get('knot') for tree in self.trees.values() if tree.io == 'output'],  names=[self.n('s'),self.n('n')])
 		self['kninp'] = concatMultiIndices([tree.get('knot') for tree in self.trees.values() if tree.io == 'input'],  names=[self.n('s'),self.n('n')])
-		self['spout'] = self.get('map_spinp').droplevel(self.n('nn')).unique()
-		self['spinp'] = self.get('map_spout').droplevel(self.n('n')).unique().rename([self.n('s'),self.n('n')])
+		self['spout'] = self.get('map_spout').droplevel(self.n('nn')).unique()
+		self['spinp'] = self.get('map_spinp').droplevel(self.n('n')).unique().rename([self.n('s'),self.n('n')])
 		inputs = set.union(*[set(tree.get('input')) for tree in self.trees.values()])
 		outputs= set.union(*[set(tree.get('output')) for tree in self.trees.values()])
 		ints = set.union(*[set(tree.get('int')) for tree in self.trees.values()])
 		self['input'] = pd.MultiIndex.from_tuples(inputs-outputs,names = [self.n('s'),self.n('n')])
 		self['output']= pd.MultiIndex.from_tuples(outputs-inputs,names = [self.n('s'),self.n('n')])
-		self['int'] = pd.MultiIndex.from_tuples((inputs.intersection(outputs)).union(ints), names = [self.n('s'),self.n('n')])
+		self['int'] = pd.MultiIndex.from_tuples((inputs.intersection(outputs)).union(ints), names = [self.n('s'),self.n('n')])		
+
+	def adjustTrees(self):
+		[getattr(self, f'adjustTree_{tree.io}')(tree) for tree in self.trees.values()];
 
-	def adjust_trees(self):
-		[self.adjust_tree_in(tree) for tree in self.trees.values() if tree.io == 'input'];
-		[self.adjust_tree_out(tree) for tree in self.trees.values() if tree.io == 'output'];
-
-	def adjust_tree_in(self,tree):
-		tree.ns['knot_o'] = 'knot_o_'+tree.name
-		tree.ns['knot_no'] = 'knot_no_'+tree.name
-		tree.ns['branch2o'] = 'branch2o_'+tree.name
-		tree.ns['branch2no']= 'branch2no_'+tree.name
+	def adjustTree_input(self,tree):
+		[tree.ns.__setitem__(k,f'{tree.name}_{k}') for k in ('knot_o','knot_no','branch2o','branch2no')];
 		tree['knot_o'] = tree.get('knot').intersection(self.get('output'))
 		tree['knot_no'] = tree.get('knot').difference(self.get('output'))
-		tree['branch2o'] = gpyDB_wheels.adj.rc_pd(tree['map'], self.get('output')).droplevel(self.n('n')).rename([self.n('s'),self.n('n')])
-		tree['branch2no'] = gpyDB_wheels.adj.rc_pd(tree['map'], ('not', self.get('output'))).droplevel(self.n('n')).rename([self.n('s'),self.n('n')])
+		tree['branch2o'] = pyDatabases.adj.rc_pd(tree['map'], self.get('output')).droplevel(self.n('n')).rename([self.n('s'),self.n('n')])
+		tree['branch2no'] = pyDatabases.adj.rc_pd(tree['map'], ('not', self.get('output'))).droplevel(self.n('n')).rename([self.n('s'),self.n('n')])
 
-	def adjust_tree_out(self,tree):
-		tree.ns['branch_o'] = 'branch_o_'+tree.name
-		tree.ns['branch_no'] = 'branch_no_'+tree.name
+	def adjustTree_output(self,tree):
+		[tree.ns.__setitem__(k,f'{tree.name}_{k}') for k in ('branch_o','branch_no')];
 		tree['branch_o'] = tree.get('branch').intersection(self.get('output'))
 		tree['branch_no'] = tree.get('branch').difference(tree.get('branch_o'))
 
-class aggTree_from_data(aggTree):
+class AggTreeFromData(AggTree):
 	def __init__(self,file_path,read_trees=None,name="",**ns):
 		""" read_trees are passed to tree_from_data """
 		super().__init__(name=name,**ns)
-		wb = gpyDB_wheels.read.simpleLoad(file_path)
+		wb = gpyDB.DbFromExcel.simpleLoad(file_path)
 		if read_trees is None:
-			read_trees = {sheet: {} for sheet in gpyDB_wheels.read.sheetnames_from_wb(wb)}
-		self.trees = {t.name: t for t in (tree_from_data(wb,k,**v) for k,v in read_trees.items())}
+			read_trees = {sheet: {} for sheet in gpyDB.DbFromExcel.sheetnames_from_wb(wb)}
+		self.trees = {t.name: t for t in (TreeFromData(wb,k,**v) for k,v in read_trees.items())}
+
+def trimNestingStructure(m, sparsity, maxIter = 10):
+	""" Trim nesting structure in pandas multiindex 'm' with a 'sparsity' pattern on the inputs. NB: Only works on pure input-like trees """
+	t = Tree(name = 'test', tree = m.tolist())()
+	nInputs = sparsity.to_frame(index=False).groupby('s').count().n
+	oneInputSectors = nInputs[nInputs == 1]
+	# Define new mapping for relevant sectors:
+	mapOneInput = pyDatabases.adjMultiIndex.applyMult(pyDatabases.adj.rc_pd(t.get('output'), oneInputSectors), 
+													  pyDatabases.adj.rc_pd(sparsity, oneInputSectors).rename(['s','nn']))
+	mMultipleGoods = pyDatabases.adj.rc_pd(m, ('not', oneInputSectors))
+	t = Tree(name = 'test', tree = mMultipleGoods.to_list())()
+	inputs = t.get('input')
+
+	# 2. Remove inputs that are not used:
+	noUse = pyDatabases.adj.rc_pd(t.get('input'), ('not', sparsity))
+	mMultipleGoods = pyDatabases.adj.rc_pd(t.get('map'), ('not', pyDatabases.adj.rc_pd(noUse, alias = {'n':'nn'})))
+
+	# 2.A: Number of nodes for each parent node in the system:
+	nNodes = mMultipleGoods.to_frame(index=False).groupby(['s','n']).count()
+
+	# Start iteration checks
+	i = 0
+	t = Tree(name = 'test', tree=mMultipleGoods.tolist())()
+	inputs_i = t.get('input')
+	while (min(nNodes['nn'])<=1) & (not inputs_i.difference(inputs).empty):
+		i = i+1
+		mMultipleGoods, nNodes, inputs_i = trim_ite(mMultipleGoods, nNodes)
+		mMultipleGoods = pyDatabases.adj.rc_pd(mMultipleGoods, ('not', inputs_i.difference(inputs).rename(['s','nn'])))
+		if i==maxIter:
+			raise StopIteration("Tree trimming did not converge")
+	return mMultipleGoods.union(mapOneInput)
+
+def trim_ite(m, nNodes):
+	# 2B: Define mapping where knots have a single node:
+	nodesOneChild = nNodes[nNodes['nn'] == 1].index
+	mapOneNode = pyDatabases.adj.rc_pd(m, nodesOneChild)
+	# We make an exception if a combination (s, x) enters as both a knot and a branch. In this case, we cannot remove the parent node of 'x' (as we need this to maintain the tree structure)
+	keepKnots = pyDatabases.adj.rc_pd(mapOneNode.droplevel('nn').unique(), mapOneNode.droplevel('n').rename(['s','n']))
+	nodesOneChild = nodesOneChild.difference(keepKnots)
+	mapOneNode = pyDatabases.adj.rc_pd(m, nodesOneChild)
+	m = pyDatabases.adj.rc_pd(m, ('not', nodesOneChild))
+	# Apply map to change parent nodes
+	mapNewNodes = pyDatabases.adjMultiIndex.applyMult(m, mapOneNode.rename(['s','nn','new'])).droplevel('nn').rename(['s','n','nn'])
+	m = pyDatabases.adj.rc_pd(m, ('not', nodesOneChild.rename(['s','nn']))).union(mapNewNodes)
+	# 2A: Return number of nodes for each one now:
+	nNodes = m.to_frame(index = False).groupby(['s','n']).count()
+	t = Tree(name='test', tree = m.tolist())()
+	return m, nNodes, t.get('input')
```

### Comparing `gmsPython-0.0.4/setup.py` & `gmspython-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="gmsPython",
-  version="0.0.4",
+  version="0.1.1",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Automating GAMS models and execution from Python",
   long_description=long_description,
   long_description_content_type="text/markdown",
-  url="https://github.com/ChampionApe/gamsPythonModels",
+  url="https://github.com/ChampionApe/gmsPython",
   packages=setuptools.find_packages(),
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
   ],
-  python_requires='>=3.8',
-  install_requires=["pandas", "scipy","openpyxl","pyDatabases","gams"],
+  python_requires='>=3.10',
+  install_requires=["pandas", "scipy","openpyxl","pyDatabases","gamsapi"],
 )
```

