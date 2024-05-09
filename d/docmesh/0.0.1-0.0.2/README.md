# Comparing `tmp/docmesh-0.0.1.tar.gz` & `tmp/docmesh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh-0.0.1.tar` & `docmesh-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0        9 2024-05-09 06:03:24.521942 docmesh-0.0.1/README.md
--rw-r--r--   0        0        0       98 2024-05-09 05:44:49.710304 docmesh-0.0.1/docmesh/__init__.py
--rw-r--r--   0        0        0      530 2024-05-09 01:46:54.072080 docmesh-0.0.1/docmesh/db/__init__.py
--rw-r--r--   0        0        0     1397 2024-05-09 04:35:40.368345 docmesh-0.0.1/docmesh/db/auth.py
--rw-r--r--   0        0        0     5169 2024-05-09 01:58:02.091018 docmesh-0.0.1/docmesh/db/neo.py
--rw-r--r--   0        0        0     3494 2024-05-09 05:38:39.438960 docmesh-0.0.1/docmesh/main.py
--rw-r--r--   0        0        0       88 2024-05-09 01:46:53.997886 docmesh-0.0.1/docmesh/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-09 01:46:54.001608 docmesh-0.0.1/docmesh/parser/output_parser.py
--rw-r--r--   0        0        0      857 2024-05-09 01:46:54.056241 docmesh-0.0.1/docmesh/prompt.py
--rw-r--r--   0        0        0      509 2024-05-09 01:46:53.974493 docmesh-0.0.1/docmesh/tools/__init__.py
--rw-r--r--   0        0        0      357 2024-05-09 01:46:53.977748 docmesh-0.0.1/docmesh/tools/base.py
--rw-r--r--   0        0        0      781 2024-05-09 01:46:53.983111 docmesh-0.0.1/docmesh/tools/entity_tools.py
--rw-r--r--   0        0        0     2493 2024-05-09 01:46:53.970975 docmesh-0.0.1/docmesh/tools/graph_tools.py
--rw-r--r--   0        0        0     7197 2024-05-09 01:46:53.980344 docmesh-0.0.1/docmesh/tools/paper_tools.py
--rw-r--r--   0        0        0      236 2024-05-09 01:58:58.649816 docmesh-0.0.1/docmesh/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-09 01:46:54.041643 docmesh-0.0.1/docmesh/utils/graph_utils.py
--rw-r--r--   0        0        0     3104 2024-05-09 01:46:54.052654 docmesh-0.0.1/docmesh/utils/semantic_scholar.py
--rw-r--r--   0        0        0      889 2024-05-09 05:42:53.106471 docmesh-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 docmesh-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-09 08:25:56.266488 docmesh-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-09 09:53:55.978803 docmesh-0.0.2/docmesh/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-09 09:23:16.324316 docmesh-0.0.2/docmesh/db/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-09 04:35:40.368345 docmesh-0.0.2/docmesh/db/auth.py
+-rw-r--r--   0        0        0     7451 2024-05-09 09:23:16.330585 docmesh-0.0.2/docmesh/db/neo.py
+-rw-r--r--   0        0        0     3237 2024-05-09 09:42:14.197261 docmesh-0.0.2/docmesh/main.py
+-rw-r--r--   0        0        0       88 2024-05-09 01:46:53.997886 docmesh-0.0.2/docmesh/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-09 01:46:54.001608 docmesh-0.0.2/docmesh/parser/output_parser.py
+-rw-r--r--   0        0        0      857 2024-05-09 01:46:54.056241 docmesh-0.0.2/docmesh/prompt.py
+-rw-r--r--   0        0        0      186 2024-05-09 09:39:35.901101 docmesh-0.0.2/docmesh/toolkit/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-09 08:25:56.296406 docmesh-0.0.2/docmesh/toolkit/entity.py
+-rw-r--r--   0        0        0      653 2024-05-09 09:23:16.347369 docmesh-0.0.2/docmesh/toolkit/paper.py
+-rw-r--r--   0        0        0      431 2024-05-09 09:39:29.458383 docmesh-0.0.2/docmesh/toolkit/recommend.py
+-rw-r--r--   0        0        0      569 2024-05-09 09:38:29.753379 docmesh-0.0.2/docmesh/tools/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-09 08:25:56.312152 docmesh-0.0.2/docmesh/tools/base.py
+-rw-r--r--   0        0        0     2192 2024-05-09 08:25:56.316922 docmesh-0.0.2/docmesh/tools/entity.py
+-rw-r--r--   0        0        0     3895 2024-05-09 09:44:23.645514 docmesh-0.0.2/docmesh/tools/graph_tools.py
+-rw-r--r--   0        0        0     4001 2024-05-09 09:23:16.357311 docmesh-0.0.2/docmesh/tools/paper.py
+-rw-r--r--   0        0        0     2275 2024-05-09 09:37:40.948496 docmesh-0.0.2/docmesh/tools/recommend.py
+-rw-r--r--   0        0        0      276 2024-05-09 09:23:16.362731 docmesh-0.0.2/docmesh/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-09 01:46:54.041643 docmesh-0.0.2/docmesh/utils/graph_utils.py
+-rw-r--r--   0        0        0     3148 2024-05-09 09:23:16.368077 docmesh-0.0.2/docmesh/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      885 2024-05-09 10:15:34.124067 docmesh-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 docmesh-0.0.2/PKG-INFO
```

### Comparing `docmesh-0.0.1/docmesh/db/auth.py` & `docmesh-0.0.2/docmesh/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.1/docmesh/db/neo.py` & `docmesh-0.0.2/docmesh/db/neo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import os
+import pandas as pd
 
