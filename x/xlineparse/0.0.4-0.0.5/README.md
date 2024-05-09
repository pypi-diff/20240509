# Comparing `tmp/xlineparse-0.0.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip` & `tmp/xlineparse-0.0.5-cp311-cp311-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 645353 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse-0.0.4.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse.libs/
--rw-r--r--  2.0 unx        0 b- defN 24-May-08 16:46 xlineparse/py.typed
--rw-r--r--  2.0 unx     7641 b- defN 24-May-08 16:46 xlineparse/__init__.py
--rwxr-xr-x  2.0 unx  2324012 b- defN 24-May-08 16:46 xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse-0.0.4.dist-info/license_files/
--rw-r--r--  2.0 unx     2674 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx      690 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/RECORD
--rw-r--r--  2.0 unx       49 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      212 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx     1071 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/license_files/LICENSE
-12 files, 2336349 bytes uncompressed, 643663 bytes compressed:  72.5%
+Zip file size: 488073 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 16:32 xlineparse/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 16:32 xlineparse-0.0.5.dist-info/
+-rw-r--r--  2.0 unx     8439 b- defN 24-May-09 16:32 xlineparse/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 16:32 xlineparse/py.typed
+-rwxr-xr-x  2.0 unx  1993680 b- defN 24-May-09 16:32 xlineparse/xlineparse.cpython-311-darwin.so
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 16:32 xlineparse-0.0.5.dist-info/license_files/
+-rw-r--r--  2.0 unx      682 b- defN 24-May-09 16:32 xlineparse-0.0.5.dist-info/RECORD
+-rw-r--r--  2.0 unx      104 b- defN 24-May-09 16:32 xlineparse-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-09 16:32 xlineparse-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     2706 b- defN 24-May-09 16:32 xlineparse-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-09 16:32 xlineparse-0.0.5.dist-info/license_files/LICENSE
+11 files, 2006731 bytes uncompressed, 486507 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: xlineparse/
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/
+Filename: xlineparse-0.0.5.dist-info/
 Comment: 
 
-Filename: xlineparse.libs/
+Filename: xlineparse/__init__.py
 Comment: 
 
 Filename: xlineparse/py.typed
 Comment: 
 
-Filename: xlineparse/__init__.py
-Comment: 
-
-Filename: xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
+Filename: xlineparse/xlineparse.cpython-311-darwin.so
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/license_files/
+Filename: xlineparse-0.0.5.dist-info/license_files/
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/METADATA
+Filename: xlineparse-0.0.5.dist-info/RECORD
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/RECORD
+Filename: xlineparse-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/entry_points.txt
+Filename: xlineparse-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/WHEEL
+Filename: xlineparse-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xlineparse-0.0.4.dist-info/license_files/LICENSE
+Filename: xlineparse-0.0.5.dist-info/license_files/LICENSE
 Comment: 
 
 Zip file comment:
```

## xlineparse/__init__.py

```diff
@@ -31,18 +31,14 @@
 @dataclass(frozen=True, kw_only=True)
 class StrEnumField:
     required: bool = True
     cls: type[enum.Enum]
 
     def as_dict(self) -> dict[str, Any]:
         values = {field.value for field in self.cls}
-        if not all(isinstance(v, str) for v in values):
-            raise NotImplementedError(
-                f"Can't convert {self.cls} as all the values are not strings"
-            )
         return dict(
             kind="STR_ENUM",
             required=self.required,
             values=sorted(values),
         )
 
 
@@ -58,50 +54,70 @@
             required=self.required,
             min_value=self.min_value,
             max_value=self.max_value,
         )
 
 
 @dataclass(frozen=True, kw_only=True)
+class IntEnumField:
+    required: bool = True
+    cls: type[enum.Enum]
+
+    def as_dict(self) -> dict[str, Any]:
+        values = {field.value for field in self.cls}
+        return dict(
+            kind="INT_ENUM",
+            required=self.required,
+            values=sorted(values),
+        )
+
+
+@dataclass(frozen=True, kw_only=True)
 class FloatField:
     required: bool = True
     min_value: float | None = None
     max_value: float | None = None
 
     def as_dict(self) -> dict[str, Any]:
         return dict(
             kind="FLOAT",
             required=self.required,
             min_value=self.min_value,
             max_value=self.max_value,
         )
 
 
