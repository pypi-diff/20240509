# Comparing `tmp/reflex_wrapper-0.0.2.tar.gz` & `tmp/reflex_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_wrapper-0.0.2.tar", last modified: Thu May  2 19:00:57 2024, max compression
+gzip compressed data, was "reflex_wrapper-0.0.3.tar", last modified: Thu May  9 01:11:42 2024, max compression
```

## Comparing `reflex_wrapper-0.0.2.tar` & `reflex_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.2/LICENSE
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     3876 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3328 2024-05-02 15:35:19.000000 reflex_wrapper-0.0.2/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/reflex_wrapper/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       26 2024-05-02 13:04:35.000000 reflex_wrapper-0.0.2/reflex_wrapper/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    11393 2024-05-02 18:59:39.000000 reflex_wrapper-0.0.2/reflex_wrapper/rx_wrapper.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     3876 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-02 19:00:44.000000 reflex_wrapper-0.0.2/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.3/LICENSE
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3914 2024-05-09 01:04:21.000000 reflex_wrapper-0.0.3/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.935625 reflex_wrapper-0.0.3/reflex_wrapper/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       37 2024-05-09 01:11:03.000000 reflex_wrapper-0.0.3/reflex_wrapper/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    13887 2024-05-09 01:10:16.000000 reflex_wrapper-0.0.3/reflex_wrapper/rx_wrapper.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-09 00:52:53.000000 reflex_wrapper-0.0.3/setup.py
```

### Comparing `reflex_wrapper-0.0.2/LICENSE` & `reflex_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_wrapper-0.0.2/PKG-INFO` & `reflex_wrapper-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: reflex_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
 Home-page: https://github.com/B4PT0R/reflex_wrapper
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reflex>=0.4.8
 
 # reflex-wrapper
 
-`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate a state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
+`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
 This design choice, while being very elegant on a technical point of view for input validation and multi-session state management, also made the objet model less intuitive to a regular python developper, who expects to create 3 independant stateful components by instantiating the component class three times and that's it. To work around this, I created a custom Component class that abstracts away these pydantic state shenanigans and allows to use reflex components as normal instances of their Component subclass. 
 
-All standard reflex components are also automatically converted into Component objects so that you don't have to think about it and just focus on creating your app.
+All standard reflex objects accessed from the rx wrapper should be automatically converted into these Components, or into objects supporting them, so that you don't have to bother about any additional overhead introduced by the wrapper and just focus on creating your app.
+
+I'm rather new to Reflex, this small project is meant as an exercise and reflects my current (limited) understanding of the library. I may have neglected to cover some important functionalities. Feel free to check the source code and suggest improvements.
 
 ## Installation
 
 ```bash
 pip install reflex-wrapper
 ```
 
@@ -63,23 +65,27 @@
 # Notice also that state variables and event handlers can be accessed directly from self
 
 # Now we can reuse this component to create a page layout
 # No need to define counter=Counter.create, the Counter class can be instantiated directly into Component objects
 
 @rx.page() # Decorators still work
 def index():
-    cnt=Counter(count=10,background='blue') # we can intialize the count state value directly from props
-    cnt.count=5
-    cnt.background='green' # we can also edit via attribute style access after instantiation
-    btn1=rx.button("Click to add 2",on_click=cnt.set_count(cnt.count+2)) # we can use state setters like this
-    cnt2=Counter(count=cnt.twice_the_count) # we can link a second counter's state to some state var of the first, thus synchronizing the second counter. 
+    cnt1=Counter(count=10,background='blue') # we can intialize the count state value directly from props
+    cnt2=Counter()
+    cnt2.count=5
+    cnt2.background='green' # we can also edit via attribute style access after instantiation
+    btn1=rx.button("Click to add 2 to the first counter",on_click=cnt1.set_count(cnt1.count+2)) # state variables / methods / setters can be accessed directly from the component instance
+    cnt3=Counter(count=cnt1.twice_the_count) # we can enforce cnt3's count to echo some (computed) state var of cnt1. (methods modifying cnt3's count will have no visible effect anymore)
+    lbl1=rx.text(cnt3.count) # will show cnt1.twice_the_count 
     box=rx.box(
-        cnt,
-        cnt2
-        btn1,
+        cnt1,
+        cnt2,
+        cnt3,
+        lbl1,
+        btn1
     )
     return box
 
 app=rx.App()
 ```
 
 ## License
```

