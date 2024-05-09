# Comparing `tmp/rq_dashboard_fast-0.3.8.tar.gz` & `tmp/rq_dashboard_fast-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rq_dashboard_fast-0.3.8.tar", max compression
+gzip compressed data, was "rq_dashboard_fast-0.4.0.tar", max compression
```

## Comparing `rq_dashboard_fast-0.3.8.tar` & `rq_dashboard_fast-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     3082 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/README.md
--rw-r--r--   0        0        0      786 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       51 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/__init__.py
--rw-r--r--   0        0        0     8422 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/rq_dashboard_fast.py
--rw-r--r--   0        0        0     5110 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/static/css/main.css
--rw-r--r--   0        0        0      575 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/base.html
--rw-r--r--   0        0        0      283 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/footer.html
--rw-r--r--   0        0        0     1016 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/header.html
--rw-r--r--   0        0        0     1933 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/job.html
--rw-r--r--   0        0        0     8856 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/jobs.html
--rw-r--r--   0        0        0     7567 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/queues.html
--rw-r--r--   0        0        0     4937 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/workers.html
--rw-r--r--   0        0        0        0 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/__init__.py
--rw-r--r--   0        0        0     3218 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_dashboard.py
--rw-r--r--   0        0        0     1893 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_jobs_utils.py
--rw-r--r--   0        0        0     1499 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_queues_utils.py
--rw-r--r--   0        0        0      706 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_worker_utils.py
--rw-r--r--   0        0        0        0 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/__init__.py
--rw-r--r--   0        0        0     7212 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/jobs.py
--rw-r--r--   0        0        0     2290 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/queues.py
--rw-r--r--   0        0        0     1823 2024-03-13 20:52:25.563944 rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/workers.py
--rw-r--r--   0        0        0     3829 1970-01-01 00:00:00.000000 rq_dashboard_fast-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     3082 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/README.md
+-rw-r--r--   0        0        0      786 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/__init__.py
+-rw-r--r--   0        0        0     8442 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/rq_dashboard_fast.py
+-rw-r--r--   0        0        0     5110 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/static/css/main.css
+-rw-r--r--   0        0        0      575 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/base.html
+-rw-r--r--   0        0        0      283 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/footer.html
+-rw-r--r--   0        0        0     1016 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/header.html
+-rw-r--r--   0        0        0     1933 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/job.html
+-rw-r--r--   0        0        0     8856 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/jobs.html
+-rw-r--r--   0        0        0     7567 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/queues.html
+-rw-r--r--   0        0        0     4937 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/workers.html
+-rw-r--r--   0        0        0        0 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/__init__.py
+-rw-r--r--   0        0        0     3184 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_dashboard.py
+-rw-r--r--   0        0        0     1893 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_jobs_utils.py
+-rw-r--r--   0        0        0     1499 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_queues_utils.py
+-rw-r--r--   0        0        0      706 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_worker_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/__init__.py
+-rw-r--r--   0        0        0     7885 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/jobs.py
+-rw-r--r--   0        0        0     2290 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/queues.py
+-rw-r--r--   0        0        0     1823 2024-05-09 00:21:07.739601 rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/workers.py
+-rw-r--r--   0        0        0     3829 1970-01-01 00:00:00.000000 rq_dashboard_fast-0.4.0/PKG-INFO
```

### Comparing `rq_dashboard_fast-0.3.8/LICENSE.md` & `rq_dashboard_fast-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/README.md` & `rq_dashboard_fast-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/pyproject.toml` & `rq_dashboard_fast-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rq-dashboard-fast"
-version = "0.3.8"
+version = "0.4.0"
 description = "rq-dashboard-fast is a FastAPI-based dashboard to monitor your Redis-Queue (RQ) Jobs, Queues, and Workers"
 authors = ["Hannes221 <hannespfau@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.109.0"
```

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/rq_dashboard_fast.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/rq_dashboard_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         self.mount("/static", StaticFiles(directory=static_directory), name="static")
 
         templates_directory = package_directory / "templates"
         self.templates = Jinja2Templates(directory=templates_directory)
         self.redis_url = redis_url
 
-        self.rq_dashboard_version = "0.3.8"
+        self.rq_dashboard_version = "0.4.0"
 
         logger = logging.getLogger(__name__)
 
         @self.get("/", response_class=HTMLResponse)
         async def get_home(request: Request):
             try:
                 protocol = request.url.scheme
@@ -152,18 +152,18 @@
                 raise HTTPException("An error occurred reading queues data json:", e)
 
         @self.get("/jobs", response_class=HTMLResponse)
         async def read_jobs(
             request: Request,
             queue_name: str = Query("all"),
             state: str = Query("all"),
-            page: str = Query(1),
+            page: int = Query(1),
         ):
             try:
-                job_data = get_jobs(self.redis_url, queue_name, state)
+                job_data = get_jobs(self.redis_url, queue_name, state, page=page)
 
                 active_tab = "jobs"
 
                 protocol = request.url.scheme
 
                 return self.templates.TemplateResponse(
                     "jobs.html",
@@ -180,18 +180,18 @@
                 logger.exception("An error occurred reading jobs data template:", e)
                 raise HTTPException("An error occurred reading jobs data template:", e)
 
         @self.get("/jobs/json", response_model=list[QueueJobRegistryStats])
         async def read_jobs(
             queue_name: str = Query("all"),
             state: str = Query("all"),
-            page: str = Query("1"),
+            page: int = Query(1),
         ):
             try:
-                job_data = get_jobs(self.redis_url, queue_name, state)
+                job_data = get_jobs(self.redis_url, queue_name, state, page=page)
 
                 return job_data
             except Exception as e:
                 logger.exception("An error occurred reading jobs data json:", e)
                 raise HTTPException("An error occurred reading jobs data json:", e)
 
         @self.get("/job/{job_id}", response_model=JobDataDetailed)
```

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/static/css/main.css` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/static/css/main.css`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/base.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/base.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/header.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/header.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/job.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/job.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/jobs.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/jobs.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/queues.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/queues.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/templates/workers.html` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/templates/workers.html`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_dashboard.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from redis import Redis
 from rq import Queue, Worker
 
 from rq_dashboard_fast import RedisQueueDashboard
 
-# RUN PYTEST IN DOCKER CONTAINER
-
 worker_name = "test"
 queue_name = "test_queue"
 
 
 async def example_task() -> int:
     return randint(0, 100)
```

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_jobs_utils.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_queues_utils.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_queues_utils.py`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/tests/test_worker_utils.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/tests/test_worker_utils.py`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/jobs.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,31 +68,40 @@
 
                 if state == "all":
                     jobs.extend(queue.get_job_ids())
                     jobs.extend(queue.finished_job_registry.get_job_ids())
                     jobs.extend(queue.failed_job_registry.get_job_ids())
                     jobs.extend(queue.started_job_registry.get_job_ids())
                     jobs.extend(queue.deferred_job_registry.get_job_ids())
-                elif state == "scheduled":
                     jobs.extend(queue.scheduled_job_registry.get_job_ids())
-                elif state == "queued":
-                    jobs.extend(queue.get_job_ids())
-                elif state == "finished":
-                    jobs.extend(queue.finished_job_registry.get_job_ids())
-                elif state == "failed":
-                    jobs.extend(queue.failed_job_registry.get_job_ids())
-                elif state == "started":
-                    jobs.extend(queue.started_job_registry.get_job_ids())
-                elif state == "deferred":
-                    jobs.extend(queue.deferred_job_registry.get_job_ids())
+                else:
+                    if state == "scheduled":
+                        jobs.extend(queue.scheduled_job_registry.get_job_ids())
+                    elif state == "queued":
+                        jobs.extend(queue.get_job_ids())
+                    elif state == "finished":
+                        jobs.extend(queue.finished_job_registry.get_job_ids())
+                    elif state == "failed":
+                        jobs.extend(queue.failed_job_registry.get_job_ids())
+                    elif state == "started":
+                        jobs.extend(queue.started_job_registry.get_job_ids())
+                    elif state == "deferred":
+                        jobs.extend(queue.deferred_job_registry.get_job_ids())
+
+                started_jobs = []
+                failed_jobs = []
+                deferred_jobs = []
+                finished_jobs = []
+                queued_jobs = []
+                scheduled_jobs = []
 
-                if state == "all" or state == "scheduled":
-                    scheduled = scheduler.get_jobs()
+                scheduled = scheduler.get_jobs()
 
-                    for job in scheduled:
+                for job in scheduled:
+                    if job.id not in scheduled_jobs:
                         scheduled_jobs.append(
                             JobData(
                                 id=job.id,
                                 name=job.description,
                                 created_at=job.created_at,
                             )
                         )
@@ -100,17 +109,17 @@
                 jobs_fetched = Job.fetch_many(jobs, connection=redis)
 
                 started_jobs = []
                 failed_jobs = []
                 deferred_jobs = []
                 finished_jobs = []
                 queued_jobs = []
-                scheduled_jobs = []
 
-                for job in jobs_fetched[start_index:end_index]:
+                jobs = jobs_fetched[start_index:end_index]
+                for job in jobs:
                     status = job.get_status()
                     if status == "started":
                         started_jobs.append(
                             JobData(
                                 id=job.id,
                                 name=job.description,
                                 created_at=job.created_at,
@@ -144,14 +153,22 @@
                         queued_jobs.append(
                             JobData(
                                 id=job.id,
                                 name=job.description,
                                 created_at=job.created_at,
                             )
                         )
+                    elif status == "scheduled":
+                        scheduled_jobs.append(
+                            JobData(
+                                id=job.id,
+                                name=job.description,
+                                created_at=job.created_at,
+                            )
+                        )
 
                 result.append(
                     QueueJobRegistryStats(
                         queue_name=queue.name,
                         scheduled=scheduled_jobs,
                         queued=queued_jobs,
                         started=started_jobs,
```

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/queues.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/queues.py`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/rq_dashboard_fast/utils/workers.py` & `rq_dashboard_fast-0.4.0/rq_dashboard_fast/utils/workers.py`

 * *Files identical despite different names*

### Comparing `rq_dashboard_fast-0.3.8/PKG-INFO` & `rq_dashboard_fast-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rq-dashboard-fast
-Version: 0.3.8
+Version: 0.4.0
 Summary: rq-dashboard-fast is a FastAPI-based dashboard to monitor your Redis-Queue (RQ) Jobs, Queues, and Workers
 Author: Hannes221
 Author-email: hannespfau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

