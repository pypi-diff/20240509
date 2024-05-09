# Comparing `tmp/django_includecontents-0.7.tar.gz` & `tmp/django_includecontents-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.7.tar", last modified: Wed May  1 05:06:06 2024, max compression
+gzip compressed data, was "django_includecontents-0.8.tar", last modified: Thu May  9 01:06:34 2024, max compression
```

## Comparing `django_includecontents-0.7.tar` & `django_includecontents-0.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     7760 2024-05-01 04:48:00.043238 django_includecontents-0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.7/includecontents/backend.py
--rw-r--r--   0        0        0     4779 2024-05-01 04:41:54.339196 django_includecontents-0.7/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.7/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    16458 2024-05-01 04:47:18.123159 django_includecontents-0.7/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1217 2024-05-01 05:06:06.539571 django_includecontents-0.7/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.7/tests/settings.py
--rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.7/tests/templates/components/card-extend.html
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.7/tests/templates/components/card.html
--rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.7/tests/templates/components/empty-props.html
--rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-0.7/tests/templates/components/escape-props.html
--rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-0.7/tests/templates/components/nested-attrs.html
--rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-0.7/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.7/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-05-01 00:06:23.461690 django_includecontents-0.7/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.7/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.7/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-0.7/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.7/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.7/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.7/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     3371 2024-05-01 04:40:17.229002 django_includecontents-0.7/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.7/tests/test_multiline.py
--rw-r--r--   0        0        0      924 2024-05-01 00:43:10.666578 django_includecontents-0.7/tests/test_tag.py
--rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 django_includecontents-0.7/PKG-INFO
+-rw-r--r--   0        0        0     7916 2024-05-09 01:00:54.828956 django_includecontents-0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.8/includecontents/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.8/includecontents/backend.py
+-rw-r--r--   0        0        0     4797 2024-05-09 01:00:11.649227 django_includecontents-0.8/includecontents/base.py
+-rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.8/includecontents/engine.py
+-rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.8/includecontents/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.8/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    16658 2024-05-08 23:15:15.339619 django_includecontents-0.8/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1236 2024-05-09 01:06:34.370901 django_includecontents-0.8/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.8/tests/settings.py
+-rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.8/tests/templates/components/card-extend.html
+-rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.8/tests/templates/components/card.html
+-rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.8/tests/templates/components/empty-props.html
+-rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-0.8/tests/templates/components/escape-props.html
+-rw-r--r--   0        0        0        5 2024-05-02 20:42:55.088146 django_includecontents-0.8/tests/templates/components/inside/cat.html
+-rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-0.8/tests/templates/components/nested-attrs.html
+-rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-0.8/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.8/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-05-01 00:06:23.461690 django_includecontents-0.8/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.8/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.8/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-0.8/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.8/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.8/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.8/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     3814 2024-05-09 01:02:34.898421 django_includecontents-0.8/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.8/tests/test_multiline.py
+-rw-r--r--   0        0        0      924 2024-05-01 00:43:10.666578 django_includecontents-0.8/tests/test_tag.py
+-rw-r--r--   0        0        0     8973 1970-01-01 00:00:00.000000 django_includecontents-0.8/PKG-INFO
```

### Comparing `django_includecontents-0.7/README.md` & `django_includecontents-0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,20 @@
 
 ```html
 <include:my-card title="Hello">
   <p>World</p>
 </include:my-card>
 ```
 
+You can use directories within `components` to group your components. For example, `components/forms/field.html`:
+
+```html
+<include:forms:field ... />
+```
+
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
 Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
 <include:my-card title={mytitle} />
 ```
```

