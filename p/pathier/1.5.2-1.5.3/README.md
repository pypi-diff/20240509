# Comparing `tmp/pathier-1.5.2.tar.gz` & `tmp/pathier-1.5.3.tar.gz`

## Comparing `pathier-1.5.2.tar` & `pathier-1.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 pathier-1.5.2/CHANGELOG.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/index.html
--rw-r--r--   0        0        0   357931 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/pathier.html
--rw-r--r--   0        0        0    64654 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/search.js
--rw-r--r--   0        0        0    21254 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    85191 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_a44f0ac069e85531_test_pathier_py.html
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_d98317d23aadd1b8___init___py.html
--rw-r--r--   0        0        0   172092 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_d98317d23aadd1b8_pathier_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/status.json
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/style.css
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/__init__.py
--rw-r--r--   0        0        0    23148 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/pathier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/py.typed
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.5.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.5.2/LICENSE.txt
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pathier-1.5.2/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pathier-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pathier-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 pathier-1.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.5.3/docs/index.html
+-rw-r--r--   0        0        0   357680 2020-02-02 00:00:00.000000 pathier-1.5.3/docs/pathier.html
+-rw-r--r--   0        0        0    64654 2020-02-02 00:00:00.000000 pathier-1.5.3/docs/search.js
+-rw-r--r--   0        0        0    21254 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0    85191 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/d_a44f0ac069e85531_test_pathier_py.html
+-rw-r--r--   0        0        0    18181 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/d_d98317d23aadd1b8___init___py.html
+-rw-r--r--   0        0        0   172092 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/d_d98317d23aadd1b8_pathier_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/status.json
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 pathier-1.5.3/htmlcov/style.css
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pathier-1.5.3/src/pathier/__init__.py
+-rw-r--r--   0        0        0    23148 2020-02-02 00:00:00.000000 pathier-1.5.3/src/pathier/pathier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathier-1.5.3/src/pathier/py.typed
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pathier-1.5.3/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pathier-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pathier-1.5.3/PKG-INFO
```

### Comparing `pathier-1.5.2/CHANGELOG.md` & `pathier-1.5.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 # Changelog
 
+## v1.5.2 (2024-05-07)
+
+#### Refactorings
+
+* add ignores arg to sizeup cli
+* make some parameter type annotations more generic
+
+#### Others
+
+* conform to markdown linter
+
 ## v1.5.1 (2024-02-16)
 
 #### Refactorings
 
 * improve type annotation coverage
 
-
 ## v1.5.0 (2024-01-23)
 
 #### New Features
 
 * add default value for `default` param when calling `json.dumps()` and add default custom tomlkit encoder
 
-
 ## v1.4.0 (2024-01-15)
 
 #### New Features
 
 * add pickle loads and dumps support
 
-
 ## v1.3.6 (2024-01-12)
 
 #### Fixes
 
 * remove pathier from dependencies
 
-
 ## v1.3.5 (2024-01-12)
 
 #### Others
 
 * remove pytest from dependencies in pyproject.toml
 
-
 ## v1.3.4 (2023-11-06)
 
 #### Fixes
 
 * specify below python 3.12
 
-
 ## v1.3.2 (2023-11-06)
 
 #### Fixes
 
 * prevent crashes by creating parents in copy()
 
 ## v1.3.1 (2023-09-11)
@@ -55,250 +60,266 @@
 * change default value to True when convert_backslashes propert doesn't exist
 
 ## v1.3.0 (2023-09-11)
 
 #### New Features
 
 * by default, calling str() on a Pathier instances will convert backslashes to forward slashes
+
 ## v1.2.1 (2023-09-11)
 
 #### Refactorings
 
 * change `replace` to `replace_strings` to avoiding overwriting base class `replace` function
+
 ## v1.2.0 (2023-09-05)
 
 #### New Features
 
 * add sizeup cli
+
 #### Docs
 
 * document sizeup script
+
 ## v1.1.0 (2023-07-02)
 
 #### New Features
 
 * add `formatted_size` property
