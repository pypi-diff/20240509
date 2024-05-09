# Comparing `tmp/pydatabases-0.1.1.tar.gz` & `tmp/pydatabases-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatabases-0.1.1.tar", last modified: Thu Apr 18 11:52:25 2024, max compression
+gzip compressed data, was "pydatabases-0.1.3.tar", last modified: Thu May  9 12:13:49 2024, max compression
```

## Comparing `pydatabases-0.1.1.tar` & `pydatabases-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.473285 pydatabases-0.1.1/
--rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      761 2024-04-18 11:52:25.472073 pydatabases-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.436880 pydatabases-0.1.1/pyDatabases/
--rw-rw-rw-   0        0        0       34 2024-04-16 22:50:27.000000 pydatabases-0.1.1/pyDatabases/__init__.py
--rw-rw-rw-   0        0        0    12902 2024-04-16 23:18:35.000000 pydatabases-0.1.1/pyDatabases/auxfuncs.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.461176 pydatabases-0.1.1/pyDatabases/gpyDB/
--rw-rw-rw-   0        0        0      101 2024-04-16 22:30:11.000000 pydatabases-0.1.1/pyDatabases/gpyDB/__init__.py
--rw-rw-rw-   0        0        0    20423 2024-04-18 07:18:37.000000 pydatabases-0.1.1/pyDatabases/gpyDB/database.py
--rw-rw-rw-   0        0        0    24830 2024-04-18 11:47:33.000000 pydatabases-0.1.1/pyDatabases/gpyDB/gpyDB.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.467479 pydatabases-0.1.1/pyDatabases/simpleDB/
--rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.1/pyDatabases/simpleDB/__init__.py
--rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.1/pyDatabases/simpleDB/simpleDB.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.469903 pydatabases-0.1.1/pyDatabases.egg-info/
--rw-rw-rw-   0        0        0      761 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:52:25.474216 pydatabases-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-18 11:51:34.000000 pydatabases-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.077406 pydatabases-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      761 2024-05-09 12:13:49.069348 pydatabases-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.018670 pydatabases-0.1.3/pyDatabases/
+-rw-rw-rw-   0        0        0       67 2024-05-08 09:08:36.000000 pydatabases-0.1.3/pyDatabases/__init__.py
+-rw-rw-rw-   0        0        0    12976 2024-05-07 13:38:36.000000 pydatabases-0.1.3/pyDatabases/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.057126 pydatabases-0.1.3/pyDatabases/gpyDB/
+-rw-rw-rw-   0        0        0      101 2024-05-08 09:08:38.000000 pydatabases-0.1.3/pyDatabases/gpyDB/__init__.py
+-rw-rw-rw-   0        0        0    20468 2024-05-09 11:27:53.000000 pydatabases-0.1.3/pyDatabases/gpyDB/database.py
+-rw-rw-rw-   0        0        0    24932 2024-05-09 11:14:06.000000 pydatabases-0.1.3/pyDatabases/gpyDB/gpyDB.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.069348 pydatabases-0.1.3/pyDatabases/simpleDB/
+-rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.3/pyDatabases/simpleDB/__init__.py
+-rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.3/pyDatabases/simpleDB/simpleDB.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.069348 pydatabases-0.1.3/pyDatabases.egg-info/
+-rw-rw-rw-   0        0        0      761 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:13:49.077406 pydatabases-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-05-09 12:11:41.000000 pydatabases-0.1.3/setup.py
```

### Comparing `pydatabases-0.1.1/LICENSE` & `pydatabases-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.1/PKG-INFO` & `pydatabases-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.1
+Version: 0.1.3
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.1/pyDatabases/auxfuncs.py` & `pydatabases-0.1.3/pyDatabases/auxfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
 	def bc(x,y,fill_value = 0):
 		""" Broadcast domain of 'x' to conform with domain of 'y'. """
 		y, y_dom, x_dom = getIndex(y), getDomains(y), getDomains(x)
 		if y_dom:
 			if not x_dom:
 				return pd.Series(x, index = y)
 			elif set(x_dom).intersection(set(y_dom)):
-				return x.add(pd.Series(y, index = y), fill_value =fill_value) if (set(x_dom)-set(y_dom)) else pd.Series(0, index = y).add(x,fill_value=fill_value)
+				return x.add(pd.Series(0, index = y), fill_value =fill_value) if (set(x_dom)-set(y_dom)) else pd.Series(0, index = y).add(x,fill_value=fill_value)
 			else:
 				return pd.Series(0, index = cartesianProductIndex([getIndex(x),y])).add(x,fill_value=fill_value)
 		else:
 			return x
 
 	@staticmethod
 	def bcAdd(x,y,fill_value = 0):