### Comparing `django_includecontents-0.7/includecontents/backend.py` & `django_includecontents-0.8/includecontents/backend.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.7/includecontents/base.py` & `django_includecontents-0.8/includecontents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 if group := re.match(r"([-:.\w]+)=\{(.+)\}", attr):
                     attr = f"{group[1]}={group[2]}"
                 attrs.append(attr)
             # Build the includecontents tag
             content = [
                 "includecontents",
                 f"_{tag_name}{'/' if self_closing else ''}",
-                f'"components/{tag_name[8:]}.html"',
+                f'"components/{tag_name[8:].replace(":", "/")}.html"',
             ]
             if attrs:
                 content.append("with")
                 content.extend(attrs)
             return django.template.base.Token(
                 django.template.base.TokenType.BLOCK,
                 " ".join(content),
```

### Comparing `django_includecontents-0.7/includecontents/engine.py` & `django_includecontents-0.8/includecontents/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.7/includecontents/loaders.py` & `django_includecontents-0.8/includecontents/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.7/includecontents/templatetags/includecontents.py` & `django_includecontents-0.8/includecontents/templatetags/includecontents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from collections import abc
 from collections.abc import MutableMapping
+from contextlib import contextmanager
 from typing import Any
 
 from django import template
 from django.template import TemplateSyntaxError, Variable
 from django.template.base import FilterExpression, NodeList, Parser, TokenType
 from django.template.context import Context
 from django.template.loader_tags import IncludeNode, construct_relative_path, do_include
@@ -102,25 +103,21 @@
     if len(bits) < 2:
         raise TemplateSyntaxError(
             f"{token_name} tag takes at least one argument: the name of the template"
         )
     nodelist, named_nodelists = get_contents_nodelists(parser, token_name)
     include_node = do_include(parser, token)
     include_node.origin = parser.origin
-    isolated_context = (
-        False if token_name.startswith("<") else include_node.isolated_context
-    )
-    include_node.isolated_context = False
+
     return IncludeContentsNode(
         token_name=token_name,
         nested_attrs=advanced_attrs,
         include_node=include_node,
         nodelist=nodelist,
         named_nodelists=named_nodelists,
-        isolated_context=isolated_context,
     )
 
 
 class RenderedContents(abc.Mapping):
     def __init__(
         self, context: Context, nodelist: NodeList, named_nodelists: dict[str, NodeList]
     ):
@@ -154,65 +151,70 @@
     def __init__(
         self,
         token_name,
         nested_attrs,
         include_node,
         nodelist,
         named_nodelists,
-        isolated_context,
     ):
         self.token_name = token_name
         self.nested_attrs = nested_attrs
         self.include_node = include_node
         self.nodelist = nodelist
         self.named_nodelists = named_nodelists
+
+        self.is_component = token_name.startswith("<")
+
+        # We'll handle the include_node context isolation ourselves.
+        isolated_context = True if self.is_component else include_node.isolated_context
+        include_node.isolated_context = False
         self.isolated_context = isolated_context
 
     def render(self, context):
         new_context = context.new() if self.isolated_context else context
         with new_context.push():
             new_context["contents"] = RenderedContents(
                 # Contents aren't rendered with isolation, hence the use of context
                 # rather than new_context.
                 context,
                 nodelist=self.nodelist,
                 named_nodelists=self.named_nodelists,
             )
-            if self.set_component_attrs(context, new_context):
-                # Don't use the extra context for the include tag if it's a component
-                # with defined props.
-                node = IncludeNode(self.include_node.template)
-                node.origin = self.origin
-                rendered = node.render(new_context)
-            else:
+            with self.set_component_attrs(context, new_context):
                 rendered = self.include_node.render(new_context)
-            if self.token_name.startswith("<"):
+            if self.is_component:
                 rendered = rendered.strip()
         return rendered
 
+    @contextmanager
     def set_component_attrs(self, context: Context, new_context: Context):
         """
         Set the attributes of the component tag in the new context.
+
+        Use as a context manager around rendering the
         """
-        if not self.token_name.startswith("<"):
-            return False
-        template = self.get_template(context)
+        if not self.is_component:
+            yield
+            return
+        template = self.get_component_template(context)
         if not template.first_comment:
-            return False
+            yield
+            return
         if (
             template.first_comment.startswith("props ")
             or template.first_comment == "props"
         ):
             first_comment = template.first_comment[6:]
         elif (
             template.first_comment.startswith("def ") or template.first_comment == "def"
         ):
             first_comment = template.first_comment[4:]
         else:
-            return False
+            yield
+            return
         used_attrs = self.include_node.extra_context or {}
         defined_attrs = []
         for bit in smart_split(first_comment.strip()):
             if match := re.match(r"^(\w+)(?:=(.+?))?,?$", bit):
                 attr, value = match.groups()
                 defined_attrs.append(attr)
                 if attr not in used_attrs:
@@ -227,32 +229,38 @@
             if key not in defined_attrs:
                 attrs[key] = value.resolve(context)
             else:
                 new_context[key] = value.resolve(context)
         for key, value in self.nested_attrs.items():
             attrs[key] = value.resolve(context)
         new_context["attrs"] = attrs
-        return True
 
-    def get_template(self, context) -> Template:
+        # Don't use the extra context for the include tag if it's a component
+        # with defined props.
+        extra_context = self.include_node.extra_context
+        yield
+        self.include_node.extra_context = extra_context
+
+    def get_component_template(self, context) -> Template:
         template = self.include_node.template.resolve(context)
         # Does this quack like a Template?
         if not callable(getattr(template, "render", None)):
             # If not, try the cache and select_template().
             template_name = template or ()
             if isinstance(template_name, str):
                 template_name = (
                     construct_relative_path(
                         self.origin.template_name,  # type: ignore
                         template_name,
                     ),
                 )
             else:
                 template_name = tuple(template_name)
-            cache = context.render_context.dicts[0].setdefault(self, {})
+            # Use the same cache as the include node to avoid duplicate template loads.
+            cache = context.render_context.dicts[0].setdefault(self.include_node, {})
             template = cache.get(template_name)
             if template is None:
                 template = context.template.engine.select_template(template_name)
                 cache[template_name] = template
         # Use the base.Template of a backends.django.Template.
         elif hasattr(template, "template"):
             template = template.template
```

### Comparing `django_includecontents-0.7/pyproject.toml` & `django_includecontents-0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.7"
+version = "0.8"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
@@ -31,14 +31,15 @@
 [project.urls]
 Repository = "https://github.com/SmileyChris/django-includecontents"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-django",
+    "pytest-mock",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `django_includecontents-0.7/tests/test_component.py` & `django_includecontents-0.8/tests/test_component.py`

 * *Files 14% similar despite different names*

```diff
@@ -136,7 +136,26 @@
 
 
 def test_escape_variables():
     output = Template(
         """<include:escape-props test=somevar another="3>2"></include:escape-props>"""
     ).render(Context({"somevar": '2>1"'}))
     assert output == 'test="2&gt;1&quot;" another="3>2"'
+
+
+def test_subdir():
+    output = Template("<include:inside:cat />").render(Context())
+    assert output == "Meow"
+
+
+def test_template_caching(mocker):
+    template = Template("""
+{% for i in '12345'|make_list %}
+    <include:empty-props i={i} />
+{% endfor %}
+""")
+    context = Context()
+    context.bind_template(template)
+    spy = mocker.spy(template.engine, "select_template")
+
+    template.render(context)
+    assert spy.call_count == 1
```

### Comparing `django_includecontents-0.7/tests/test_tag.py` & `django_includecontents-0.8/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.7/PKG-INFO` & `django_includecontents-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.7
+Version: 0.8
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/SmileyChris/django-includecontents
 Requires-Python: >=3.8
 Requires-Dist: django
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-django; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Django IncludeContents tag
 
 Provides a component-like `{% includecontents %}` tag to Django.
 
@@ -155,14 +156,20 @@
 
 ```html
 <include:my-card title="Hello">
   <p>World</p>
 </include:my-card>
 ```
 
+You can use directories within `components` to group your components. For example, `components/forms/field.html`:
+
+```html
+<include:forms:field ... />
+```
+
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
 Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
 <include:my-card title={mytitle} />
 ```
```