### Comparing `reflex_wrapper-0.0.2/reflex_wrapper/rx_wrapper.py` & `reflex_wrapper-0.0.3/reflex_wrapper/rx_wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Module used as a wrapper around the reflex library to ease custom components creation.
 Defines a generic Component class that automates State init boilerplate and provides a more user-friendly interface to interact with components
 """
 
 import reflex
 from functools import wraps
 from copy import copy
+import uuid
 
 def get_class_dict(cls,excluded=()):
     """
     Returns a dict representing a given class, excluding chosen attributes
     """
     class_dict = {
         '__name__': cls.__name__,
@@ -52,14 +53,67 @@
         if isinstance(obj,Component):
             return obj._render()
         elif isinstance(obj,reflex.Component):
             return obj
         else:
             raise TypeError(f"{obj} should be a component object")
 
+
+def use_state(default,vartype=None):
+    """
+    Creates a state with a single var 'value' set to default and returns the corresponding state var and setter
+    """
+    vartype=vartype or type(default)
+    attributes={
+        'value':default,
+        '__annotations__':{'value':vartype}
+    }
+    cls_name="State_"+str(uuid.uuid4())
+    state=type(cls_name,(reflex.State,),attributes)
+    state_var=state.value
+    state_setter=state.set_value
+    return state_var,state_setter
+
+class StateWrapper:
+
+    """
+    Class acting as a reflex.State proxy, allowing to pass reflex (computed) vars as default values for other state variables.
+    Meant to achieve staightforward state synchronization between components with a priori independent states.
+    """
+
+    def __init__(self,state):
+        self.state=state
+        self.dict=dict()
+
+    def __getattr__(self,attr):
+        if attr in self.dict:
+            return self.dict[attr]
+        else:
+            return getattr(self.state,attr)
+    
+    def __setattr__(self,attr,value):
+        if attr in ['state','dict']:
+            super().__setattr__(attr,value)
+        else:
+            if isinstance(value,reflex.Var):
+                self.dict[attr]=value
+            else:
+                setattr(self.state,attr,value)
+
+    def __delattr__(self,attr):
+        if attr in ['state','dict']:
+            super().__delattr__(attr)
+        else:
+            if attr in self.dict:
+                del self.dict[attr]
+            else:
+                delattr(self.state,attr)
+
+
+
 class Component:
 
     _excluded=(
         '_excluded',
         '_state_model',
         '_state_attrs',
         '_constructor',
@@ -108,15 +162,15 @@
         cls._state_model._instance_count += 1
         instance_state_cls_name = f"{cls._state_model.__name__}_n{cls._state_model._instance_count}"
         instance_state_class = type(instance_state_cls_name, (cls._state_model, reflex.State), {})
         return instance_state_class
     
     def _is_state_attr(self,attr):
         """
