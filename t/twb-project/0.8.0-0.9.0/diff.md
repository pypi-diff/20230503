# Comparing `tmp/twb_project-0.8.0.tar.gz` & `tmp/twb_project-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.8.0.tar", max compression
+gzip compressed data, was "twb_project-0.9.0.tar", max compression
```

## Comparing `twb_project-0.8.0.tar` & `twb_project-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.8.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.8.0/README.md
--rw-r--r--   0        0        0      760 2023-05-02 05:53:55.856803 twb_project-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.8.0/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.8.0/twb/bip.py
--rw-r--r--   0        0        0    17118 2023-04-20 02:58:09.579621 twb_project-0.8.0/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.8.0/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.8.0/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.8.0/twb/logger.py
--rw-r--r--   0        0        0     1605 2023-05-02 05:31:50.969415 twb_project-0.8.0/twb/logger_init.py
--rw-r--r--   0        0        0    10620 2023-05-02 05:58:56.480996 twb_project-0.8.0/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.8.0/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.8.0/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.8.0/twb/utils.py
--rw-r--r--   0        0        0     3417 2023-05-02 05:44:59.869020 twb_project-0.8.0/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.8.0/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.0/README.md
+-rw-r--r--   0        0        0      760 2023-05-03 04:36:49.662491 twb_project-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.0/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.0/twb/bip.py
+-rw-r--r--   0        0        0    18740 2023-05-03 04:39:07.821059 twb_project-0.9.0/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.0/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.0/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.0/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.0/twb/logger.py
+-rw-r--r--   0        0        0     1594 2023-05-02 23:19:18.752642 twb_project-0.9.0/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.0/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.0/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.0/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.0/twb/utils.py
+-rw-r--r--   0        0        0     5284 2023-05-03 04:25:54.008631 twb_project-0.9.0/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.0/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.0/PKG-INFO
```

### Comparing `twb_project-0.8.0/LICENSE` & `twb_project-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/README.md` & `twb_project-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/pyproject.toml` & `twb_project-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.8.0"
+version = "0.9.0"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.8.0/twb/bip.py` & `twb_project-0.9.0/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/builder.py` & `twb_project-0.9.0/twb/builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,61 @@
+import json
 import logging
 import os
+from functools import partial
+from multiprocessing import Pool
+from typing import List, Tuple, Optional
 import time
-from typing import List, Union, Callable
-import xmltodict
-import py7zr
-import json
 import uuid
 
-from .logger import universal_logger_init, twb_logger, cleanup_logger
-from .utils import get_file_list, compress_zstd, get_memory_consumption, cleanup_dir, get_curr_version, \
-    prepare_output_dir, COMPRESSION_EXTENSION
-from .bip import BlockInteriorProcessor, DefaultBIP
-from .parallelization import RDSProcessManager, RDSProcessController
+import xmltodict
+from py7zr import py7zr
+
+from .builder_helpers import extract_categories
+from .logger_init import _init_logger_main_process, _init_logger_sub_process, _init_logger_multiprocessing
+from .utils import get_file_list, prepare_output_dir, get_curr_version, cleanup_dir, compress_zstd, \
+    COMPRESSION_EXTENSION
+from .warehouse import Warehouse, get_warehouse_filenames
 
-_DEFAULT_REVISIONS_PER_BLOCK = 1000000
-_DEFAULT_START_INDEX = 0
 _DEFAULT_NUM_PROC = 1
