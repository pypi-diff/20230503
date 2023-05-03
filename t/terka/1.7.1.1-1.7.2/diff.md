# Comparing `tmp/terka-1.7.1.1.tar.gz` & `tmp/terka-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.7.1.1.tar", last modified: Mon May  1 11:33:09 2023, max compression
+gzip compressed data, was "terka-1.7.2.tar", last modified: Wed May  3 19:51:38 2023, max compression
```

## Comparing `terka-1.7.1.1.tar` & `terka-1.7.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-01 11:33:09.858424 terka-1.7.1.1/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-01 11:33:09.858424 terka-1.7.1.1/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      905 2023-05-01 11:32:59.000000 terka-1.7.1.1/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.1.1/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41987 2023-04-30 09:58:41.000000 terka-1.7.1.1/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.1.1/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.1.1/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.1.1/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.1.1/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.1.1/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    29368 2023-04-30 19:47:46.000000 terka-1.7.1.1/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.1.1/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.1.1/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7860 2023-04-30 11:10:05.000000 terka-1.7.1.1/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-01 11:33:09.858424 terka-1.7.1.1/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-01 11:33:09.000000 terka-1.7.1.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-03 19:51:38.947424 terka-1.7.2/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-03 19:51:38.947424 terka-1.7.2/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-03 15:07:59.000000 terka-1.7.2/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44610 2023-05-03 19:48:27.000000 terka-1.7.2/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/top_level.txt
```

### Comparing `terka-1.7.1.1/setup.py` & `terka-1.7.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.7.1.1",
+    version="1.7.2",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.7.1.1/terka/adapters/orm.py` & `terka-1.7.2/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/adapters/repository.py` & `terka-1.7.2/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/collaborators.py` & `terka-1.7.2/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/commands.py` & `terka-1.7.2/terka/domain/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,15 +537,16 @@
             if entity_type == "tasks":
                 existing_task = self.repo.list(Task, {"id": kwargs["id"]})
                 if not existing_task:
                     raise ValueError(
                         f"Task with id {kwargs['id']} is not found!")
                 obj = TaskCommentary(**kwargs)
                 self.repo.add(obj)
-                self.repo.update(Task, kwargs["id"], {"modification_date": datetime.now()})
+                self.repo.update(Task, kwargs["id"],
+                                 {"modification_date": datetime.now()})
                 session.commit()
             elif entity_type == "projects":
                 existing_project = self.repo.list(Project,
                                                   {"id": kwargs["id"]})
                 if not existing_project:
                     raise ValueError(
                         f"Project with id {kwargs['id']} is not found!")
@@ -572,14 +573,15 @@
                 sprint = self.repo.list(Sprint, {"id": kwargs["id"]})
                 if not sprint:
                     raise ValueError(
                         f"Sprint with id {kwargs['id']} is not found!")
                 obj = SprintCommentary(**kwargs)
                 self.repo.add(obj)
                 session.commit()
+            self.printer.print_new_object(obj)
         elif command == "delete":
             if entity not in (Task, ):
                 raise ValueError("'delete' operation only allowed for tasks!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
                 if not (task := self.repo.get_by_id(Task, task_id)):
                     exit(f"Task id {task_id} is not found")
@@ -629,90 +631,98 @@
                                 "sprint": sprint_id
                             })):
                         exit("task is not in sprint")
                     self.repo.delete(SprintTask, sprint_task[0].id)
             session.commit()
         elif command == "connect":
             if entity not in (Task, Project):
