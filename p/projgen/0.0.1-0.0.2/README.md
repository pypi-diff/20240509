# Comparing `tmp/projgen-0.0.1.tar.gz` & `tmp/projgen-0.0.2.tar.gz`

## Comparing `projgen-0.0.1.tar` & `projgen-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 projgen-0.0.1/projgen.json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 projgen-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projgen-0.0.1/src/projgen/__init__.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 projgen-0.0.1/src/projgen/__main__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 projgen-0.0.1/.gitignore
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 projgen-0.0.1/README.md
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 projgen-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 projgen-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 projgen-0.0.2/projgen.json
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 projgen-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projgen-0.0.2/src/projgen/__init__.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 projgen-0.0.2/src/projgen/__main__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 projgen-0.0.2/.gitignore
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 projgen-0.0.2/README.md
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 projgen-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 projgen-0.0.2/PKG-INFO
```

### Comparing `projgen-0.0.1/src/projgen/__main__.py` & `projgen-0.0.2/src/projgen/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,37 @@
 import datetime
 import random
 
 PROJECT_DESCRIPTION = \
 """Your current project started at [red]{start}[/red] and ends at [red]{end}[/red].
 Project specifics:{specs}"""
 
+EMPTY_DB = \
+"""{
+	"currentProject": {
+	  "start": "begin by running `main.py update`.",
+	  "end": "1970-01-01 12:00:00",
+	  "specifics": {
+	  }
+	},
+	"pastProjects": [],
+	"database": {
+	  "type": {
+		"Game": ["gameGenre", "gameMethod"]
+	  },
+	  "gameGenre": {
+		"shmup": []
+	  },
+	  "gameMethod": {
+		"godot": [],
+		"sdl": []
+	  }
+	}
+  }"""
+
 app = typer.Typer()
 
 def get_specific(specific: str, db: dict):
     return random.choice(list(db['database'][specific].keys()))
 
 @app.command()
 def status():
@@ -87,12 +110,19 @@
     with open("./projgen.json", "r") as f:
         data = json.loads(f.read())
     for key, value in data['database'].items():
         print(f"[bold]{key}[/bold]:")
         for k, v in value.items():
             print(f"·\t{k}: {v}")
 
+@app.command()
+def new_db():
+    input("Press enter to make a new ProjGen DB. ")
+    with open("./projgen.json", "w") as f:
+        f.write(EMPTY_DB)
+    print("A new database has been created!")
+
 def main():
     app()
 
 if __name__ == '__main__':
     main()
```