-_DEFAULT_LOG_LEVEL = logging.DEBUG
+_DEFAULT_LOG_LEVEL = logging.INFO
 
 
 class Builder:
     """
-    The core class to generate the blocks from Wikipedia Edit History chunk.
-
-    Basic usage:
-
-        import twb
-        builder = twb.Builder()  # Create an instance.
-        builder.preload('./test/sample_data/minimal_sample.xml')  # Preload the files to be processed.
-        builder.build('./test/output')  # Build the blocks.
-
-    You must preload the files to be processed before building the blocks.
-    Preload function accepts a path to a file or a directory, and can be called multiple times (for multiple files).
-
     Attributes:
+        output_dir (str): The output directory.
         num_proc (int): The number of processes to use.
-        log_dir (str): The dir to the log file.
         log_level (int): The log level.
-        revisions_per_block (int): The number of revisions per block.
-        files (List[str]): The list of files to be processed. It will be finalized when the build() method is called.
+        compress (bool): Whether to compress the output files.
+        files (list): A list of files to be read.
     """
 
     def __init__(self,
-                 log_dir: Union[str, None] = None,
-                 num_proc: Union[int, None] = _DEFAULT_NUM_PROC,
-                 revisions_per_block: int = _DEFAULT_REVISIONS_PER_BLOCK,
-                 log_level: int = _DEFAULT_LOG_LEVEL):
+                 output_dir: str,
+                 num_proc: int = _DEFAULT_NUM_PROC,
+                 log_level: int = _DEFAULT_LOG_LEVEL,
+                 max_size: int = 16,
+                 compress: bool = True):
         """
-        :param log_dir: the dir to the log file (default: None) (Will be cleaned up if exists)
-        :param num_proc: the number of processes (default: 1) (Set to None to use all available processes)
-        :param revisions_per_block: the number of revisions per block (default: 300000)
-        :param log_level: the log level (default: logging.DEBUG)
+        :param output_dir: the output directory
+        :param num_proc: the number of processes to use (default: 1)
+        :param log_level: the log level (default: logging.INFO)
+        :param max_size: the maximum size of an uncompressed warehouse (default: 12)
+        :param compress: whether to compress the output files (default: True)
         """
-        self.log_dir = log_dir
+        self.output_dir = output_dir
         self.num_proc = num_proc
-        self.revisions_per_block = revisions_per_block
         self.log_level = log_level
+        self.max_size = max_size
+        self.compress = compress
 
-        self.files = []
-
-        # Clean up the log dir if exists.
-        cleanup_logger(log_name='builder', log_dir=log_dir)
+        self.files: List[str] = []
 
-        # Initialize the logger.
-        universal_logger_init(log_name='builder', log_dir=log_dir, log_level=log_level)
+        _init_logger_main_process(log_level=self.log_level)
 
     def preload(self, path: str):
         """
         Preload the files to be processed.
         It will not actually load to the memory until the build() method is called.
         :param path: the path of a file or a directory
         :raise ValueError: if the path is empty
@@ -75,352 +63,395 @@
         """
         if not path:
             raise ValueError('The path cannot be empty.')
         if not os.path.exists(path):
             raise FileNotFoundError('The path does not exist.')
         self.files.extend(get_file_list(path))
 
-    def build(self,
-              output_dir: str,
-              start_index: int = _DEFAULT_START_INDEX,
-              processor: BlockInteriorProcessor = DefaultBIP(),
-              compress: bool = True):
+    def _worker_initializer(self, q):
         """
-        Build the blocks.
-        :param output_dir: the output directory for the blocks (will be created if not exists)
-        :param start_index: the starting index of the blocks (default: 0)
-        :param processor: the interior processor for blocks (default: DefaultBIP)
-        :param compress: whether to compress the blocks (default: True)
-        :raise Warning: if there is no file to process
+        Initialize the worker process.
         """
-        # Log the version.
-        twb_logger.info(f'TWB Package Version: {get_curr_version()}')
+        # Initialize the logger within the sub-process.
+        _init_logger_sub_process(q, log_level=self.log_level)
 
-        log_dir = self.log_dir
-        num_proc = self.num_proc
-        revisions_per_block = self.revisions_per_block
-        log_level = self.log_level
-        zip_file_list = self.files
-
-        # If there is no file to process, raise a warning and return.
-        if len(zip_file_list) == 0:
-            raise Warning('There is no file to process.')
+    def _decompress_executor(self, file_path: str) -> List[str]:
+        # Initialize temporary directory.
+        temp_dir = os.path.join(self.output_dir, 'temp')
+        os.makedirs(temp_dir, exist_ok=True)
+
+        archive_filename = os.path.basename(file_path)
+        decompressed_dir_name = '.'.join(archive_filename.split('.')[:-1])
+        decompressed_dir_path = os.path.join(temp_dir, decompressed_dir_name)
+        os.makedirs(decompressed_dir_path, exist_ok=True)
 