+from typing import Any
 from pandas.core.frame import DataFrame
 
 from neomodel import db, config
 from neomodel import (
     StructuredNode,
     StructuredRel,
     StringProperty,
     IntegerProperty,
     DateTimeProperty,
     RelationshipTo,
     RelationshipFrom,
 )
 from neomodel.integration.pandas import to_dataframe
 
+from ..utils.semantic_scholar import (
+    get_paper_id,
+    get_references,
+    get_paper_details,
+    PaperIdNotFound,
+)
+
 if (url := os.getenv("NEO4J_URL")) is None:
     raise ValueError("You have not set neo4j database url using environment `NEO4J_URL`.")
 else:
     config.DATABASE_URL = url
     # HACK: server may kill idle connection, to avoid being hung for
     # a long time, we kill the connection first, the max lifetime
     # should be less then 4 mins (240 seconds)
@@ -35,14 +44,19 @@
 class Entity(StructuredNode):
     name = StringProperty(unique_index=True)
 
     reads = RelationshipTo("Paper", "read", model=ReadRel)
     follows = RelationshipTo("Entity", "follow", model=FollowRel)
     followers = RelationshipFrom("Entity", "follow", model=FollowRel)
 
+    @property
+    def serialize(self) -> dict[str, Any]:
+        data = {"name": self.name}
+        return data
+
 
 class Paper(StructuredNode):
     paper_id = StringProperty(unique_index=True)
     title = StringProperty()
     abstract = StringProperty()
     summary = StringProperty()
     publication_date = DateTimeProperty()
@@ -50,103 +64,152 @@
     citation_count = IntegerProperty()
     pdf = StringProperty()
 
     readers = RelationshipFrom("Entity", "read", model=ReadRel)
     references = RelationshipTo("Paper", "cite")
     citations = RelationshipFrom("Paper", "cite")
 
+    @property
+    def serialize(self) -> dict[str, Any]:
+        data = {
+            "paper_id": self.paper_id,
+            "title": self.title,
+            "abstract": self.abstract,
+            "summary": self.summary,
+            "publication_date": self.publication_date,
+            "reference_count": self.reference_count,
+            "citation_count": self.citation_count,
+            "pdf": self.pdf,
+        }
+        return data
+
+
+def _nodelist_to_dataframe(nodes: list[StructuredNode]) -> DataFrame:
+    df = pd.DataFrame.from_dict([node.serialize for node in nodes])
+    return df
+
+
+def get_entity(entity_name: str) -> Entity:
+    entity = Entity.nodes.get(name=entity_name)
+    return entity
+
 
 @db.transaction
-def get_entity(name: str) -> Entity:
-    entity = Entity.nodes.get(name=name)
+def add_entity(name: str) -> Entity:
+    entity: Entity = Entity.create_or_update({"name": name})
     return entity
 
 
 @db.transaction
