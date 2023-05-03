# Comparing `tmp/pysqa-0.0.8.tar.gz` & `tmp/pysqa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqa-0.0.8.tar", last modified: Thu May 14 16:24:07 2020, max compression
+gzip compressed data, was "dist/pysqa-0.0.9.tar", last modified: Wed Aug 19 05:34:30 2020, max compression
```

## Comparing `pysqa-0.0.8.tar` & `pysqa-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 16:24:07.000000 pysqa-0.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2020-05-14 16:22:45.000000 pysqa-0.0.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-05-14 16:22:45.000000 pysqa-0.0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-05-14 16:24:07.000000 pysqa-0.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4010 2020-05-14 16:22:45.000000 pysqa-0.0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16112 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3598 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/modular.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6442 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/queueadapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/queues.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9771 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa/wrapper/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/gent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/lsf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/moab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1982 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/sge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1835 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/slurm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2020-05-14 16:22:45.000000 pysqa-0.0.8/pysqa/wrapper/torque.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-05-14 16:24:07.000000 pysqa-0.0.8/pysqa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-05-14 16:24:07.000000 pysqa-0.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2020-05-14 16:22:45.000000 pysqa-0.0.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-05-14 16:22:45.000000 pysqa-0.0.8/versioneer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2020-08-19 05:32:52.000000 pysqa-0.0.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-08-19 05:32:52.000000 pysqa-0.0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-08-19 05:34:30.000000 pysqa-0.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4010 2020-08-19 05:32:52.000000 pysqa-0.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16262 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/basic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3632 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/modular.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6905 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/queueadapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/queues.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10075 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/wrapper/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/gent.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/lsf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/moab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/sge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1963 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/slurm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/torque.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-08-19 05:34:30.000000 pysqa-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2020-08-19 05:32:52.000000 pysqa-0.0.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-08-19 05:32:52.000000 pysqa-0.0.9/versioneer.py
```

### Comparing `pysqa-0.0.8/LICENSE` & `pysqa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/PKG-INFO` & `pysqa-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pysqa
-Version: 0.0.8
+Version: 0.0.9
 Summary: pysqa - simple queue adapter
 Home-page: https://github.com/pyiron/pysqa
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Description: The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
 Keywords: pysqa
```

### Comparing `pysqa-0.0.8/README.md` & `pysqa-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/basic.py` & `pysqa-0.0.9/pysqa/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
             module_name = None
         else:
             raise ValueError()
         if self._config["queue_type"] != "REMOTE":
             self._commands = getattr(importlib.import_module(module_name), class_name)()
         self._queues = Queues(self.queue_list)
         self._remote_flag = False
+        self._ssh_delete_file_on_remote = True
+
+    @property
+    def ssh_delete_file_on_remote(self):
+        return self._ssh_delete_file_on_remote
 
     @property
     def remote_flag(self):
         return self._remote_flag
 
     @property
     def config(self):
```

### Comparing `pysqa-0.0.8/pysqa/cmd.py` & `pysqa-0.0.9/pysqa/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
             elif opt in ("-t", "--run_time"):
                 run_time_max = arg
             elif opt in ("-c", "--command"):
                 command = arg
             elif opt in ("-r", "--reservation"):
                 mode_reservation = arg
             elif opt in ("-i", "--id"):
-                job_id = int(arg)
+                if arg != "":
+                    job_id = int(arg)
             elif opt in ("-d", "--delete"):
                 mode_delete = True
             elif opt in ("-d", "--status"):
                 mode_status = True
             elif opt in ("-l", "--list"):
                 mode_list = True
             elif opt in ("-h", "--help"):
```

### Comparing `pysqa-0.0.8/pysqa/modular.py` & `pysqa-0.0.9/pysqa/modular.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/queueadapter.py` & `pysqa-0.0.9/pysqa/queueadapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 
         Returns:
             dict:
         """
         return self._adapter.config
 
     @property
+    def ssh_delete_file_on_remote(self):
+        return self._adapter.ssh_delete_file_on_remote
+
+    @property
     def remote_flag(self):
         """
 
         Returns:
             bool:
         """
         return self._adapter.remote_flag
@@ -101,23 +105,24 @@
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
         command=None,
     ):
         """
+        Submits command to the given queue.
 
         Args:
-            queue (str/None):
-            job_name (str/None):
-            working_directory (str/None):
-            cores (int/None):
-            memory_max (int/None):
-            run_time_max (int/None):
-            command (str/None):
+            queue (str/None):  Name of the queue to submit to, must be one of the names configured for this adapter
+            job_name (str/None):  Name of the job for the underlying queuing system
+            working_directory (str/None):  Directory to run the job in
+            cores (int/None):  Number of hardware threads requested
+            memory_max (int/None):  Amount of memory requested per node in GB
+            run_time_max (int/None):  Maximum runtime in seconds
+            command (str/None):  shell command to run in the job
 
         Returns:
             int:
         """
         return self._adapter.submit_job(
             queue=queue,
             job_name=job_name,
```

### Comparing `pysqa-0.0.8/pysqa/queues.py` & `pysqa-0.0.9/pysqa/queues.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/remote.py` & `pysqa-0.0.9/pysqa/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,29 @@
         self._ssh_host = config['ssh_host']
         self._ssh_username = config['ssh_username']
         self._ssh_known_hosts = os.path.abspath(os.path.expanduser(config['known_hosts']))
         self._ssh_key = os.path.abspath(os.path.expanduser(config['ssh_key']))
         self._ssh_remote_config_dir = config['ssh_remote_config_dir']
         self._ssh_remote_path = config['ssh_remote_path']
         self._ssh_local_path = os.path.abspath(os.path.expanduser(config['ssh_local_path']))
+        if 'ssh_delete_file_on_remote' in config.keys():
+            self._ssh_delete_file_on_remote = config['ssh_delete_file_on_remote']
+        else:
+            self._ssh_delete_file_on_remote = True
         if 'ssh_port' in config.keys():
             self._ssh_port = config['ssh_port']
         else:
             self._ssh_port = 22
         self._ssh_continous_connection = 'ssh_continous_connection' in config.keys()
         if self._ssh_continous_connection:
             self._ssh_connection = self._open_ssh_connection()
         else:
             self._ssh_connection = None
         self._remote_flag = True
-
+        
     def convert_path_to_remote(self, path):
         working_directory = os.path.abspath(os.path.expanduser(path))
         return self._get_remote_working_dir(
             working_directory=working_directory
         )
 
     def submit_job(
@@ -160,15 +164,18 @@
             else:
                 ssh = self._open_ssh_connection()
             sftp_client = ssh.open_sftp()
         else:
             sftp_client = sftp
         for file_src, file_dst in tqdm(file_dict.items()):
             if transfer_back:
-                sftp_client.get(file_dst, file_src)
+                try:
+                    sftp_client.get(file_dst, file_src)
+                except FileNotFoundError:
+                    pass
             else:
                 sftp_client.put(file_src, file_dst)
         if sftp is None:
             sftp_client.close()
 
     def _open_ssh_connection(self):
         ssh = paramiko.SSHClient()
```

### Comparing `pysqa-0.0.8/pysqa/wrapper/gent.py` & `pysqa-0.0.9/pysqa/wrapper/gent.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/wrapper/lsf.py` & `pysqa-0.0.9/pysqa/wrapper/lsf.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/wrapper/moab.py` & `pysqa-0.0.9/pysqa/wrapper/moab.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa/wrapper/sge.py` & `pysqa-0.0.9/pysqa/wrapper/sge.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,17 +45,17 @@
                 {sub_child.tag: sub_child.text for sub_child in child} for child in leaf
             ]
 
         tree = ETree.fromstring(queue_status_output)
         df_running_jobs = pandas.DataFrame(leaf_to_dict(leaf=tree[0]))
         df_pending_jobs = pandas.DataFrame(leaf_to_dict(leaf=tree[1]))
         df_merge = df_running_jobs.append(df_pending_jobs, sort=True)
-        df_merge.state[df_merge.state == "r"] = "running"
-        df_merge.state[df_merge.state == "qw"] = "pending"
-        df_merge.state[df_merge.state == "Eqw"] = "error"
+        df_merge.loc[df_merge.state == "r", 'state'] = "running"
+        df_merge.loc[df_merge.state == "qw", 'state'] = "pending"
+        df_merge.loc[df_merge.state == "Eqw", 'state'] = "error"
         return pandas.DataFrame(
             {
                 "jobid": pandas.to_numeric(df_merge.JB_job_number),
                 "user": df_merge.JB_owner,
                 "jobname": df_merge.JB_name,
                 "status": df_merge.state,
             }
```

### Comparing `pysqa-0.0.8/pysqa/wrapper/slurm.py` & `pysqa-0.0.9/pysqa/wrapper/slurm.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,19 @@
             job_id_lst, user_lst, status_lst, job_name_lst = zip(
                 *[
                     (int(jobid), user, status.lower(), jobname)
                     for jobid, user, status, jobname in line_split_lst
                 ]
             )
         else: 
-            job_id_lst, user_lst, status_lst, job_name_lst = [], [], [],[]
-        return pandas.DataFrame(
+            job_id_lst, user_lst, status_lst, job_name_lst = [], [], [], []
+        df = pandas.DataFrame(
             {
                 "jobid": job_id_lst,
                 "user": user_lst,
                 "jobname": job_name_lst,
                 "status": status_lst,
             }
         )
+        df.loc[df.status == "r", 'status'] = "running"
+        df.loc[df.status == "pd", 'status'] = "pending"
+        return df
```

### Comparing `pysqa-0.0.8/pysqa/wrapper/torque.py` & `pysqa-0.0.9/pysqa/wrapper/torque.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/pysqa.egg-info/PKG-INFO` & `pysqa-0.0.9/pysqa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pysqa
-Version: 0.0.8
+Version: 0.0.9
 Summary: pysqa - simple queue adapter
 Home-page: https://github.com/pyiron/pysqa
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Description: The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
 Keywords: pysqa
```

### Comparing `pysqa-0.0.8/setup.py` & `pysqa-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.8/versioneer.py` & `pysqa-0.0.9/versioneer.py`

 * *Files identical despite different names*