@@ -318,20 +318,23 @@
 			else:
 				return pd.Series(0, index = cartesianProductIndex([getIndex(x),getIndex(y)])).add(x,fill_value=fill_value).add(y, fill_value=fill_value)
 		else:
 			return x+y
 
 	@staticmethod
 	def applyMultIdx(idx, mapping):
-		return pd.Series(0, index = idx).add(pd.Series(0, index = adj.rc_pd(mapping, idx))).dropna().index.reorder_levels(idx.names+[k for k in mapping.names if k not in idx.names])
+		if idx.empty:
+			return pd.MultiIndex.from_tuples([], names = idx.names+ [k for k in mapping.names if k not in idx.names])
+		else:
+			return pd.Series(0, index = idx).add(pd.Series(0, index = adj.rc_pd(mapping, idx))).dropna().index.reorder_levels(idx.names+[k for k in mapping.names if k not in idx.names])
 
 	@staticmethod
 	def applyMultSrs(s, mapping):
 		if s.empty:
-			return pd.Series([], index = pd.MultiIndex.from_tuples([], names = s.index.names + [k for k in mapping.names if k not in s.index.names]))
+			return pd.Series([], index = adjMultiIndex.applyMultIdx(s.index, mapping))
 		else:
 			return s.add(pd.Series(0, index = adj.rc_pd(mapping,s)))
 
 	@staticmethod
 	def applyMult(symbol, mapping):
 		return adjMultiIndex.applyMultIdx(symbol, mapping) if isinstance(symbol, pd.Index) else adjMultiIndex.applyMultSrs(symbol, mapping)
```

### Comparing `pydatabases-0.1.1/pyDatabases/gpyDB/database.py` & `pydatabases-0.1.3/pyDatabases/gpyDB/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from pyDatabases.auxfuncs import *
 import gams.transfer as gt, gams
 from gams.core.gmd import gmdcc
 from copy import deepcopy
 
 #global settings
 gmdTypeDict = {getattr(gmdcc,f'dt_{k}'): k for k in ('set','par','var','equ','alias')} # map from integer types in gmd database to string types
-default_attributes_variables = {k:i for k,i in zip(['level','marginal','lower','upper','scale'],range(-5,0))}
-default_attributes_parameters= {k:i for k,i in zip(['value'],range(-1,0))}
+default_attributes_variables = gt._internals.constants.VAR_DEFAULT_VALUES['free']
 # _numtypes = (int,float,np.generic)
 
 ### --------	1. Type inference	-------- ###
 def typePd(symbol, name = None, type = None, **kwargs):
 	""" Series are designated as variables per default. set type = 'par' to add as parameter. 
 		A set is defined as a 'subset' if symbol.name != name"""
-	if isinstance(symbol, pd.Series):
+	if isinstance(symbol, (pd.Series, pd.DataFrame)):
 		return type if type else 'var'
 	elif isinstance(symbol, pd.MultiIndex):
 		return 'map' if symbol.nlevels>1 else set_or_subset(symbol.name, name)
 	elif isinstance(symbol, pd.Index):
-		return set_or_subset(symbol.name, name)
+		return set_or_subset(symbol.name, noneInit(name, symbol.name))
 	else:
 		return 'scalarPar' if type in ('par', 'scalarPar') else 'scalarVar'
 
 def set_or_subset(s_name,name):
 	return 'set' if s_name == name else 'subset'
 
 def typeGms(symbol):
@@ -80,18 +79,26 @@
 			return None
 
 	@property
 	def domains(self):
 		return [] if self.index is None else self.index.names
 
 	@property
-	def df(self):
-		""" Only works if self.vals is a pandas series + type is either variable/parameter."""
-		return self.vals.to_frame(name='level' if self.type == 'var' else 'value')
+	def np(self):
+		return np.hstack([self.vals.values.reshape(len(self),1), 
+				np.vstack([np.full(len(self), v) for k,v in self.defaultAttrs.items() if k != 'level']).T])
+
+	@property
+	def defaultAttrs(self):
+		return default_attributes_variables
 
+	@property
+	def df(self):
+		""" Relevant for variable types"""
+		return pd.DataFrame(self.np, index = self.index, columns = default_attributes_variables.keys())
 
 ### --------	3. GAMS to pandas/gpy	-------- ###
 ### --------		3.1. Gmd to gpy		-------- ###
 class readGmd:
 	def __init__(self, db, g2np):
 		self.db = db
 		self.gmd = self.db._gmd