-                raise ValueError("'connect' operation only allowed for tasks and project!")
+                raise ValueError(
+                    "'connect' operation only allowed for tasks and project!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
                 if entity_type == "projects":
                     asana_project_id = kwargs.get("external_project")
                     asana_project = self.repo.get_by_id(AsanaProject, task_id)
                     if not asana_project:
-                        obj = AsanaProject(id=task_id, asana_project_id=asana_project_id)
+                        obj = AsanaProject(id=task_id,
+                                           asana_project_id=asana_project_id)
                         self.repo.add(obj)
                     else:
-                        self.repo.update(AsanaProject, task_id, {"asana_project_id": asana_project_id})
+                        self.repo.update(
+                            AsanaProject, task_id,
+                            {"asana_project_id": asana_project_id})
                 elif entity_type == "tasks":
                     asana_task_id = kwargs.get("external_task")
                     asana_task = self.repo.get_by_id(AsanaProject, task_id)
                     if not asana_task:
-                        obj = AsanaTask(project=task.project, id=task_id, asana_task_id=kwargs.get("external_task"))
+                        obj = AsanaTask(
+                            project=task.project,
+                            id=task_id,
+                            asana_task_id=kwargs.get("external_task"))
                         self.repo.add(obj)
                     else:
-                        self.repo.update(AsanaTask, task_id, {"asana_task_id": asana_task_id})
+                        self.repo.update(AsanaTask, task_id,
+                                         {"asana_task_id": asana_task_id})
             self.repo.session.commit()
         elif command == "add":
-            if entity not in (Task, ):
-                raise ValueError("'add' operation only allowed for tasks!")
+            if entity not in (Task, Story, Epic):
+                raise ValueError(
+                    "'add' operation only allowed for tasks, epics, and stories!"
+                )
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
-                if not (added_task := self.repo.get_by_id(Task, task_id)):
-                    exit(f"Task id {task_id} is not found")
+                if not (added_task := self.repo.get_by_id(entity, task_id)):
+                    exit(
+                        f"{entity.__class__.__name__} id {task_id} is not found"
+                    )
 
                 if epic_id := kwargs.get("epic_id"):
                     epic = self.repo.list(Epic, {"id": epic_id})
                     if not epic:
                         exit(f"Epic id {epic_id} is not found")
                     obj = EpicTask(task=task_id, epic=epic_id)
                     if self.repo.list(EpicTask, {
                             "task": obj.task,
                             "epic": obj.epic
                     }):
                         exit("task already added to epic")
                     self.repo.add(obj)
+                    self.execute("tag", "tasks", {
+                        "id": obj.task,
+                        "tags": f"epic:{obj.epic}"
+                    })
                 if story_id := kwargs.get("story_id"):
                     story = self.repo.list(Story, {"id": story_id})
                     if not story:
                         exit(f"Story id {story_id} is not found")
                     obj = StoryTask(task=task_id, story=story_id)
                     if self.repo.list(StoryTask, {
                             "task": obj.task,
                             "story": obj.story
                     }):
                         exit("task already added to story")
                     self.repo.add(obj)
+                    self.execute("tag", "tasks", {
+                        "id": obj.task,
+                        "tags": f"story:{obj.story}"
+                    })
                 if sprint_id := kwargs.get("sprint_id"):
                     sprint = self.repo.get_by_id(Sprint, sprint_id)
                     if not sprint:
                         exit(f"Sprint id {sprint_id} is not found")
                     if sprint.status.name == "COMPLETED":
                         exit("Cannot add task to a finished sprint")
-                    obj = SprintTask(task=task_id,
-                                     sprint=sprint_id,
-                                     is_active_link=True)
-                    if self.repo.list(SprintTask, {
-                            "task": obj.task,
-                            "sprint": obj.sprint
-                    }):
-                        exit("task already added to sprint")
-                    self.repo.add(obj)
-                    sprint_task_id = obj.id
-                else:
-                    sprint_task_id = None
-                # Update task status and due date
-                if sprint_task_id:
-                    task_params = {"id": added_task.id}
-                    if added_task.status.name == "BACKLOG":
-                        task_params.update({"status": "TODO"})
-                    if not added_task.due_date or added_task.due_date > sprint.end_date:
-                        task_params.update({"due_date": sprint.end_date})
-                    self.execute("update", "tasks", task_params)
+                    if entity in (Task, ):
+                        self._add_task_to_sprint(added_task, sprint)
+                    else:
+                        for entity_task in added_task.tasks:
+                            if entity_task.tasks.status.name not in (
+                                    "DONE", "DELETED"):
+                                self._add_task_to_sprint(
+                                    entity_task.tasks, sprint)
                 if story_points := kwargs.get("story_points"):
                     if not sprint_task_id:
                         sprint_task = self.execute("get", "sprint_tasks",
                                                    {"task": task_id})
                         if not sprint_task:
                             exit(
                                 f"Task id {task_id} is not part of any sprint")
@@ -779,19 +789,23 @@
                                         old_value = old_settings[key].name
                                     except:
                                         old_value = old_settings[key]
                                     if entity_type == "projects":
                                         event = ProjectEvent
                                     elif entity_type == "tasks":
                                         event = TaskEvent
-                                    self.repo.add(
-                                        event(task, key, old_value, value,
-                                              now))
+                                    if old_value != value:
+                                        update_event = event(
+                                            task, key, old_value, value, now)
+                                        self.repo.add(update_event)
+                                        self.printer.print_new_object(
+                                            update_event)
                             if hasattr(entity, "modification_date"):
-                                self.repo.update(entity, task, {"modification_date": now})
+                                self.repo.update(entity, task,
+                                                 {"modification_date": now})
                         else:
                             print(
                                 "No changes were proposed to the existing entity"
                             )
                     session.commit()
                 return entity, None
             else:
@@ -802,15 +816,16 @@
                 for task in tasks:
                     if task.isdigit():
                         entities = self.repo.get_by_id(entity, task)
                         task_id = task
                     else:
                         entities = self.repo.get(entity, task)
                         task_id = entities.id
-                    if entity_type in ("tasks", "projects", "sprints", "epics", "stories"):
+                    if entity_type in ("tasks", "projects", "sprints", "epics",
+                                       "stories"):
                         task = entities
                         if kwargs.get("description"):
                             current_entry = task.description
                             current_type = "description"
                         elif kwargs.get("name"):
                             current_entry = task.name
                             current_type = "name"
@@ -819,16 +834,16 @@
                             current_type = "goal"
                         else:
                             raise ValueError(
                                 "Either name or description should be specified!"
                             )
 
                     message_template = generate_message_template(
-                        CurrentEntry(current_entry, current_type, entity_type), task,
-                        self.repo)
+                        CurrentEntry(current_entry, current_type, entity_type),
+                        task, self.repo)
                     with tempfile.NamedTemporaryFile(suffix=".tmp") as tf:
                         tf.write(message_template.encode("utf-8"))
                         tf.flush()
                         run(["vim", "+2", tf.name])
                         tf.seek(0)
                         new_entry = tf.read()
 
