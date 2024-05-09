# Comparing `tmp/opentldr-0.4.3.tar.gz` & `tmp/opentldr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.4.3.tar", last modified: Tue Apr 30 20:19:16 2024, max compression
+gzip compressed data, was "opentldr-0.5.0.tar", last modified: Thu May  9 19:51:13 2024, max compression
```

## Comparing `opentldr-0.4.3.tar` & `opentldr-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:16.333557 opentldr-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 20:19:11.000000 opentldr-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:11.000000 opentldr-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-30 20:19:16.333557 opentldr-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-30 20:19:11.000000 opentldr-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 20:19:11.000000 opentldr-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:19:16.333557 opentldr-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:16.329557 opentldr-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:16.333557 opentldr-0.4.3/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28235 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    30752 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 20:19:11.000000 opentldr-0.4.3/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:16.333557 opentldr-0.4.3/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-30 20:19:16.000000 opentldr-0.4.3/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 20:19:16.000000 opentldr-0.4.3/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:19:16.000000 opentldr-0.4.3/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 20:19:16.000000 opentldr-0.4.3/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 20:19:16.000000 opentldr-0.4.3/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:19:16.333557 opentldr-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:19:11.000000 opentldr-0.4.3/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:19:11.000000 opentldr-0.4.3/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 20:19:11.000000 opentldr-0.4.3/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:19:11.000000 opentldr-0.4.3/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:13.954115 opentldr-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 19:51:09.000000 opentldr-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:09.000000 opentldr-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-09 19:51:13.954115 opentldr-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-09 19:51:09.000000 opentldr-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 19:51:09.000000 opentldr-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:51:13.954115 opentldr-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:13.950115 opentldr-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:13.954115 opentldr-0.5.0/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34236 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 19:51:09.000000 opentldr-0.5.0/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:13.954115 opentldr-0.5.0/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-09 19:51:13.000000 opentldr-0.5.0/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 19:51:13.000000 opentldr-0.5.0/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:51:13.000000 opentldr-0.5.0/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 19:51:13.000000 opentldr-0.5.0/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 19:51:13.000000 opentldr-0.5.0/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:51:13.954115 opentldr-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 19:51:09.000000 opentldr-0.5.0/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 19:51:09.000000 opentldr-0.5.0/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-09 19:51:09.000000 opentldr-0.5.0/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-09 19:51:09.000000 opentldr-0.5.0/tests/test_workflow.py
```

### Comparing `opentldr-0.4.3/LICENSE` & `opentldr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.4.3/PKG-INFO` & `opentldr-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.4.3
+Version: 0.5.0
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -25,62 +25,61 @@
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
-OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
+OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
-- A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
+- A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
 - A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
-This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
-to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
+This GitHub repo handles the back-end code that is only required if you wish to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is available to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
-OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
+OpenTLDR uses a Neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
 
-OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain class being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
+OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain classes being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
 
 ## Domain
 
 The OpenTLDR library includes class definitions for all of the objects represented in the KnowledgeGraph. This standardizes the graph, so that multiple analytic workflows can easily achieve compatability.
 
 Each Domain class includes the following properties:
 - uid - a text string that acts as a unique identifier that is created the first time the data object is saved and can be queried.
 - meta - a json object that can be used to decorate any node or edge with additional properties that your workflow might use (but that are not expected to be implemented by others)
 
-The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
+The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
 
 ![ontology image](resources/ontology.png)
 
-The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with capitalized camel case lettering without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which is can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
+The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with upper camel case capitalization without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
 
 ## Workflow
 
 The OpenTLDR Workflow uses PaperMill to execute the sequences of analytic notebooks and parameterize them. This should not impede the notebooks from  being run manually when desired, but it does enforce the expected workflow order of execution that should be used when running evaluation scoring for an end-to-end analytic workflow.
 
 ### The Default Workflow Parameters
 
 There are a few paramters that are used throughout the standard workflow.
 
 #### Output Folder
-This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results but are replaced the next time the workflow is executed. Therefore, they should only be used as read-only copies.
+This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results.  They copies are overwritten each time the workflow is executed. The original notebooks should always be treated as read-only copies.
 
 <pre>
 output_folder = "./READ_ONLY_OUTPUT"
 </pre>
 
 #### Notebook Order
-This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed for manual execution, but the order in which they appear in this list is the order in which the `Workflow` class will run them.
+This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed manually, but the `Workflow` class always executes in the order they appear in this list. 
 
 <pre>
 notebook_order = [
     "Step_0_Initialize.ipynb",
   ...
     "Step_6_Evaluate.ipynb"
     ]
@@ -98,15 +97,15 @@
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
 ## DataRepo
-The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above `variables_to_set` specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -128,9 +127,9 @@
 
 kg = KnowledgeGraph()
 cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo `cr` that writes to the KnowledgeGraph `kg` from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.4.3/README.md` & `opentldr-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,62 +2,61 @@
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
-OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
+OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
-- A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
+- A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
 - A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
-This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
-to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
+This GitHub repo handles the back-end code that is only required if you wish to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is available to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
-OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
+OpenTLDR uses a Neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
 
-OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain class being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
+OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain classes being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
 
 ## Domain
 
 The OpenTLDR library includes class definitions for all of the objects represented in the KnowledgeGraph. This standardizes the graph, so that multiple analytic workflows can easily achieve compatability.
 
 Each Domain class includes the following properties:
 - uid - a text string that acts as a unique identifier that is created the first time the data object is saved and can be queried.
 - meta - a json object that can be used to decorate any node or edge with additional properties that your workflow might use (but that are not expected to be implemented by others)
 
-The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
+The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
 
 ![ontology image](resources/ontology.png)
 
-The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with capitalized camel case lettering without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which is can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
+The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with upper camel case capitalization without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
 
 ## Workflow
 
 The OpenTLDR Workflow uses PaperMill to execute the sequences of analytic notebooks and parameterize them. This should not impede the notebooks from  being run manually when desired, but it does enforce the expected workflow order of execution that should be used when running evaluation scoring for an end-to-end analytic workflow.
 
 ### The Default Workflow Parameters
 
 There are a few paramters that are used throughout the standard workflow.
 
 #### Output Folder
-This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results but are replaced the next time the workflow is executed. Therefore, they should only be used as read-only copies.
+This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results.  They copies are overwritten each time the workflow is executed. The original notebooks should always be treated as read-only copies.
 
 <pre>
 output_folder = "./READ_ONLY_OUTPUT"
 </pre>
 
 #### Notebook Order
-This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed for manual execution, but the order in which they appear in this list is the order in which the `Workflow` class will run them.
+This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed manually, but the `Workflow` class always executes in the order they appear in this list. 
 
 <pre>
 notebook_order = [
     "Step_0_Initialize.ipynb",
   ...
     "Step_6_Evaluate.ipynb"
     ]
@@ -75,15 +74,15 @@
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
 ## DataRepo
-The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above `variables_to_set` specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -105,9 +104,9 @@
 
 kg = KnowledgeGraph()
 cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo `cr` that writes to the KnowledgeGraph `kg` from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.4.3/pyproject.toml` & `opentldr-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.4.3"
+version = "0.5.0"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.4.3/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.0/src/opentldr/AbstractDataRepo.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import json
 
 from .KnowledgeGraph import KnowledgeGraph
 from .log import log
 
 class AbstractDataRepo:
     '''
-    baseclass for all Data Repositories, inmcludes shared methods and ingest ordering.
+    baseclass for all Data Repositories, includes shared methods and ingest ordering.
     '''
     # knowledgegraph for import/export
     kg:KnowledgeGraph=None
 