@@ -361,15 +368,15 @@
 		return idx.to_frame(index=False).values.astype(str).astype(object)
 	@staticmethod
 	def textVector(s):
 		""" Explanatory text accompanying index symbols; for now, pass empty vector with suitable shape."""
 		return np.full((len(s),1), '', dtype = 'object')
 	@staticmethod
 	def gpyVar2np(s):
-		return gmdFromGpy.gpyIdx2np(s.vals.index), np.vstack([s.vals.values]+[np.full(len(s), k) for k in list(gt._internals.constants.VAR_DEFAULT_VALUES['free'].values())[1:]]).T
+		return gmdFromGpy.gpyIdx2np(s.vals.index), s.np
 	@staticmethod
 	def gpyPar2np(s):
 		return gmdFromGpy.gpyIdx2np(s.vals.index), s.vals.values.reshape(len(s),1)
 	@staticmethod
 	def gpyScalarVar2np(s):
 		return np.empty((1,0), dtype =object), np.array([list((gt._internals.constants.VAR_DEFAULT_VALUES['free'] |{'level': s.vals}).values())])
 	@staticmethod
```

### Comparing `pydatabases-0.1.1/pyDatabases/gpyDB/gpyDB.py` & `pydatabases-0.1.3/pyDatabases/gpyDB/gpyDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,23 @@
 	###################################################################################################
 	def __init__(self, obj = None, ws = None, alias = None, **kwargs):
 		getattr(self, f'init_{obj.__class__.__name__}')(obj, ws = ws, **kwargs)
 		self.updateAlias(alias=alias)
 
 	def init_NoneType(self, noneObj, db = None, **kwargs):
 		getattr(self, f'initFromDb_{db.__class__.__name__}')(db, **kwargs)
-	def init_str(self, pickle_path, ws = None):
+	def init_str(self, pickle_path, ws = None, name = None):
 		with open(pickle_path, "rb") as file:
 			p = pickle.load(file)
+		if name:
+			p.name = name # update name
+		p.g2np = g2np_
+		if not os.path.exists(p.work_folder):
+			p.work_folder = os.getcwd()
+		p.database = None if 'database' in p.dropattrs else os.path.join(p.data_folder, f'{p.name}.gdx')
 		self.init_dict(p.__dict__, ws = noneInit(ws, p.work_folder))
 	def init_GpyDB(self, db, ws = None):
 		d = {k: v if k in dropattrs_ else deepcopy(v) for k,v in db.__dict__.items()} # copy all attributes
 		self.init_dict(d, ws = noneInit(ws, db.ws))
 
 	def init_dict(self, d, ws = None):
 		self.__dict__ = d
@@ -79,24 +85,25 @@
 		self.g2np = g2np_
 		self.data_folder = noneInit(data_folder, os.getcwd())
 		self.dropattrs = noneInit(dropattrs, dropattrs_.copy())
 		self.initDb(db)
 		self.series = SeriesDB(database = self.gmd())
 
 	@staticmethod
-	def initFast(name, series = None, data_folder = None, dropattrs = None):
+	def initFast(name = "db", series = None, data_folder = None, dropattrs = None, alias = None):
 		""" Initialize class without the gams related attributes """
 		class Empty:
 			def __init__(self): pass
 		obj = Empty()
 		obj.__class__ = GpyDB
 		obj.name = name
 		obj.data_folder = noneInit(data_folder, os.getcwd())
 		obj.dropattrs = noneInit(dropattrs, dropattrs_.copy())
 		obj.series = noneInit(series, SeriesDB())
+		obj.updateAlias(alias = alias)
 		return obj
 
 	def setWs(self, ws):
 		self.ws = self.initWs(ws)
 		self.work_folder = self.ws.working_directory
 	@staticmethod
 	def initWs(ws):
@@ -145,18 +152,14 @@
 		if 'database' not in self.dropattrs:
 			self.database.export(os.path.join(self.data_folder,self.name))
 		return {key: value for key,value in self.__dict__.items() if key not in (self.dropattrs+['database'])}
 
 	def __setstate__(self,dict_):
 		""" Don't include ws. Don't include db. """
 		self.__dict__ = dict_
-		self.g2np = g2np_
-		if not os.path.exists(self.work_folder):
-			self.work_folder = os.getcwd()
-		self.database = None if 'database' in self.dropattrs else os.path.join(self.data_folder, f'{self.name}.gdx')
 
 	def export(self,name=None,repo=None):
 		name = self.name if name is None else name
 		repo = self.data_folder if repo is None else repo
 		with open(os.path.join(repo,name), "wb") as file:
 			pickle.dump(self,file)
 