-        # Prepare the output directory.
-        prepare_output_dir(output_dir)
-
-        # Create the temporary directory.
-        temp_dir = os.path.join(output_dir, 'temp')
-        os.makedirs(temp_dir)
-
-        # Decompress the files in parallel.
-        twb_logger.info('Starting RDS process manager...')
-
-        process_manager_context = {
-            'processor': processor,  # The interior processor for blocks.
-            'compress': compress,  # Whether to compress the blocks.
-            'revisions_per_block': revisions_per_block,  # Number of revisions per block.
-            'total_count': len(zip_file_list),  # Total number of files to process.
-        }
-
-        curr_count = 0
-        total_count = len(zip_file_list)
-
-        def _success_callback(result):
-            nonlocal curr_count
-            curr_count += 1
-            curr_processed_progress = curr_count / total_count * 100 if total_count > 0 else -1
-            twb_logger.info(f'{curr_count} / {total_count} ==> ({curr_processed_progress:.2f}%)')
-
-        def _error_callback(e):
-            twb_logger.error('An error occurred in a sub-process which makes it terminated.',
-                             'Check next error log for details.')
-            twb_logger.error(e)
-
-            nonlocal curr_count
-            curr_count += 1
-            curr_processed_progress = curr_count / total_count * 100 if total_count > 0 else -1
-            twb_logger.info(f'{curr_count} / {total_count} ==> ({curr_processed_progress:.2f}%) (Terminated)')
-
-        start_time = time.time()
-
-        pm = RDSProcessManager(
-            log_name='builder',
-            log_dir=log_dir,
-            log_level=log_level,
-            num_proc=num_proc,
-            start_index=start_index
-        )
-        for path in zip_file_list:
-            pm.apply_async(
-                executable=_file_processor,
-                args=(path, output_dir, process_manager_context),
-                callback=_success_callback,
-                error_callback=_error_callback,
-            )
-
-        pm.close()
-        pm.join()
-
-        end_time = time.time()
-        execution_duration = end_time - start_time
-        twb_logger.info(f"!!! All done. (Took {execution_duration:.2f} seconds in total)")
-
-        # Clean up the temporary directory.
-        cleanup_dir(temp_dir)
-
-
-def _file_processor(controller: RDSProcessController,
-                    path: str,
-                    output_dir: str,
-                    context: dict):
-    # If the file does not exist, skip it.
-    if not os.path.exists(path):
-        controller.logfatal(f'File does not exist: {path}')
-        return
-
-    # If the file is not a 7z file, skip it.
-    if not path.endswith('.7z'):
-        controller.logwarn(f'Skipped because the file is not a 7z file. ({path})')
-        return
-
-    # Get the block interior processor from the running context.
-    block_interior_processor = context.get('processor', DefaultBIP())
-    should_compress = context.get('compress', True)
-    revisions_per_block = context.get('revisions_per_block', _DEFAULT_REVISIONS_PER_BLOCK)
-
-    # Generate a temporary id for the file.
-    temp_id = uuid.uuid4().hex
-
-    # Compute the path for the temporary directory in this task (associated with this temp_id).
-    temp_dir = os.path.join(output_dir, 'temp', temp_id)
-
-    # Register the temporary directory for cleanup previous temporary folders associated with the same pid.
-    controller.register(temp_dir)
-
-    # Create the temporary directory.
-    os.makedirs(temp_dir)
-
-    # Create the temporary directories for compression and decompression.
-    compression_temp_dir = os.path.join(temp_dir, 'compression_temp')
-    os.makedirs(compression_temp_dir)
-    decompression_temp_dir = os.path.join(temp_dir, 'decompression_temp')
-    os.makedirs(decompression_temp_dir)
-
-    # If the temporary directories are not created properly, skip it.
-    if not os.path.exists(compression_temp_dir) or not os.path.exists(decompression_temp_dir):
-        controller.logfatal(f'Failed to create temporary directories for archive: {path}')
-        return
-
-    # Log the start time.
-    very_start_time = time.time()
-
-    # First try block, catching issues during decompression.
-    try:
-        # Decompress the file. It has multi-threading support built-in and enabled by default.
-        with py7zr.SevenZipFile(path, mode='r', mp=False) as z:
+        with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
             start_time = time.time()
-            z.extractall(path=decompression_temp_dir)
+            z.extractall(path=decompressed_dir_path)
             end_time = time.time()
             execution_duration = end_time - start_time