@@ -844,16 +859,20 @@
                     current_type: " ".join(updated_entry)
                 }
                 self.execute("update", entity_type, new_kwargs)
                 return entities, None, None
         elif command == "start":
             sprint_id = kwargs.get("id")
             kwargs.update({"status": "ACTIVE"})
-            self.execute("update", "sprints", kwargs)
             [sprint] = self.execute("get", "sprints", {"id": sprint_id})
+            if sprint.end_date < datetime.today().date():
+                self.console.print(
+                    "[red]Cannot start the sprint, end date in the past[/red]")
+                exit()
+            self.execute("update", "sprints", kwargs)
             for sprint_task in sprint.tasks:
                 task = sprint_task.tasks
                 task_params = {"id": task.id}
                 if task.status.name == "BACKLOG":
                     task_params.update({"status": "TODO"})
                 if not task.due_date or task.due_date > sprint.end_date:
                     task_params.update({"due_date": sprint.end_date})
@@ -906,18 +925,30 @@
             elif entity_type in ("sprints", "epics", "stories"):
                 kwargs.update({"status": "COMPLETED"})
                 [entity] = self.execute("get", entity_type,
                                         {"id": kwargs.get("id")})
 
                 if entity_type == "sprints":
                     entity.complete(entity.tasks)
+                    for entity_task in entity.tasks:
+                        if entity_task.tasks.status.name not in ("DONE",
+                                                                 "DELETED"):
+                            self.execute(
+                                "update", "tasks", {
+                                    "id": entity_task.task,
+                                    "status": "BACKLOG",
+                                    "due_date": None
+                                })
                 else:
                     entity.complete(entity.tasks)
                     for entity_task in entity.tasks:
-                        self.execute("update", "tasks", {"id": entity_task.task, "status": "DONE"})
+                        self.execute("update", "tasks", {
+                            "id": entity_task.task,
+                            "status": "DONE"
+                        })
                 self.execute("update", entity_type, kwargs)
         elif command == "track":
             if entity_type != "tasks":
                 raise ValueError("can track only tasks")
             if "hours" in kwargs and "minutes" in kwargs:
                 exit("specify only -H (hours) or -M (minutes) value")
             if "hours" in kwargs or "minutes" in kwargs:
@@ -931,14 +962,46 @@
                 del kwargs["id"]
                 self.execute("create", "time_entry", kwargs)
             else:
                 exit("tracking missing -H (hours) or -M (minutes) value")
         else:
             raise ValueError(f"Uknown command: {command}")
 
