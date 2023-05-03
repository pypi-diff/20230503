# Comparing `tmp/griptape-0.7.1.tar.gz` & `tmp/griptape-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.7.1.tar", max compression
+gzip compressed data, was "griptape-0.7.2.tar", max compression
```

## Comparing `griptape-0.7.1.tar` & `griptape-0.7.2.tar`

### file list

```diff
@@ -1,121 +1,120 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.7.1/LICENSE
--rw-r--r--   0        0        0     3938 2023-04-30 20:17:25.931115 griptape-0.7.1/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.7.1/griptape/__init__.py
--rw-r--r--   0        0        0      252 2023-04-30 17:35:29.017295 griptape-0.7.1/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0      350 2023-04-30 17:13:30.434774 griptape-0.7.1/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      614 2023-04-30 17:35:28.969088 griptape-0.7.1/griptape/artifacts/error_artifact.py
--rw-r--r--   0        0        0      595 2023-04-30 17:35:28.959962 griptape-0.7.1/griptape/artifacts/text_artifact.py
--rw-r--r--   0        0        0      259 2023-04-28 14:34:39.021439 griptape-0.7.1/griptape/converters/__init__.py
--rw-r--r--   0        0        0      220 2023-04-28 14:34:39.020206 griptape-0.7.1/griptape/converters/base_converter.py
--rw-r--r--   0        0        0     2710 2023-04-30 17:35:29.011420 griptape-0.7.1/griptape/converters/chatgpt_plugin_converter.py
--rw-r--r--   0        0        0     1075 2023-04-30 17:35:28.978469 griptape-0.7.1/griptape/converters/langchain_tool_converter.py
--rw-r--r--   0        0        0      180 2023-04-28 15:15:41.999422 griptape-0.7.1/griptape/core/__init__.py
--rw-r--r--   0        0        0     2035 2023-04-27 23:20:01.169051 griptape-0.7.1/griptape/core/activity_mixin.py
--rw-r--r--   0        0        0     4055 2023-04-30 19:31:02.383166 griptape-0.7.1/griptape/core/base_tool.py
--rw-r--r--   0        0        0      533 2023-04-28 15:15:42.001353 griptape-0.7.1/griptape/core/decorators.py
--rw-r--r--   0        0        0      819 2023-04-27 20:13:16.211614 griptape-0.7.1/griptape/core/tool_loader.py
--rw-r--r--   0        0        0     1084 2023-04-30 19:54:49.004253 griptape-0.7.1/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.7.1/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.7.1/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.7.1/griptape/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.7.1/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-30 17:35:28.980331 griptape-0.7.1/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.7.1/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.7.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.7.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.7.1/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.7.1/griptape/drivers/storage/__init__.py
--rw-r--r--   0        0        0      320 2023-04-27 20:13:16.212485 griptape-0.7.1/griptape/drivers/storage/base_storage_driver.py
--rw-r--r--   0        0        0     1365 2023-04-30 19:56:37.363730 griptape-0.7.1/griptape/drivers/storage/dynamodb_storage_driver.py
--rw-r--r--   0        0        0      557 2023-04-27 20:13:16.212694 griptape-0.7.1/griptape/drivers/storage/memory_storage_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.7.1/griptape/executors/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-30 19:24:30.470925 griptape-0.7.1/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3326 2023-04-30 17:35:28.975177 griptape-0.7.1/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     2203 2023-04-30 17:35:28.958452 griptape-0.7.1/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.7.1/griptape/memory/__init__.py
--rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.7.1/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.7.1/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.7.1/griptape/memory/run.py
--rw-r--r--   0        0        0     2024 2023-04-30 17:51:16.198545 griptape-0.7.1/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      120 2023-04-30 19:23:55.559304 griptape-0.7.1/griptape/ramps/__init__.py
--rw-r--r--   0        0        0      526 2023-04-30 19:23:55.545401 griptape-0.7.1/griptape/ramps/base_ramp.py
--rw-r--r--   0        0        0     2590 2023-04-30 19:51:59.711107 griptape-0.7.1/griptape/ramps/storage_ramp.py
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.7.1/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.7.1/griptape/rules/__init__.py
--rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.7.1/griptape/rules/json.py
--rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.7.1/griptape/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.7.1/griptape/rules/rule.py
--rw-r--r--   0        0        0     2183 2023-04-30 17:35:28.976419 griptape-0.7.1/griptape/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.1/griptape/schemas/artifacts/__init__.py
--rw-r--r--   0        0        0      313 2023-04-30 16:38:23.177438 griptape-0.7.1/griptape/schemas/artifacts/artifact_schema.py
--rw-r--r--   0        0        0      269 2023-04-30 17:35:28.962971 griptape-0.7.1/griptape/schemas/artifacts/error_artifact_schema.py
--rw-r--r--   0        0        0      266 2023-04-30 17:35:28.966009 griptape-0.7.1/griptape/schemas/artifacts/text_artifact_schema.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.7.1/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.1/griptape/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.7.1/griptape/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.7.1/griptape/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.7.1/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.7.1/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.7.1/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.7.1/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.7.1/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.7.1/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.7.1/griptape/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.1/griptape/schemas/structures/__init__.py
--rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.7.1/griptape/schemas/structures/agent_schema.py
--rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.7.1/griptape/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.7.1/griptape/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.7.1/griptape/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.1/griptape/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.7.1/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.7.1/griptape/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.7.1/griptape/schemas/tasks/__init__.py
--rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.7.1/griptape/schemas/tasks/prompt_task_schema.py
--rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.7.1/griptape/schemas/tasks/task_schema.py
--rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.7.1/griptape/schemas/tasks/toolkit_task_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.1/griptape/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.7.1/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.7.1/griptape/structures/__init__.py
--rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.7.1/griptape/structures/agent.py
--rw-r--r--   0        0        0     2890 2023-04-30 17:35:28.986270 griptape-0.7.1/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     4369 2023-04-30 19:31:02.389059 griptape-0.7.1/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.7.1/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     3052 2023-04-30 17:35:29.008055 griptape-0.7.1/griptape/structures/workflow.py
--rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.7.1/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      535 2023-04-30 17:51:16.195968 griptape-0.7.1/griptape/summarizers/base_summarizer.py
--rw-r--r--   0        0        0     1231 2023-04-30 19:16:29.911126 griptape-0.7.1/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.7.1/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     8697 2023-04-30 19:34:32.449147 griptape-0.7.1/griptape/tasks/action_subtask.py
--rw-r--r--   0        0        0     3751 2023-04-30 17:35:28.970533 griptape-0.7.1/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     1677 2023-04-30 17:35:29.009441 griptape-0.7.1/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     3705 2023-04-30 19:31:02.377122 griptape-0.7.1/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.7.1/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.7.1/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0     2006 2023-04-30 19:31:02.384987 griptape-0.7.1/griptape/templates/prompts/base.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.7.1/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.7.1/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0      351 2023-04-30 19:31:02.380912 griptape-0.7.1/griptape/templates/prompts/ramp.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.7.1/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.7.1/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.7.1/griptape/templates/prompts/tasks/prompt.j2
--rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.7.1/griptape/templates/prompts/tasks/tool/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.7.1/griptape/templates/prompts/tasks/tool/subtasks.j2
--rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.7.1/griptape/templates/prompts/tasks/tool/tool.j2
--rw-r--r--   0        0        0      351 2023-04-28 16:20:57.373167 griptape-0.7.1/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.7.1/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      111 2023-04-30 19:36:10.118646 griptape-0.7.1/griptape/templates/ramps/storage.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.7.1/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.7.1/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.7.1/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.7.1/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.7.1/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.7.1/griptape/utils/__init__.py
--rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.7.1/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.7.1/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.7.1/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.7.1/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.7.1/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.7.1/griptape/utils/python_runner.py
--rw-r--r--   0        0        0      177 2023-04-30 19:16:29.912716 griptape-0.7.1/griptape/utils/text.py
--rw-r--r--   0        0        0     1144 2023-04-30 21:00:26.887580 griptape-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 griptape-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4585 2023-05-02 23:30:51.255832 griptape-0.7.2/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.7.2/griptape/__init__.py
+-rw-r--r--   0        0        0      252 2023-04-30 17:35:29.017295 griptape-0.7.2/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0      790 2023-05-01 15:10:00.633569 griptape-0.7.2/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      614 2023-04-30 17:35:28.969088 griptape-0.7.2/griptape/artifacts/error_artifact.py
+-rw-r--r--   0        0        0      595 2023-04-30 17:35:28.959962 griptape-0.7.2/griptape/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      259 2023-04-28 14:34:39.021439 griptape-0.7.2/griptape/converters/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-28 14:34:39.020206 griptape-0.7.2/griptape/converters/base_converter.py
+-rw-r--r--   0        0        0     2710 2023-04-30 17:35:29.011420 griptape-0.7.2/griptape/converters/chatgpt_plugin_converter.py
+-rw-r--r--   0        0        0     1075 2023-04-30 17:35:28.978469 griptape-0.7.2/griptape/converters/langchain_tool_converter.py
+-rw-r--r--   0        0        0      180 2023-04-28 15:15:41.999422 griptape-0.7.2/griptape/core/__init__.py
+-rw-r--r--   0        0        0     2035 2023-04-27 23:20:01.169051 griptape-0.7.2/griptape/core/activity_mixin.py
+-rw-r--r--   0        0        0     4110 2023-05-01 15:24:09.937386 griptape-0.7.2/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      533 2023-04-28 15:15:42.001353 griptape-0.7.2/griptape/core/decorators.py
+-rw-r--r--   0        0        0      819 2023-04-27 20:13:16.211614 griptape-0.7.2/griptape/core/tool_loader.py
+-rw-r--r--   0        0        0     1084 2023-04-30 19:54:49.004253 griptape-0.7.2/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.7.2/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.7.2/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.7.2/griptape/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.7.2/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-30 17:35:28.980331 griptape-0.7.2/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.7.2/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.7.2/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.7.2/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.7.2/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.7.2/griptape/drivers/storage/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-27 20:13:16.212485 griptape-0.7.2/griptape/drivers/storage/base_storage_driver.py
+-rw-r--r--   0        0        0     1365 2023-04-30 19:56:37.363730 griptape-0.7.2/griptape/drivers/storage/dynamodb_storage_driver.py
+-rw-r--r--   0        0        0      557 2023-04-27 20:13:16.212694 griptape-0.7.2/griptape/drivers/storage/memory_storage_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.7.2/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     1916 2023-05-01 15:10:15.434624 griptape-0.7.2/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3326 2023-04-30 17:35:28.975177 griptape-0.7.2/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     2203 2023-04-30 17:35:28.958452 griptape-0.7.2/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.7.2/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.7.2/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.7.2/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.7.2/griptape/memory/run.py
+-rw-r--r--   0        0        0     2024 2023-04-30 17:51:16.198545 griptape-0.7.2/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      120 2023-04-30 19:23:55.559304 griptape-0.7.2/griptape/ramps/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-30 19:23:55.545401 griptape-0.7.2/griptape/ramps/base_ramp.py
+-rw-r--r--   0        0        0     2708 2023-05-03 17:33:46.267063 griptape-0.7.2/griptape/ramps/storage_ramp.py
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.7.2/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.7.2/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.7.2/griptape/rules/json.py
+-rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.7.2/griptape/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.7.2/griptape/rules/rule.py
+-rw-r--r--   0        0        0     2183 2023-04-30 17:35:28.976419 griptape-0.7.2/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.2/griptape/schemas/artifacts/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-30 16:38:23.177438 griptape-0.7.2/griptape/schemas/artifacts/artifact_schema.py
+-rw-r--r--   0        0        0      269 2023-04-30 17:35:28.962971 griptape-0.7.2/griptape/schemas/artifacts/error_artifact_schema.py
+-rw-r--r--   0        0        0      266 2023-04-30 17:35:28.966009 griptape-0.7.2/griptape/schemas/artifacts/text_artifact_schema.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.7.2/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.2/griptape/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.7.2/griptape/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.7.2/griptape/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.7.2/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.7.2/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.7.2/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.7.2/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.7.2/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.7.2/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.7.2/griptape/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.2/griptape/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.7.2/griptape/schemas/structures/agent_schema.py
+-rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.7.2/griptape/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.7.2/griptape/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.7.2/griptape/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.2/griptape/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.7.2/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.7.2/griptape/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.7.2/griptape/schemas/tasks/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.7.2/griptape/schemas/tasks/prompt_task_schema.py
+-rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.7.2/griptape/schemas/tasks/task_schema.py
+-rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.7.2/griptape/schemas/tasks/toolkit_task_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.2/griptape/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.7.2/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.7.2/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.7.2/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2890 2023-04-30 17:35:28.986270 griptape-0.7.2/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     4369 2023-04-30 19:31:02.389059 griptape-0.7.2/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.7.2/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     3052 2023-04-30 17:35:29.008055 griptape-0.7.2/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.7.2/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-30 17:51:16.195968 griptape-0.7.2/griptape/summarizers/base_summarizer.py
+-rw-r--r--   0        0        0     1383 2023-05-03 17:33:46.265382 griptape-0.7.2/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.7.2/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     8697 2023-04-30 19:34:32.449147 griptape-0.7.2/griptape/tasks/action_subtask.py
+-rw-r--r--   0        0        0     3751 2023-04-30 17:35:28.970533 griptape-0.7.2/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     1677 2023-04-30 17:35:29.009441 griptape-0.7.2/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     3705 2023-04-30 19:31:02.377122 griptape-0.7.2/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.7.2/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.7.2/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0     2165 2023-05-03 17:16:51.696175 griptape-0.7.2/griptape/templates/prompts/base.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.7.2/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.7.2/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0      351 2023-04-30 19:31:02.380912 griptape-0.7.2/griptape/templates/prompts/ramp.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.7.2/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.7.2/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.7.2/griptape/templates/prompts/tasks/prompt.j2
+-rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.7.2/griptape/templates/prompts/tasks/tool/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.7.2/griptape/templates/prompts/tasks/tool/subtasks.j2
+-rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.7.2/griptape/templates/prompts/tasks/tool/tool.j2
+-rw-r--r--   0        0        0      351 2023-04-28 16:20:57.373167 griptape-0.7.2/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.7.2/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      111 2023-04-30 19:36:10.118646 griptape-0.7.2/griptape/templates/ramps/storage.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.7.2/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.7.2/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.7.2/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.7.2/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.7.2/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.7.2/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.7.2/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.7.2/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.7.2/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.7.2/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.7.2/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.7.2/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0     1142 2023-05-03 17:35:24.769479 griptape-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5999 1970-01-01 00:00:00.000000 griptape-0.7.2/PKG-INFO
```

### Comparing `griptape-0.7.1/LICENSE` & `griptape-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/README.md` & `griptape-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,52 +31,69 @@
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
 With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
 
 ```python
 from decouple import config
-from griptape.tools import WebScraper, Calculator
-from griptape import utils
+from griptape.core import ToolLoader
+from griptape.drivers import OpenAiPromptDriver, MemoryStorageDriver
+from griptape.executors import LocalExecutor
 from griptape.memory import Memory
-from griptape.tasks import PromptTask, ToolkitTask
+from griptape.ramps import StorageRamp
 from griptape.structures import Pipeline
-from griptape.core import ToolLoader
+from griptape.tasks import ToolkitTask, PromptTask
+from griptape.tools import WebScraper
+
+storage = StorageRamp(
+    driver=MemoryStorageDriver()
+)
 
 scraper = WebScraper(
-    openai_api_key=config("OPENAI_API_KEY")
+    ramps={
+        "get_content": [storage]
+    }
 )
-calculator = Calculator()
 
 pipeline = Pipeline(
     memory=Memory(),
     tool_loader=ToolLoader(
-        tools=[calculator, scraper]
+        tools=[scraper],
+        executor=LocalExecutor()
     )
 )
 
 pipeline.add_tasks(
     ToolkitTask(
-        tool_names=[calculator.name, scraper.name]
+        tool_names=[scraper.name]
     ),
     PromptTask(
-        "Say the following like a pirate: {{ input }}"
+        "Say the following in spanish: {{ input }}"
     )
 )
 
-pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
+result = pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
+
+print(result.output.value)
 
-print(utils.Conversation(pipeline.memory).to_string())
 
 ```
 
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
-> Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model  
-> A: Arr, me hearties! Large language models have been developed and set sail since 2018, includin' BERT, GPT-2, GPT-3 [...]
+```
+Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model
+[chain of thought output... will vary depending on the model driver you're using]
+A: Los modelos de lenguaje de gran tamaño son herramientas utilizadas para tareas de 
+procesamiento del lenguaje natural, como detectar falsedades, completar oraciones y comprender 
+el lenguaje. Algunos modelos notables incluyen BERT, GPT-2, GPT-3, GPT-Neo y GLaM. The Pile es 
+un conjunto de datos extenso utilizado para el modelado del lenguaje. Estos modelos han sido 
+desarrollados e investigados en trabajos como TruthfulQA, HellaSwag y BERT: Pre-entrenamiento 
+de transformadores bidireccionales profundos para la comprensión del lenguaje.
+```
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
```

### Comparing `griptape-0.7.1/griptape/artifacts/error_artifact.py` & `griptape-0.7.2/griptape/artifacts/error_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/artifacts/text_artifact.py` & `griptape-0.7.2/griptape/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/converters/chatgpt_plugin_converter.py` & `griptape-0.7.2/griptape/converters/chatgpt_plugin_converter.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/converters/langchain_tool_converter.py` & `griptape-0.7.2/griptape/converters/langchain_tool_converter.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/core/activity_mixin.py` & `griptape-0.7.2/griptape/core/activity_mixin.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/core/base_tool.py` & `griptape-0.7.2/griptape/core/base_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     def __attrs_post_init__(self):
         from griptape.ramps import BaseRamp
 
         # https://www.attrs.org/en/stable/api.html#attrs.resolve_types
         attrs.resolve_types(self.__class__, globals(), locals())
 
     @ramps.validator
