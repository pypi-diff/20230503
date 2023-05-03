# Comparing `tmp/multi_repo_automation-0.3.0.tar.gz` & `tmp/multi_repo_automation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_repo_automation-0.3.0.tar", max compression
+gzip compressed data, was "multi_repo_automation-0.3.1.tar", max compression
```

## Comparing `multi_repo_automation-0.3.0.tar` & `multi_repo_automation-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1284 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/LICENSE
--rw-r--r--   0        0        0     2516 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/README.md
--rw-r--r--   0        0        0    26172 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/__init__.py
--rw-r--r--   0        0        0    19015 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/editor.py
--rw-r--r--   0        0        0     4901 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/tools.py
--rw-r--r--   0        0        0     2249 2023-04-20 16:16:46.695219 multi_repo_automation-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 multi_repo_automation-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1284 2023-05-03 10:03:30.049856 multi_repo_automation-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2516 2023-05-03 10:03:30.049856 multi_repo_automation-0.3.1/README.md
+-rw-r--r--   0        0        0    26172 2023-05-03 10:03:30.049856 multi_repo_automation-0.3.1/multi_repo_automation/__init__.py
+-rw-r--r--   0        0        0    19032 2023-05-03 10:03:30.049856 multi_repo_automation-0.3.1/multi_repo_automation/editor.py
+-rw-r--r--   0        0        0     4880 2023-05-03 10:03:30.049856 multi_repo_automation-0.3.1/multi_repo_automation/tools.py
+-rw-r--r--   0        0        0     2247 2023-05-03 10:03:51.642015 multi_repo_automation-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 multi_repo_automation-0.3.1/PKG-INFO
```

### Comparing `multi_repo_automation-0.3.0/LICENSE` & `multi_repo_automation-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-0.3.0/README.md` & `multi_repo_automation-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-0.3.0/multi_repo_automation/__init__.py` & `multi_repo_automation-0.3.1/multi_repo_automation/__init__.py`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-0.3.0/multi_repo_automation/editor.py` & `multi_repo_automation-0.3.1/multi_repo_automation/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                             new_data.splitlines(keepends=True),
                         )
                     )
                 else:
                     with open(self.filename, "w", encoding="utf-8") as file_:
                         file_.write(new_data)
                     if os.path.exists(".pre-commit-config.yaml") and self.run_pre_commit:
-                        proc = run(["pre-commit", "run", "--files", self.filename], False)
+                        proc = run(["pre-commit", "run", "--color=never", "--files", self.filename], False)
                         if proc.returncode != 0 and os.environ.get("DEBUG", "false").lower() in ("true", "1"):
                             proc = run(["pre-commit", "run", "--files", self.filename], False)
                             if proc.returncode != 0:
                                 edit([self.filename])
         return False
 
     @abstractmethod
```

### Comparing `multi_repo_automation-0.3.0/multi_repo_automation/tools.py` & `multi_repo_automation-0.3.1/multi_repo_automation/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     remote: str
     stabilization_branches: List[str]
     stabilization_version_to_branch: Dict[str, str]
     folders_to_clean: List[str]
     clean: bool
 
 
-_REPO_CONFIG: Union[Repo, Dict[str, None]] = {}  # pylint: disable=invalid-name
+_REPO_CONFIG: Union[Repo, Dict[str, None]] = {}
 
 
 def set_repo_config(repo_config: Repo) -> None:
     """Set the repository configuration."""
 
     global _REPO_CONFIG  # pylint: disable=global-statement
     _REPO_CONFIG = repo_config
@@ -100,33 +100,33 @@
         if os.path.isfile(".repo.yaml"):
             with open(".repo.yaml", encoding="utf-8") as file:
                 repo = cast(Repo, yaml.safe_load(file))
 
         if "remote" not in repo:
             remotes = run(["git", "remote", "--verbose"], stdout=subprocess.PIPE).stdout.strip().split("\n")
             for remote in remotes:
-                if remote.startswith("upstream "):
+                if remote.startswith("upstream\t"):
                     repo["remote"] = "upstream"
                     break
 
-            if "name" not in repo:
+            if "remote" not in repo:
                 for remote in remotes:
-                    if remote.startswith("origin "):
+                    if remote.startswith("origin\t"):
                         repo["remote"] = "origin"
                         break
 
-            if "name" not in repo:
+            if "remote" not in repo:
                 for remote in remotes:
-                    repo["remote"] = remote.split()[0]
+                    repo["remote"] = remote.split("\t")[0]
                     break
 
         if "name" not in repo:
             remotes = run(["git", "remote", "--verbose"], stdout=subprocess.PIPE).stdout.strip().split("\n")
             for remote in remotes:
-                if remote.startswith(f"{repo['remote']} "):
+                if remote.startswith(f"{repo['remote']}\t"):
                     repo["name"] = remote.split()[1].split(":")[1].replace(".git", "")
                     break
 
         if "dir" not in repo:
             repo["dir"] = os.getcwd()
 
     return repo
```

### Comparing `multi_repo_automation-0.3.0/pyproject.toml` & `multi_repo_automation-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "multi-repo-automation"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library for automation updates on multiple repositories."
 readme = "README.md"
 keywords = ["pre-commit"]
 license = "BSD-2-Clause"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -34,28 +34,28 @@
 ]
 authors = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 repository = "https://github.com/sbrunner/multi-repo-automation"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 PyYAML = "6.0"
-requests = "2.28.2"
+requests = "2.29.0"
 "ruamel.yaml" = "0.17.21"
-identify = "2.5.22"
+identify = "2.5.23"
 c2cciutils = { version = "1.5.2", optional = true }
-tomlkit = "0.11.7"
+tomlkit = "0.11.8"
 configupdater = "3.1.1"
 
 [tool.poetry.extras]
 update_stabilization_branches = ["c2cciutils"]
 
 [tool.poetry.group.dev.dependencies]
 prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.9.0" }
 types-PyYAML = "6.0.12.9"
-types-requests = "2.28.11.17"
+types-requests = "2.29.0.0"
 
 [tool.poetry.scripts]
 mra-update-stabilization-branches = 'multi_repo_automation:update_stabilization_branches_main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "poetry-plugin-tweak-dependencies-version"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multi_repo_automation-0.3.0/PKG-INFO` & `multi_repo_automation-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-repo-automation
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for automation updates on multiple repositories.
 Home-page: https://github.com/sbrunner/multi-repo-automation
 License: BSD-2-Clause
 Keywords: pre-commit
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Requires-Python: >=3.8,<4.0
```