-        Checks whether an attr is a state attr
+        Checks whether an attr is a user-defined state attr
         """
         if self.state is None:
             return False
         else:
             return attr in self.__class__._state_attrs
         
     def _is_state_variable(self,attr):
@@ -127,102 +181,106 @@
     
     def _is_state_setter(self,attr):
         """
         Checks whether an attr is a state variable setter
         """
         return attr.startswith('set_') and self._is_state_variable(attr[4:])
     
+    def _is_state(self,attr):
+        """
+        Check whether an attr is a valid state attr
+        """
+        return self._is_state_attr(attr) or self._is_state_setter(attr)
+    
     def _set_default(self,key,value):
         """
         Sets the default value of a state variable
         """
         self.state.__fields__[key].default=value
 
-    def _set_defaults_from_props(self,props):
+    def _set_defaults_from_props(self):
         """
         Sets defaults for state variables from props passed to the component
         Skip if the prop already refers to another state variable (possibly from another component) 
         """
-        for key in list(props.keys()):
+        for key,value in self.props.items():
             if self._is_state_variable(key):
-                value=props.pop(key)
-                if not isinstance(value,reflex.Var):
+                if isinstance(value,(reflex.Var,reflex.vars.ComputedVar)):
+                    setattr(self.state,key,value)
+                else:
                     self._set_default(key,value)
-        return props
+                    
+    def _get_reflex_props(self):
+        """
+        filters out state variables from props before passing them to the reflex constructor
+        """
+        return {k:v for k,v in self.props.items() if not self._is_state(k)}
     
     def get_component(self,*childen,**props):
         """
         This method should be overriden when defining a custom component class
         """
         raise NotImplementedError("Custom components must implement a get_component method.")
 
     def _create(self,*children,**props):
         """
         Returns the corresponding reflex.Component instance and attach the state to it
         """
-        props=self._set_defaults_from_props(props)
         component=auto_render(self.get_component)(*children,**props)
-        component.State=self.state
+        #component.State=self.state
         return component
     
     def _initialize(self):
         """
         Initializes the reflex.Component constructor:
         If none is specified at class level, this is a custom component so we initialize its state and constructor accordingly
         If one is already specified at class level, this is a default component, so we use its constructor directly.
         """
         if self.__class__._constructor is None:
-            self.state=self.__class__._get_instance_state_class()
+            self.state=StateWrapper(self.__class__._get_instance_state_class())
             self.constructor=self._create
         else:
             self.constructor=self.__class__._constructor
 
     def __init__(self,*children,**props):
         self.parent=None
-        self.component=None
         self.state=None
         self.constructor=None
         self._initialize()
         self.props = dict(**props)
+        # the 'children' prop, if any, gets precedence over children passed as nested args (similar to React)
         children=self.props.get('children') or children
         for child in children:
             if isinstance(child,Component):
                 child.parent=self
         self.props['children']=children
+        self._set_defaults_from_props()
 
     def __getattr__(self,key):
         """
         Delegate attribute access to state / props