+
 #### Docs
 
 * update readme
 
 ## v1.0.0 (2023-07-02)
 
 #### Performance improvements
 
 * BREAKING: replace() accepts a list of 2-tuples instead of only an old and new string
+
 #### Refactorings
 
 * BREAKING: change `format_size()` to `format_bytes()`
 * BREAKING: change `size` to a property
+
 #### Docs
 
 * update readme
 
 ## v0.14.1 (2023-06-21)
 
 #### Performance improvements
 
 * toml files will have their datatypes converted to python types when loaded
+
 #### Others
 
 * specify minimum tomlkit version
+
 ## v0.14.0 (2023-06-10)
 
 #### New Features
 
 * add type aliases for `Pathier | pathlib.Path` and `Pathier | pathlib.Path | str`
+
 ## v0.13.0 (2023-06-01)
 
 #### Refactorings
 
 * size() returns 0 for non-existent files instead of None
 
 ## v0.12.0 (2023-05-26)
 
 #### New Features
 
 * add `keepends` parameter to split function
 * add `sep` parameter to join function
 * add properties to track last read vs last modified times
-#### Others
-
 
+#### Others
 
 ## v0.11.0 (2023-04-29)
 
 #### New Features
 
 * add join and split methods
 * add append method
+
 #### Docs
 
 * update readme
 
-
 ## v0.10.0 (2023-04-29)
 
 #### New Features
 
 * add replace function
 * add execute function
+
 #### Docs
 
 * update readme
 * improve doc string formatting
+
 #### Others
 
 * build v0.10.0
 * update changelog
 * remove unused import
 
-
 ## v0.9.0 (2023-04-28)
 
 #### New Features
 
 * add backup function
+
 #### Others
 
 * build v0.9.0
 * update changelog
 
-
 ## v0.8.0 (2023-04-15)
 
 #### New Features
 
 * wrap importing typing.Self in try/except to accomodate python 3.10
+
 #### Refactorings
 
 * import Self from typing_extensions
+
 #### Others
 
 * build v0.8.0
 * update changelog
 * remove uneeded dependency
 * set requires-python to >=3.10
 * build v0.7.0
 * remove uneeded dependency
 
-
 ## v0.7.0 (2023-04-11)
 
 #### New Features
 
 * add remove_from_PATH and make in_PATH a property
 * add functions to add path to sys.path
 * add 'PathLike' reference for annotating types that can be Pathier, pathlib.Path, or str
+
 #### Others
 
 * build v0.7.0
 * update changelog
 * update readme
 
-
 ## v0.6.0 (2023-04-02)
 
 #### New Features
 
 * add mkcwd() method
+
 #### Others
 
 * build v0.6.0
 * update changelog
 * update readme
 
-
 ## v0.5.0 (2023-04-01)
 
 #### New Features
 
 * add separate() method
+
 #### Fixes
 
 * separate() returned tuple instead of new Pathier object
+
 #### Others
 
 * build v0.5.0
 * update changelog
 * update readme
 
-
 ## v0.4.0 (2023-04-01)
 
 #### New Features
 
 * add move_under() method
+
 #### Others
 
 * build v0.4.0
 * update changelog
 * update readme
 
-
 ## v0.3.0 (2023-03-31)
 
 #### New Features
 
 * add modified_more_recently()
 * add is_older()
 * add is_larger() method
 * add mod_delta property
 * add mod_time property
 * add dob property
 * add age property
 * add format arg to size()
 * add format_size() static method
 * add size property
+
 #### Fixes
 
 * remove some erroneous text that found its way into some doc strings
+
 #### Refactorings
 
 * remove time module import
 * rename mod_time to mod_date
 * change size from property to function
+
 #### Others
 
 * build v0.3.0
 * update changelog
 * add to readme
 * remove unused import
 
-
 ## v0.2.0 (2023-03-31)
 
 #### New Features
 
 * add moveup() and __sub__() methods
