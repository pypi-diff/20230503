# Comparing `tmp/GptCode-1.0.6.tar.gz` & `tmp/GptCode-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GptCode-1.0.6.tar", last modified: Tue May  2 07:59:54 2023, max compression
+gzip compressed data, was "GptCode-1.0.7.tar", last modified: Tue May  2 12:41:11 2023, max compression
```

## Comparing `GptCode-1.0.6.tar` & `GptCode-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.186029 GptCode-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.158025 GptCode-1.0.6/GptCode/
--rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.6/GptCode/__init__.py
--rw-rw-rw-   0        0        0     4771 2023-05-02 07:58:08.000000 GptCode-1.0.6/GptCode/gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.178028 GptCode-1.0.6/GptCode.egg-info/
--rw-rw-rw-   0        0        0      167 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2023-05-02 07:59:54.184028 GptCode-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-02 07:59:54.187029 GptCode-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      371 2023-05-02 07:59:50.000000 GptCode-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:41:11.964079 GptCode-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-02 12:41:11.949077 GptCode-1.0.7/GptCode/
+-rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.7/GptCode/__init__.py
+-rw-rw-rw-   0        0        0     4896 2023-05-02 12:40:28.000000 GptCode-1.0.7/GptCode/gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:41:11.959080 GptCode-1.0.7/GptCode.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-05-02 12:41:11.000000 GptCode-1.0.7/GptCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-02 12:41:11.000000 GptCode-1.0.7/GptCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:41:11.000000 GptCode-1.0.7/GptCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 12:41:11.000000 GptCode-1.0.7/GptCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2023-05-02 12:41:11.963078 GptCode-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:41:11.965080 GptCode-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-05-02 12:41:08.000000 GptCode-1.0.7/setup.py
```

### Comparing `GptCode-1.0.6/GptCode/gpt.py` & `GptCode-1.0.7/GptCode/gpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,18 @@
         :return: 翻译结果
         """
         trans = f"请把以下语言翻译为{aim_language}。"
         response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': trans+prompt}])
         return response
 
     def extract_picture_prompt(self,prompt):
-        extract = "以下句子描述了一张图片，请从中提取出对图片的描述，或者想象一下图片的描述，描述请尽量详细。"
+        extract = "如果无法完成描述，请只回复0，不回复其他信息。以下句子描述了一张图片，请从中提取出对图片的描述，或者想象一下图片的描述，描述请尽量详细."
         response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': extract + prompt}])
+        if response[0] == '0':
+            return prompt
         return response
 
     def get_answer(self, messages):
         response = openai.ChatCompletion.create(model=self.model, messages=messages)
         answer = response.choices[0].message['content']
         return answer
 
@@ -93,15 +95,15 @@
         :param prompt:问题描述
         :param reference: 是否列出参考的资料来源
         :param use_history: 是否参考历史对话信息
         :param history_number: 参考历史对话信息的条数
         :return: 此次问题的回复
         """
         if reference:
-            prompt = self.generate_prompt(prompt)
+            prompt = self.generate_pxrompt(prompt)
         self.conversation_list.append({"role": "user", "content": prompt})
         if use_history:
             # 基于历史history_number条提问记录和当前问题进行回答,虽然会结合上下文，但是会比较耗token
             response = self.get_answer(messages=self.system_setting_list + self.conversation_list[-history_number:])
         else:
             # 只基于当前问题进行回答
             response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': prompt}])
```