-        Any state variable (reflex.Var) passed as state prop takes precedence over local state variables.
         """
-        if self._is_state_variable(key):
-            if key in self.props:
-                value=self.props[key]
-                if isinstance(value,reflex.Var):
-                    return value
-                else:
-                    return getattr(self.state,key)
-            else:
-                return getattr(self.state,key)
-        elif self._is_state_setter(key) or self._is_state_attr(key):
+        if self._is_state(key):
             return getattr(self.state,key)
         elif key in self.props:
             return self.props[key]
         else:
             raise AttributeError(f"Invalid attribute key: '{key}'")
         
     def __setattr__(self,key,value):
         """
         Delegate attribute setting to state / props
         """
         if key in ['parent','constructor','component','state','props']:
             super().__setattr__(key,value)
         elif self._is_state_variable(key):
-            if not isinstance(value,reflex.Var):
+            if not isinstance(value,(reflex.Var,reflex.vars.ComputedVar)):
                 self._set_default(key,value)
+            else:
+                setattr(self.state,key,value)
             self.props[key]=value
         elif self._is_state_setter(key) or self._is_state_attr(key):
             raise AttributeError("Cannot override a state method.")
         else:
             self.props[key]=value
 
     def _render(self):
@@ -236,15 +294,15 @@
         for child in self.props['children']:
             if isinstance(child,Component):
                 child=child._render()
             rendered_children.append(child)
 
         # Then render the props
         props={}
-        for key,prop in self.props.items():
+        for key,prop in self._get_reflex_props().items():
             if not key=='children':
                 if isinstance(prop,Component):
                     prop=prop._render()
                 props[key]=prop
         
         # Render the component by calling the constructor
         self.component=self.constructor(*rendered_children,**props)
@@ -265,69 +323,100 @@
 
     def __init__(self,*args,**kwargs):
         reflex.App.__init__(self,*args,**kwargs)
 
     def add_page(self,component,*args,**kwargs):
         super().add_page(auto_render(component),*args,**kwargs)
 
+def capitalize(string):
+    if len(string)>0:
+        return string[0].upper()+string[1:]
+    else:
+        return ""
+
+def resolve_attr_chain(chain):
+    obj=reflex
+    path='reflex'
+    for attr in chain:
+        if hasattr(obj,attr):
+            path+=f'.{attr}'
+            obj=getattr(obj,attr)
+        else:
+            raise AttributeError(f"{path} has no attribute '{attr}'.")
+    return obj
+
+def chain_as_path(chain):
+    return 'reflex.'+'.'.join(chain)
+
+def chain_as_name(chain):
+    return ''.join(capitalize(name) for name in chain)
 
 class rx_submodule:
-    
-    _dict = {}
 
-    def __init__(self, submodule_name):
-        self.submodule_name = submodule_name
-        try:
-            self.module = getattr(reflex, submodule_name)
-        except AttributeError:
-            raise ImportError(f"The submodule {submodule_name} could not be found in the reflex library.")
+    """
+    Class representing a reflex submodule, to implement attribute chain lookup from the rx class.
+    Does the routing to the appropriate component/object/submodule
+    """
+
+    def __init__(self,chain):
+        self.chain=chain
+        self.path=chain_as_path(self.chain)
+        self.obj=resolve_attr_chain(self.chain)
 
     def __getattr__(self, key):
-        full_key = f"{self.submodule_name.capitalize()}{key.capitalize()}"
-        if full_key in rx_submodule._dict:
-            return rx_submodule._dict[full_key]
-        else:
-            try:
-                attr = getattr(self.module, key)
-                new_cls = get_builtin_component(name=full_key, constructor=attr)
-                rx_submodule._dict[full_key] = new_cls
-                return new_cls
-            except AttributeError:
-                raise AttributeError(f"No component named {key} in the {self.submodule_name} submodule.")
+        chain=self.chain+[key]
+        path=chain_as_path(chain)
+        if path in rx._dict:
+            return rx._dict[path]
+        elif hasattr(self.obj,key) and callable(getattr(self.obj,key)):
+            name=chain_as_name(chain)
+            new_cls=get_builtin_component(name=name,constructor=getattr(self.obj,key))
+            rx._dict[path]=new_cls
+            return new_cls
+        elif hasattr(self.obj,key):
+            return rx_submodule(chain)
+        else:
+            raise AttributeError(f"{self.path} has no attribute named {key}.")
 
 
 class rx_meta(type):
 
     """
-    Meta class to override __getattr__ in the RX class
-    Does the routing to the appropriate object
+    Metaclass to override __getattr__ in the rx class
+    Does the routing to the appropriate component/object/submodule
     """
 
     def __getattr__(cls, key):
         if key in cls._reserved:
             return getattr(reflex,key)
-        elif key in cls._submodules:
-            return rx_submodule(key)
         elif key in globals():
             return globals()[key]
-        elif key in cls._dict:
-            return cls._dict[key]
-        elif hasattr(reflex,key):
-            new_cls=get_builtin_component(name=key.capitalize(),constructor=getattr(reflex,key))
-            cls._dict[key]=new_cls
+        
+        chain=[key]
+        path=chain_as_path(chain)
+
+        if path in rx._dict:
+            return rx._dict[path]
+        elif hasattr(reflex,key) and callable(getattr(reflex,key)):
+            name=chain_as_name(chain)
+            new_cls=get_builtin_component(name=name,constructor=getattr(reflex,key))
+            rx._dict[path]=new_cls
             return new_cls
+        elif hasattr(reflex,key):
+            return rx_submodule(chain)
         else:
-            raise AttributeError(f"No reflex component named {key}.")
+            raise AttributeError(f"reflex has no attribute named {key}.")
+
 
 class rx(metaclass=rx_meta):
     """
     Class used as a replacement of the reflex module, supporting Components objects