-            archive_filename = os.path.basename(path)
-            controller.logdebug(f'Decompression took {execution_duration:.2f} seconds. ({archive_filename})')
-        decompressed_files = get_file_list(decompression_temp_dir)
-    except Exception as e:
-        controller.logerr(f'Decompression failed at {path} with error:', e)
-        cleanup_dir(temp_dir)
-        return
-
-    # Second try block, catching issues during processing (XML parsing, etc).
-    try:
-        def get_new_output_path():
-            """
-            Get the path of the next output file.
-            """
-            nonlocal controller, compression_target_dir
-            controller.logdebug('Ready to declare index (cp).')
-            curr_index = str(controller.declare_index()).zfill(8)  # 8 digits in total for scalability.
-            controller.logdebug('Done declaring index (cp).')
-            return os.path.join(compression_target_dir, f'block_{curr_index}.jsonl')
-
-        compression_target_dir = compression_temp_dir if should_compress else output_dir
-
-        total_article_count = 0
-        total_block_count = 1
-        total_revision_count = 0
-
-        revision_count = 0
-        memory_usage_records = []
-        all_memory_usage_records = []
-        curr_output_path = get_new_output_path()
+            logging.debug(f'Decompression took {execution_duration:.2f} seconds. ({archive_filename})')
+        decompressed_files = get_file_list(decompressed_dir_path)
+
+        return decompressed_files
 
-        def _super_callback(article: dict):
+    def _process_executor(self, xml_path: str) -> List[str]:
+        """
+        Process the file.
+        :param xml_path: the path of the file to be processed.
+        :return: the number of URLs processed
+        """
+        # Initialize processed directory.
+        processed_dir = os.path.join(self.output_dir, 'temp', 'processed')
+        os.makedirs(processed_dir, exist_ok=True)
+
+        article_id: Optional[str] = None
+        article_title: Optional[str] = None
+        article_info: Optional[dict] = None
+
+        # A JSONL file.
+        processed_filepath: Optional[str] = None
+
+        # A JSON file (which is metadata exclusively for this article).
+        processed_metadata_filepath: Optional[str] = None
+
+        processed_files = []
+
+        def _create_new_article(new_article_id: str):
+            nonlocal article_id, article_info, processed_filepath, processed_metadata_filepath
+            article_id = new_article_id
+            # NOTE: We do not clean up the title because the title should be seen before the article id.
+            article_info = dict()
+
+            # Will be used for file names.
+            random_id = uuid.uuid4().hex
+
+            # Create the processed file for this article.
+            processed_filepath = os.path.join(processed_dir, f'{random_id}.jsonl')
+            processed_metadata_filepath = os.path.join(processed_dir, f'{random_id}.metadata')
+
+            # Create empty files.
+            with open(processed_filepath, 'w') as processed_file:
+                processed_file.truncate(0)
+            with open(processed_metadata_filepath, 'w') as processed_metadata_file:
+                processed_metadata_file.truncate(0)
+
+        def _cleanup_article():
+            nonlocal article_id, article_info, article_title, processed_filepath, processed_metadata_filepath
+            article_id = None
+            article_info = None
+            article_title = None
+            processed_filepath = None
+            processed_metadata_filepath = None
+
+        def _finalizing_metadata():
             """
-            The super callback for the XML parser. It will be called recursively for each article.
+            After finishing writing an article, we will finalize the metadata file.
             """
-            controller.logdebug('_super_callback() calling.')
+            nonlocal article_id, article_info, article_title, processed_filepath, processed_metadata_filepath
+            if article_id is None:
+                return
+            with open(processed_metadata_filepath, 'w') as processed_metadata_file:
+                article_info['id'] = article_id
+                article_info['title'] = article_title
+                article_info['categories'] = extract_categories(article_info['last_valid_text_content'])
+                del article_info['last_valid_text_content']
+                json.dump(article_info, processed_metadata_file, indent=2)
+            processed_files.append((processed_filepath, processed_metadata_filepath))
+
+        def _inner_callback(path, item):
+            nonlocal article_id, article_info, article_title, processed_filepath, processed_metadata_filepath
+            if path[-1][0] == 'title':
+                # When a new article title is encountered, clean up the previous article and save the title for later.
+                _finalizing_metadata()
+                _cleanup_article()
+                article_title = item.strip()
+            if path[-1][0] == 'id':
+                # When a new article id is encountered, create a new file for processing the article.
+                _create_new_article(new_article_id=item.strip())
+            if type(item) is dict and 'text' in item and '#text' in item['text']:
+                to_be_written = {
+                    'article_id': article_id,
+                    'revision_id': item['id'],
+                    'timestamp': item['timestamp'],
+                }
+                del item['id']
+                if 'parentid' in item:
+                    to_be_written['parent_id'] = item['parentid']
+                    del item['parentid']
+                del item['timestamp']
+                to_be_written.update(item)
+                with open(processed_filepath, 'a') as processed_file:
+                    processed_file.write(json.dumps(to_be_written) + '\n')
+
+                # Prepare text content for extracting categories.
+                text_content = item['text']['#text']
+                if len(text_content) > 0 and text_content[0] != '#REDIRECT':
+                    # Extract categories.
+                    article_info['source_revision'] = to_be_written['revision_id']
+                    article_info['last_valid_text_content'] = text_content
+            return True
 