-    # order in content should be imported to ensure dependencies.
+    # order content should be imported to ensure dependencies.
     import_order=[
             "ReferenceNode",
             "ReferenceEdge",
             "Source",
             "Content",
             "User",
             "Request",
@@ -47,15 +47,15 @@
             # name = Chris\n
             Another line.\n
             And one at the end.\n
 
         Will return ({'uid': '1234', 'name':'Chris}, 'This is a text block.\nAnother line.\nAnd one at the end')    
         '''
         # Identifies a property key
-        property_regex=re.compile(r'^#\s*[a-z_]*\s*\:\s*')
+        property_regex=re.compile(r'^#\s*[a-z_]+\s*\:\s*')
         
         content_text=""
         properties={}
 
         for line in text.splitlines():
             match= property_regex.search(line)
             if match:
@@ -80,14 +80,15 @@
         if 'active' in path or 'content' in path or 'article' in path:
             return "Content"
         if 'request' in path or 'query' in path or 'user' in path:
             if 'text' in annotations:
                 return "Request"
             if 'name' in annotations:
                 return "User"
+            # TODO: Nothing is returned if no text and no name
         if 'eval' in path or 'evalkey' in path or 'evaluation' in path:
             return "EvalKey"
         if 'feedback' in path:
             return "Feedback"
 
     def clean_up_nodes(self) -> list[str]:
         out:list[str]=[]
```

### Comparing `opentldr-0.4.3/src/opentldr/DataRepo.py` & `opentldr-0.5.0/src/opentldr/DataRepo.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,18 @@
 
     def __init__(self, kg:KnowledgeGraph, config:dict):
         if config is None:
             log.warn("No config file passed to DataRepo, defaulting to using environment variables.")
             config="{}"
 
         type = self._configOrEnv("repo_type",config);
+        # TODO: The s3/files check here make the "case _" branch unreachable.
+        # I recommend deleting the check here.  Making it easier to expand cases below in the future.
         if type is None or type not in ['s3','files']:
-            message=("DataRepo factory requires a dictionary structure as a parameter that includes at least a 'repo_type' entry set to one of 's3' or 'file'.")
+            message=("DataRepo factory requires a dictionary structure as a parameter that includes at least a 'repo_type' entry set to one of 's3' or 'files'.")
             log.error(message)
             raise TypeError(message)
         
         match type:
             case "s3":
                 bucket_name=self._configOrEnv("bucket",config)
                 aws_access_key_id=self._configOrEnv("aws_access_key_id",config)
@@ -64,16 +66,16 @@
             case _:
                 message:str = "Invalid 'type' config ('{type}').".format(type=type)
                 log.error(message)
                 raise NotImplementedError(message)
 
     def importData(self) -> list[str]:
         if self.repo is None:
-            log.error("No to DataRepo was configured.")
+            log.error("No DataRepo was configured.")
         return self.repo.importData()
 
     def describe(self) -> str:
         if self.repo is None:
-            log.error("No to DataRepo was configured.")
+            log.error("No DataRepo was configured.")
         return self.repo.describe()
```

### Comparing `opentldr-0.4.3/src/opentldr/DataRepoJson.py` & `opentldr-0.5.0/src/opentldr/DataRepoJson.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
 class DataRepoJsonFiles(AbstractDataRepo):
     '''
     Reads a single .json text file from the path and populates the KG using it.
     This is a great way to export checkpoints for a KG and re-import them later.
     '''
 
-    filename:str = "./repo.json"
-    data:dict = {}
-
-
     def __init__(self, kg:KnowledgeGraph, filename:str):
         self.kg=kg
         self.filename = filename
         self.verify()
 
 
     def verify(self):
@@ -84,28 +80,28 @@
 
         path = self.ingest_path
         alt_path = os.path.join(self.ingest_path,"requests")
         if os.path.exists(alt_path) and os.path.isdir(alt_path) and os.access(alt_path,os.R_OK):
             log.debug("Found data type directory in specified repo path.")
             path=alt_path
 
-        default_source_name = "File System Directory:{path}".format(path=path)
+        default_source_name = "File System Directory:{path}".format(path=path)      # TODO: Never used.  Delete.
         list_of_uids = []
 
         # read in each text file from directory
         for filename in os.listdir(path):
 
             # ignore anything but files that end in .txt
             if os.path.splitext(filename)[1] != ".txt" or not os.path.isfile(os.path.join(path, filename)):
                 continue
 
             full_path=os.path.join(path, filename)
             with open(full_path) as f:
                 text = f.read()
-                request=self.importTextRequest(kg=self.kg, text=text)
+                request=self.importTextRequest(kg=self.kg, text=text)       # TODO: importTextRequest never defined
                 list_of_uids.append(request.uid)
                 log.info("Imported: {data}".format(data=request.to_text()))
 
         return list_of_uids
 
     def importActiveData(self) -> list[str]:
         log.info("Importing Active Data from File System...")
@@ -124,15 +120,15 @@
             # ignore anything but files that end in .txt
             if os.path.splitext(filename)[1] != ".txt" or not os.path.isfile(full_path):
                 continue
 
             with open(full_path) as f:
                 text = f.read()
                 url="file://{path}".format(path=os.path.abspath(full_path))
-                content=self.importTextContent(kg=self.kg, text=text, url=url, default_source_name=default_source_name)
+                content=self.importTextContent(kg=self.kg, text=text, url=url, default_source_name=default_source_name)  # TODO: importTextRequest never defined
                 list_of_uids.append(content.uid)
                 log.info("Imported: {data}".format(data=content.to_text()))
 
         return list_of_uids
     
     def importFeedbackData(self) -> list[str]:
         message:str = "Importing MongoDB Feedback Data is not implemented yet."
```

### Comparing `opentldr-0.4.3/src/opentldr/Domain.py` & `opentldr-0.5.0/src/opentldr/Domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # from neomodel.cardinality import One, ZeroOrOne, ZeroOrMore, OneOrMore
 from neomodel.sync_.cardinality import One, ZeroOrOne, ZeroOrMore, OneOrMore
 
 from .log import log
 
 def jsonToKg(kg,json_string):
     '''
-    hydrate a json string to a Domain object. This requires the "class" attribute to 
+    Hydrate a json string to a Domain object. This requires the "class" attribute to
     determine the correct class type, so it only works on these classes.
     '''
     raw = json.loads(json)
     log.info("Ingesting JSON into an OpenTLDR Domain object and then the KG.")
     print("JSON: ",raw)
     if isinstance(raw,list):
         for item in raw:
@@ -43,15 +43,15 @@
     for f in formats:
         try:
             d=datetime.strptime(date_string,f)
             return d
         except:
             pass # try try again
     # give up with a nicely formatted date, even if wrong
-    log.error("Unable to parse date out of '{date}'.".format(date=date))
+    log.error("Unable to parse date out of '{date}'.  Returning now.".format(date=date))
     return datetime.now 
 
 
 # UTILITY MIX-IN CLASSES
 
 class OpenTldrMeta():
     '''
@@ -60,15 +60,15 @@
     interface for PyDantic for data manipulation and JSON.
     '''
     uid=nm.UniqueIdProperty()
     metadata=nm.JSONProperty(default={})
        
     def to_text(self) -> str:
         '''
-        to_text() returns a user readable string representing the values in the object.
+        to_text() returns a unique, user readable string representing the object.
         '''
         return "uid: {uid}".format(uid=self.uid)
 
 
 class OpenTldrNode():
     '''
     OpenTldrNode is mixed in to each node class to support json import/export.
@@ -95,22 +95,21 @@
         connection = self.to_json_connect(kg, data)
         if connection is not None:
             data.update(connection)
         return json.dumps(data)
 
     def to_json_connect(self, kg, json_dict) -> dict:
         '''
-        override to_json_connect to insert edge data into the node.
-
+        Override to_json_connect to insert edge data into the node.
         '''
         pass
 
     def from_json_connect(self, kg, json_dict):
         '''
-        override from_json_connect to rebuild edge data from serialized node.
+        Override from_json_connect to rebuild edge data from serialized node.
         '''
         pass
 
 
 
 class OpenTldrEdge():
     '''
@@ -143,22 +142,21 @@
         connection = self.to_json_connect(kg, data)
         if connection is not None:
             data.update(connection)
         return json.dumps(data)
 
     def to_json_connect(self, kg, json_dict) -> dict:
         '''
-        override to_json_connect to insert edge data into the node.
-
+        Override to_json_connect to insert edge data into the node.
         '''
         pass
 
     def from_json_connect(self, kg, json_dict):
         '''
-        override from_json_connect to rebuild edge data from serialized node.
+        Override from_json_connect to rebuild edge data from serialized node.
         '''
         pass
 
     @classmethod
     def from_json(cls, kg, json_string):
         json_dict=json.loads(json_string)
         if "connection" in json_dict:
@@ -208,15 +206,15 @@
     and we need to refer back to the Node from where they were detected.
     '''
     pass
 
 class Uncertain():
     '''
     Uncertain is a mixin class that adds a confidence value (0.0-1.0) to a Node or Edge.
-    This is implemented to store the float value and generate description qualatiative
+    This is implemented to store the float value and generate description qualitative
     text clauses for the ranges of this confidence value.
     '''
     confidence = nm.FloatProperty(default=1.0)
     def uncertainty_to_text(self) -> str:
         if self.confidence < 0.05:
             return "with almost no chance"
         if self.confidence >= 0.05 and self.confidence < 0.20:
@@ -232,19 +230,21 @@
         if self.confidence >= 0.55 and self.confidence < 1.0:
             return "with almost certainty"
         return "with certainty"
 
 class Scored():
     '''
     Scored is a mixin class that adds a score value (0.0-1.0) to a Node or Edge.
-    This is implemented to store the float value and generate descriptive qualatative
+    This is implemented to store the float value and generate descriptive qualitative
     text clauses for the ranges of this score value.
     '''
-    score = nm.FloatProperty(default=1.0)
+    score = nm.FloatProperty(default=-1.0)
     def score_to_text(self) -> str:
+        if self.score < 0.0:
+            return "unknown"
         if self.score < 0.15:
             return "very low"
         if self.score >= 0.15 and self.score < 0.40:
             return "low"
         if self.score >= 0.4 and self.score < 0.6:
             return "medium"
         if self.score >= 0.6 and self.score < 0.85:
@@ -272,16 +272,14 @@
     def is_hypothesized(self) -> bool:
         return self.hypothesized
 
     def set_hypothesized(self, is_hypothesized:bool):
         self.hypothesized=is_hypothesized
 
     def get_connection_json(self) -> dict:
-        left:ReferenceNode = self.start_node()
-        right:ReferenceNode = self.end_node()
         return {
             "start": self.start_node().uid,
             "relation": "edges",
             "end": self.end_node().uid
         }
 
     def to_text(self) -> str:
@@ -291,15 +289,15 @@
                                                            right=right.text,
                                                            relationship=self.text,
                                                            type=self.type)
 
 
 class ReferenceNode(nm.StructuredNode, OpenTldrText, OpenTldrMeta, OpenTldrNode):
     '''
-    ReferenceNode allos for general reference data nodes to be introduced into the 
+    ReferenceNode allows for general reference data nodes to be introduced into the
     knowledge graph and used abstractly (e.g., to relate extracted entities to known things).
     This uses the OpenTldrText mixin to implement text and type properties.
     The hypothesized property is a boolean that indicates if this was inferred (e.g., discovered)
     or provided as fact via external reference data (e.g., imported). 
     '''
     hypothesized = nm.BooleanProperty(default=False)
 
@@ -324,22 +322,22 @@
 
 # Active Data
 
 
 class Source(nm.StructuredNode, OpenTldrMeta, OpenTldrNode):
     '''
     Source nodes indicate the generator of various content. This may be an author or distributor
-    of information. The name property is used to uniquely identify the source.
+    of information. The name property is used to uniquely identify the Source.
     '''
     name = nm.StringProperty(unique_index=True, required=True)
 
 
 class IsFrom(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    IsFrom edges connect Content nodesM to the Source nodes in the knowledge graph.
+    IsFrom edges connect Content nodes to the Source nodes in the knowledge graph.
     '''
     def to_text(self) -> str:
         return "The {content_type} '{content_title}' is from the source {end}.".format(
             content_type= self.start_node().type,
             content_title=self.start_node().title,
             end=self.end_node().name)
 
@@ -389,29 +387,29 @@
         return "The entity '{entity}' is mentioned in the '{title}'.".format(
             entity=self.start_node().text,
             title=self.end_node().title)
 
 
 class RefersTo(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge, Uncertain):
     '''
-    RefersTo edges connects an extracted Entity node to the ReferenceNode that is it believed
+    RefersTo edges connects an extracted Entity node to the ReferenceNode that it is believed
     to represent with the uncertainity value provided. 
     '''
     def to_text(self) -> str:
         return "The entity '{entity}' {uncertainty} refers to '{ref}'.".format(
             entity=self.start_node().text,
             ref=self.end_node().text,
             uncertainty=self.uncertainty_to_text())
 
 
 class Entity(nm.StructuredNode, OpenTldrText, OpenTldrMeta, OpenTldrNode):
     '''
     Entity nodes represent specific things that are "mentioned_in" in Citable nodes 
     (e.g., Content or Requests) that "refers_to" some ReferenceNode information. The text property
-    contains the text for the entity identified and they type property expresses what it is.
+    contains the text for the entity identified and the type property expresses what it is.
     The "refers_to" edge can be uncertain (e.g., sematic similarity of text and type consistency). 
     '''
     refers_to=nm.RelationshipTo(ReferenceNode,'REFERS_TO', model = RefersTo, cardinality=ZeroOrMore)  
     mentioned_in = nm.RelationshipTo("CitableNode", 'MENTIONED_IN', model=MentionedIn, cardinality=OneOrMore)
 
     def get_refers_to(self) -> list[Source]:
         return self.refers_to
@@ -442,14 +440,15 @@
     '''
 
     def to_text(self) -> str:
         return "The request '{request}' was requested by {user}.".format(
             request=self.start_node().title,
             user=self.end_node().name)
 
+
 class Request(CitableNode, OpenTldrMeta, OpenTldrNode):
     '''
     Request nodes information requests that are made by users to indicate what information they
     are interested in and how to tailor that information for them. A "text" property (String) 
     holds the text of the information request and the "title" property (String) provides a 
     short labels for the request to avoid repeating long request text. The "requested_by" edge
     links each request to one User node.
@@ -464,25 +463,24 @@
 
     def to_text(self) -> str:
         return "The request titled '{title}'.".format(title=self.title)
 
     def to_json_connect(self, kg, json_dict) -> dict:
         out:dict= {}
         user:User = self.requested_by.single()
-        log.warn("USER: {}".format(user))
-
+        
         if "user" not in json_dict:
             out["user"]=user.name
         if "email" not in json_dict:
             out["email"]=user.email
 
         return out
 
     def from_json_connect(self, kg, json_dict):
-        # Ensure there is an requested_by relation
+        # Ensure there is a requested_by relation
         if "user" in json_dict:
             user=kg.get_user_by_name(json_dict["user"])
             if user is None:
                 email="unknown"
                 if "email" in json_dict:
                     email = json_dict["email"]
                 user=kg.add_user(json_dict["user"],email)
@@ -577,15 +575,15 @@
     to be used in that part of the TLDR.
     '''
     pass
 
 
 class BasedOn(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    BasedOn edges connect a TldrEntry node to a Recommendation ndoe to indicate why that
+    BasedOn edges connect a TldrEntry node to a Recommendation node to indicate why that
     entry is being included in the TLDR and may be used for things like ordering the entries
     to show the most recommended first.
     '''
     pass
 
 
 class TldrEntry(nm.StructuredNode, OpenTldrMeta, OpenTldrNode):
@@ -613,24 +611,24 @@
             content_type= self.includes.single().summarizes.single().type,
             request= self.based_on.single().relates_to.single().title,
             score=self.based_on.single().score_to_text())
 
 
 class Contains(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge, Scored):
     '''
-    connects a Tldr to each of the TldrEntry objects that is make it up. The assumption
-    here is that the score property (float 0.0 - 1.0) on the edge provides a decending ordering for
+    Connects a Tldr to each of the TldrEntry objects that makes it up. The assumption
+    here is that the score property (float 0.0 - 1.0) on the edge provides a descending ordering for
     the entries connected by these links.
     '''
     pass
 
 
 class ResponseTo(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    ResponseTo edges connect a Tldr to the Request for which is was generated.
+    ResponseTo edges connect a Tldr to the Request for which it was generated.
     '''
     pass
 
 
 class Tldr(nm.StructuredNode, OpenTldrMeta, OpenTldrNode):
     '''
     Tldr nodes represent an instance of the TLDR report for the date (in 'date' property of type
@@ -659,76 +657,84 @@
 
 
 # FEEDBACK
 
 
 class FeedbackForEntry(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    edges connect a Feedback to the TLDR Entry for which is was generated.
+    Edges connect a Feedback to the TLDR Entry for which it was generated.
     '''
-    pass
+    pass #TODO: complete this methods
 
 
 class FeedbackForRequest(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    edges connect a Feedback to the Request for which is was generated.
+    Edges connect a Feedback to the Request for which it was generated.
     '''
-    pass
+    pass #TODO: complete this method
 
 
 class Feedback(nm.StructuredNode, OpenTldrMeta, OpenTldrNode, Scored):
     '''
-    Feedback relatest events back to a Request node to TldrEntry node to provide a method for
+    Feedback relates events back to a Request node to TldrEntry node to provide a method for
     storing events (for example giving it stars or logging accessing the source article)
     
-    Feedback score ("score" property is float with expected range of 0.0 - 1.0) to indicating
+    Feedback score ("score" property is float with expected range of 0.0 - 1.0) indicating
     how relevant that entry is with respect to the request. These edges are generally created
     by the UI when the user rates an entry (e.g., clicking on a star rating).
+
+    Feedback clicked ("clicked" property is a date) indicates when the last time the source
+    link for the TLDR entry was clicked by the user.
     '''
-    date = nm.DateProperty(required=True)
-    events = nm.JSONProperty(required=True)
+    click_date = nm.DateProperty(required=False)
 
-    feedback_for_entry = nm.RelationshipTo(Content, 'FEEDBACK_FOR_ENTRY', model=FeedbackForEntry, cardinality=One)
-    feedback_for_request = nm.RelationshipTo(Request, 'FEEDBACK_FOR_REQUEST', model=FeedbackForRequest, cardinality=One)
+    about_entry = nm.RelationshipTo(TldrEntry, 'ABOUT', model=FeedbackForEntry, cardinality=One)
+    from_request = nm.RelationshipTo(Request, 'FROM', model=FeedbackForRequest, cardinality=One)
     
-    def to_text(self) -> str:
-        return "The feedback for the entry '{entry}' for the request '{request}' is {amount}.".format(
-            content = self.key_for_content.single().to_text(),
-            request = self.key_for_request.single().to_text(),
-            amount = self.score_to_text())
-
+    def to_text(self) -> str:   
+        click_status = "not clicked"
+        if self.click_date is not None:
+            click_status= "clicked on {date}".format(date=self.click_date.strftime("%m/%d/%Y"))
+        
+        rate_status = "unrated"
+        if self.score is not None:
+            rate_status = "rated as {rate}".format(rate=self.score_to_text())
+
+        return "The feedback is that entry '{entry}' was {rate_status} and {click_status}.".format(
+                content = self.key_for_content.single().to_text(),
+                rate_status = rate_status,
+                click_status = click_status);
+       
 
 # EVALUATION 
 
 
 class KeyForContent(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    edges connect a EvaluationKey to a Content node.
+    Edges connect a EvaluationKey to a Content node.
     '''
-    pass
+    pass #TODO: complete this method
 
 
 class KeyForRequest(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
-    edges connect a EvaluationKey to a Request.
+    Edges connect a EvaluationKey to a Request.
     '''
-    pass
+    pass #TODO: complete this method
 
 
 class EvalKey(nm.StructuredNode, OpenTldrMeta, OpenTldrNode, Scored):
     '''
     EvalKey is an indication of the relationship between a Content (e.g., a news article) and a
     Request (i.e., what the user is interested in). This represents a "correct" tailoring pair.
     This also includes a score and text to help identify what was most relevant in the pair.
     '''
     text = nm.StringProperty(required=True)
     key_for_content = nm.RelationshipTo(Content, 'KEY_FOR_CONTENT', model=KeyForContent, cardinality=One)
     key_for_request = nm.RelationshipTo(Request, 'KEY_FOR_REQUEST', model=KeyForRequest, cardinality=One)
-    
-    
 
     def to_json_connect(self, kg, json_dict) -> dict:
         out:dict= {}
         if "request" not in json_dict:
             out["request"]=self.key_for_request.single().title
         if "content" not in json_dict:
             out["content"]=self.key_for_content.single().title
```

### Comparing `opentldr-0.4.3/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.0/src/opentldr/FileSystemDataRepo.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 
 class FileSystemDataRepo(AbstractDataRepo):
     '''
     Reads all the text files in the provided directory path. Creates a Source node for the directory and parses the text files.
     This extracts lines with property definitions (e.g., "date: 05/14/1960 08:00PM") and puts the rest into the text body.
     Creates a Content node, for each file and adds it to the knowledge graph.
     '''
-    ingest_path:str = "."
-    files:list[str] = []
 
-    def __init__(self, kg:KnowledgeGraph, ingest_path="."):
+    def __init__(self, kg:KnowledgeGraph, ingest_path="."):     # TODO: "." seems like a bad default. "files" would be better.
         self.kg=kg
         self.ingest_path = ingest_path
         self.files=self.getAllFiles(ingest_path)
 
 
     def describe(self) -> str:
         return "File system at ('{path}') contains {n} files.".format(path=self.ingest_path, n=len(self.files))  
@@ -41,14 +39,15 @@
             if not os.path.exists(current):
                 log.debug("Doesn't exist: {name}.".format(name=current))
             
             if not os.access(current,os.R_OK):
                 log.warning("Cannot read: {name}.".format(name=current))
             return []    
 
+    # TODO: Move repeated method to superclass
     def _importByClass(self,raw:dict,clazz:str) -> list[str]:
         list_of_uids=[]
         if clazz in raw:
             for item in raw[clazz]:
                 item['class']=clazz
                 o = dictToKg(self.kg,item)
                 list_of_uids.append(o.uid)
```

### Comparing `opentldr-0.4.3/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.0/src/opentldr/KnowledgeGraph.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 
 class KnowledgeGraph:
     '''
     KnowledgeGraph is the API for OpenTLDR's interface to Neo4j graph database. It attempts to make the
     driver connection using OS, .env, and then default values for connections. This API maps neo4j
     nodes/edges to types specified in the Domain module (using Neomodel OGM and some custom cypher).
 
-    In order to be successfull, you will need to have a neo4j server running, reachable on the network,
+    In order to be successful, you will need to have a neo4j server running, reachable on the network,
     and with environment variables (either in OS or .env files) similar to these:
 
         NEO4J_CONNECTION='bolt://localhost:7687'
         NEO4J_USERNAME=neo4jUser
         NEO4J_PASSWORD=neo4jPassword
         NEO4J_DATABASE=neo4j
 
     This class can be used in several different ways, including:
         (1) import opentldr.KnowledgeGraph ... kg=KnowledgeGraph() ... (use kg here) ... kg.close() 
         (2) with opentldr.KnowledgeGraph as kg: ... (use kg here, and then it will autoclose)
 
     '''
 
-# -----------------
-# Setup Methods
-# -----------------
+    # -----------------
+    # Setup Methods
+    # -----------------
 
     # Default values come from first of: (1) .env file, (2) os environment, or (3) these hardcoded values
     connection=_getenv('NEO4J_CONNECTION','neo4j://localhost:7687')
     user= _getenv('NEO4J_USERNAME','neo4j')
     password= _getenv('NEO4J_PASSWORD','neo4jPassword')
     database= _getenv('NEO4J_DATABASE','neo4j')
     driver = GraphDatabase.driver(connection, auth=(user,password))
@@ -65,15 +65,15 @@
         if database is not None:
             self.database=database
          
         if neo4j_driver is None:        
             log.info("Connecting to Neo4J using environment specification.")
             log.info("\tconnection:\t{v}".format(v=self.connection))
             log.info("\tuser:\t\t{v}".format(v=self.user))
-            #log.info("\tpassword:\t{v}".format(v=self.password))
+            #log.info("\tpassword:\t{v}".format(v=self.password))           # don't display sensitive information
             log.info("\tdatabase:\t{v}".format(v=self.database))
             self.connect()
         else:
             log.info("Using Neo4j driver passed into initialization.")
             self.connect(neo4j_driver)
 
     def __del__(self):
@@ -83,48 +83,48 @@
     def __enter__(self):
         return self
     
     def __exit__(self,ctx_type, ctx_value, ctx_traceback):
         if self.driver is not None:
             self.driver.close()
 
-# -----------------
-# General Utility Methods
-# -----------------
+    # -----------------
+    # General Utility Methods
+    # -----------------
 
     def neo4j_query(self, cql):
         '''
-        performs a cypher call to the knowledge base and returns results in the standard neo4j driver format.
+        Performs a cypher call to the knowledge base and returns results in the standard neo4j driver format.
         Use this if you are following neo4j documentation, otherwise use cypher_query().
         '''
         if self.driver == None:
             self.connect()
 
         try:
             records, summary, keys = self.driver.execute_query(cql, database_=self.database,)
             log.info("The query `{query}` returned {records_count} records in {time} ms.".format(
                 query=summary.query, records_count=len(records),
                 time=summary.result_available_after))
             return records, summary
         except Exception as e:
             log.error(e)
 
-    def neomodel_query(self,cypher_query):
+    def neomodel_query(self,cypher_query, params: dict={}):
         '''
-        performs a cypher query in the standard neomodel method, which will return a list of lists of neomodel.
+        Performs a cypher query in the standard neomodel method, which will return a list of lists of neomodel.
         Use this if you are following Neomodel documentation, otherwise use cypher_query().
         '''
         if self.driver == None:
             self.connect()
         
-        return nm.db.cypher_query(cypher_query, resolve_objects = True)
+        return nm.db.cypher_query(cypher_query, resolve_objects=True, params=params)
 
     def connect(self, driver=None):
         '''
-        ensures that a connection to Neo4j has been established and is functioning.
+        Ensures that a connection to Neo4j has been established and is functioning.
         '''
         try:
             if driver==None:
                 driver = GraphDatabase.driver(self.connection, auth=(self.user,self.password))
             
             log.info("Testing Neo4j Connectivity...")
             driver.verify_connectivity()
@@ -149,24 +149,24 @@
         except Exception as e:
             log.error(e)
             log.error("There was an issue connecting to Neo4J server, please verify that it is running and configured correctly.")            
             raise e
     
     def getNeo4jDriver(self):
         '''
-        returns the Neo4j driver class being used (usually neo4j.GraphDatabase.driver) so that direct neo4j calls can be
+        Returns the Neo4j driver class being used (usually neo4j.GraphDatabase.driver) so that direct neo4j calls can be
         made or it can be passed into other libraries.
         '''
         if self.driver==None:
             self.connect()
         return self.driver
 
     def close(self):
         '''
-        shutsdown the current connection to neo4j. This should be done as the end of each program / notebook.
+        Shuts down the current connection to neo4j. This should be done at the end of each program / notebook.
         If you use the "with statement" context control, this will be called automatically when the code block ends.
         '''
         if self.driver!=None:
             self.driver.close()
         self.driver=None
 
     def _ensure_saved(self,node:OpenTldrMeta):
@@ -175,91 +175,92 @@
         So, we can use this to determine if an object has been saved or not and respond appropriately.
         '''
         if node.uid is None:
             log.warn("Nodes must be persisted with node.save() before being connected. Forcing this now.")
             return node.save()
         return node
 
-    def get_all_node_uids_by_tag(self, tag:str ) -> list[str]:
+    def get_all_node_uids_by_tag(self, tag:str) -> list[str]:
         '''
-        returns the list of uids for the tag specified as a string.
+        Returns the list of uids for the tag specified as a string.
         '''
         return self.cypher_query("MATCH (n:{tag}) RETURN n.uid".format(tag=tag))
 
-    def get_all_nodes_by_tag(self, tag:str ):
+    def get_all_nodes_by_tag(self, tag:str):
         '''
-        returns the list of uids for the tag specified as a string.
+        Returns the list of uids for the tag specified as a string.
         '''
         return self.cypher_query("MATCH (n:{tag}) RETURN n".format(tag=tag),"n")
 
+    # -----------------
+    # KnowedgeGraph API
+    # -----------------
 
-# -----------------
-# KnowedgeGraph API 
-# -----------------
-
-    def cypher_query(self,cypher_query,extract_variable=None) ->list:
+    def cypher_query(self,cypher_query, extract_variable=None, params: dict={}) -> list:
         '''
-        performs a cypher query and returns a single simple list of Neomodel objects based on the variable indicated (or first).
+        Performs a cypher query and returns a single simple list of Neomodel objects based on the variable indicated (or first).
         Use this for most OpenTLDR queries because it is much simpler to process for iterating on the results.
         For example: cypher_query("MATCH (a)-[b]->(c) RETURN a,b,c","a") only returns a list of only the "a" results.
         So, cypher_query("MATCH (a)-[b]->(c) RETURN a","a") would give the same result list by dropping the "b" and "c" results.
+        Reduce the risk of Cypher injection attacks by passing Cypher parameters in params.
         '''
         if self.driver == None:
             self.connect()
         
-        results, meta = nm.db.cypher_query(cypher_query, resolve_objects = True)
+        results, meta = nm.db.cypher_query(cypher_query, resolve_objects=True, params=params)
         
         index=0
         if extract_variable is not None:
             index=meta.index(extract_variable)
         else:
             if len(meta)>1:
                 log.warn("cypher_query is defaulting to return the first element of multiple return values in results.")      
 
         return [item[index] for item in results]
 
-    def cypher_query_one(self,cypher_query,extract_variable=None):
+    def cypher_query_one(self,cypher_query,extract_variable=None, params: dict={}):
         '''
-        performs a query that is intended to LIMIT the return values to one single Neomodel object. This simplifies the processing
+        Performs a query that is intended to LIMIT the return values to one single Neomodel object. This simplifies the processing
         of the query results to consistently only get a single object for the extract_variable, it is undefined which unless you sort them.
         For example: cypher_query_one("MATCH (a)-[b]->(c) RETURN a,b,c","a") returns the FIRST object of result "a".
         So, cypher_query_one("MATCH (a)-[b]->(c) RETURN a LIMIT 1","a") gives the same result (faster).
-        '''
-        results = self.cypher_query(cypher_query,extract_variable)
+        Reduce the risk of Cypher injection attacks by passing Cypher parameters in params.
+       '''
+        results = self.cypher_query(cypher_query,extract_variable, params=params)
 
         # Limits the output to the first actual object (i.e., not a list)        
         if results is not None and len(results)>0:
             return results[0]
         else:
             return None  
         
     def cypher_import(self,filename):
         '''
-        processes a text file containing cypher commands and executes them on the KnowledgeGraph.
+        Processes a text file containing cypher commands and executes them on the KnowledgeGraph.
         '''
         count=0
         with open(filename) as fp:
             lines = fp.readlines()
             for line in lines:
                 if len(line.strip()) == 0:
-                    continue;   
+                    continue
                 with self.driver.session() as session:
                     session.run(line)
                 count=count+1
         log.info("Imported {count} lines of Cypher from {filename}".format(count=count, filename=filename))
 
     def delete_all(self):
         '''
-        clears the neo4j graph database.
+        Clears the neo4j graph database.
         '''
         self.cypher_query("MATCH(x) DETACH DELETE x")
 
     def shortest_path(self,start:OpenTldrMeta,end:OpenTldrMeta):
         '''
-        this is a special cypher command to run neo4j's shortest path algorithm and return the path (list of edges) found.
+        This is a special cypher command to run neo4j's shortest path algorithm and return the path (list of edges) found.
         We remove EvalKey, Recommendation, Tldr, Source, and User nodes to avoid irrelevant paths that circumvent Reference Data.
         '''
         results,meta = self.neomodel_query("""
             MATCH path=shortestPath((s)-[*..10]-(e))
             WHERE s.uid='{start_id}'
             AND e.uid='{end_id}'                         
             AND NONE(n IN nodes(path) WHERE 'Recommendation' IN LABELS(n))
@@ -272,189 +273,210 @@
                      
         if len(results) == 0:
             return None
         else:
             return results[0][meta.index("path")]
 
     def get_by_uid(self, uid:str):
-        return self.cypher_query_one("MATCH (n) WHERE n.uid='{uid}' RETURN n".format(uid=uid))
+        return self.cypher_query_one("MATCH (n) WHERE n.uid=$uid RETURN n", params={"uid": uid})
 
-# -----------------
-# Reference Data API
-# -----------------
+    # -----------------
+    # Reference Data API
+    # -----------------
+
+    ## Reference Nodes in KG are labeled as ReferenceNode
 
-## Reference Nodes in KG these are labeled as ReferenceNode
-         
     def add_reference_node(self, text:str, type:str, hypothesized:bool=False) -> ReferenceNode:
         '''
-        creates a new ReferenceNode object in KG.
+        Creates a new ReferenceNode object in KG.
         '''
         return ReferenceNode(text=text, type=type, hypothesized=hypothesized).save()
     
+    def get_reference_node_by_uid(self,uid:str) -> ReferenceNode:
+        '''
+        Returns a single ReferenceNode as indicated by the uid or None if it does not exist in KG.
+        '''
+        return ReferenceNode.nodes.get_or_none(uid=uid);
+
+    def get_all_reference_nodes(self) -> list[ReferenceNode]:
+        '''
+        Returns a list of all the ReferenceNodes in the KG.
+        '''
+        return self.cypher_query("MATCH (n:ReferenceNode) RETURN n","n")
+
     def update_reference_node(self, node:ReferenceNode) -> ReferenceNode:
         '''
-        updates the KG with changes to a ReferenceNode properties
+        Updates the KG with changes to a ReferenceNode properties
         '''
         return node.save()
     
     def delete_reference_node(self, node:ReferenceNode):
         '''
-        removes the passed ReferenceNode and the edges connected to them.
+        Removes the passed ReferenceNode and the edges connected to them.
         '''
-        self.cypher_query("MATCH (n:ReferenceNode) WHERE n.uid='{uid}' DETACH DELETE n".format(uid=node.uid))
+        self.cypher_query("MATCH (n:ReferenceNode) WHERE n.uid=$uid DETACH DELETE n", params={"uid": node.uid})
    
     def delete_all_reference_nodes(self):
         '''
-        removes all of the ReferenceNode and the edges connected to them.
+        Removes all of the ReferenceNode and the edges connected to them.
         '''
         self.cypher_query("MATCH (n:ReferenceNode) DETACH DELETE n")
 
     def get_reference_node_by_uid(self,uid:str) -> ReferenceNode:
         '''
-        returns a single ReferenceNode as indicated by the uid or None if it does not exist in KG.
+        Returns a single ReferenceNode as indicated by the uid or None if it does not exist in KG.
         '''
         return ReferenceNode.nodes.get_or_none(uid=uid);
 
     def get_all_reference_nodes(self) -> list[ReferenceNode]:
         '''
-        returns a list of all the ReferenceNodes in the KG.
+        Returns a list of all the ReferenceNodes in the KG.
         '''
         return self.cypher_query("MATCH (n:ReferenceNode) RETURN n","n")
 
-## Reference Edges - in KG these are labeled as REFERENCE_EDGE but Neomodel classes are ReferenceEdge
-    
+      
+  ## Reference Edges - in KG these are labeled as REFERENCE_EDGE but Neomodel classes are ReferenceEdge
+
+
     def add_reference_edge(self, from_node:ReferenceNode, to_node:ReferenceNode, text:str, type:str, hypothesized:bool=False):
         '''
-        adds a ReferenceEdge between two ReferenceNodes. Note these edges are only between ReferenceNodes.
+        Adds a ReferenceEdge between two ReferenceNodes. Note these edges are only between ReferenceNodes.
         '''
         from_node:ReferenceNode=self._ensure_saved(from_node)
         to_node:ReferenceNode=self._ensure_saved(to_node)
         edge=from_node.edges.connect(to_node,{'type':type, 'text':text, 'hypothesized':hypothesized})
         return edge.save()
     
-    def update_reference_edge(self, edge:ReferenceEdge) -> ReferenceEdge:
+    def get_reference_edge_by_uid(self,uid:str) -> ReferenceEdge:
         '''
-        updates the KG with changes to a ReferenceEdge's properties
+        Returns a single ReferenceEdge as indicated by the uid or None if it does not exist in KG.
         '''
-        return edge.save()
+        self.cypher_query_one("MATCH (a)-[r:REFERENCE_EDGE]->(b) WHERE r.uid=$uid RETURN r", params={"uid": uid})
 
-    def delete_reference_edge(self, edge:ReferenceEdge):
+    def get_all_reference_edges(self) -> list[ReferenceEdge]:
         '''
-        removes all ReferenceNode and the edges connected to them.
+        Returns a list of all of the ReferenceEdges in the KG.
         '''
-        self.cypher_query("MATCH (a)-[r:REFERENCE_EDGE]->(b) WHERE r.uid='{uid}' DETACH DELETE r".format(uid=edge.uid))
+        return self.cypher_query("MATCH (a)-[n:REFERENCE_EDGE]->(b) RETURN n","n")
 
-    def delete_all_reference_edges(self):
+    def update_reference_edge(self, edge:ReferenceEdge) -> ReferenceEdge:
         '''
-        removes all of the ReferenceEdges from KG.
+        Updates the KG with changes to a ReferenceEdge's properties
         '''
-        self.cypher_query("MATCH (a)-[r:REFERENCE_EDGE]->(b) DETACH DELETE r")
+        return edge.save()
 
-    def get_reference_edge_by_uid(self,uid:str) -> ReferenceEdge:
+    def delete_reference_edge(self, edge:ReferenceEdge):
         '''
-        returns a single ReferenceEdge as indicated by the uid or None if it does not exist in KG.
+        Removes the ReferenceEdge.
         '''
-        self.cypher_query_one("MATCH (a)-[r:REFERENCE_EDGE]->(b) WHERE r.uid='{uid}' RETURN r".format(uid=uid))
+        self.cypher_query("MATCH (a)-[r:REFERENCE_EDGE]->(b) WHERE r.uid=$uid DETACH DELETE r", params={"uid": edge.uid})
 
-    def get_all_reference_edges(self) -> list[ReferenceEdge]:
+    def delete_all_reference_edges(self):
         '''
-        returns a list of all of the ReferenceEdges in the KG.
+        Removes all of the ReferenceEdges from KG.
         '''
-        return self.cypher_query("MATCH (a)-[n:REFERENCE_EDGE]->(b) RETURN n","n")
+        self.cypher_query("MATCH (a)-[r:REFERENCE_EDGE]->(b) DETACH DELETE r")
 
-# -----------------
-# Active Data
-# -----------------
+    # =================
+    # Active Data
+    # =================
+
+    # -----------------
+    # Source Nodes - refer to the origin of content
+    # -----------------
 
-## Source Nodes - refer to the origin of content
-        
     def add_source(self, name:str) -> Source:
         '''
-        creates new source node, or if one by the same name already exists it reuses it.
+        Creates new Source node, or if one by the same name already exists it reuses it.
         '''
         source = Source.nodes.get_or_none(name=name)
         if source is None:
             source= Source(name=name).save()
         else:
             log.warn("Found existing Source node for name {name}, returning pre-existing node.".format(name=name))
         return source
-    
+
+    def get_source_by_uid(self, uid: str) -> Source:
+        '''
+        Gets an existing Source node by uid or None if it does not exist
+        '''
+        return Source.nodes.get_or_none(uid=uid)
+
+    def get_source_by_name(self, name: str) -> Source:
+        '''
+        Gets an existing Source node by name or None if it does not exist
+        '''
+        return Source.nodes.get_or_none(name=name)
+
+    def get_all_sources(self) -> list[Source]:
+        return Source.nodes
+
     def update_source(self, node:Source) -> Source:
         '''
-        updates the KG with changes to a Source properties
+        Updates the KG with changes to a Source's properties.
         '''
         return node.save()
     
     def delete_source(self, node:Source):
         '''
-        removes the passed Source node and the edges connected to them.
+        Removes the passed Source node and the edges connected to it.
         '''
-        self.cypher_query("MATCH (n:Source) WHERE n.uid='{uid}' DETACH DELETE n".format(uid=node.uid))
+        self.cypher_query("MATCH (n:Source) WHERE n.uid=$uid DETACH DELETE n", params={"uid": node.uid})
    
     def delete_all_sources(self):
         '''
-        removes all of the Sources and the edges connected to them.
+        Removes all of the Sources and the edges connected to them.
         '''
         self.cypher_query("MATCH (n:Source) DETACH DELETE n")
 
-    def get_source_by_uid(self, uid:str) -> Source:
-        '''
-        gets an existing Source node by uid or None if it does not exist
-        '''
-        return Source.nodes.get_or_none(uid=uid)
-    
-    def get_source_by_name(self, name:str) -> Source:
-        '''
-        gets an existing Source node by name or None if it does not exist
-        '''
-        return Source.nodes.get_or_none(name=name)
-    
-    def get_all_sources(self) -> list[Source]:
-        return Source.nodes
-
-## Content Nodes - contain article content and link to their Source
+    # -----------------
+    # Content Nodes - contain article content and link to their Source
+    # -----------------
 
     def add_content(self, source:Source, type:str, url:str, date:datetime.date, title:str, text:str) -> Content:
         content = Content.nodes.get_or_none(url=url)
         if content is None:
             content=Content(url=url,date=date,title=title,text=text, type=type).save()
             content.is_from.connect(source)
         else:
             log.warn("Found existing Content node for url {url}, returning pre-existing node.".format(url=url))
         return content
 
-    def get_all_content(self) -> list[Content]:
-        content = Content.nodes
-        return content
-
     def get_content_by_uid(self, uid:str) -> Content:
         content = Content.nodes.get_or_none(uid=uid)
         return content
 
+    def get_content_by_title(self, title: str) -> Request:
+        return self.cypher_query_one("""
+            MATCH (c:Content) WHERE c.title=$title 
+            RETURN c """,
+            "c", params={"title": title})
+
     def get_content_by_url(self, url:str) -> Content:
         content = Content.nodes.get_or_none(url=url)
         return content
 
-    def get_content_by_source(self,source:Source) -> list[Content]:
-        return source.get_content()
-    
     def get_content_by_date(self,date:datetime.date) -> list[Content]:
         content = Content.nodes.get_or_none(date=date)
         return content
-    
-    def get_content_by_title(self,title:str) -> Request:
-       return self.cypher_query_one("""
-            MATCH (c:Content) WHERE c.title='{title}'
-            RETURN c """.format(title=title),"c")
-    
+
+    def get_content_by_source(self,source:Source) -> list[Content]:
+        return source.get_content()
+
     def get_content_by_recommendation(self,recommendation:Recommendation) -> list[Content]:
         return recommendation.get_content()
-    
-# Active Data / Entity
-    
+
+    def get_all_content(self) -> list[Content]:
+        content = Content.nodes
+        return content
+
+    # -----------------
+    # Active Data / Entity
+    # -----------------
+
     def add_entity(self, content:Content, text:str, type:str ) -> Entity:
         entity=Entity(text=text,type=type).save()
         entity.mentioned_in.connect(content)
         return entity
     
     def add_refers_to_edge(self, entity:Entity, reference:ReferenceNode, confidence=1.0 ):
         entity.refers_to.connect(reference, {'confidence': confidence })
@@ -463,35 +485,42 @@
         entities = Entity.nodes.get_or_none(uid=uid)
         return entities
      
     def get_entity_by_url(self, url:str) -> Entity:
         entities = Entity.nodes.get_or_none(url=url)
         return entities
     
-    def get_all_entities(self) -> list[Entity]:
-        entities = Entity.nodes
-        return entities
-
     def get_entities_by_content(self,content:Content) -> list[Entity]:
         return self.cypher_query("""
-            MATCH (c:Content) WHERE c.uid='{content_uid}'
+            MATCH (c:Content) WHERE c.uid=$content_uid
             MATCH (e:Entity)
             MATCH (e)-[y:MENTIONED_IN]->(c)
-            RETURN e """.format(
-                content_uid=content.uid),"e")
+            RETURN e """,
+            "e", params={"content_uid": content.uid})
 
-    def get_content_by_date(self,date:datetime.date) -> list[Content]:
-        content = Content.nodes.get_or_none(date=date)
-        return content
+    def get_entities_by_request(self,request:Request) -> list[Entity]:
+        return self.cypher_query("""
+            MATCH (r:Request) WHERE r.uid=$request_uid
+            MATCH (e:Entity)
+            MATCH (e)-[y:MENTIONED_IN]->(r)
+            RETURN e """,
+            "e", params={"request_uid": request.uid})
+
+    def get_all_entities(self) -> list[Entity]:
+        entities = Entity.nodes
+        return entities
 
-# -----------------
-# Requests API 
-# -----------------
+    # -----------------
+    # Requests API
+    # -----------------
+
+    # -----------------
+    # Users
+    # -----------------
 
-# Users
 
     def add_user(self, name:str, email:str) -> User:
         user = User.nodes.get_or_none(name=name)
         if user is None:
             user=User(name=name, email=email).save()
         else:
             log.warn("Found existing User node for name {name}, returning pre-existing node.".
@@ -506,68 +535,76 @@
         user = User.nodes.get_or_none(name=name)
         return user
     
     def get_all_users(self) -> list[User]:
         users = User.nodes
         return users
 
+    # -----------------
+    # Requests
+    # -----------------
 
-# Requests
-    
     def add_request(self, title:str, text:str, user:User) -> Request:
         request = Request.nodes.get_or_none(title=title)
         if request is None or request.requested_by.single().uid != user.uid:
             request = Request(title=title, text=text).save()
             request.requested_by.connect(user)
         else:
             log.warn("Found existing Request node for {title}, returning pre-existing node.".format(title=title))
         return request
 
     def get_request_by_uid(self, uid:str) -> Request:
         request = Request.nodes.get_or_none(uid=uid)
         return request
 
-    def get_request(self, name:str) -> Request:
-        request = Request.nodes.get_or_none(name=name)
-        return request
-    
-    def get_all_requests(self) -> list[Request]:
-        requests = Request.nodes
-        return requests
-    
-    def get_requests_by_user_uid(self,uid:str) -> list[Request]: 
+    def get_requests_by_user(self, user: User) -> list[Request]:
+        return self.get_requests_by_user_uid(user.uid)
+
+    def get_requests_by_user_uid(self, uid: str) -> list[Request]:
         return self.cypher_query("""
-            MATCH (u:User) WHERE u.uid='{user_id}'
+            MATCH (u:User) WHERE u.uid=$user_id
             MATCH (q:Request)
             MATCH (q)-[y:REQUESTED_BY]->(u)
-            RETURN q """.format(
-                user_id=uid),"q")
-    
-    def get_requests_by_user(self,user:User) -> list[Request]:
-       return self.get_requests_by_user_uid(user.uid)
-    
+            RETURN q """,
+            "q", params={"user_id": uid})
+
     def get_request_by_title(self,title:str) -> Request:
        return self.cypher_query_one("""
-            MATCH (q:Request) WHERE q.title='{title}'
-            RETURN q """.format(title=title),"q")
+            MATCH (q:Request) WHERE q.title=$title
+            RETURN q """,
+            "q", params={"title": title})
 
-    def get_entities_by_request(self,request:Request) -> list[Entity]:
+    def get_all_requests(self) -> list[Request]:
+        requests = Request.nodes
+        return requests
+
+    def delete_request(self,request:Request):
+        return self.delete_entities_by_request_uid(request.uid)
+    
+    def delete_request_by_uid(self,request_uid:str):
+        self.delete_entities_by_request_uid(request_uid)
+        return self.cypher_query("""
+            MATCH (r:Request) WHERE r.uid=$uid
+            DETACH DELETE (r) """, params={'uid':request_uid})
+    
+    def delete_entities_by_request_uid(self,request_uid:str):
         return self.cypher_query("""
-            MATCH (r:Request) WHERE r.uid='{request_uid}'
+            MATCH (r:Request) WHERE r.uid=$uid
             MATCH (e:Entity)
             MATCH (e)-[y:MENTIONED_IN]->(r)
-            RETURN e """.format(
-                request_uid=request.uid),"e")
-
-# -----------------
-# Workflow Products API 
-# -----------------
-
-# Recommedations
+            DETACH DELETE (e)""", params={'uid':request_uid})
     
+    # -----------------
+    # Workflow Products API
+    # -----------------
+
+    # -----------------
+    # Recommendations
+    # -----------------
+
     def add_recommendation(self, score:float, content:Content, request:Request) -> Recommendation:
         if content.uid is None or request.uid is None:
             log.error("Adding Recommendation requires an existing and saved Content and Request node. Attempting to save them...")
             content.save()
             request.save()
         
         recommendation = self.get_recommendation(content,request)
@@ -575,206 +612,275 @@
             recommendation= Recommendation(score=score).save()
             recommendation.recommends.connect(content)
             recommendation.relates_to.connect(request)
         else:
             log.warn("Found existing Recommendation node between content and request, returning pre-existing node.")
         return recommendation
     
+    def get_recommendation(self, content:Content, request:Request) -> Recommendation:
+        return self.cypher_query_one("""
+            MATCH (q:Request) WHERE q.uid=$request_id
+            MATCH (a:Content) WHERE a.uid=$content_id
+            MATCH (r:Recommendation)
+            MATCH (r)-[x:RECOMMENDS]->(a)
+            MATCH (r)-[y:RELATES_TO]->(q)
+            RETURN r LIMIT 1 """,
+            "r", params={
+                "request_id": request.uid,
+                "content_id": content.uid})
+
     def get_recommendation_by_id(self, uid:str) -> Recommendation:
         recommendation = Recommendation.nodes.get_or_none(uid=uid)
         return recommendation
 
-    def get_recommendation(self, content:Content, request:Request) -> Recommendation:      
-        return self.cypher_query_one("""
-            MATCH (q:Request) WHERE q.uid='{request_id}'
-            MATCH (a:Content) WHERE a.uid='{content_id}'
+    def get_recommendations_by_request(self,request:Request) -> list[Recommendation]:
+        return self.cypher_query("""
+            MATCH (q:Request) WHERE q.uid=$request_id
             MATCH (r:Recommendation)
-            MATCH (r)-[x:RECOMMENDS]->(a)
             MATCH (r)-[y:RELATES_TO]->(q)
-            RETURN r LIMIT 1 """.format(
-                request_id=request.uid,
-                content_id=content.uid),"r")  
+            RETURN r ORDER BY r.score DESC """,
+            "r", params={"request_id": request.uid})
+
+    def get_all_recommendations(self) -> list[Recommendation]:
+        recommendations = Recommendation.nodes
+        return recommendations
 
     def delete_recommendation(self, recommendation:Recommendation):
-        recommendation.delete();
+        recommendation.delete()
     
     def delete_all_recommendations(self):
         self.cypher_query("MATCH (r:Recommendation) DETACH DELETE (r)")
          
-    def get_all_recommendations(self) -> list[Recommendation]:
-        recommendations = Recommendation.nodes
-        return recommendations
-    
-    def get_recommendations_by_request(self,request:Request) -> list[Recommendation]:
-        return self.cypher_query("""
-            MATCH (q:Request) WHERE q.uid='{request_id}'
-            MATCH (r:Recommendation)
-            MATCH (r)-[y:RELATES_TO]->(q)
-            RETURN r ORDER BY r.score DESC """.format(
-                request_id=request.uid),"r")
-
+    # -----------------
     # Summaries
-    
+    # -----------------
+
     def add_summary(self, text:str, content:Content, recommendation:Recommendation=None) -> Summary:
         summary = self.get_summary(content,recommendation)
         if summary is None:
             summary= Summary(text=text).save()
             summary.summarizes.connect(content)
             if recommendation is not None:
                 summary.focus_on.connect(recommendation)
         else:
             log.warn("Found existing Summary node, returning pre-existing node.")
         return summary
     
-    def get_summary_by_id(self, uid:str) -> Summary:
-        summary = Summary.nodes.get_or_none(uid=uid)
-        return summary
-
-    def get_summary(self, content:Content, recommendation:Recommendation) -> Summary:      
+    def get_summary(self, content:Content, recommendation:Recommendation) -> Summary:
         return self.cypher_query_one("""
-            MATCH (r:Recommendation) WHERE r.uid='{recommendation_id}'
-            MATCH (a:Content) WHERE a.uid='{content_id}'
+            MATCH (r:Recommendation) WHERE r.uid=$recommendation_id
+            MATCH (a:Content) WHERE a.uid=$content_id
             MATCH (s:Summary)
             MATCH (s)-[x:SUMMARIZES]->(a)
             MATCH (s)-[y:FOCUS_ON]->(r)
-            RETURN s """.format(
-                recommendation_id=recommendation.uid,
-                content_id=content.uid),"s")                 
+            RETURN s """,
+            "s", params={
+                "recommendation_id": recommendation.uid,
+                "content_id": content.uid})
     
-    def get_summaries_by_content(self, content:Content) -> list[Summary]:      
+    def get_summary_by_id(self, uid:str) -> Summary:
+        summary = Summary.nodes.get_or_none(uid=uid)
+        return summary
+
+    def get_summaries_by_content(self, content:Content) -> list[Summary]:
         return self.cypher_query("""
-            MATCH (a:Content) WHERE a.uid='{content_id}'
+            MATCH (a:Content) WHERE a.uid=$content_id
             MATCH (s:Summary)
             MATCH (s)-[x:SUMMARIZES]->(a)
-            RETURN s """.format(content_id=content.uid))                 
+            RETURN s """,
+            params={"content_id": content.uid})
 
     def get_summaries_by_recommendation(self, recommendation:Recommendation) -> list[Summary]:      
         return self.cypher_query("""
-            MATCH (r:Recommendation) WHERE r.uid='{recommendation_id}'
+            MATCH (r:Recommendation) WHERE r.uid=$recommendation_id
             MATCH (s:Summary)
             MATCH (s)-[x:FOCUS_ON]->(r)
-            RETURN s """.format(recommendation_id=recommendation.uid),"s")                 
+            RETURN s """,
+            "s", params={"recommendation_id": recommendation.uid})
 
     def get_all_summary(self) -> list[Summary]:
         summary = Summary.nodes
         return summary
     
-# Tldr
-    
-    def add_tldr(self, request:Request, date:datetime.date) -> Tldr:
+    # -----------------
+    # Tldr
+    # -----------------
+
+    def add_tldr(self, request: Request, date: datetime.date) -> Tldr:
         tldr = self.get_tldr(request, date)
         if tldr is None:
-            tldr= Tldr(date=date).save()
+            tldr = Tldr(date=date).save()
             tldr.response_to.connect(request)
         else:
             log.warn("Found existing Tldr node for request on given date, returning pre-existing node.")
         return tldr
-    
-    def add_entry_to_tldr(self, tldr:Tldr, score:float, recommendation:Recommendation, summary:Summary, content:Content) -> TldrEntry:
-        tldr_entry=TldrEntry(link=content.url).save()
-        tldr_entry.includes.connect(summary)
-        tldr_entry.based_on.connect(recommendation)
-        tldr.contains.connect(tldr_entry, {'score': score })
 
-    def get_tldr_by_uid(self, uid:str) -> Tldr:
+    def get_tldr(self, request: Request, date: datetime.date) -> Tldr:
+        return self.get_tldr_by_uid_and_date(request.uid, date)
+
+    def get_tldr_by_uid(self, uid: str) -> Tldr:
         tldr = Tldr.nodes.get_or_none(uid=uid)
         return tldr
-    
-    def get_tldr_entry_by_uid(self, uid:str) -> Tldr:
-        tldr_entry = TldrEntry.nodes.get_or_none(uid=uid)
-        return tldr_entry
-
-    def delete_tldr_entry(self, tldr_entry:TldrEntry):
-        tldr_entry.delete()
-
-    def delete_tldr(self, tldr:Tldr):
-        for tldr_entry in tldr.contains.all():
-            self.delete_tldr_entry(tldr_entry)
-        tldr.delete()
-
-    def delete_tldr_entries_by_tldr(self, tldr:Tldr):
-        for tldr_entry in tldr.contains.all():
-            self.delete_tldr_entry(tldr_entry)
-
-    def delete_all_tldrs(self):
-        for tldr in Tldr.nodes:
-            self.delete_tldr(tldr)
 
-    def get_tldrs_by_date(self, date:datetime.date):
+    def get_tldrs_by_date(self, date: datetime.date):
         results = self.cypher_query("""
-            MATCH (t:Tldr) WHERE t.date='{date}'
-            RETURN t """.format(date=date),"t")
+            MATCH (t:Tldr) WHERE t.date=$date
+            RETURN t """,
+            "t", params={"date": date})
         if results is None:
             return None
         else:
             return results[0]
 
-    def get_tldrs_before_date(self, date:datetime.date):
+    def get_tldrs_before_date(self, date: datetime.date):
         return self.cypher_query("""
-            MATCH (t:Tldr) WHERE t.date<'{date}'
-            RETURN t """.format(date=date),"t")                 
+            MATCH (t:Tldr) WHERE t.date<$date
+            RETURN t """,
+            "t", params={"date": date})
+
+    def get_tldr_by_request(self, request: Request) -> list[Tldr]:
+        return self.get_tldr_by_request_uid(request.uid)
+
+    def get_tldr_by_request_uid(self, request_uid: str) -> list[Tldr]:
+        return self.cypher_query("""
+            MATCH (q:Request) WHERE q.uid=$request_uid
+            MATCH (t:Tldr)
+            MATCH (t)-[y:RESPONSE_TO]->(q)
+            RETURN t """,
+            "t", params={"request_uid": request_uid})
+
+    def get_tldr_by_uid_and_date(self, request_uid: str, date: datetime.date) -> Tldr:
+        return self.cypher_query_one("""
+            MATCH (q:Request) WHERE q.uid=$request_uid
+            MATCH (t:Tldr) where t.date=$date
+            MATCH (t)-[y:RESPONSE_TO]->(q)
+            RETURN t """,
+            "t", params={
+                "date": date,
+                "request_uid": request_uid})
 
     def get_all_tldrs(self) -> list[Tldr]:
         tldrs = Tldr.nodes
         return tldrs
-    
+
+    def delete_tldr(self, tldr:Tldr):
+        self.delete_tldr_entries_by_tldr(tldr)
+        tldr.delete()
+
+    def delete_all_tldrs(self):
+        for tldr in Tldr.nodes:
+            self.delete_tldr(tldr)
+
+    # -----------------
+    # Tldr Entries
+    # -----------------
+
+    def add_entry_to_tldr(self, tldr:Tldr, score:float, recommendation:Recommendation, summary:Summary, content:Content) -> TldrEntry:
+        tldr_entry=TldrEntry(link=content.url).save()
+        tldr_entry.includes.connect(summary)
+        tldr_entry.based_on.connect(recommendation)
+        tldr.contains.connect(tldr_entry, {'score': score })
+        return tldr_entry
+
+    def get_tldr_entry_by_uid(self, uid:str) -> Tldr:
+        tldr_entry = TldrEntry.nodes.get_or_none(uid=uid)
+        return tldr_entry
+
     def get_entries_by_tldr(self, tldr:Tldr) -> list[TldrEntry]:
         return self.cypher_query("""
-            MATCH (t:Tldr) WHERE t.uid='{tldr_id}'
+            MATCH (t:Tldr) WHERE t.uid=$tldr_id
             MATCH (e:TldrEntry)
             MATCH (t)-[x:CONTAINS]->(e)
-            RETURN e ORDER BY e.score DESC""".format(tldr_id=tldr.uid),"e")                 
+            RETURN e ORDER BY e.score DESC""",
+            "e", params={"tldr_id": tldr.uid})
 
-    def get_tldr_by_request(self,request:Request) -> list[Tldr]:
-        return self.get_tldr_by_request_uid(request.uid)
-    
-    def get_tldr_by_request_uid(self,request_uid:str) -> list[Tldr]:
-        return self.cypher_query("""
-            MATCH (q:Request) WHERE q.uid='{request_uid}'
-            MATCH (t:Tldr)
-            MATCH (t)-[y:RESPONSE_TO]->(q)
-            RETURN t """.format(
-                request_uid=request_uid),"t")
+    def delete_tldr_entry(self, tldr_entry:TldrEntry):
+        tldr_entry.delete()
 
-    def get_tldr_by_uid_and_date(self,request_uid:str, date:datetime.date) -> Tldr:
-        return self.cypher_query_one("""
-            MATCH (q:Request) WHERE q.uid='{request_uid}'
-            MATCH (t:Tldr) where t.date='{date}'
-            MATCH (t)-[y:RESPONSE_TO]->(q)
-            RETURN t """.format( date=date,
-                request_uid=request_uid),"t")
-    
-    def get_tldr(self,request:Request, date:datetime.date) -> Tldr:
-        return self.get_tldr_by_uid_and_date(request.uid, date)
+    def delete_tldr_entries_by_tldr(self, tldr:Tldr):
+        for tldr_entry in tldr.contains.all():
+            self.delete_tldr_entry(tldr_entry)
 
+	#-----------------
+	# Feedback
+	#-----------------
+
+    def add_feedback_click(self, entry:TldrEntry, date:datetime.date) -> Feedback:
+        feedback = self.get_feedback_by_tldr_entry(entry)
+        if feedback is None:
+            feedback= Feedback(click=date).save()
+            feedback.about_entry.connect(entry)
+            request= self.get_requests_by_tldr_entry(entry)
+            feedback.from_request.connect(request)
+        else:
+            feedback.click_date=date
+            feedback.save()
+            log.warn("Updated click date of existing Feedback.")
+
+        return feedback
+
+    def add_feedback_rating(self, entry:TldrEntry, score:float) -> Feedback:
+        feedback = self.get_feedback_by_tldr_entry(entry)
+        if feedback is None:
+            feedback= Feedback(score=score).save()
+            feedback.about_entry.connect(entry)
+            request= self.get_requests_by_tldr_entry(entry)
+            feedback.from_request.connect(request)
+        else:
+            feedback.score=score
+            feedback.save()
+            log.warn("Updated scoring of existing Feedback.")
+
+        return feedback
+
+    def get_feedback_by_tldr_entry(self, entry:TldrEntry) -> Feedback:
+         return self.cypher_query_one("""
+            MATCH (f:Feedback)
+            MATCH (e:TldrEntry) WHERE e.uid=$uid
+            MATCH (f)-[x:ABOUT]->(e)
+            RETURN f """, "f", params={"uid":entry.uid})     
+    
+    def get_feedback_by_request(self, request:Request) -> list[Feedback]:
+         return self.cypher_query("""
+            MATCH (f:Feedback)
+            MATCH (r:Request) WHERE e.uid=$uid
+            MATCH (f)-[x:FROM]->(r)
+            RETURN f """, "f", params={"uid":request.uid})
+
+	#-----------------
+	# EvalKey Nodes - rubric for evaluation metrics
+	#-----------------
 
-## EvalKey Nodes - rubric for evaluation metrics
 
     def add_evalkey(self, content:Content, request:Request, score:float, text:str) -> EvalKey:
         key = EvalKey(text=text, score=score).save()
         key.key_for_content.connect(content)
         key.key_for_request.connect(request)
         return key
 
-    def get_all_evalkeys(self) -> list[EvalKey]:
-        evalkeys = EvalKey.nodes
-        return evalkeys
-
-    def get_evalkey_by_uid(self, uid:str) -> Content:
+    def get_evalkey_by_uid(self, uid: str) -> Content:
         key = EvalKey.nodes.get_or_none(uid=uid)
         return key
-    
-    def get_evalkeys_by_request(self,request:Request) -> list[Content]:
+
+    def get_evalkeys_by_request(self, request: Request) -> list[Content]:
         return self.cypher_query("""
-            MATCH (q:Request) WHERE q.uid='{request_id}'
+            MATCH (q:Request) WHERE q.uid=$request_id
             MATCH (e:EvalKey)-[eq:KEY_FOR_REQUEST]->(q)
-            RETURN e """.format(request_id=request.uid),"e")
-    
-    def get_evalkey_by_content_and_request(self, content:Content, request:Request) -> EvalKey:
+            RETURN e """,
+            "e", params={"request_id": request.uid})
+
+    def get_evalkey_by_content_and_request(self, content: Content, request: Request) -> EvalKey:
         return self.cypher_query_one("""
-            MATCH (c:Content) WHERE c.uid='{content_id}'
-            MATCH (q:Request) WHERE q.uid='{request_id}'
+            MATCH (c:Content) WHERE c.uid=$content_id
+            MATCH (q:Request) WHERE q.uid=$request_id
             MATCH (c)<-[ec:KEY_FOR_CONTENT]-(e:EvalKey)-[eq:KEY_FOR_REQUEST]->(q)
-            RETURN e """.format( content_id=content.uid, request_id=request.uid),"e")
+            RETURN e """,
+            "e", params={
+                "content_id": content.uid,
+                "request_id": request.uid})
+
+    def get_all_evalkeys(self) -> list[EvalKey]:
+        evalkeys = EvalKey.nodes
+        return evalkeys
 
     def delete_all_evalkeys(self):
         self.cypher_query("MATCH (r:EvalKey) DETACH DELETE (r)")
```

### Comparing `opentldr-0.4.3/src/opentldr/S3DataRepo.py` & `opentldr-0.5.0/src/opentldr/S3DataRepo.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 import boto3
 import json
 import os
 import tempfile
 
 class S3DataRepo(AbstractDataRepo):
 
-    bucket = None
-    bucket_name= ""
-    prefix:str = None
-
     files:list = []
 
     def __init__(self, kg:KnowledgeGraph, bucket_name:str, aws_access_key_id:str, aws_secret_access_key:str, prefix:str=None) :
         self.kg=kg
         session = boto3.Session( aws_access_key_id, aws_secret_access_key)
         s3 = session.resource('s3')
         self.bucket_name = bucket_name
@@ -28,15 +24,15 @@
                 if not o.key.endswith("/"): #skip directories
                     self.files.append(o)
 
 
     def describe(self) -> str:
         return "S3 Bucket Content ('{bucket}')".format(bucket=self.bucket_name)
 
-
+    # TODO: Move repeated method to superclass
     def _importByClass(self,raw:dict,clazz:str) -> list[str]:
         list_of_uids=[]
         if clazz in raw:
             for item in raw[clazz]:
                 item['class']=clazz
                 o = dictToKg(self.kg,item)
                 list_of_uids.append(o.uid)
```

### Comparing `opentldr-0.4.3/src/opentldr/Workflow.py` & `opentldr-0.5.0/src/opentldr/Workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 os.environ["PYDEVD_DISABLE_FILE_VALIDATION"]="1"
 
 import papermill as pm
 
 class Workflow:
 
-    def __init__(self, workflow):
+    def __init__(self, workflow: dict):
         self.workflow=workflow
         self.verify()
 
     @classmethod
     def from_json(cls,j:str):
         wf:Workflow = cls(json.loads(j))
         return wf
@@ -36,25 +36,25 @@
         workflow["Output"] = output_folder
         nblist = []
         for notebook in notebook_order:
             nblist.append([notebook, variables])
         workflow["Notebooks"] = nblist
         return cls(workflow)
 
-    def import_json(self,j):
-        output = j["Output"]
+    def import_json(self,j):                        # TODO: This method doesn't import anything to anywhere
+        output = j["Output"]                        # TODO: Never used
         notebooks:list[list] = j["Notebooks"]
         for step in notebooks:
             notebook:str=step[0]
             config:dict=step[1]
             print ("Notebook: {notebook} is config is: {config}".format(notebook=notebook,config=config))
 
     def verify(self):
         '''
-        walk thru the structure of the workflow and ensure it is setup correctly.
+        Walk thru the structure of the workflow and ensure it is setup correctly.
         '''
         has_errors:bool=False
         errors:str=""
 
         # Verify Output
         path=self.workflow["Output"]
         if path is None:
@@ -108,23 +108,23 @@
 
     def export_workflow(self, filepath:str) ->json:
         with open(filepath, 'w', encoding='utf-8') as f:
             json.dump(self.workflow, f, ensure_ascii=False, indent=4)
 
     def ensure_path(self,path):
         '''
-        ensure_path(path) simply creates a directory if it is not there already.
+        Ensure_path(path) simply creates a directory if it is not there already.
         '''
         if not os.path.exists(path):
             os.makedirs(path)
             log.info("Created output directory: "+path)
 
     def execute_notebook(self, notebook:str, variables:dict, output_path:str) -> float:
         '''
-        execute_notebook runs a single notebook file in PaperMill returns the run time in seconds
+        Execute_notebook runs a single notebook file in PaperMill returns the run time in seconds
         '''
         try:
             out_notebook:str = os.path.join(output_path,notebook.replace('/',"_"))
             log.debug("Now executing notebook '{notebook}' with params '{params}' and output '{output}'.".format(notebook=notebook,params=variables,output=output_path))
 
             step_start=perf_counter()
             pm.execute_notebook(notebook, out_notebook, variables)
@@ -133,15 +133,15 @@
         
         except Exception as e:
             log.error("There was an error executing the notebook ({nb}), please verify the parameters and that the notebook runs successfully on its own.".format(nb=notebook))
             raise e
 
     def run(self):
         '''
-        run the defined workflow files in order in PaperMill
+        Run the defined workflow files in order in PaperMill
         '''
         output_path=self.workflow["Output"]
         self.ensure_path(output_path)
         workflow_start=perf_counter()
         c=1
         for step in self.workflow["Notebooks"]:
             notebook:str=step[0]
```

### Comparing `opentldr-0.4.3/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.0/src/opentldr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.4.3
+Version: 0.5.0
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -25,62 +25,61 @@
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
-OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
+OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
-- A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
+- A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
 - A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
-This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
-to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
+This GitHub repo handles the back-end code that is only required if you wish to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is available to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
-OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
+OpenTLDR uses a Neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
 
-OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain class being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
+OpenTLDR uses the KnowledgeGraph's API to build up a series of objects and relationships (see the Domain module) over a series of steps in the automated workflow (see the Workflow module). This includes loading content (e.g., news articles), which means that the graph database can become large. The KnowledgeGraph API is designed to be verb-oriented and functional, with the Domain classes being the nouns and providing useful data objects. The primary reason for this API design was to keep the Notebooks simple, clean, and transactional to the KnowledgeGraph. The default query methods return either a single or list of objects defined by a Domain class.
 
 ## Domain
 
 The OpenTLDR library includes class definitions for all of the objects represented in the KnowledgeGraph. This standardizes the graph, so that multiple analytic workflows can easily achieve compatability.
 
 Each Domain class includes the following properties:
 - uid - a text string that acts as a unique identifier that is created the first time the data object is saved and can be queried.
 - meta - a json object that can be used to decorate any node or edge with additional properties that your workflow might use (but that are not expected to be implemented by others)
 
-The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
+The ontology of the KnowledgeGraph is represented graphically to indicate how the different node and edge types interconnect. As long as the Domain objects and KnowledgeGraph API are used, it should be difficult to end up with incorrect connections. Every edge type is also a uniquely named Domain object with a uid and meta properties. 
 
 ![ontology image](resources/ontology.png)
 
-The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with capitalized camel case lettering without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which is can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
+The colors in this image can be replicated in the neo4j interface using the `scripts/neo4j_styles.grass` file, which can be drag and dropped on the main neo4j webpage. Note that the naming convention for neo4j suggests that nodes be labeled with upper camel case capitalization without spaces (which is the same as the naming of the python Domain classes) and edges are all caps with underlines as spaces (which can sometimes be confusing when switching between the python Domain class names and the labels in the graph and cypher code).
 
 ## Workflow
 
 The OpenTLDR Workflow uses PaperMill to execute the sequences of analytic notebooks and parameterize them. This should not impede the notebooks from  being run manually when desired, but it does enforce the expected workflow order of execution that should be used when running evaluation scoring for an end-to-end analytic workflow.
 
 ### The Default Workflow Parameters
 
 There are a few paramters that are used throughout the standard workflow.
 
 #### Output Folder
-This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results but are replaced the next time the workflow is executed. Therefore, they should only be used as read-only copies.
+This indicates where the automated workflow should place the outputed Notebooks. Note that these are copies of the original notebooks that show the execution results.  They copies are overwritten each time the workflow is executed. The original notebooks should always be treated as read-only copies.
 
 <pre>
 output_folder = "./READ_ONLY_OUTPUT"
 </pre>
 
 #### Notebook Order
-This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed for manual execution, but the order in which they appear in this list is the order in which the `Workflow` class will run them.
+This parameter is a list of strings, where each string is the relative path of a Notebook file to run. We tend to name these with the order that they are executed manually, but the `Workflow` class always executes in the order they appear in this list. 
 
 <pre>
 notebook_order = [
     "Step_0_Initialize.ipynb",
   ...
     "Step_6_Evaluate.ipynb"
     ]
@@ -98,15 +97,15 @@
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
 ## DataRepo
-The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above `variables_to_set` specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -128,9 +127,9 @@
 
 kg = KnowledgeGraph()
 cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo `cr` that writes to the KnowledgeGraph `kg` from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.4.3/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.0/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