+    (its __getattr__ is implemented by the metaclass defined above)
     """
-    _reserved=['page','var','cached_var','Base','State','theme','theme_panel','Var']
-    _submodules=['chakra']
+    _reserved=['page','var','cached_var','Base','State','theme','theme_panel','Var','Config']
     _dict=dict()
```

### Comparing `reflex_wrapper-0.0.2/reflex_wrapper.egg-info/PKG-INFO` & `reflex_wrapper-0.0.3/reflex_wrapper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: reflex_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
 Home-page: https://github.com/B4PT0R/reflex_wrapper
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reflex>=0.4.8
 
 # reflex-wrapper
 
-`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate a state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
+`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
 This design choice, while being very elegant on a technical point of view for input validation and multi-session state management, also made the objet model less intuitive to a regular python developper, who expects to create 3 independant stateful components by instantiating the component class three times and that's it. To work around this, I created a custom Component class that abstracts away these pydantic state shenanigans and allows to use reflex components as normal instances of their Component subclass. 
 
-All standard reflex components are also automatically converted into Component objects so that you don't have to think about it and just focus on creating your app.
+All standard reflex objects accessed from the rx wrapper should be automatically converted into these Components, or into objects supporting them, so that you don't have to bother about any additional overhead introduced by the wrapper and just focus on creating your app.
+
+I'm rather new to Reflex, this small project is meant as an exercise and reflects my current (limited) understanding of the library. I may have neglected to cover some important functionalities. Feel free to check the source code and suggest improvements.
 
 ## Installation
 
 ```bash
 pip install reflex-wrapper
 ```
 
@@ -63,23 +65,27 @@
 # Notice also that state variables and event handlers can be accessed directly from self
 
 # Now we can reuse this component to create a page layout
 # No need to define counter=Counter.create, the Counter class can be instantiated directly into Component objects
 
 @rx.page() # Decorators still work
 def index():
-    cnt=Counter(count=10,background='blue') # we can intialize the count state value directly from props
-    cnt.count=5
-    cnt.background='green' # we can also edit via attribute style access after instantiation
-    btn1=rx.button("Click to add 2",on_click=cnt.set_count(cnt.count+2)) # we can use state setters like this
-    cnt2=Counter(count=cnt.twice_the_count) # we can link a second counter's state to some state var of the first, thus synchronizing the second counter. 
+    cnt1=Counter(count=10,background='blue') # we can intialize the count state value directly from props
+    cnt2=Counter()
+    cnt2.count=5
+    cnt2.background='green' # we can also edit via attribute style access after instantiation
+    btn1=rx.button("Click to add 2 to the first counter",on_click=cnt1.set_count(cnt1.count+2)) # state variables / methods / setters can be accessed directly from the component instance
+    cnt3=Counter(count=cnt1.twice_the_count) # we can enforce cnt3's count to echo some (computed) state var of cnt1. (methods modifying cnt3's count will have no visible effect anymore)
+    lbl1=rx.text(cnt3.count) # will show cnt1.twice_the_count 
     box=rx.box(
-        cnt,
-        cnt2
-        btn1,
+        cnt1,
+        cnt2,
+        cnt3,
+        lbl1,
+        btn1
     )
     return box
 
 app=rx.App()
 ```
 
 ## License
```

### Comparing `reflex_wrapper-0.0.2/setup.py` & `reflex_wrapper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reflex_wrapper",
-    version="0.0.2",
+    version="0.0.3",
     author="Baptiste Ferrand",
     author_email="bferrand.maths@gmail.com",
     description="A custom wrapper on top of the reflex library to ease creating and interacting with custom components.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/B4PT0R/reflex_wrapper",
     packages=setuptools.find_packages(),
```