@@ -442,27 +445,27 @@
 		[db[vi].__setattr__('vals', AggDB.renameIdx(db(vi), k ,v)) for vi in db.varDom(k,types=['map'])[k]];
 		return db
 
 	def renameIdx(idx, k, v):
 		return idx.rename({k:v}) if isinstance(idx, pd.MultiIndex) else idx.rename(v)
 
 	# ----------------------- 3-4. Read sets/update sets from database  ------------------------- #
-	def updSetsFromSyms(db, types = None, clean = True, ignore_alias = False, clean_alias = False):
+	def updSetsFromSyms(db, types = None, clean = True, ignore_alias = True, clean_alias = False):
 		if clean:
 			AggDB.cleanSets(db)
 		AggDB.readSets(db ,types = types, ignore_alias=ignore_alias)
 		if clean_alias:
 			AggDB.cleanAliases(db, types)
 		AggDB.readAliasedSets(db, ignore_alias)
 		if clean:
 			AggDB.updateSubsetsFromSets(db)
 			AggDB.updateMapsFromSets(db)
 		return db
 
-	def readSets(db, types=None, ignore_alias=False):
+	def readSets(db, types=None, ignore_alias=True):
 		""" read and define set elements from all symbols of type 'types'. """
 		if ignore_alias:
 			[db.aom(gpy(symbol.index.get_level_values(setName).unique())) for symbol in db.getTypes(noneInit(types,['var','par'])).values() for setName in (set(symbol.domains)-db.alias_notin_db)];
 		else:
 			[db.aom(gpy(symbol.index.get_level_values(setName).unique())) for symbol in db.getTypes(noneInit(types,['var','par'])).values() for setName in set(symbol.domains)];
 
 	def cleanSets(db):
@@ -516,15 +519,15 @@
 	# ----------------------- 6. Methods for aggregating database ------------------------- #
 	def aggDB(db, mapping, aggBy=None, replaceWith=None, aggLike = None):
 		""" Aggregate symbols in db according to mapping. This does so inplace, i.e. the set aggBy is altered. 
 			Note: The aggregation assumes that mapping is 'one-to-many'; if this is not the case, a warning is printed (if checkUnique) """
 		aggBy,replaceWith = noneInit(aggBy, mapping.names[0]), noneInit(replaceWith,mapping.names[-1])
 		defaultAggLike = {k: {'func': 'Sum', 'kwargs': {}} for v,l in db.varDom(aggBy, types = ['var','par']).items() for k in l}
 		aggLike = defaultAggLike if aggLike is None else defaultAggLike | aggLike
-		[db.__setitem__(k, AggDB.aggDB_set(k, mapping, aggBy, replaceWith)) for k in db.varDom(aggBy,types=['set'])]; # this alters sets and potentially aliases if they are also defined in the database
+		[db.__setitem__(k, AggDB.aggDB_set(k, mapping, aggBy, replaceWith)) for k in set(db.aliasDict0[aggBy])-db.alias_notin_db]; # this alters sets and potentially aliases if they are also defined in the database
 		[db.__setitem__(vi, AggDB.aggDB_subset(db, vi, mapping.set_names(k,level=aggBy), k, replaceWith)) for k,v in db.varDom(aggBy, types=['subset']).items() for vi in v];
 		[db.__setitem__(vi, AggDB.aggDB_mapping(db, vi, mapping.set_names(k,level=aggBy), k, replaceWith)) for k,v in db.varDom(aggBy, types=['map']).items() for vi in v];
 		[db.__setitem__(vi, getattr(AggDB,f"aggVar{aggLike[vi]['func']}")(db(vi), mapping.set_names(k,level=aggBy),k,replaceWith,**aggLike[vi]['kwargs'])) for k,v in db.varDom(aggBy).items() for vi in v];
 		return db
 
 	def aggDB_set(k, mapping, aggBy, replaceWith):
 		return mapping.get_level_values(replaceWith).unique().rename(k)
```

### Comparing `pydatabases-0.1.1/pyDatabases/simpleDB/simpleDB.py` & `pydatabases-0.1.3/pyDatabases/simpleDB/simpleDB.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.1/pyDatabases.egg-info/PKG-INFO` & `pydatabases-0.1.3/pyDatabases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.1
+Version: 0.1.3
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.1/setup.py` & `pydatabases-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="pyDatabases",
-  version="0.1.1",
+  version="0.1.3",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Small collection of database classes based primarily pandas, secondarily scipy and GAMS.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/pyDatabases",
   packages=setuptools.find_packages(),
```