-def get_paper(paper_id: str) -> Paper:
-    paper = Paper.nodes.get(paper_id=paper_id)
-    return paper
+def follow_entity(follower_name: str, follow_name: str) -> None:
+    follower_entity = get_entity(follower_name)
+    follow_entity = get_entity(follow_name)
+    follower_entity.follows.connect(follow_entity)
 
 
 @db.transaction
-def add_entity(name: str) -> None:
-    entity: Entity = Entity.create_or_update({"name": name})
+def list_follows(entity_name: str) -> DataFrame:
+    entity = get_entity(entity_name)
+    follows: list[Entity] = entity.follows.all()
+    return _nodelist_to_dataframe(follows)
 
-    return entity
+
+@db.transaction
+def list_popular_entities(n: int) -> DataFrame:
+    # XXX: use cypher query language, since OGM is not well supported
+    query = """
+        MATCH (e:Entity)
+        RETURN e.name AS name,
+        COUNT {
+            (:Entity) -[:follow]-> (e)
+        } AS num_followers,
+        COUNT {
+            (e) -[:read]-> (:Paper)
+        } AS num_reads
+        ORDER BY num_followers DESC, num_reads DESC
+        LIMIT $n
+    """
+    df = to_dataframe(
+        db.cypher_query(
+            query,
+            params={"n": n},
+        )
+    )
+
+    return df
+
+
+def get_paper_from_id(paper_id: str) -> Paper:
+    paper = Paper.nodes.get(paper_id=paper_id)
+    return paper
+
+
+def get_paper_from_title(title: str) -> Paper:
+    paper = Paper.nodes.get(title=title)
+    return paper
 
 
 @db.transaction
-def add_paper(paper: DataFrame, references: DataFrame) -> Paper:
+def _add_paper(paper: DataFrame, references: DataFrame) -> Paper:
     paper: Paper = Paper.create_or_update(*paper.to_dict(orient="records"))[0]
 
     if references.shape[0] != 0:
         references: list[Paper] = Paper.create_or_update(*references.to_dict(orient="records"))
 
         for reference in references:
             paper.references.connect(reference)
 
     return paper
 
 
-@db.transaction
-def read_paper(name: str, paper_id: str) -> None:
-    entity = get_entity(name=name)
-    paper = get_paper(paper_id=paper_id)
-    entity.reads.connect(paper)
+def add_paper(title: str) -> Paper:
+    paper_id = get_paper_id(title)
+    if paper_id is None:
+        raise PaperIdNotFound(f"Cannot find semantic scholar paper id for {title}.")
+    paper = get_paper_details([paper_id])
+
+    references_ids = get_references(paper_id)
+    if len(references_ids) == 0:
+        references = pd.DataFrame()
+    else:
+        references = get_paper_details(references_ids)
+
+    paper = _add_paper(paper, references)
+    return paper
 
 
 @db.transaction
-def follow_entity(follower_name: str, follow_name: str) -> None:
-    follower_entity = get_entity(follower_name)
-    follow_entity = get_entity(follow_name)
-    follower_entity.follows.connect(follow_entity)
+def read_paper(entity_name: str, paper_id: str) -> None:
+    entity = get_entity(entity_name)
+    paper = get_paper_from_id(paper_id=paper_id)
+    entity.reads.connect(paper)
 
 
 @db.transaction
-def get_latest_papers(name: str, n: int) -> DataFrame:
+def list_latest_papers(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e:Entity) -[r:read]-> (p:Paper)
         WHERE e.name = $name
         RETURN p.paper_id AS paper_id, p.title AS title
         ORDER BY r.read_time DESC
         LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"name": name, "n": n},
-        )
-    )
-
-    return df
-
-
-@db.transaction
-def get_latest_citegraph(name: str, n: int) -> DataFrame:
-    # XXX: use cypher query language, since OGM is not well supported
-    query = """
-        MATCH (e1:Entity) -[r:read]-> (p1:Paper) -[:cite]-> (p2:Paper) <-[:read]- (e2:Entity)
-        WHERE e1.name = $name AND e2.name = $name
-        RETURN p1.paper_id AS p1_paper_id, p2.paper_id AS p2_paper_id
-        ORDER BY r.read_time DESC
-        LIMIT $n;
-    """
-    df = to_dataframe(
-        db.cypher_query(
-            query,
-            params={"name": name, "n": n},
+            params={"name": entity_name, "n": n},
         )
     )
 
     return df
 
 
 @db.transaction