+    def _add_task_to_sprint(self, task, sprint):
+        if self.repo.list(SprintTask, {"task": task.id, "sprint": sprint.id}):
+            exit("task already added to sprint")
+        if sprint.status.name == "ACTIVE":
+
+            story_points = input(
+                f"Please enter story points estimation for task <{task.id}>: {task.name}: "
+            )
+            if not story_points.isnumeric():
+                self.console.print(
+                    "[red]Provide number when specifying story points[/red]")
+                exit()
+        else:
+            story_points = 0
+        obj = SprintTask(task=task.id,
+                         story_points=story_points,
+                         sprint=sprint.id,
+                         is_active_link=True)
+        self.repo.add(obj)
+        sprint_task_id = obj.task
+        if sprint_task_id:
+            task_params = {"id": task.id}
+            if task.status.name == "BACKLOG":
+                task_params.update({"status": "TODO"})
+            if not task.due_date or task.due_date > sprint.end_date:
+                task_params.update({"due_date": sprint.end_date})
+            self.execute("update", "tasks", task_params)
+            self.execute("tag", "tasks", {
+                "id": task.id,
+                "tags": f"sprint:{sprint.id}"
+            })
+
     def _read_config(self) -> Dict[str, Any]:
         with open(f"{self.home_dir}/.terka/config.yaml", "r",
                   encoding="utf-8") as f:
             config = yaml.safe_load(f)
         return config
```

### Comparing `terka-1.7.1.1/terka/domain/commentary.py` & `terka-1.7.2/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/epic.py` & `terka-1.7.2/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/event_history.py` & `terka-1.7.2/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/project.py` & `terka-1.7.2/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/sprint.py` & `terka-1.7.2/terka/domain/sprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
     def __init__(self,
                  start_date: datetime = None,
                  end_date: datetime = None,
                  status: str = "PLANNED",
                  goal: str = None,
                  **kwargs) -> None:
+        if not start_date and not end_date:
+            raise ValueError("Please add start and end date of the sprint")
         if start_date.date()  < datetime.today().date():
             raise ValueError(f"start date cannot be less than today")
         if not start_date:
             raise ValueError(
                 "Please provide start date for the sprint in YYYY-MM-DD format"
             )
         self.start_date = start_date
@@ -36,15 +38,14 @@
         self.end_date = end_date
         if end_date.date() < start_date.date():
             raise ValueError(f"Sprint end date cannot be less than start date")
         if end_date.date() < datetime.today().date():
             raise ValueError(f"Sprint end date cannot be less than today")
         self.status = self._validate_status(status)
         self.goal = goal
-        self.tasks: Set[Task, ...] = set()
         self.is_completed = False
 
     def _validate_status(self, status):
         if status and status not in [s.name for s in SprintStatus]:
             raise ValueError(f"{status} is invalid status")
         else:
             return status
```

### Comparing `terka-1.7.1.1/terka/domain/story.py` & `terka-1.7.2/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/tag.py` & `terka-1.7.2/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/task.py` & `terka-1.7.2/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/domain/time_tracker.py` & `terka-1.7.2/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/entrypoints/cli.py` & `terka-1.7.2/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/service_layer/printer.py` & `terka-1.7.2/terka/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,23 @@
 class Printer:
 
     def __init__(self, repo, box=rich.box.SIMPLE) -> None:
         self.console = Console()
         self.box = box
         self.repo = repo
 
-    def print_new_object(self, obj, project):
+    def print_new_object(self, obj, project=None):
         table = Table(box=self.box)
         attributes = self._get_attributes(obj)
         for column, value in attributes:
             if value:
                 table.add_column(column)
         table.add_row(*list(zip(*attributes))[1])
         if table.row_count:
+            self.console.print(f"Added new {obj.__class__.__name__}")
             self.console.print(table)
 
     def print_history(self, entities):
         table = Table(box=self.box)
         print("History:")
         for column in ("date", "type", "old_value", "new_value"):
             table.add_column(column)
@@ -190,15 +191,16 @@
                               entity.description, project, str(len(tasks)))
         if table.row_count:
             self.console.print(table)
         if print_options.show_tasks and tasks:
             self.print_task(entities=tasks,
                             repo=repo,
                             print_options=print_options,
-                            show_window=False)
+                            show_window=False,
+                            view_level=composite_type[:-1])
         if print_options.show_tasks and completed_tasks:
             self.print_task(entities=completed_tasks,
                             repo=repo,
                             print_options=print_options,
                             show_window=False)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entity.commentaries):