+def decimal_to_str(d: decimal.Decimal | None) -> str | None:
+    if d is None:
+        return None
+    return f"{d:f}"
+
+
 @dataclass(frozen=True, kw_only=True)
 class DecimalField:
     required: bool = True
-    max_decimal_places: int | None = None
+    round_decimal_places: int | None = None
     min_value: decimal.Decimal | None = None
     max_value: decimal.Decimal | None = None
 
     def as_dict(self) -> dict[str, Any]:
         return dict(
             kind="DECIMAL",
             required=self.required,
-            max_decimal_places=self.max_decimal_places,
-            min_value=None if self.min_value is None else str(self.min_value),
-            max_value=None if self.max_value is None else str(self.max_value),
+            round_decimal_places=self.round_decimal_places,
+            min_value=decimal_to_str(self.min_value),
+            max_value=decimal_to_str(self.max_value),
         )
 
 
 @dataclass(frozen=True, kw_only=True)
 class BoolField:
     required: bool = True
     true_value: str
-    false_value: str  # can only be "" if .required
+    false_value: str | None  # can only be "" if .required
 
     def as_dict(self) -> dict[str, Any]:
         return dict(
             kind="BOOL",
             required=self.required,
             true_value=self.true_value,
             false_value=self.false_value,
@@ -149,14 +165,15 @@
         )
 
 
 Field = (
     StrField
     | StrEnumField
     | IntField
+    | IntEnumField
     | FloatField
     | DecimalField
     | BoolField
     | DatetimeField
     | DateField
     | TimeField
 )
@@ -169,25 +186,35 @@
         t, field = get_args(t)
     if get_origin(t) is Union or get_origin(t) is UnionType:
         args = set(get_args(t))
         assert len(args) == 2
         args -= {None, NoneType}
         (t,) = args
         required = False
+    # Once more in case the Union was nested
+    if get_origin(t) is Annotated:
+        t, field = get_args(t)
 
     if t is str and field is None:
         field = StrField()
     elif t is int and field is None:
         field = IntField()
     elif t is float and field is None:
         field = FloatField()
     elif t is decimal.Decimal and field is None:
         field = DecimalField()
     elif issubclass(t, enum.Enum) and field is None:
-        field = StrEnumField(cls=t)
+        if all(isinstance(v.value, str) for v in t):
+            field = StrEnumField(cls=t)
+        elif all(isinstance(v.value, int) for v in t):
+            field = IntEnumField(cls=t)
+        else:
+            raise NotImplementedError(
+                f"Can't convert {t} as all the values are not strings|ints"
+            )
 
     if field is None:
         raise RuntimeError(f"Type {t} needs Annotated[x, XField(...)]")
 
     field = replace(field, required=required)
     return field
 
@@ -229,18 +256,20 @@
             delimiter=self.delimiter,
             quote_str=self.quote_str,
             trailing_delimiter=self.trailing_delimiter,
             lines=[line.as_dict() for line in self.lines],
         )
         self._parser = _xlineparse.Parser(json.dumps(jsonable))
         # Set up enum conversion map, maybe there's a more efficient way of doing this..
-        self._enum_conversions: dict[str, dict[int, StrEnumField]] = defaultdict(dict)
+        self._enum_conversions: dict[str, dict[int, StrEnumField | IntEnumField]] = (
+            defaultdict(dict)
+        )
         for line in self.lines:
             for i, field in enumerate(line.fields, start=1):
-                if isinstance(field, StrEnumField):
+                if isinstance(field, (StrEnumField, IntEnumField)):
                     self._enum_conversions[line.name][i] = field
 
     @staticmethod
     def from_type(
         delimiter: str,
         quote_str: str | None,  # do we quote strings like "foo"
         trailing_delimiter: bool,
@@ -257,18 +286,21 @@
             lines=lines,
         )
 
     def parse_line(self, line: str) -> tuple[Any, ...]:
         try:
             parsed = self._parser.parse_line(line)
         except ValueError as e:
+            line = line.rstrip("\n")
             raise LineParseError(f"Failed to parse line: '{line}'\n {e.args[0]}")
         if self._enum_conversions:
             first, *_ = parsed
-            enum_conversion: dict[int, StrEnumField] = self._enum_conversions[first]
+            enum_conversion: dict[int, StrEnumField | IntEnumField] = (
+                self._enum_conversions[first]
+            )
             parsed = tuple(
                 (
                     enum_conversion[i].cls(v)
                     if (v is not None and i in enum_conversion)
                     else v
                 )
                 for i, v in enumerate(parsed)
```

## Comparing `xlineparse-0.0.4.dist-info/METADATA` & `xlineparse-0.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xlineparse
-Version: 0.0.4
+Version: 0.0.5
 Classifier: Programming Language :: Python
 Requires-Dist: maturin ==1.4.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'dev'
 Requires-Dist: mypy ==1.6.* ; extra == 'dev'
 Requires-Dist: pip ==24.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'test'
 Provides-Extra: dev
@@ -82,15 +82,15 @@
     trailing_delimiter=False,
     lines=[
         xlp.Line(
             name="a",
             fields=[
                 xlp.DecimalField(
                     required=True,
-                    max_decimal_places=None,
+                    round_decimal_places=None,
                     min_value=Decimal("2.0"),
                     max_value=None,
                 )
             ],
         )
     ],
 )
@@ -99,16 +99,16 @@
 #  Will return:
 
 ("a", Decimal("2.0"))
 ```
 
 # TODO:
 
+- Maybe the big decimals are just floats?
 - Allow delimiters to be escaped.
-- `IntEnum`
 - Can we make enums quicker by moving to Rust?
 
 # Install/Develop
 
 ```shell
 uv pip install -e '.[dev]'
 maturin develop
```

## Comparing `xlineparse-0.0.4.dist-info/RECORD` & `xlineparse-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
+xlineparse/__init__.py,sha256=MhfzHodtfuhqqPQevDlhowLkIlRoe9wjK93k872ALDE,8439
 xlineparse/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xlineparse/__init__.py,sha256=OevPOvXbavzGJu5873ic96OUzU7xqNFpom6VLtNqY5E,7641
-xlineparse/xlineparse.cpython-312-i386-linux-gnu.so,sha256=Z5iCTXEgl1yBonwWMretnIiWqZ3W9EwlQ1zF6CmgVFo,2324012
-xlineparse-0.0.4.dist-info/METADATA,sha256=-I8UyG7Xcebb9RNzQMfP4N3THpqNsFAdRa4cIWfr6t4,2674
-xlineparse-0.0.4.dist-info/RECORD,,
-xlineparse-0.0.4.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
-xlineparse-0.0.4.dist-info/WHEEL,sha256=Ae3Tfi6BqeCLKeRR5nIV4A0W4paDC7wSiuTKW2pKNx4,212
-xlineparse-0.0.4.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
+xlineparse/xlineparse.cpython-311-darwin.so,sha256=wQ235T3vTvsffKQQiG4pt7PJzmshN5sCG01D9sCRVaw,1993680
+xlineparse-0.0.5.dist-info/RECORD,,
+xlineparse-0.0.5.dist-info/WHEEL,sha256=VDwrPQtzDuffEE5m5yHKwmmjpDZ_O8uqexNrjjw47eg,104
+xlineparse-0.0.5.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
+xlineparse-0.0.5.dist-info/METADATA,sha256=INv-5QwvG_H7nOr4oW44umWtIMQDZokKxqaqa5viC5k,2706
+xlineparse-0.0.5.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
```

## Comparing `xlineparse-0.0.4.dist-info/license_files/LICENSE` & `xlineparse-0.0.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