+
 #### Others
 
 * build v0.2.0
 * update changelog
 * update readme
 * change __sub__ docstring
 
-
 ## v0.1.0 (2023-03-31)
 
 #### New Features
 
 * add touch()
+
 #### Others
 
 * build v0.1.0
 * update changelog
 * update .gitignore
 
-
 ## v0.0.0 (2023-03-28)
 
 #### New Features
 
 * add copy method to Pathier class.
+
 #### Fixes
 
 * wrong string in __all__.
+
 #### Others
 
 * build v0.0.0
 * add to readme.
-* add test for copy function.
+* add test for copy function.
```

### Comparing `pathier-1.5.2/docs/pathier.html` & `pathier-1.5.3/docs/pathier.html`

 * *Files 0% similar despite different names*

```diff
@@ -201,41 +201,42 @@
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">sizeup</span><span class="p">():</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Print the sub-directories and their sizes of the current working directory.&quot;&quot;&quot;</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">(</span><span class="s2">&quot;sizeup&quot;</span><span class="p">)</span>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
 </span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
 </span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>        <span class="s2">&quot;--ignore&quot;</span><span class="p">,</span>
 </span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
 </span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;Directory patterns to ignore.&quot;</span><span class="p">,</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="p">)</span>
 </span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>    <span class="n">matcher</span> <span class="o">=</span> <span class="n">younotyou</span><span class="o">.</span><span class="n">Matcher</span><span class="p">(</span><span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
 </span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="n">sizes</span><span class="p">:</span> <span class="nb">dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
 </span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">folders</span> <span class="o">=</span> <span class="p">[</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>        <span class="n">folder</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">iterdir</span><span class="p">()</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>        <span class="k">if</span> <span class="n">folder</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">folder</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">matcher</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>        <span class="k">if</span> <span class="n">folder</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">folder</span><span class="p">)</span> <span class="ow">in</span> <span class="n">matcher</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="p">]</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Sizing up </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">)</span><span class="si">}</span><span class="s2"> directories...&quot;</span><span class="p">)</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="k">with</span> <span class="n">printbuddies</span><span class="o">.</span><span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">))</span> <span class="k">as</span> <span class="n">prog</span><span class="p">:</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">folders</span><span class="p">:</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="n">prog</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Scanning &#39;</span><span class="si">{</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">size</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">total_size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]</span> <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">size_list</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>        <span class="p">(</span><span class="n">folder</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]))</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">keys</span><span class="p">()),</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">f</span><span class="p">:</span> <span class="n">sizes</span><span class="p">[</span><span class="n">f</span><span class="p">],</span> <span class="n">reverse</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>    <span class="p">]</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="nb">print</span><span class="p">(</span><span class="n">griddle</span><span class="o">.</span><span class="n">griddy</span><span class="p">(</span><span class="n">size_list</span><span class="p">,</span> <span class="p">[</span><span class="s2">&quot;Dir&quot;</span><span class="p">,</span> <span class="s2">&quot;Size&quot;</span><span class="p">]))</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Total size of &#39;</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&#39;: </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">total_size</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">printbuddies</span><span class="o">.</span><span class="n">track</span><span class="p">(</span><span class="n">folders</span><span class="p">,</span> <span class="s2">&quot;Scanning directories&quot;</span><span class="p">):</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">size</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>            <span class="k">pass</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">total_size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]</span> <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="n">size_list</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>        <span class="p">(</span><span class="n">folder</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]))</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">keys</span><span class="p">()),</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">f</span><span class="p">:</span> <span class="n">sizes</span><span class="p">[</span><span class="n">f</span><span class="p">],</span> <span class="n">reverse</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="p">]</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="nb">print</span><span class="p">(</span><span class="n">griddle</span><span class="o">.</span><span class="n">griddy</span><span class="p">(</span><span class="n">size_list</span><span class="p">,</span> <span class="p">[</span><span class="s2">&quot;Dir&quot;</span><span class="p">,</span> <span class="s2">&quot;Size&quot;</span><span class="p">]))</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Total size of &#39;</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&#39;: </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">total_size</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;1.5.2&quot;</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;1.5.3&quot;</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Pathier">
                             <input id="Pathier-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
