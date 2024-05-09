# Comparing `tmp/repository_manager-0.8.2-py2.py3-none-any.whl.zip` & `tmp/repository_manager-0.8.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6209 bytes, number of entries: 9
--rw-r--r--  2.0 unx      300 b- defN 24-Feb-13 23:06 repository_manager/__init__.py
--rw-r--r--  2.0 unx     6615 b- defN 24-Feb-13 23:06 repository_manager/repository_manager.py
--rw-r--r--  2.0 unx      116 b- defN 24-Feb-17 17:12 repository_manager/version.py
--rw-r--r--  2.0 unx     1059 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4860 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      816 b- defN 24-Feb-17 17:12 repository_manager-0.8.2.dist-info/RECORD
-9 files, 13978 bytes uncompressed, 4775 bytes compressed:  65.8%
+Zip file size: 6254 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      328 b- defN 24-May-09 03:46 repository_manager/__init__.py
+-rw-r--r--  2.0 unx     6813 b- defN 24-May-09 03:46 repository_manager/repository_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 24-May-09 03:46 repository_manager/version.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4860 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      816 b- defN 24-May-09 03:46 repository_manager-0.8.3.dist-info/RECORD
+9 files, 14205 bytes uncompressed, 4820 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: repository_manager/repository_manager.py
 Comment: 
 
 Filename: repository_manager/version.py
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/LICENSE
+Filename: repository_manager-0.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/METADATA
+Filename: repository_manager-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/WHEEL
+Filename: repository_manager-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/entry_points.txt
+Filename: repository_manager-0.8.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/top_level.txt
+Filename: repository_manager-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: repository_manager-0.8.2.dist-info/RECORD
+Filename: repository_manager-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## repository_manager/__init__.py

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 # coding: utf-8
 from repository_manager.version import __version__, __author__, __credits__
 from repository_manager.repository_manager import Git, main
+
 """
 report-manager
 
 Manage your git projects
 """
 
 __version__ = __version__
 __author__ = __author__
 __credits__ = __credits__
+
+__all__ = ["Git", "main"]
```

## repository_manager/repository_manager.py

```diff
@@ -15,46 +15,54 @@
         self.git_projects = []
         self.set_to_default_branch = False
         self.threads = os.cpu_count()
 
     def git_action(self, command, directory=None):
         if directory is None:
             directory = self.repository_directory