-def get_unread_follows_papers(name: str, n: int) -> DataFrame:
+def list_unread_follows_papers(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e1:Entity) -[:follow]-> (:Entity) -[r:read]-> (p:Paper)
         WHERE e1.name = $name
         AND NOT EXISTS {
             (p) <-[:read]- (e2:Entity)
             WHERE e2.name = $name
@@ -154,23 +217,23 @@
         RETURN p.title AS title, p.pdf AS pdf
         ORDER BY r.read_time, p.citation_count DESC
         LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"name": name, "n": n},
+            params={"name": entity_name, "n": n},
         )
     )
 
     return df
 
 
 @db.transaction
-def get_unread_influential_papers(name: str, date_time: str) -> DataFrame:
+def list_unread_influential_papers(entity_name: str, date_time: str) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (p:Paper)
         WHERE p.publication_date >= DATETIME($date_time).epochSeconds
         AND NOT EXISTS {
             (p) <-[:read]- (e:Entity)
             WHERE e.name = $name
@@ -178,12 +241,32 @@
         RETURN p.title AS title, p.pdf AS pdf
         ORDER BY p.citation_count DESC
         limit 10;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"date_time": date_time, "name": name},
+            params={"date_time": date_time, "name": entity_name},
+        )
+    )
+
+    return df
+
+
+@db.transaction
+def get_latest_citegraph(entity_name: str, n: int) -> DataFrame:
+    # XXX: use cypher query language, since OGM is not well supported
+    query = """
+        MATCH (e1:Entity) -[r:read]-> (p1:Paper) -[:cite]-> (p2:Paper) <-[:read]- (e2:Entity)
+        WHERE e1.name = $name AND e2.name = $name
+        RETURN p1.paper_id AS p1_paper_id, p2.paper_id AS p2_paper_id
+        ORDER BY r.read_time DESC
+        LIMIT $n;
+    """
+    df = to_dataframe(
+        db.cypher_query(
+            query,
+            params={"name": entity_name, "n": n},
         )
     )
 
     return df
```

### Comparing `docmesh-0.0.1/docmesh/main.py` & `docmesh-0.0.2/docmesh/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,40 +7,17 @@
 from fastapi import status, Depends, HTTPException, Response, FastAPI
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 from langchain.agents import AgentExecutor, create_react_agent
 from langchain_openai import ChatOpenAI
 from langchain_community.chat_message_histories import SQLChatMessageHistory
 from langchain_core.runnables.history import RunnableWithMessageHistory
 
-from docmesh.db.auth import get_entity_from_auth
-from docmesh.tools import (
-    FollowEntityTool,
-    AddPaperTool,
-    GetLatestPaperTool,
-    PaperSummaryTool,
-    UnreadFollowsTool,
-    UnreadInfluentialTool,
-    CiteGraphTool,
-    CiteGraphVisualizeTool,
-    PopularPaperTool,
-)
 from docmesh.prompt import MEMORY_REACT_PROMPT
-
-AVAILABLE_TOOLS = [
-    FollowEntityTool,
-    AddPaperTool,
-    GetLatestPaperTool,
-    PaperSummaryTool,
-    UnreadFollowsTool,
-    UnreadInfluentialTool,
-    CiteGraphTool,
-    CiteGraphVisualizeTool,
-    PopularPaperTool,
-]
-
+from docmesh.db.auth import get_entity_from_auth
+from docmesh.toolkit import EntityToolkit, PaperToolkit, RecommendToolkit
 
 app = FastAPI()
 auth_scheme = HTTPBearer()
 
 
 class AgentBody(BaseModel):
     session_id: str
@@ -71,15 +48,19 @@
 
 def _execute_agent(entity_name: str, query: str, session_id: str) -> str:
     # setup react prompt
     prompt = MEMORY_REACT_PROMPT
     # setup llm
     llm = ChatOpenAI(model="gpt-4-0125-preview")
     # set up all tools