-    def validate_ramps(self, _, ramps: dict[str, BaseRamp]) -> None:
-        ramp_names = ramps.keys()
+    def validate_ramps(self, _, ramps: dict[str, list[BaseRamp]]) -> None:
+        ramp_names = [item.name for sublist in ramps.values() for item in sublist]
 
         if len(ramp_names) > len(set(ramp_names)):
             raise ValueError("ramp names have to be unique")
 
     @property
     def class_name(self):
         return self.__class__.__name__
```

### Comparing `griptape-0.7.1/griptape/core/decorators.py` & `griptape-0.7.2/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/core/tool_loader.py` & `griptape-0.7.2/griptape/core/tool_loader.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/__init__.py` & `griptape-0.7.2/griptape/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.7.2/griptape/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.7.2/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.7.2/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.7.2/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.7.2/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.7.2/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/storage/dynamodb_storage_driver.py` & `griptape-0.7.2/griptape/drivers/storage/dynamodb_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/drivers/storage/memory_storage_driver.py` & `griptape-0.7.2/griptape/drivers/storage/memory_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/executors/base_executor.py` & `griptape-0.7.2/griptape/executors/base_executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import json
+import logging
 from typing import TYPE_CHECKING, Union
 import inspect
 import os
 from abc import ABC, abstractmethod
 from griptape.artifacts import BaseArtifact, TextArtifact
 
 if TYPE_CHECKING:
@@ -33,25 +34,18 @@
         return value
 
     def executor_result_to_artifact(self, result: Union[BaseArtifact, str]) -> BaseArtifact:
         if isinstance(result, BaseArtifact):
             return result
         else:
             try:
-                from griptape.schemas import TextArtifactSchema, ErrorArtifactSchema
+                return BaseArtifact.from_dict(json.loads(result))
+            except Exception:
+                logging.exception("Error converting executor result to an artifact; defaulting to TextArtifact")
 
-                result_dict = json.loads(result)
-
-                if result_dict["type"] == "TextArtifact":
-                    return TextArtifactSchema().load(result_dict)
-                elif result_dict["type"] == "ErrorArtifact":
-                    return ErrorArtifactSchema().load(result_dict)
-                else:
-                    return TextArtifact(result)
-            except Exception as e:
                 return TextArtifact(result)
 
     @abstractmethod
     def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
         ...
 
     def tool_dir(self, tool: BaseTool):
```

### Comparing `griptape-0.7.1/griptape/executors/docker_executor.py` & `griptape-0.7.2/griptape/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/executors/local_executor.py` & `griptape-0.7.2/griptape/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/memory/buffer_memory.py` & `griptape-0.7.2/griptape/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/memory/memory.py` & `griptape-0.7.2/griptape/memory/memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/memory/summary_memory.py` & `griptape-0.7.2/griptape/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/ramps/base_ramp.py` & `griptape-0.7.2/griptape/ramps/base_ramp.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/ramps/storage_ramp.py` & `griptape-0.7.2/griptape/ramps/storage_ramp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
+from llama_index import Document, GPTListIndex
 from schema import Schema, Literal
 from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
 from griptape.core.decorators import activity
 from griptape.ramps import BaseRamp
 from attr import define, field
 from griptape.summarizers import PromptDriverSummarizer
 from griptape.drivers import OpenAiPromptDriver