```

#### html2text {}

```diff
@@ -66,43 +66,44 @@
 _1_5    """Print the sub-directories and their sizes of the current working
 directory."""
 _1_6    parser = argparse.ArgumentParser("sizeup")
 _1_7    parser.add_argument(
 _1_8        "-i",
 _1_9        "--ignore",
 _2_0        nargs="*",
-_2_1        default=None,
+_2_1        default=[],
 _2_2        type=str,
 _2_3        help="Directory patterns to ignore.",
 _2_4    )
 _2_5    args = parser.parse_args()
 _2_6    matcher = younotyou.Matcher(exclude_patterns=args.ignore)
 _2_7    sizes: dict[str, int] = {}
 _2_8    folders = [
 _2_9        folder
 _3_0        for folder in Pathier.cwd().iterdir()
-_3_1        if folder.is_dir() and str(folder) not in matcher
+_3_1        if folder.is_dir() and str(folder) in matcher
 _3_2    ]
 _3_3    print(f"Sizing up {len(folders)} directories...")
-_3_4    with printbuddies.ProgBar(len(folders)) as prog:
-_3_5        for folder in folders:
-_3_6            prog.display(f"Scanning '{folder.name}'")
-_3_7            sizes[folder.name] = folder.size
-_3_8    total_size = sum(sizes[folder] for folder in sizes)
-_3_9    size_list = [
-_4_0        (folder, Pathier.format_bytes(sizes[folder]))
-_4_1        for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
+_3_4    for folder in printbuddies.track(folders, "Scanning directories"):
+_3_5        try:
+_3_6            sizes[folder.name] = folder.size
+_3_7        except Exception as e:
+_3_8            pass
+_3_9    total_size = sum(sizes[folder] for folder in sizes)
+_4_0    size_list = [
+_4_1        (folder, Pathier.format_bytes(sizes[folder]))
+_4_2        for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
 reverse=True)
-_4_2    ]
-_4_3    print(griddle.griddy(size_list, ["Dir", "Size"]))
-_4_4    print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
+_4_3    ]
+_4_4    print(griddle.griddy(size_list, ["Dir", "Size"]))
+_4_5    print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
 (total_size)}")
-_4_5
 _4_6