-        pipe = subprocess.Popen(command,
-                                shell=True,
-                                cwd=directory,
-                                stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE)
+        pipe = subprocess.Popen(
+            command,
+            shell=True,
+            cwd=directory,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
         (out, error) = pipe.communicate()
         result = f"{str(out, 'utf-8')}{str(error, 'utf-8')}"
         pipe.wait()
         return result
 
     def set_repository_directory(self, repository_directory):
         if os.path.exists(repository_directory):
             self.repository_directory = repository_directory.replace(os.sep, "/")
         else:
-            print(f'Path specified does not exist: {repository_directory.replace(os.sep, "/")}')
+            print(
+                f'Path specified does not exist: {repository_directory.replace(os.sep, "/")}'
+            )
 
     def set_git_projects(self, git_projects):
         self.git_projects = git_projects
 
     def set_default_branch(self, set_to_default_branch):
         self.set_to_default_branch = set_to_default_branch
 
     def set_threads(self, threads):
         try:
             threads = int(threads)
             if threads > 0 or threads < os.cpu_count():
                 self.threads = threads
             else:
-                print(f"Did not recognize {threads} as a valid value, defaulting to CPU Count: {os.cpu_count()}")
+                print(
+                    f"Did not recognize {threads} as a valid value, defaulting to CPU Count: {os.cpu_count()}"
+                )
                 self.threads = os.cpu_count()
         except Exception as e:
-            print(f"Did not recognize {threads} as a valid value, defaulting to CPU Count: {os.cpu_count()}\nError: {e}")
+            print(
+                f"Did not recognize {threads} as a valid value, defaulting to CPU Count: {os.cpu_count()}\nError: {e}"
+            )
             self.threads = os.cpu_count()
 
     def append_git_project(self, git_project):
         self.git_projects.append(git_project)
 
     def clone_projects_in_parallel(self):
         pool = Pool(processes=self.threads)
@@ -64,60 +72,81 @@
         print(self.git_action(f"git clone {git_project}"))
 
     def pull_projects_in_parallel(self):
         pool = Pool(processes=self.threads)
         pool.map(self.pull_project, os.listdir(self.repository_directory))
 
     def pull_project(self, git_project):
-        print(f'Scanning: {self.repository_directory}/{git_project}\n'
-              f'Pulling latest changes for {git_project}\n'
-              f'{self.git_action(command="git pull", directory=os.path.normpath(os.path.join(self.repository_directory, git_project)))}')
+        print(
+            f"Scanning: {self.repository_directory}/{git_project}\n"
+            f"Pulling latest changes for {git_project}\n"
+            f'{self.git_action(command="git pull", directory=os.path.normpath(os.path.join(self.repository_directory, git_project)))}'
+        )
         if self.set_to_default_branch:
-            default_branch = self.git_action("git symbolic-ref refs/remotes/origin/HEAD",
-                                             directory=f"{self.repository_directory}/{git_project}")
+            default_branch = self.git_action(
+                "git symbolic-ref refs/remotes/origin/HEAD",
+                directory=f"{self.repository_directory}/{git_project}",
+            )
             default_branch = re.sub("refs/remotes/origin/", "", default_branch).strip()
-            print(f"Checking out default branch ",
-                  self.git_action(f'git checkout "{default_branch}"',
-                                  directory=f"{self.repository_directory}/{git_project}"))
+            print(
+                "Checking out default branch ",
+                self.git_action(
+                    f'git checkout "{default_branch}"',
+                    directory=f"{self.repository_directory}/{git_project}",
+                ),
+            )
 
 
 def usage():
-    print(f"Usage: \n"
-          f"-h | --help           [ See usage for script ]\n"
-          f"-b | --default-branch [ Checkout default branch ]\n"
-          f"-c | --clone          [ Clone projects specified  ]\n"
-          f"-d | --directory      [ Directory to clone/pull projects ]\n"
-          f"-f | --file           [ File with repository links   ]\n"
-          f"-p | --pull           [ Pull projects in parent directory ]\n"
-          f"-r | --repositories   [ Comma separated Git URLs ]\n"
-          f"-t | --threads        [ Number of parallel threads - Default 4 ]\n"
-          f"\n"
-          f"repository-manager \n\t"
-          f"--clone \n\t"
-          f"--pull \n\t"
-          f"--directory '/home/user/Downloads'\n\t"
-          f"--file '/home/user/Downloads/repositories.txt' \n\t"
-          f"--repositories 'https://github.com/Knucklessg1/media-downloader,https://github.com/Knucklessg1/genius-bot'\n\t"
-          f"--threads 8")
+    print(
+        "Usage: \n"
+        "-h | --help           [ See usage for script ]\n"
+        "-b | --default-branch [ Checkout default branch ]\n"
+        "-c | --clone          [ Clone projects specified  ]\n"
+        "-d | --directory      [ Directory to clone/pull projects ]\n"
+        "-f | --file           [ File with repository links   ]\n"
+        "-p | --pull           [ Pull projects in parent directory ]\n"
+        "-r | --repositories   [ Comma separated Git URLs ]\n"
+        "-t | --threads        [ Number of parallel threads - Default 4 ]\n"
+        "\n"
+        "repository-manager \n\t"
+        "--clone \n\t"
+        "--pull \n\t"
+        "--directory '/home/user/Downloads'\n\t"
+        "--file '/home/user/Downloads/repositories.txt' \n\t"
+        "--repositories 'https://github.com/Knucklessg1/media-downloader,https://github.com/Knucklessg1/genius-bot'\n\t"
+        "--threads 8"
+    )
 
 
 def repository_manager(argv):
     gitlab = Git()
     projects = []
     default_branch_flag = False
     clone_flag = False
     pull_flag = False
     directory = os.curdir
     file = None
     repositories = None
     threads = os.cpu_count()
     try:
-        opts, args = getopt.getopt(argv, "hbcpd:f:r:t:",
-                                   ["help", "default-branch", "clone", "pull", "directory=", "file=", "repositories=",
-                                    "threads="])
+        opts, args = getopt.getopt(
+            argv,
+            "hbcpd:f:r:t:",
+            [
+                "help",
+                "default-branch",
+                "clone",
+                "pull",
+                "directory=",
+                "file=",
+                "repositories=",
+                "threads=",
+            ],
+        )
     except getopt.GetoptError:
         usage()
         sys.exit(2)
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             usage()
             sys.exit()
@@ -143,15 +172,15 @@
     else:
         print(f"Directory not found: {directory}")
         usage()
         sys.exit(2)
 
     # Verify file with repositories exists
     if os.path.exists(file):
-        file_repositories = open(file, 'r')
+        file_repositories = open(file, "r")
         for repository in file_repositories:
             projects.append(repository)
     else:
         print(f"File not found: {file}")
         usage()
         sys.exit(2)
```

## repository_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.2'
-__author__ = 'Audel Rouhi'
-__credits__ = 'Audel Rouhi'
+__version__ = '0.8.3'
+__author__ = "Audel Rouhi"
+__credits__ = "Audel Rouhi"
```

## Comparing `repository_manager-0.8.2.dist-info/LICENSE` & `repository_manager-0.8.3.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `repository_manager-0.8.2.dist-info/METADATA` & `repository_manager-0.8.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Manage your git projects
 Home-page: https://github.com/Knuckles-Team/repository-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/repository-manager)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/repository-manager)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/repository-manager)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/repository-manager)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/repository-manager)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/repository-manager)
 
-*Version: 0.8.2*
+*Version: 0.8.3*
 
 Manage your Git projects
 
 Run all Git supported tasks using Git Actions command
 
 This repository is actively maintained - Contributions are welcome!
```