@@ -255,48 +257,53 @@
             task_print_options = deepcopy(print_options)
             task_print_options.show_commentaries = False
             self.print_task(entities=tasks,
                             repo=repo,
                             print_options=task_print_options,
                             story_points=story_points,
                             kwargs=kwargs,
-                            show_window=False)
+                            show_window=False,
+                            view_level="sprint")
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entities[0].commentaries):
             self.print_commentaries(commentaries)
         if viz := print_options.show_viz:
             if "cfd" in viz:
                 dates = [
-                    date.strftime("%Y-%m-%d")
-                    for date in pd.date_range(entity.start_date, entity.end_date).
-                    to_pydatetime().tolist()
+                    date.strftime("%Y-%m-%d") for date in pd.date_range(
+                        entity.start_date,
+                        entity.end_date).to_pydatetime().tolist()
                 ]
                 status_changes = views.status_changes(repo.session, 2)
                 placeholders = pd.DataFrame(data=list(
                     itertools.product([task.id for task in tasks], dates)),
                                             columns=["task", "date"])
-                history = self._restore_status_history(placeholders, status_changes)
+                history = self._restore_status_history(placeholders,
+                                                       status_changes)
                 # TODO: aggreggate history ty date and number of tasks within the state
                 # plt.date_form('Y-m-d')
                 # y = range(1, 10)
                 # y2 = range(2, 20, 2)
                 # y3 = range(3, 30, 3)
                 # y4 = range(4, 40, 4)
                 # y5 = range(5, 50, 5)
                 # plt.plot(dates, y2,  fillx=True, color="green", label="TODO")
                 # plt.plot(dates, y3,  fillx=False, color="blue", label="IN_PROGRESS")
                 # plt.plot(dates, y4,  fillx=False, color="red", label="REVIEW")
                 # plt.plot(dates, y5,  fillx=False, color="black", label="DONE")
                 # plt.plot_size(50, 15)
                 # plt.show()
             if "time" in viz:
-                time_entries = views.time_spent(repo.session, entity.start_date,
+                time_entries = views.time_spent(repo.session,
+                                                entity.start_date,
                                                 entity.end_date)
                 dates = [entry.get("date") for entry in time_entries]
-                times = [entry.get("time_spent_hours") for entry in time_entries]
+                times = [
+                    entry.get("time_spent_hours") for entry in time_entries
+                ]
                 plt.date_form('Y-m-d')
                 plt.plot_size(100, 15)
                 plt.title("Time tracker")
                 plt.bar(dates, times)
                 plt.show()
 
     def print_project(self, entities, print_options, kwargs=None):
@@ -388,14 +395,15 @@
     def print_task(self,
                    entities,
                    repo,
                    print_options,
                    custom_sort=None,
                    show_window=True,
                    story_points=None,
+                   view_level="tasks",
                    kwargs=None):
         table = Table(box=self.box, title="TASKS")
         if story_points:
             default_columns = ("id", "name", "description", "story points",
                                "status", "priority", "project", "due_date",
                                "tags", "collaborators", "time_spent")
         else:
@@ -420,27 +428,29 @@
                               reverse=True)
         table, completed_tasks, completed_story_points = self._print_task(
             table=table,
             entities=entities,
             default_columns=default_columns,
             repo=repo,
             story_points=story_points,
-            show_window=show_window)
+            show_window=show_window,
+            view_level=view_level)
         if table.row_count:
             self.console.print(table)
         if print_options.show_completed and completed_tasks:
             table = Table(box=self.box)
             table, *rest = self._print_task(
                 table=table,
                 entities=completed_tasks,
                 default_columns=default_columns,
                 repo=repo,
                 story_points=completed_story_points,
                 show_window=show_window,
-                all_tasks=False)
+                all_tasks=False,
+                view_level=view_level)
             if table.row_count:
                 self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
                 self.console.print(table)
 
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
         import inspect
         attributes = []
@@ -481,17 +491,17 @@
 
     def _format_time_spent(self, time_spent: int) -> str:
         time_spent_hours = time_spent // 60
         time_spent_minutes = time_spent % 60
         if time_spent_hours and time_spent_minutes:
             time_spent = f"{time_spent_hours}H:{time_spent_minutes}M"
         elif time_spent_hours:
-            time_spent = f"{time_spent_hours}H"
+            time_spent = f"{time_spent_hours}H:00M"
         elif time_spent_minutes:
-            time_spent = f"{time_spent_minutes}M"
+            time_spent = f"00H:{time_spent_minutes}M"
         else:
             time_spent = ""
         return time_spent
 
     def _get_filtered_entities(self, entities, kwargs):
         if kwargs:
             filtering_attributes = set(list(kwargs))
@@ -530,15 +540,16 @@
     def _print_task(self,
                     table,
                     entities,
                     default_columns,
                     repo,
                     story_points=None,
                     all_tasks=True,
-                    show_window=True):
+                    show_window=True,
+                    view_level="tasks"):
         if all_tasks:
             completed_tasks = []
         else:
             completed_tasks = None
             completed_story_points = None
         if story_points:
             completed_story_points = []
@@ -553,16 +564,29 @@
         for entity in entities:
             if story_points:
                 story_point = entity[1]
                 entity = entity[0]
             else:
                 story_point = None
             if tags := entity.tags:
-                tag_texts = sorted([tag.base_tag.text for tag in list(tags)])
-                tag_string = ",".join(tag_texts)
+                tag_texts = []
+                for tag in list(tags):
+                    tag_text = tag.base_tag.text
+                    if not tag_text.startswith(view_level):
+                        if tag_text.startswith("sprint"):
+                            tag_texts.append(f"[yellow]{tag_text}[/yellow]")
+                        elif tag_text.startswith("epic"):
+                            tag_texts.append(f"[green]{tag_text}[/green]")
+                        elif tag_text.startswith("story"):
+                            tag_texts.append(f"[magenta]{tag_text}[/magenta]")
+                        elif tag_text.startswith("bug"):
+                            tag_texts.append(f"[red]{tag_text}[/red]")
+                        else:
+                            tag_texts.append(tag_text)
+                tag_string = ",".join(sorted(tag_texts))
             else:
                 tag_string = ""
             if collaborators := entity.collaborators:
                 collaborators_texts = sorted([
                     collaborator.users.name
                     for collaborator in list(collaborators)
                     if collaborator.users
@@ -624,33 +648,31 @@
         #     self.print_commentaries(commentaries)
         # # TODO: not working
         # if print_options.show_history and (history := entity.history):
         #     self.print_history(history)
         return table, completed_tasks, completed_story_points
 
     def _restore_status_history(self, placeholders, status_history):
-        partial_history = status_history[status_history["last_status_for_date"].notnull()]
-        current_values = status_history[["task", "current_status"]].drop_duplicates()
+        partial_history = status_history[
+            status_history["last_status_for_date"].notnull()]
+        current_values = status_history[["task",
+                                         "current_status"]].drop_duplicates()
         if not partial_history.empty:
             joined = pd.merge(placeholders,
                               partial_history,
                               on=["task", "date"],
                               how="left")
             joined = joined.replace({np.nan: None})
             joined["filled_backward"] = joined.groupby(
                 "task")["first_status_for_date"].bfill()
             joined["filled_forward"] = joined.groupby(
                 "task")["last_status_for_date"].ffill()
             joined["filled_forward"] = joined.groupby(
-                "task")["filled_forward"].fillna(
-                    joined.pop("filled_backward"))
-            joined = pd.merge(joined,
-                              current_values,
-                              on="task",
-                              how="left")
+                "task")["filled_forward"].fillna(joined.pop("filled_backward"))
+            joined = pd.merge(joined, current_values, on="task", how="left")
             joined["status"] = joined["filled_forward"]
         else:
             joined = pd.merge(placeholders,
                               current_values,
                               on="task",
                               how="left")
         return joined[["date", "task", "status"]]
```

### Comparing `terka-1.7.1.1/terka/service_layer/services.py` & `terka-1.7.2/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/service_layer/ui.py` & `terka-1.7.2/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/service_layer/vertical_layout.css` & `terka-1.7.2/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/service_layer/views.py` & `terka-1.7.2/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.1.1/terka/utils.py` & `terka-1.7.2/terka/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,17 @@
 def convert_status(status: str):
     conversion_dict = {
         "b": "BACKLOG",
         "t": "TODO",
         "i": "IN_PROGRESS",
         "r": "REVIEW",
         "d": "DONE",
-        "x": "DELETED"
+        "x": "DELETED",
+        "a": "ACTIVE",
+        "p": "PLANNED"
     }
     return conversion_dict.get(status[0].lower(), "BACKLOG")
 
 
 def convert_date(date: str):
     if not date:
         return date
```

### Comparing `terka-1.7.1.1/terka.egg-info/SOURCES.txt` & `terka-1.7.2/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