-_4_7__version__ = "1.5.2"
+_4_7
+_4_8__version__ = "1.5.3"
 ??
 class Pathier(pathlib.Path): View Source
 _ _1_7class Pathier(pathlib.Path):
 _ _1_8    """Subclasses the standard library pathlib.Path class."""
 _ _1_9
 _ _2_0    def __new__(
 _ _2_1        cls,
```

### Comparing `pathier-1.5.2/docs/search.js` & `pathier-1.5.3/docs/search.js`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/coverage_html.js` & `pathier-1.5.3/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/d_a44f0ac069e85531_test_pathier_py.html` & `pathier-1.5.3/htmlcov/d_a44f0ac069e85531_test_pathier_py.html`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/d_d98317d23aadd1b8___init___py.html` & `pathier-1.5.3/htmlcov/d_d98317d23aadd1b8___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src\pathier\__init__.py: 40%</title>
+    <title>Coverage for src\pathier\__init__.py: 38%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src\pathier\__init__.py</b>:
-            <span class="pc_cov">40%</span>
+            <span class="pc_cov">38%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">25 statements &nbsp;</span>
+            <span class="text">26 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">10<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">15<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">16<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_d98317d23aadd1b8_pathier_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-05-07 16:38 -0500
+            created at 2024-05-09 16:46 -0500
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,67 +77,69 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">griddle</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">noiftimer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">printbuddies</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">younotyou</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">pathier</span> <span class="key">import</span> <span class="nam">Pathier</span><span class="op">,</span> <span class="nam">Pathish</span><span class="op">,</span> <span class="nam">Pathy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"Pathier"</span><span class="op">,</span> <span class="str">"Pathy"</span><span class="op">,</span> <span class="str">"Pathish"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">griddle</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">noiftimer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">printbuddies</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">younotyou</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">pathier</span> <span class="key">import</span> <span class="nam">Pathier</span><span class="op">,</span> <span class="nam">Pathish</span><span class="op">,</span> <span class="nam">Pathy</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"Pathier"</span><span class="op">,</span> <span class="str">"Pathy"</span><span class="op">,</span> <span class="str">"Pathish"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="op">@</span><span class="nam">noiftimer</span><span class="op">.</span><span class="nam">time_it</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">def</span> <span class="nam">sizeup</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""Print the sub-directories and their sizes of the current working directory."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">(</span><span class="str">"sizeup"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">"-i"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">"--ignore"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"*"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">type</span><span class="op">=</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"Directory patterns to ignore."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">matcher</span> <span class="op">=</span> <span class="nam">younotyou</span><span class="op">.</span><span class="nam">Matcher</span><span class="op">(</span><span class="nam">exclude_patterns</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">ignore</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">sizes</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">folders</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">folder</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">Pathier</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">iterdir</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">if</span> <span class="nam">folder</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">str</span><span class="op">(</span><span class="nam">folder</span><span class="op">)</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">matcher</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"Sizing up {len(folders)} directories..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">with</span> <span class="nam">printbuddies</span><span class="op">.</span><span class="nam">ProgBar</span><span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">folders</span><span class="op">)</span><span class="op">)</span> <span class="key">as</span> <span class="nam">prog</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">folders</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="nam">prog</span><span class="op">.</span><span class="nam">display</span><span class="op">(</span><span class="str">f"Scanning '{folder.name}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="op">@</span><span class="nam">noiftimer</span><span class="op">.</span><span class="nam">time_it</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">sizeup</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""Print the sub-directories and their sizes of the current working directory."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">(</span><span class="str">"sizeup"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">"-i"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="str">"--ignore"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"*"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">default</span><span class="op">=</span><span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">type</span><span class="op">=</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"Directory patterns to ignore."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">matcher</span> <span class="op">=</span> <span class="nam">younotyou</span><span class="op">.</span><span class="nam">Matcher</span><span class="op">(</span><span class="nam">exclude_patterns</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">ignore</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">sizes</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">folders</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">folder</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">Pathier</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">iterdir</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="key">if</span> <span class="nam">folder</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">str</span><span class="op">(</span><span class="nam">folder</span><span class="op">)</span> <span class="key">in</span> <span class="nam">matcher</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"Sizing up {len(folders)} directories..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">printbuddies</span><span class="op">.</span><span class="nam">track</span><span class="op">(</span><span class="nam">folders</span><span class="op">,</span> <span class="str">"Scanning directories"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="nam">sizes</span><span class="op">[</span><span class="nam">folder</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">folder</span><span class="op">.</span><span class="nam">size</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">total_size</span> <span class="op">=</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">sizes</span><span class="op">[</span><span class="nam">folder</span><span class="op">]</span> <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">sizes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">size_list</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="op">(</span><span class="nam">folder</span><span class="op">,</span> <span class="nam">Pathier</span><span class="op">.</span><span class="nam">format_bytes</span><span class="op">(</span><span class="nam">sizes</span><span class="op">[</span><span class="nam">folder</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">sorted</span><span class="op">(</span><span class="nam">list</span><span class="op">(</span><span class="nam">sizes</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">f</span><span class="op">:</span> <span class="nam">sizes</span><span class="op">[</span><span class="nam">f</span><span class="op">]</span><span class="op">,</span> <span class="nam">reverse</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="nam">griddle</span><span class="op">.</span><span class="nam">griddy</span><span class="op">(</span><span class="nam">size_list</span><span class="op">,</span> <span class="op">[</span><span class="str">"Dir"</span><span class="op">,</span> <span class="str">"Size"</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes(total_size)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.5.1"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="nam">total_size</span> <span class="op">=</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">sizes</span><span class="op">[</span><span class="nam">folder</span><span class="op">]</span> <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">sizes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="nam">size_list</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="op">(</span><span class="nam">folder</span><span class="op">,</span> <span class="nam">Pathier</span><span class="op">.</span><span class="nam">format_bytes</span><span class="op">(</span><span class="nam">sizes</span><span class="op">[</span><span class="nam">folder</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="key">for</span> <span class="nam">folder</span> <span class="key">in</span> <span class="nam">sorted</span><span class="op">(</span><span class="nam">list</span><span class="op">(</span><span class="nam">sizes</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">f</span><span class="op">:</span> <span class="nam">sizes</span><span class="op">[</span><span class="nam">f</span><span class="op">]</span><span class="op">,</span> <span class="nam">reverse</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="nam">griddle</span><span class="op">.</span><span class="nam">griddy</span><span class="op">(</span><span class="nam">size_list</span><span class="op">,</span> <span class="op">[</span><span class="str">"Dir"</span><span class="op">,</span> <span class="str">"Size"</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes(total_size)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.5.2"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_d98317d23aadd1b8_pathier_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-05-07 16:38 -0500
+            created at 2024-05-09 16:46 -0500
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,64 +1,66 @@
-************ CCoovveerraaggee ffoorr ssrrcc\\ppaatthhiieerr\\____iinniitt____..ppyy:: 4400%% ************
+************ CCoovveerraaggee ffoorr ssrrcc\\ppaatthhiieerr\\____iinniitt____..ppyy:: 3388%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2255 ssttaatteemmeennttss ?  1100 rruunn 1155 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 2266 ssttaatteemmeennttss ?  1100 rruunn 1166 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-
-07 16:38 -0500
+09 16:46 -0500
 _1import argparse 
-_2import griddle 
-_3import noiftimer 
-_4import printbuddies 
-_5import younotyou 
-_6 
-_7from .pathier import Pathier, Pathish, Pathy 
-_8 
-_9__all__ = ["Pathier", "Pathy", "Pathish"] 
-_1_0 
+_2 
+_3import griddle 
+_4import noiftimer 
+_5import printbuddies 
+_6import younotyou 
+_7 
+_8from .pathier import Pathier, Pathish, Pathy 
+_9 
+_1_0__all__ = ["Pathier", "Pathy", "Pathish"] 
 _1_1 
-_1_2@noiftimer.time_it() 
-_1_3def sizeup(): 
-_1_4 """Print the sub-directories and their sizes of the current working
+_1_2 
+_1_3@noiftimer.time_it() 
+_1_4def sizeup(): 
+_1_5 """Print the sub-directories and their sizes of the current working
 directory.""" 
-_1_5 parser = argparse.ArgumentParser("sizeup") 
-_1_6 parser.add_argument( 
-_1_7 "-i", 
-_1_8 "--ignore", 
-_1_9 nargs="*", 
-_2_0 default=None, 
-_2_1 type=str, 
-_2_2 help="Directory patterns to ignore.", 
-_2_3 ) 
-_2_4 args = parser.parse_args() 
-_2_5 matcher = younotyou.Matcher(exclude_patterns=args.ignore) 
-_2_6 sizes: dict[str, int] = {} 
-_2_7 folders = [ 
-_2_8 folder 
-_2_9 for folder in Pathier.cwd().iterdir() 
-_3_0 if folder.is_dir() and str(folder) not in matcher 
-_3_1 ] 
-_3_2 print(f"Sizing up {len(folders)} directories...") 
-_3_3 with printbuddies.ProgBar(len(folders)) as prog: 
-_3_4 for folder in folders: 
-_3_5 prog.display(f"Scanning '{folder.name}'") 
+_1_6 parser = argparse.ArgumentParser("sizeup") 
+_1_7 parser.add_argument( 
+_1_8 "-i", 
+_1_9 "--ignore", 
+_2_0 nargs="*", 
+_2_1 default=[], 
+_2_2 type=str, 
+_2_3 help="Directory patterns to ignore.", 
+_2_4 ) 
+_2_5 args = parser.parse_args() 
+_2_6 matcher = younotyou.Matcher(exclude_patterns=args.ignore) 
+_2_7 sizes: dict[str, int] = {} 
+_2_8 folders = [ 
+_2_9 folder 
+_3_0 for folder in Pathier.cwd().iterdir() 
+_3_1 if folder.is_dir() and str(folder) in matcher 
+_3_2 ] 
+_3_3 print(f"Sizing up {len(folders)} directories...") 
+_3_4 for folder in printbuddies.track(folders, "Scanning directories"): 
+_3_5 try: 
 _3_6 sizes[folder.name] = folder.size 
-_3_7 total_size = sum(sizes[folder] for folder in sizes) 
-_3_8 size_list = [ 
-_3_9 (folder, Pathier.format_bytes(sizes[folder])) 
-_4_0 for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
+_3_7 except Exception as e: 
+_3_8 pass 
+_3_9 total_size = sum(sizes[folder] for folder in sizes) 
+_4_0 size_list = [ 
+_4_1 (folder, Pathier.format_bytes(sizes[folder])) 
+_4_2 for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
 reverse=True) 
-_4_1 ] 
-_4_2 print(griddle.griddy(size_list, ["Dir", "Size"])) 
-_4_3 print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
+_4_3 ] 
+_4_4 print(griddle.griddy(size_list, ["Dir", "Size"])) 
+_4_5 print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
 (total_size)}") 
-_4_4 
-_4_5 
-_4_6__version__ = "1.5.1" 
+_4_6 
+_4_7 
+_4_8__version__ = "1.5.2" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-
-07 16:38 -0500
+09 16:46 -0500
```

### Comparing `pathier-1.5.2/htmlcov/d_d98317d23aadd1b8_pathier_py.html` & `pathier-1.5.3/htmlcov/d_d98317d23aadd1b8_pathier_py.html`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/favicon_32.png` & `pathier-1.5.3/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/index.html` & `pathier-1.5.3/htmlcov/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-05-07 16:42 -0500
+            created at 2024-05-09 16:46 -0500
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -59,18 +59,18 @@
                 <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded</th>
                 <th class="right" aria-sort="none" data-shortcut="c">coverage</th>
             </tr>
         </thead>
         <tbody>
             <tr class="file">
                 <td class="name left"><a href="d_d98317d23aadd1b8___init___py.html">src\pathier\__init__.py</a></td>
-                <td>25</td>
-                <td>15</td>
+                <td>26</td>
+                <td>16</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 25">40%</td>
+                <td class="right" data-ratio="10 26">38%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_d98317d23aadd1b8_pathier_py.html">src\pathier\pathier.py</a></td>
                 <td>246</td>
                 <td>27</td>
                 <td>0</td>
                 <td class="right" data-ratio="219 246">89%</td>
@@ -82,30 +82,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="210 210">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>481</td>
-                <td>42</td>
+                <td>482</td>
+                <td>43</td>
                 <td>0</td>
-                <td class="right" data-ratio="439 481">91%</td>
+                <td class="right" data-ratio="439 482">91%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-05-07 16:42 -0500
+            created at 2024-05-09 16:46 -0500
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531_test_pathier_py.html"/>
         <a id="nextFileLink" class="nav" href="d_d98317d23aadd1b8___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-07 16:42 -0500
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-09 16:46 -0500
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_s_r_c_\_p_a_t_h_i_e_r_\_____i_n_i_t_____._p_y 25         15      0        40%
+_s_r_c_\_p_a_t_h_i_e_r_\_____i_n_i_t_____._p_y 26         16      0        38%
 _s_r_c_\_p_a_t_h_i_e_r_\_p_a_t_h_i_e_r_._p_y  246        27      0        89%
 _t_e_s_t_s_\_t_e_s_t___p_a_t_h_i_e_r_._p_y   210        0       0        100%
-Total                   481        42      0        91%
+Total                   482        43      0        91%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-07 16:42 -0500
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-09 16:46 -0500
```

### Comparing `pathier-1.5.2/htmlcov/keybd_closed.png` & `pathier-1.5.3/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/keybd_open.png` & `pathier-1.5.3/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/htmlcov/status.json` & `pathier-1.5.3/htmlcov/status.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944444444444445%*

 * *Differences: {"'files'": "{'d_d98317d23aadd1b8___init___py': {'hash': 'cfdd9dd6e6b80e275786d3ed0c4911b5', "*

 * *            "'index': {'nums': {insert: [(2, 26), (4, 16)], delete: [4, 2]}}}}"}*

```diff
@@ -14,23 +14,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "tests\\test_pathier.py"
             }
         },
         "d_d98317d23aadd1b8___init___py": {
-            "hash": "ccf2a9333ffe176a351d3c38570c545d",
+            "hash": "cfdd9dd6e6b80e275786d3ed0c4911b5",
             "index": {
                 "html_filename": "d_d98317d23aadd1b8___init___py.html",
                 "nums": [
                     0,
                     1,
-                    25,
+                    26,
                     0,
-                    15,
+                    16,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src\\pathier\\__init__.py"
             }
         },
```

### Comparing `pathier-1.5.2/htmlcov/style.css` & `pathier-1.5.3/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/src/pathier/__init__.py` & `pathier-1.5.3/src/pathier/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,34 +14,35 @@
 def sizeup():
     """Print the sub-directories and their sizes of the current working directory."""
     parser = argparse.ArgumentParser("sizeup")
     parser.add_argument(
         "-i",
         "--ignore",
         nargs="*",
-        default=None,
+        default=[],
         type=str,
         help="Directory patterns to ignore.",
     )
     args = parser.parse_args()
     matcher = younotyou.Matcher(exclude_patterns=args.ignore)
     sizes: dict[str, int] = {}
     folders = [
         folder
         for folder in Pathier.cwd().iterdir()
-        if folder.is_dir() and str(folder) not in matcher
+        if folder.is_dir() and str(folder) in matcher
     ]
     print(f"Sizing up {len(folders)} directories...")
-    with printbuddies.ProgBar(len(folders)) as prog:
-        for folder in folders:
-            prog.display(f"Scanning '{folder.name}'")
+    for folder in printbuddies.track(folders, "Scanning directories"):
+        try:
             sizes[folder.name] = folder.size
+        except Exception as e:
+            pass
     total_size = sum(sizes[folder] for folder in sizes)
     size_list = [
         (folder, Pathier.format_bytes(sizes[folder]))
         for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f], reverse=True)
     ]
     print(griddle.griddy(size_list, ["Dir", "Size"]))
     print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes(total_size)}")
 
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
```

### Comparing `pathier-1.5.2/src/pathier/pathier.py` & `pathier-1.5.3/src/pathier/pathier.py`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/LICENSE.txt` & `pathier-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/README.md` & `pathier-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pathier-1.5.2/pyproject.toml` & `pathier-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pathier"
 description = "Extends the standard library pathlib.Path class."
-version = "1.5.2"
+version = "1.5.3"
 dependencies = ["tomlkit>=0.11.8", "typing_extensions", "griddle", "noiftimer", "printbuddies", "younotyou"]
 readme = "README.md"
 keywords = ["pathlib", "path", "json", "toml", "shutil", "extender", "extension"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <3.12"
 
 [[project.authors]]
```

### Comparing `pathier-1.5.2/PKG-INFO` & `pathier-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathier
-Version: 1.5.2
+Version: 1.5.3
 Summary: Extends the standard library pathlib.Path class.
 Project-URL: Homepage, https://github.com/matt-manes/pathier
 Project-URL: Documentation, https://github.com/matt-manes/pathier/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/pathier/tree/main/src/pathier
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: extender,extension,json,path,pathlib,shutil,toml
```