-            nonlocal total_article_count, total_block_count, total_revision_count
-            nonlocal revision_count, memory_usage_records, all_memory_usage_records, curr_output_path
+        try:
+            with open(xml_path, 'rb') as xml_file:
+                xmltodict.parse(
+                    xml_file,
+                    item_depth=3,
+                    item_callback=_inner_callback,
+                )
+
+            # Finalize the last article.
+            _finalizing_metadata()
+
+            return processed_files
+
+        except Exception as e:
+            logging.critical(f'Error occurred when processing the file [{xml_file}]: {e}')
+            return []
+
+    def _warehouse_executor(self, assigned_warehouse: str, combo_files_list: List[Tuple[str, str]]):
+        try:
+            warehouse_filename, warehouse_metadata_filename = get_warehouse_filenames(assigned_warehouse)
+            warehouse_path = os.path.join(self.output_dir, warehouse_filename)
+            warehouse_metadata_path = os.path.join(self.output_dir, warehouse_metadata_filename)
+
+            warehouse_file = open(warehouse_path, 'a')
+
+            for processed_file, metadata_file in combo_files_list:
+                # Get current byte length of the warehouse file.
+                start_len_warehouse = warehouse_file.tell()
+
+                # Read the file line by line, and move directly to the warehouse (without last empty line).
+                with open(processed_file, 'r') as f:
+                    for line in iter(f.readline, ''):
+                        warehouse_file.write(line + '\n')
+
+                end_len_warehouse = warehouse_file.tell()
+
+                # Insert the metadata file into the warehouse metadata file (with byte start and end).
+                new_metadata = json.load(open(metadata_file, 'r'))
+                new_metadata['byte_start'] = start_len_warehouse
+                new_metadata['byte_end'] = end_len_warehouse
+                with open(warehouse_metadata_path, 'a') as f:
+                    f.write(json.dumps(new_metadata) + '\n')
+
+                # Remove the modified file.
+                os.remove(processed_file)
+                os.remove(metadata_file)
+
+            warehouse_file.close()
+
+        except Exception as e:
+            logging.critical(f'Error occurred when moving the file to the warehouse. {e}')
+
+        return assigned_warehouse
+
+    def _cleanup_executor(self, warehouse_filename: str):
+        try:
+            original_file_path = os.path.join(self.output_dir, warehouse_filename)
+            if not os.path.exists(original_file_path):
+                logging.critical(f'The file {warehouse_filename} [{original_file_path}] does not exist.')
+                return None
+
+            compressed_path = original_file_path + COMPRESSION_EXTENSION
+            compress_zstd(original_file_path, compressed_path)
+            os.remove(original_file_path)
+
+            return compressed_path
+
+        except:
+            logging.critical(f'Error occurred when compressing warehouse [{warehouse_filename}].')
+            return None
 
-            controller.logdebug('_super_callback() started.')
+    def build(self):
+        """
+        Build the blocks after apply the modifiers.
+        """
+        # Log the version.
+        logging.info(f'Builder Version: {get_curr_version()}')
 
-            # If previous batch is full, store the max memory usage and reset the counters.
-            if revision_count >= revisions_per_block:
-                # Store the max memory usage in previous batch.
-                all_memory_usage_records.append(max(memory_usage_records))
-                # Update the block count.
-                total_block_count += 1
-                # Reset the counters.
-                revision_count = 0
-                memory_usage_records = []
-                curr_output_path = get_new_output_path()
-
-            # Compute the number of revisions in the current article.
-            if 'revision' in article and type(article['revision']) is list:
-                curr_article_revision_count = len(article['revision'])
-            else:
-                curr_article_revision_count = 1
+        warehouse = Warehouse(
+            output_dir=self.output_dir,
+            max_size=self.max_size,
+            compress=self.compress,
+        )
 