-    tools = [tool(entity_name=entity_name) for tool in AVAILABLE_TOOLS]
+    tools = [
+        *EntityToolkit(entity_name=entity_name).get_tools(),
+        *PaperToolkit(entity_name=entity_name).get_tools(),
+        *RecommendToolkit(entity_name=entity_name).get_tools(),
+    ]
     # setup ReAct agent
     agent = create_react_agent(llm, tools, prompt)
     # setup agent executor
     agent_executor = AgentExecutor(agent=agent, tools=tools, verbose=True, handle_parsing_errors=True)
     # setup memory database
     memory_store = os.getenv("MYSQL_URL")
     # bind agent and memory
```

### Comparing `docmesh-0.0.1/docmesh/parser/output_parser.py` & `docmesh-0.0.2/docmesh/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.1/docmesh/prompt.py` & `docmesh-0.0.2/docmesh/prompt.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.1/docmesh/tools/graph_tools.py` & `docmesh-0.0.2/docmesh/tools/graph_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,60 @@
 import numpy as np
 import networkx as nx
 import matplotlib.pyplot as plt
 
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
+from datetime import datetime
 from langchain.callbacks.manager import CallbackManagerForToolRun
 
 from .base import BaseAgentTool
 from ..utils.graph_utils import find_max_degree_nodes
+from ..db.neo import get_latest_citegraph
+
+
+class CiteGraphToolInput(BaseModel):
+    n: str = Field(description="number of papers")
+
+
+class CiteGraphTool(BaseAgentTool):
+    name: str = "cite graph generation tool"
+    description: str = (
+        "useful when you need to generate a cite graph from papers, "
+        "return a gml format of cite graph for a given number."
+    )
+    args_schema: Type[BaseModel] = CiteGraphToolInput
+    handle_tool_error: bool = True
+
+    def _run(
+        self,
+        n: str,
+        run_manager: Optional[CallbackManagerForToolRun] = None,
+    ) -> str:
+        try:
+            n = int(n)
+        except Exception:
+            self._raise_tool_error(
+                "Input argument `n` should be an integer, please check your inputt. "
+                "You can directly call this function to generate cite graph for latest papers. "
+                "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
+            )
+
+        # fetch latest citegraph
+        df = get_latest_citegraph(entity_name=self.entity_name, n=n)
+
+        G = nx.Graph()
+        G.add_edges_from(zip(df["p1_paper_id"], df["p2_paper_id"]))
+
+        # generate gml file
+        gml_file = f"{datetime.now().strftime('%Y-%m-%d-%H%M%S')}.gml"
+        nx.write_gml(G, gml_file)
+
+        return f"\nCite graph is generate as gml file {gml_file}.\n"
 
 
 class CiteGraphVisualizeToolInput(BaseModel):
     gml_file: str = Field(description="gml file to visualize")
 
 
 class CiteGraphVisualizeTool(BaseAgentTool):
```

### Comparing `docmesh-0.0.1/docmesh/utils/semantic_scholar.py` & `docmesh-0.0.2/docmesh/utils/semantic_scholar.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from typing import Optional, Any
 from pandas.core.frame import DataFrame
 
 from retry import retry
 
 
+class PaperIdNotFound(Exception):
+    ...
+
+
 def _sleep1() -> None:
     # semantic scholar api is restricted under 1 qps
     # so we sleep 1 second anyway to avoid rate limit
     time.sleep(1)
 
 
 def _get_headers() -> dict[str, str]:
```

### Comparing `docmesh-0.0.1/pyproject.toml` & `docmesh-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "docmesh"
-description = "Agent helps you digging the paper connection!"
+description = "Agent helps you dig the paper connection!"
 authors = [
     {name="Zhengkai Yang", email="kyle.yang1995@gmail.com"},
 ]
 readme = "README.md"
 dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
```

### Comparing `docmesh-0.0.1/PKG-INFO` & `docmesh-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: docmesh
-Version: 0.0.1
-Summary: Agent helps you digging the paper connection!
+Version: 0.0.2
+Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -21,7 +21,8 @@
 Requires-Dist: pymysql>=0.9.3
 Requires-Dist: sqlalchemy>=2
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docmesh
+
```