-from griptape.utils.text import to_vector_index
 
 if TYPE_CHECKING:
     from griptape.drivers import BaseStorageDriver, BasePromptDriver
 
 
 @define
 class StorageRamp(BaseRamp):
@@ -48,16 +48,19 @@
             ): str
         })
     })
     def search_entry(self, value: dict) -> BaseArtifact:
         text = self.driver.load(value["id"])
 
         if text:
+            index = GPTListIndex.from_documents([Document(text)])
+            query_engine = index.as_query_engine()
+
             return TextArtifact(
-                str(to_vector_index(text).query(f"Search query: {value['query']}")).strip()
+                str(query_engine.query(f"Search text with query: {value['query']}")).strip()
             )
         else:
             return ErrorArtifact("Entry not found")
 
     @activity(config={
         "name": "summarize",
         "description": "Can be used to generate a summary of a storage entry",
```

### Comparing `griptape-0.7.1/griptape/schemas/__init__.py` & `griptape-0.7.2/griptape/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/schemas/drivers/openai_prompt_driver_schema.py` & `griptape-0.7.2/griptape/schemas/drivers/openai_prompt_driver_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/schemas/polymorphic_schema.py` & `griptape-0.7.2/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/schemas/tasks/toolkit_task_schema.py` & `griptape-0.7.2/griptape/schemas/tasks/toolkit_task_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/structures/agent.py` & `griptape-0.7.2/griptape/structures/agent.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/structures/pipeline.py` & `griptape-0.7.2/griptape/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/structures/structure.py` & `griptape-0.7.2/griptape/structures/structure.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/structures/structure_with_memory.py` & `griptape-0.7.2/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/structures/workflow.py` & `griptape-0.7.2/griptape/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/summarizers/base_summarizer.py` & `griptape-0.7.2/griptape/summarizers/base_summarizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/summarizers/prompt_driver_summarizer.py` & `griptape-0.7.2/griptape/summarizers/prompt_driver_summarizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import logging
 from attr import define, field
-from griptape.utils.text import to_vector_index
+from llama_index import Document, GPTListIndex
 from griptape.utils import J2
 from griptape.drivers import BasePromptDriver
 from griptape.summarizers.base_summarizer import BaseSummarizer
 
 if TYPE_CHECKING:
     from griptape.memory import Run
 
@@ -28,12 +28,17 @@
                 return previous_summary
         except Exception as e:
             logging.error(f"Error summarizing memory: {type(e).__name__}({e})")
 
             return previous_summary
 
     def summarize_text(self, text: str) -> str:
+        index = GPTListIndex.from_documents([Document(text)])
+        query_engine = index.as_query_engine(
+            response_mode="tree_summarize"
+        )
+
         return str(
-            to_vector_index(text).query(
+            query_engine.query(
                 "Generate a summary. Include URLs in the summary."
             )
         ).strip()
```

### Comparing `griptape-0.7.1/griptape/tasks/action_subtask.py` & `griptape-0.7.2/griptape/tasks/action_subtask.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tasks/base_task.py` & `griptape-0.7.2/griptape/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tasks/prompt_task.py` & `griptape-0.7.2/griptape/tasks/prompt_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tasks/toolkit_task.py` & `griptape-0.7.2/griptape/tasks/toolkit_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/templates/prompts/base.j2` & `griptape-0.7.2/griptape/templates/prompts/base.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-You are a truthful assistant that follows rules and doesn't make up things. You can perform actions to answer questions and complete tasks step-by-step. To perform an action use this conversation format:
+You are an assistant that follows rules, acts truthfully, and doesn't make things up. You can perform actions to answer questions and complete tasks step-by-step. If an action fails you can be creative and try to fix it or try other options. To perform an action use this conversation format:
 
 Input: <original request>
 Thought: <your step-by-step thought process about how you can complete the request>
-Action: JSON object with the following JSON Schema: {{ action_schema }}
+Action: minified JSON object with the following JSON Schema: {{ action_schema }}
 Observation: <action result>
 ...repeat Thought/Action/Observation until you can respond to the original request
 Thought: I have enough information to respond to the original request
 Output: <your final response>
 
-"Input:", "Thought:", "Action:", "Observation:", and "Output:" have to ALWAYS start on a new line.
+"Input:", "Thought:", "Action:", "Observation:", and "Output:" must ALWAYS start on a new line.
+
+Action must ALWAYS be a minified JSON object on a single line.
 
 If you don't need to perform an action or if you don't know which action to perform, ignore Thought/Action/Observation and go straight to Output.
 
 Actions of type "tool"
 {% if tool_names|length > 0 %}
 You can use tool activities to complete tasks. You have access to the following tools: [{{ tool_names }}]. NEVER make up tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user.
```

### Comparing `griptape-0.7.1/griptape/tokenizers/base_tokenizer.py` & `griptape-0.7.2/griptape/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.7.2/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.7.2/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.7.2/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/utils/command_runner.py` & `griptape-0.7.2/griptape/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/utils/j2.py` & `griptape-0.7.2/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/griptape/utils/python_runner.py` & `griptape-0.7.2/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.1/pyproject.toml` & `griptape-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.7.1"
+version = "0.7.2"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
@@ -31,15 +31,15 @@
 stringcase = ">=1"
 schema = ">=0.7"
 pyyaml = ">=6"
 langchain = ">=0.0.120"
 fastapi = ">=0.80"
 uvicorn = ">= 0.20"
 python-decouple=">=3"
-llama_index = "==0.4.23"
+llama_index = "~0.6.0"
 boto3 = "^1.26.123"
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-mock = "*"
 pytest-cover = "*"
 twine = ">=4"
```

### Comparing `griptape-0.7.1/PKG-INFO` & `griptape-0.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.7.1
+Version: 0.7.2
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Requires-Dist: docker (>=6)
 Requires-Dist: fastapi (>=0.80)
 Requires-Dist: graphlib
 Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: langchain (>=0.0.120)
-Requires-Dist: llama_index (==0.4.23)
+Requires-Dist: llama_index (>=0.6.0,<0.7.0)
 Requires-Dist: marshmallow (>=3)
 Requires-Dist: marshmallow-enum (>=1.5)
 Requires-Dist: openai (>=0.27)
 Requires-Dist: python-decouple (>=3)
 Requires-Dist: python-dotenv (>=0.21)
 Requires-Dist: pyyaml (>=6)
 Requires-Dist: rich (>=13)
@@ -72,52 +72,69 @@
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
 With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
 
 ```python
 from decouple import config
-from griptape.tools import WebScraper, Calculator
-from griptape import utils
+from griptape.core import ToolLoader
+from griptape.drivers import OpenAiPromptDriver, MemoryStorageDriver
+from griptape.executors import LocalExecutor
 from griptape.memory import Memory
-from griptape.tasks import PromptTask, ToolkitTask
+from griptape.ramps import StorageRamp
 from griptape.structures import Pipeline
-from griptape.core import ToolLoader
+from griptape.tasks import ToolkitTask, PromptTask
+from griptape.tools import WebScraper
+
+storage = StorageRamp(
+    driver=MemoryStorageDriver()
+)
 
 scraper = WebScraper(
-    openai_api_key=config("OPENAI_API_KEY")
+    ramps={
+        "get_content": [storage]
+    }
 )
-calculator = Calculator()
 
 pipeline = Pipeline(
     memory=Memory(),
     tool_loader=ToolLoader(
-        tools=[calculator, scraper]
+        tools=[scraper],
+        executor=LocalExecutor()
     )
 )
 
 pipeline.add_tasks(
     ToolkitTask(
-        tool_names=[calculator.name, scraper.name]
+        tool_names=[scraper.name]
     ),
     PromptTask(
-        "Say the following like a pirate: {{ input }}"
+        "Say the following in spanish: {{ input }}"
     )
 )
 
-pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
+result = pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
+
+print(result.output.value)
 
-print(utils.Conversation(pipeline.memory).to_string())
 
 ```
 
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
-> Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model  
-> A: Arr, me hearties! Large language models have been developed and set sail since 2018, includin' BERT, GPT-2, GPT-3 [...]
+```
+Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model
+[chain of thought output... will vary depending on the model driver you're using]
+A: Los modelos de lenguaje de gran tamaño son herramientas utilizadas para tareas de 
+procesamiento del lenguaje natural, como detectar falsedades, completar oraciones y comprender 
+el lenguaje. Algunos modelos notables incluyen BERT, GPT-2, GPT-3, GPT-Neo y GLaM. The Pile es 
+un conjunto de datos extenso utilizado para el modelado del lenguaje. Estos modelos han sido 
+desarrollados e investigados en trabajos como TruthfulQA, HellaSwag y BERT: Pre-entrenamiento 
+de transformadores bidireccionales profundos para la comprensión del lenguaje.
+```
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
```