-            # Update the counters.
-            revision_count += curr_article_revision_count
-            total_revision_count += curr_article_revision_count
-            total_article_count += 1
+        start_time = time.time()
 
-            controller.logdebug(f'Total revision count: {total_revision_count}')
+        # Prepare the output directory.
+        prepare_output_dir(self.output_dir)
 
-            # Store the article into the current output file.
-            _store_article_to_jsonl(article=article, output_path=curr_output_path)
+        total_count = len(self.files)
 
-            controller.logdebug(f'Stored.')
+        global_temp_dir = os.path.join(self.output_dir, 'temp')
+        os.makedirs(global_temp_dir, exist_ok=True)
 
-            # Record the memory usage.
-            memory_usage_records.append(get_memory_consumption())
+        # Initialize multiprocessing logger.
+        ql, q = _init_logger_multiprocessing(log_level=self.log_level)
 
-            controller.logdebug(f'Memory: {memory_usage_records[-1]} MB')
+        # Tasks is a list of tuples (task_type, args).
+        # Task types: 'decompress', 'process', 'warehouse', 'cleanup'
+        tasks: List[Tuple[str, Tuple]] = []
 
-        controller.logdebug(f'Big parsing loop started. (revisions_per_block={revisions_per_block})')
+        available_process_count = self.num_proc
 
-        # We store articles into JSONL files in a streaming manner, along the way of parsing XML files.
-        # Therefore, we don't have to keep all the results in the memory, which is a huge problem.
-        for path in decompressed_files:
-            _parse_xml(xml_path=path, processor=block_interior_processor, super_callback=_super_callback)
+        modification_pool = Pool(
+            processes=self.num_proc,
+            initializer=self._worker_initializer,
+            initargs=(q,)
+        )
 
-        controller.logdebug('Big parsing loop done.')
+        processed_count = 0
+        finished_count = 0
 
-        if len(memory_usage_records) > 0:
-            all_memory_usage_records.append(max(memory_usage_records))
+        def _decompress_callback(decompressed_files: List[str]):
+            nonlocal available_process_count
 
-        controller.logdebug(f'Parsing done. {total_article_count} articles processed.',
-                            f'({total_revision_count} revisions are processed into {total_block_count} blocks)',
-                            f'(Highest Memory: {max(all_memory_usage_records)} MB)')
+            logging.debug(f'Decompressed: {decompressed_files}')
 
-        cleanup_dir(decompression_temp_dir)  # Delete temporary files used for decompression.
+            for decompressed_file in decompressed_files:
+                next_task_type = 'process'
+                next_args = (decompressed_file,)
+                tasks.insert(0, (next_task_type, next_args))
 
-        controller.logdebug(f'Cleaning up decompression temp dir done.')
+            available_process_count += 1
 
-        if should_compress:
-            # Store the results to JSONL files.
-            json_files = get_file_list(compression_temp_dir)
+        def _process_callback(processed_files: List[Tuple[str, str]]):
+            nonlocal warehouse, available_process_count, processed_count
+            processed_count += 1
 
-            controller.logdebug(f'Compression started. {len(json_files)} files to compress.')
+            processed_file_to_metadata_map = {
+                processed_file: metadata_file for processed_file, metadata_file in processed_files
+            }
 
-            # Compress the files.
-            for json_file in json_files:
-                controller.logdebug(f'Compressing {json_file}...')
-                _compress_file(path=json_file, output_dir=output_dir, controller=controller)
+            logging.info(f'({processed_count / total_count * 100:.2f}% = {processed_count} / {total_count}) | '
+                         f'Processed segments: {len(processed_file_to_metadata_map)}')
 
-            controller.logdebug(f'Compression done. {len(json_files)} files compressed in total.')
+            assigned_warehouses = warehouse.bulk_assign([processed_file for processed_file, _ in processed_files])
 
-    except Exception as e:
-        controller.logerr(f'Parsing failed at {path}:', e)
-    finally:
-        # Clean up the temporary directory.
-        cleanup_dir(temp_dir)
-        controller.logdebug(f'Temporary directory cleaned up: {temp_id}.')
+            for assigned_warehouse, processed_files in assigned_warehouses.items():
+                metadata_files = [processed_file_to_metadata_map[processed_file] for processed_file in processed_files]
+                combo_files_list = zip(processed_files, metadata_files)
+                next_task_type = 'warehouse'
+                next_args = (assigned_warehouse, combo_files_list)
+                tasks.insert(0, (next_task_type, next_args))
 
-        very_end_time = time.time()
-        total_execution_duration = very_end_time - very_start_time
-        controller.loginfo(f'File done: {archive_filename}. (Duration: {total_execution_duration:.2f}s)')
+            available_process_count += 1
 
-        controller.unregister()
+        def _warehouse_callback(warehouse_basename):
+            nonlocal warehouse, available_process_count, finished_count
 
+            logging.debug(f'Saved into warehouse: {warehouse_basename}')
 
-def _parse_xml(xml_path: str, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
-    """
-    Parse the XML file into a list of JSON objects.
-    :param xml_path: the path of the XML file
-    :param processor: the interior processor for blocks
-    :return: the list of parsed results
-    """
-    def _inner_callback(path, item):
-        nonlocal super_callback
+            cleanup_path = warehouse.release_warehouse(warehouse_basename)
+            if cleanup_path is not None:
+                next_task_type = 'cleanup'
+                next_args = (cleanup_path,)
+                tasks.insert(0, (next_task_type, next_args))
 
-        tag_name = path[-1][0]
-        item_type = type(item)
+            finished_count += 1
+            available_process_count += 1
 
-        # If the item is a page, we don't need to process it.
-        if tag_name != 'page':
-            return True
+        def _cleanup_callback(cleanup_path):
+            nonlocal available_process_count
+            logging.info(f'Warehouse packed: {cleanup_path}')
 
-        # If the item is not a dictionary, it means that the item is a leaf node, and we don't expect it to be a block.
-        if item_type is not dict:
-            return True
+            available_process_count += 1
 
-        logging.debug(f'Memory: {get_memory_consumption()} MB')
+        def _success_callback(task_type, file_path):
+            if task_type == 'decompress':
+                _decompress_callback(file_path)
+            elif task_type == 'process':
+                _process_callback(file_path)
+            elif task_type == 'warehouse':
+                _warehouse_callback(file_path)
+            elif task_type == 'cleanup':
+                _cleanup_callback(file_path)
 
-        logging.debug(f'Start callback: <{tag_name}>.')
-        super_callback(item)
-        logging.debug(f'Callback done: <{tag_name}>.')
-
-        return True
-
-    with open(xml_path, 'rb') as xml_file:
-        xmltodict.parse(
-            xml_file,
-            item_depth=processor.read_depth,
-            item_callback=_inner_callback,
-        )
+        def _error_callback(e):
+            logging.critical(f'Process terminated-level error: {e}')
 
-        logging.debug(f'Parsing done: {xml_path}')
+        # Built-up initial tasks.
+        for curr_file_path in self.files:
+            tasks.append(('decompress', (curr_file_path,)))
+
+        # Main semaphore loop.
+        while tasks or available_process_count < self.num_proc:
+            if tasks and available_process_count > 0:
+                available_process_count -= 1
+                task_type, args = tasks.pop(0)
+                if task_type == 'decompress':
+                    file_path, = args
+                    modification_pool.apply_async(
+                        func=self._decompress_executor,
+                        args=(file_path,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                elif task_type == 'process':
+                    xml_file_path, = args
+                    modification_pool.apply_async(
+                        func=self._process_executor,
+                        args=(xml_file_path,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                elif task_type == 'warehouse':
+                    assigned_warehouse, combo_files_list = args
+                    modification_pool.apply_async(
+                        func=self._warehouse_executor,
+                        args=(assigned_warehouse, combo_files_list),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                elif task_type == 'cleanup':
+                    warehouse_filename, = args
+                    modification_pool.apply_async(
+                        func=self._cleanup_executor,
+                        args=(warehouse_filename,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                else:
+                    logging.critical(f'Unknown task type: {task_type}')
+                    available_process_count += 1
+            else:
+                time.sleep(0.1)
 
+        logging.info('Main loop finished. Waiting for cleanup...')
 
-def _store_article_to_jsonl(article: dict, output_path: str):
-    """
-    Store the blocks to a JSONL file.
-    :param article: the article to store
-    :param output_path: the path to store the JSONL file
-    :return: the list of JSONL file paths
-    """
-    logging.debug(f'Dumping JSONL for {output_path}...')
-    dumped_article_jsonl = json.dumps(article) + '\n'
-    logging.debug(f'Storing JSONL (len: {len(dumped_article_jsonl)}) to {output_path}...')
-    try:
-        with open(output_path, 'a', buffering=10 * 1024 * 1024) as f:
-            logging.debug(f'Writing to {output_path}...')
-            f.write(dumped_article_jsonl)
-    except Exception as e:
-        logging.fatal(f'Error in writing article: {e}')
-    logging.debug(f'Storing JSONL done: {output_path}.')
+        if self.compress:
+            for final_warehouse in warehouse.available_warehouses:
+                next_task_type = 'cleanup'
+                warehouse_filename = get_warehouse_filenames(final_warehouse)[0]
+                next_args = (warehouse_filename,)
+                tasks.append((next_task_type, next_args))
+
+        # Final cleanup loop.
+        while tasks or available_process_count < self.num_proc:
+            if tasks and available_process_count > 0:
+                available_process_count -= 1
+                task_type, args = tasks.pop(0)
+                if task_type == 'cleanup':
+                    warehouse_filename, = args
+                    modification_pool.apply_async(
+                        func=self._cleanup_executor,
+                        args=(warehouse_filename,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                else:
+                    logging.critical(f'Unknown task type: {task_type}')
+                    available_process_count += 1
+            else:
+                time.sleep(0.1)
 
+        logging.info(f'Cleanup loop finished.')
 
-def _compress_file(path: str, output_dir: str, controller: RDSProcessController):
-    """
-    Compress a file.
-    :param path: the path of the file to compress
-    :param output_dir: the directory to store the compressed file
-    :return:
-    """
-    # If the file is not a JSONL file, skip it.
-    if not path.endswith('.jsonl'):
-        controller.logwarn(f'Skipped because the file is not a JSONL file. ({path})')
-        return
-
-    output_path = os.path.join(output_dir, os.path.basename(path) + COMPRESSION_EXTENSION)
-
-    try:
-        # Compress the file using Zstandard.
-        # TODO: Might be able to specify multiprocessing or multithreading. Check the documentation.
-        #  If possible, we should use multithreading in order to utilize the CPU cores in this case.
-        compress_zstd(input_path=path, output_path=output_path)
-    except Exception as e:
-        controller.logerr(f'Compression failed at {path}:', e)
+        # Clean up the global temporary directory.
+        cleanup_dir(global_temp_dir)
+
+        end_time = time.time()
+        execution_duration = end_time - start_time
+
+        # Log the end of the task.
+        logging.info(f'All done! Finished all files. (took {execution_duration:.2f}s in total)')
```

### Comparing `twb_project-0.8.0/twb/decompressor.py` & `twb_project-0.9.0/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/downloader.py` & `twb_project-0.9.0/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/logger.py` & `twb_project-0.9.0/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/logger_init.py` & `twb_project-0.9.0/twb/logger_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def _cleanup_logger_handlers(logger: logging.Logger):
     while logger.hasHandlers():
         logger.removeHandler(logger.handlers[0])
 
 
-def _init_logger_main_process(name: str, log_level: int):
+def _init_logger_main_process(log_level: int):
     stream_handler = _get_logger_stream_handler(log_level=log_level)
     logger = logging.getLogger()
     _cleanup_logger_handlers(logger)
     logger.setLevel(log_level)
     logger.addHandler(stream_handler)
```

### Comparing `twb_project-0.8.0/twb/modifier.py` & `twb_project-0.9.0/twb/modifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.output_dir = output_dir
         self.num_proc = num_proc
         self.log_level = log_level
 
         self.files: List[str] = []
         self.modifiers: List[ModifierProfile] = []
 
-        _init_logger_main_process(name='modifier', log_level=self.log_level)
+        _init_logger_main_process(log_level=self.log_level)
 
     def preload(self, path: str):
         """
         Preload the files to be processed.
         It will not actually load to the memory until the build() method is called.
         :param path: the path of a file or a directory
         :raise ValueError: if the path is empty
```

### Comparing `twb_project-0.8.0/twb/parallelization.py` & `twb_project-0.9.0/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/reader.py` & `twb_project-0.9.0/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/twb/utils.py` & `twb_project-0.9.0/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.8.0/setup.py` & `twb_project-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.8.0/PKG-INFO` & `twb_project-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.8.0
+Version: 0.9.0
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

