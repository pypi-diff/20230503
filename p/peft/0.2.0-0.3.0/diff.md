# Comparing `tmp/peft-0.2.0.tar.gz` & `tmp/peft-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peft-0.2.0.tar", last modified: Thu Mar  9 03:40:24 2023, max compression
+gzip compressed data, was "peft-0.3.0.tar", last modified: Wed May  3 19:45:13 2023, max compression
```

## Comparing `peft-0.2.0.tar` & `peft-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.019381 peft-0.2.0/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    11357 2022-11-25 03:51:31.000000 peft-0.2.0/LICENSE
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19038 2023-03-09 03:40:24.019160 peft-0.2.0/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    18136 2023-03-09 03:29:10.000000 peft-0.2.0/README.md
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      665 2023-03-07 08:32:29.000000 peft-0.2.0/pyproject.toml
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)       38 2023-03-09 03:40:24.019428 peft-0.2.0/setup.cfg
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3045 2023-03-09 03:39:56.000000 peft-0.2.0/setup.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.013880 peft-0.2.0/src/
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.015203 peft-0.2.0/src/peft/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1669 2023-03-09 03:39:56.000000 peft-0.2.0/src/peft/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5540 2023-02-08 03:17:30.000000 peft-0.2.0/src/peft/mapping.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    42460 2023-03-09 03:10:09.000000 peft-0.2.0/src/peft/peft_model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.017730 peft-0.2.0/src/peft/tuners/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1060 2023-01-18 13:18:53.000000 peft-0.2.0/src/peft/tuners/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    25768 2023-03-07 19:21:00.000000 peft-0.2.0/src/peft/tuners/lora.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6690 2023-03-07 08:32:05.000000 peft-0.2.0/src/peft/tuners/p_tuning.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3714 2023-02-08 03:17:39.000000 peft-0.2.0/src/peft/tuners/prefix_tuning.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4863 2023-02-15 06:00:38.000000 peft-0.2.0/src/peft/tuners/prompt_tuning.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.018858 peft-0.2.0/src/peft/utils/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1216 2023-02-17 10:05:15.000000 peft-0.2.0/src/peft/utils/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      730 2023-02-02 07:51:43.000000 peft-0.2.0/src/peft/utils/adapters_utils.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6535 2023-03-07 12:27:48.000000 peft-0.2.0/src/peft/utils/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5927 2023-02-24 12:53:39.000000 peft-0.2.0/src/peft/utils/other.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3229 2023-02-08 06:57:59.000000 peft-0.2.0/src/peft/utils/save_and_load.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-03-09 03:40:24.016195 peft-0.2.0/src/peft.egg-info/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19038 2023-03-09 03:40:23.000000 peft-0.2.0/src/peft.egg-info/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      551 2023-03-09 03:40:23.000000 peft-0.2.0/src/peft.egg-info/SOURCES.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        1 2023-03-09 03:40:23.000000 peft-0.2.0/src/peft.egg-info/dependency_links.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      197 2023-03-09 03:40:23.000000 peft-0.2.0/src/peft.egg-info/requires.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        5 2023-03-09 03:40:23.000000 peft-0.2.0/src/peft.egg-info/top_level.txt
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.266616 peft-0.3.0/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    11357 2022-11-25 03:51:31.000000 peft-0.3.0/LICENSE
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20550 2023-05-03 19:45:13.266499 peft-0.3.0/PKG-INFO
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19627 2023-05-03 19:37:00.000000 peft-0.3.0/README.md
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      665 2023-03-07 08:32:29.000000 peft-0.3.0/pyproject.toml
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)       38 2023-05-03 19:45:13.266649 peft-0.3.0/setup.cfg
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3134 2023-05-03 19:42:54.000000 peft-0.3.0/setup.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.262706 peft-0.3.0/src/
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.264205 peft-0.3.0/src/peft/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1757 2023-05-03 19:42:47.000000 peft-0.3.0/src/peft/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      720 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/import_utils.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4427 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/mapping.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    52633 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/peft_model.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.265878 peft-0.3.0/src/peft/tuners/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1180 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    29964 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/adalora.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15972 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/adaption_prompt.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    31010 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/lora.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6755 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/p_tuning.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3785 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/prefix_tuning.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4935 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/prompt_tuning.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.266325 peft-0.3.0/src/peft/utils/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1398 2023-04-17 11:33:24.000000 peft-0.3.0/src/peft/utils/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6823 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/config.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8356 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/other.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5829 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/save_and_load.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.264772 peft-0.3.0/src/peft.egg-info/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20550 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/PKG-INFO
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      605 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/SOURCES.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        1 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/dependency_links.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      289 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/requires.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        5 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/top_level.txt
```

### Comparing `peft-0.2.0/LICENSE` & `peft-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peft-0.2.0/PKG-INFO` & `peft-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peft
-Version: 0.2.0
+Version: 0.3.0
 Summary: Parameter-Efficient Fine-Tuning (PEFT)
 Home-page: https://github.com/huggingface/peft
 Author: The HuggingFace team
 Author-email: sourab@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: docs_specific
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
@@ -47,18 +48,19 @@
 
 Parameter-Efficient Fine-Tuning (PEFT) methods enable efficient adaptation of pre-trained language models (PLMs) to various downstream applications without fine-tuning all the model's parameters. Fine-tuning large-scale PLMs is often prohibitively costly. In this regard, PEFT methods only fine-tune a small number of (extra) model parameters, thereby greatly decreasing the computational and storage costs. Recent State-of-the-Art PEFT techniques achieve performance comparable to that of full fine-tuning. 
 
 Seamlessly integrated with 🤗 Accelerate for large scale models leveraging DeepSpeed and Big Model Inference. 
 
 Supported methods:
 
-1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2106.09685.pdf)
+1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
-3. P-Tuning: [GPT Understands, Too](https://arxiv.org/pdf/2103.10385.pdf)
-4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/pdf/2104.08691.pdf) 
+3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
+4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
+5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -86,38 +88,40 @@
 |   Model         | Full Finetuning | PEFT-LoRA PyTorch  | PEFT-LoRA DeepSpeed with CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | bigscience/T0_3B (3B params) | 47.14GB GPU / 2.96GB CPU  | 14.4GB GPU / 2.96GB CPU | 9.8GB GPU / 17.8GB CPU |
 | bigscience/mt0-xxl (12B params) | OOM GPU | 56GB GPU / 3GB CPU | 22GB GPU / 52GB CPU |
 | bigscience/bloomz-7b1 (7B params) | OOM GPU | 32GB GPU / 3.8GB CPU | 18.1GB GPU / 35GB CPU |
 
 Performance of PEFT-LoRA tuned [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) on [`ought/raft/twitter_complaints`](https://huggingface.co/datasets/ought/raft/viewer/twitter_complaints) leaderboard. 
-A point to note is that we didn't try to sequeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
+A point to note is that we didn't try to squeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
 So, we are already seeing comparable performance to SoTA with parameter efficient tuning. Also, the final checkpoint size is just `19MB` in comparison to `11GB` size of the backbone [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) model.
 
 |   Submission Name        | Accuracy |
 | --------- | ---- |
 | Human baseline (crowdsourced) |	0.897 |
 | Flan-T5 | 0.892 |
 | lora-t0-3b | 0.863 |
 
 **Therefore, we can see that performance comparable to SoTA is achievable by PEFT methods with consumer hardware such as 16GB and 24GB GPUs.**
 
+An insightful blogpost explaining the advantages of using PEFT for fine-tuning FlanT5-XXL: [https://www.philschmid.de/fine-tune-flan-t5-peft](https://www.philschmid.de/fine-tune-flan-t5-peft)
+
 ### Parameter Efficient Tuning of Diffusion Models
 
 GPU memory required by different settings during training is given below. The final checkpoint size is `8.8 MB`.
 
 Hardware: Single A100 80GB GPU with CPU RAM above 64GB
 
-|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpoitning  |
+|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpointing  |
 | --------- | ---- | ---- | ---- |
 | CompVis/stable-diffusion-v1-4 | 27.5GB GPU / 3.97GB CPU | 15.5GB GPU / 3.84GB CPU | 8.12GB GPU / 3.77GB CPU | 
 
 
 **Training**
-An example of using LoRA for parameter efficient dreambooth training is given in `~examples/lora_dreambooth/train_dreambooth.py`
+An example of using LoRA for parameter efficient dreambooth training is given in [`examples/lora_dreambooth/train_dreambooth.py`](examples/lora_dreambooth/train_dreambooth.py)
 
 ```bash
 export MODEL_NAME= "CompVis/stable-diffusion-v1-4" #"stabilityai/stable-diffusion-2-1"
 export INSTANCE_DIR="path-to-instance-images"
 export CLASS_DIR="path-to-class-images"
 export OUTPUT_DIR="path-to-save-model"
 
@@ -147,38 +151,41 @@
 ```
 
 Try out the 🤗 Gradio Space which should run seamlessly on a T4 instance:
 [smangrul/peft-lora-sd-dreambooth](https://huggingface.co/spaces/smangrul/peft-lora-sd-dreambooth).
 
 ![peft lora dreambooth gradio space](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/peft_lora_dreambooth_gradio_space.png)
 
+**NEW** ✨ Multi Adapter support and combining multiple LoRA adapters in a weighted combination 
+![peft lora dreambooth weighted adapter](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/weighted_adapter_dreambooth_lora.png)
+
 ### Parameter Efficient Tuning of LLMs for RLHF components such as Ranker and Policy
-- Here is an exmaple in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) 
-- Example using PEFT for both reward model and policy [ToDo]
+- Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
+- Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
-- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
+- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
 An example of using LoRA for the task of adapting `LayoutLMForTokenClassification` on `FUNSD` dataset is given in `~examples/token_classification/PEFT_LoRA_LayoutLMForTokenClassification_on_FUNSD.py`. We can observe that with only `0.62 %` of parameters being trainable, we achieve performance (F1 0.777) comparable to full finetuning (F1 0.786) (without any hyerparam tuning runs for extracting more performance), and the checkpoint of this is only `2.8MB`. Now, if there are `N` such datasets, just have these PEFT models one for each dataset and save a lot of storage without having to worry about the problem of catastrophic forgetting or overfitting of backbone/base model.
 
-Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset suing differenct PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
+Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset using different PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
 
 
 ## PEFT + 🤗 Accelerate
 
-PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices etc during training.
+PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices, etc during training.
 Use 🤗 Accelerate for inferencing on consumer hardware with small resources.
 
 ### Example of PEFT model training using 🤗 Accelerate's DeepSpeed integration
 
 DeepSpeed version required `v0.8.0`. An example is provided in `~examples/conditional_generation/peft_lora_seq2seq_accelerate_ds_zero3_offload.py`. 
   a. First, run `accelerate config --config_file ds_zero3_cpu.yaml` and answer the questionnaire. 
   Below are the contents of the config file.
@@ -239,22 +246,24 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-| --------- | ---- | ---- | ---- | ----  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  |
-| Bloom          | ✅  | ✅  | ✅  | ✅  |
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B   | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
+|--------------| ---- | ---- | ---- | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ---- |
 | T5        | ✅   | ✅   | ✅   | ✅   |
 | BART      | ✅   | ✅   | ✅   | ✅   |
 
@@ -294,14 +303,20 @@
 ### Image Classification
 
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ----  |
 | ViT           | ✅  |   |   |   | 
 | Swin           | ✅  |   |   |   | 
 
+### Image to text (Multi-modal models)
+
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
+| --------- | ---- | ---- | ---- | ----  |
+| Blip-2           | ✅  |   |   |   | 
+
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
@@ -366,18 +381,21 @@
 
 2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
 
 3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
 `P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
 new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
 
+4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+
 ## Backlog:
-1. Explore and possibly integrate `(IA)^3`
-2. Add tests
-3. Add more use cases and examples
+- [x] Add tests
+- [x] Multi Adapter training and inference support
+- [x] Add more use cases and examples
+- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
```

### Comparing `peft-0.2.0/README.md` & `peft-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
 Parameter-Efficient Fine-Tuning (PEFT) methods enable efficient adaptation of pre-trained language models (PLMs) to various downstream applications without fine-tuning all the model's parameters. Fine-tuning large-scale PLMs is often prohibitively costly. In this regard, PEFT methods only fine-tune a small number of (extra) model parameters, thereby greatly decreasing the computational and storage costs. Recent State-of-the-Art PEFT techniques achieve performance comparable to that of full fine-tuning. 
 
 Seamlessly integrated with 🤗 Accelerate for large scale models leveraging DeepSpeed and Big Model Inference. 
 
 Supported methods:
 
-1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2106.09685.pdf)
+1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
-3. P-Tuning: [GPT Understands, Too](https://arxiv.org/pdf/2103.10385.pdf)
-4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/pdf/2104.08691.pdf) 
+3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
+4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
+5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -60,38 +61,40 @@
 |   Model         | Full Finetuning | PEFT-LoRA PyTorch  | PEFT-LoRA DeepSpeed with CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | bigscience/T0_3B (3B params) | 47.14GB GPU / 2.96GB CPU  | 14.4GB GPU / 2.96GB CPU | 9.8GB GPU / 17.8GB CPU |
 | bigscience/mt0-xxl (12B params) | OOM GPU | 56GB GPU / 3GB CPU | 22GB GPU / 52GB CPU |
 | bigscience/bloomz-7b1 (7B params) | OOM GPU | 32GB GPU / 3.8GB CPU | 18.1GB GPU / 35GB CPU |
 
 Performance of PEFT-LoRA tuned [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) on [`ought/raft/twitter_complaints`](https://huggingface.co/datasets/ought/raft/viewer/twitter_complaints) leaderboard. 
-A point to note is that we didn't try to sequeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
+A point to note is that we didn't try to squeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
 So, we are already seeing comparable performance to SoTA with parameter efficient tuning. Also, the final checkpoint size is just `19MB` in comparison to `11GB` size of the backbone [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) model.
 
 |   Submission Name        | Accuracy |
 | --------- | ---- |
 | Human baseline (crowdsourced) |	0.897 |
 | Flan-T5 | 0.892 |
 | lora-t0-3b | 0.863 |
 
 **Therefore, we can see that performance comparable to SoTA is achievable by PEFT methods with consumer hardware such as 16GB and 24GB GPUs.**
 
+An insightful blogpost explaining the advantages of using PEFT for fine-tuning FlanT5-XXL: [https://www.philschmid.de/fine-tune-flan-t5-peft](https://www.philschmid.de/fine-tune-flan-t5-peft)
+
 ### Parameter Efficient Tuning of Diffusion Models
 
 GPU memory required by different settings during training is given below. The final checkpoint size is `8.8 MB`.
 
 Hardware: Single A100 80GB GPU with CPU RAM above 64GB
 
-|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpoitning  |
+|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpointing  |
 | --------- | ---- | ---- | ---- |
 | CompVis/stable-diffusion-v1-4 | 27.5GB GPU / 3.97GB CPU | 15.5GB GPU / 3.84GB CPU | 8.12GB GPU / 3.77GB CPU | 
 
 
 **Training**
-An example of using LoRA for parameter efficient dreambooth training is given in `~examples/lora_dreambooth/train_dreambooth.py`
+An example of using LoRA for parameter efficient dreambooth training is given in [`examples/lora_dreambooth/train_dreambooth.py`](examples/lora_dreambooth/train_dreambooth.py)
 
 ```bash
 export MODEL_NAME= "CompVis/stable-diffusion-v1-4" #"stabilityai/stable-diffusion-2-1"
 export INSTANCE_DIR="path-to-instance-images"
 export CLASS_DIR="path-to-class-images"
 export OUTPUT_DIR="path-to-save-model"
 
@@ -121,38 +124,41 @@
 ```
 
 Try out the 🤗 Gradio Space which should run seamlessly on a T4 instance:
 [smangrul/peft-lora-sd-dreambooth](https://huggingface.co/spaces/smangrul/peft-lora-sd-dreambooth).
 
 ![peft lora dreambooth gradio space](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/peft_lora_dreambooth_gradio_space.png)
 
+**NEW** ✨ Multi Adapter support and combining multiple LoRA adapters in a weighted combination 
+![peft lora dreambooth weighted adapter](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/weighted_adapter_dreambooth_lora.png)
+
 ### Parameter Efficient Tuning of LLMs for RLHF components such as Ranker and Policy
-- Here is an exmaple in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) 
-- Example using PEFT for both reward model and policy [ToDo]
+- Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
+- Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
-- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
+- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
 An example of using LoRA for the task of adapting `LayoutLMForTokenClassification` on `FUNSD` dataset is given in `~examples/token_classification/PEFT_LoRA_LayoutLMForTokenClassification_on_FUNSD.py`. We can observe that with only `0.62 %` of parameters being trainable, we achieve performance (F1 0.777) comparable to full finetuning (F1 0.786) (without any hyerparam tuning runs for extracting more performance), and the checkpoint of this is only `2.8MB`. Now, if there are `N` such datasets, just have these PEFT models one for each dataset and save a lot of storage without having to worry about the problem of catastrophic forgetting or overfitting of backbone/base model.
 
-Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset suing differenct PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
+Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset using different PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
 
 
 ## PEFT + 🤗 Accelerate
 
-PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices etc during training.
+PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices, etc during training.
 Use 🤗 Accelerate for inferencing on consumer hardware with small resources.
 
 ### Example of PEFT model training using 🤗 Accelerate's DeepSpeed integration
 
 DeepSpeed version required `v0.8.0`. An example is provided in `~examples/conditional_generation/peft_lora_seq2seq_accelerate_ds_zero3_offload.py`. 
   a. First, run `accelerate config --config_file ds_zero3_cpu.yaml` and answer the questionnaire. 
   Below are the contents of the config file.
@@ -213,22 +219,24 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-| --------- | ---- | ---- | ---- | ----  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  |
-| Bloom          | ✅  | ✅  | ✅  | ✅  |
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B   | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
+|--------------| ---- | ---- | ---- | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ---- |
 | T5        | ✅   | ✅   | ✅   | ✅   |
 | BART      | ✅   | ✅   | ✅   | ✅   |
 
@@ -268,14 +276,20 @@
 ### Image Classification
 
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ----  |
 | ViT           | ✅  |   |   |   | 
 | Swin           | ✅  |   |   |   | 
 
+### Image to text (Multi-modal models)
+
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
+| --------- | ---- | ---- | ---- | ----  |
+| Blip-2           | ✅  |   |   |   | 
+
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
@@ -340,18 +354,21 @@
 
 2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
 
 3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
 `P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
 new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
 
+4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+
 ## Backlog:
-1. Explore and possibly integrate `(IA)^3`
-2. Add tests
-3. Add more use cases and examples
+- [x] Add tests
+- [x] Multi Adapter training and inference support
+- [x] Add more use cases and examples
+- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
```

### Comparing `peft-0.2.0/pyproject.toml` & `peft-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peft-0.2.0/setup.py` & `peft-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 
 from setuptools import find_packages, setup
 
 extras = {}
 extras["quality"] = ["black ~= 22.0", "ruff>=0.0.241"]
 extras["docs_specific"] = ["hf-doc-builder"]
 extras["dev"] = extras["quality"] + extras["docs_specific"]
+extras["test"] = extras["dev"] + ["pytest", "pytest-xdist", "parameterized", "datasets"]
 
 setup(
     name="peft",
-    version="0.2.0",
+    version="0.3.0",
     description="Parameter-Efficient Fine-Tuning (PEFT)",
     license_files=["LICENSE"],
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
```

### Comparing `peft-0.2.0/src/peft/__init__.py` & `peft-0.3.0/src/peft/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from .mapping import MODEL_TYPE_TO_PEFT_MODEL_MAPPING, PEFT_TYPE_TO_CONFIG_MAPPING, get_peft_config, get_peft_model
 from .peft_model import (
     PeftModel,
     PeftModelForCausalLM,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
 )
 from .tuners import (
+    AdaptionPromptConfig,
+    AdaptionPromptModel,
     LoraConfig,
     LoraModel,
+    AdaLoraConfig,
+    AdaLoraModel,
     PrefixEncoder,
     PrefixTuningConfig,
     PromptEmbedding,
     PromptEncoder,
     PromptEncoderConfig,
     PromptEncoderReparameterizationType,
     PromptTuningConfig,
```

### Comparing `peft-0.2.0/src/peft/mapping.py` & `peft-0.3.0/src/peft/mapping.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,49 +16,39 @@
 from .peft_model import (
     PeftModel,
     PeftModelForCausalLM,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
 )
-from .tuners import LoraConfig, PrefixTuningConfig, PromptEncoderConfig, PromptTuningConfig
+from .tuners import (
+    AdaLoraConfig,
+    AdaptionPromptConfig,
+    LoraConfig,
+    PrefixTuningConfig,
+    PromptEncoderConfig,
+    PromptTuningConfig,
+)
 from .utils import PromptLearningConfig
 
 
 MODEL_TYPE_TO_PEFT_MODEL_MAPPING = {
     "SEQ_CLS": PeftModelForSequenceClassification,
     "SEQ_2_SEQ_LM": PeftModelForSeq2SeqLM,
     "CAUSAL_LM": PeftModelForCausalLM,
     "TOKEN_CLS": PeftModelForTokenClassification,
 }
 
 PEFT_TYPE_TO_CONFIG_MAPPING = {
+    "ADAPTION_PROMPT": AdaptionPromptConfig,
     "PROMPT_TUNING": PromptTuningConfig,
     "PREFIX_TUNING": PrefixTuningConfig,
     "P_TUNING": PromptEncoderConfig,
     "LORA": LoraConfig,
-}
-
-TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING = {
-    "t5": ["q", "v"],
-    "mt5": ["q", "v"],
-    "bart": ["q_proj", "v_proj"],
-    "gpt2": ["c_attn"],
-    "bloom": ["query_key_value"],
-    "opt": ["q_proj", "v_proj"],
-    "gptj": ["q_proj", "v_proj"],
-    "gpt_neox": ["query_key_value"],
-    "gpt_neo": ["q_proj", "v_proj"],
-    "bert": ["query", "value"],
-    "roberta": ["query", "value"],
-    "xlm-roberta": ["query", "value"],
-    "electra": ["query", "value"],
-    "deberta-v2": ["query_proj", "value_proj"],
-    "deberta": ["in_proj"],
-    "layoutlm": ["query", "value"],
+    "ADALORA": AdaLoraConfig,
 }
 
 
 def get_peft_config(config_dict):
     """
     Returns a Peft config object from a dictionary.
 
@@ -107,39 +97,24 @@
 
     if getattr(peft_config, "encoder_hidden_size", None) is None:
         setattr(peft_config, "encoder_hidden_size", token_dim)
 
     return peft_config
 
 
-def _prepare_lora_config(peft_config, model_config):
-    if peft_config.target_modules is None:
-        if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING:
-            raise ValueError("Please specify `target_modules` in `peft_config`")
-        peft_config.target_modules = TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING[model_config["model_type"]]
-    if len(peft_config.target_modules) == 1:
-        peft_config.fan_in_fan_out = True
-        peft_config.enable_lora = [True, False, True]
-    if peft_config.inference_mode:
-        peft_config.merge_weights = True
-    return peft_config
-
-
 def get_peft_model(model, peft_config):
     """
     Returns a Peft model object from a model and a config.
 
     Args:
         model ([`transformers.PreTrainedModel`]): Model to be wrapped.
         peft_config ([`PeftConfig`]): Configuration object containing the parameters of the Peft model.
     """
-
-    model_config = model.config.to_dict()
+    model_config = model.config.to_dict() if hasattr(model.config, "to_dict") else model.config
     peft_config.base_model_name_or_path = model.__dict__.get("name_or_path", None)
-    if peft_config.task_type not in MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys():
-        peft_config = _prepare_lora_config(peft_config, model_config)
+    if peft_config.task_type not in MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys() and not isinstance(
+        peft_config, PromptLearningConfig
+    ):
         return PeftModel(model, peft_config)
-    if not isinstance(peft_config, PromptLearningConfig):
-        peft_config = _prepare_lora_config(peft_config, model_config)
-    else:
+    if isinstance(peft_config, PromptLearningConfig):
         peft_config = _prepare_prompt_learning_config(peft_config, model_config)
     return MODEL_TYPE_TO_PEFT_MODEL_MAPPING[peft_config.task_type](model, peft_config)
```

### Comparing `peft-0.2.0/src/peft/peft_model.py` & `peft-0.3.0/src/peft/peft_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,246 +24,247 @@
 from accelerate.utils import get_balanced_memory
 from huggingface_hub import hf_hub_download
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from transformers import PreTrainedModel
 from transformers.modeling_outputs import SequenceClassifierOutput, TokenClassifierOutput
 from transformers.utils import PushToHubMixin
 
-from .tuners import LoraModel, PrefixEncoder, PromptEmbedding, PromptEncoder
+from .tuners import (
+    AdaLoraModel,
+    AdaptionPromptModel,
+    LoraModel,
+    PrefixEncoder,
+    PromptEmbedding,
+    PromptEncoder,
+)
 from .utils import (
     TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     WEIGHTS_NAME,
     PeftConfig,
     PeftType,
     PromptLearningConfig,
     TaskType,
+    _set_adapter,
     _set_trainable,
     get_peft_model_state_dict,
     set_peft_model_state_dict,
     shift_tokens_right,
 )
 
 
+PEFT_TYPE_TO_MODEL_MAPPING = {
+    PeftType.LORA: LoraModel,
+    PeftType.PROMPT_TUNING: PromptEmbedding,
+    PeftType.P_TUNING: PromptEncoder,
+    PeftType.PREFIX_TUNING: PrefixEncoder,
+    PeftType.ADALORA: AdaLoraModel,
+    PeftType.ADAPTION_PROMPT: AdaptionPromptModel,
+}
+
+
 class PeftModel(PushToHubMixin, torch.nn.Module):
     """
-    Parameter-Efficient Fine-Tuning Model. Base model encompassing various Peft methods.
+    Base model encompassing various Peft methods.
 
     Args:
-        model ([`PreTrainedModel`]): The base transformer model used for Peft.
+        model ([`~transformers.PreTrainedModel`]): The base transformer model used for Peft.
         peft_config ([`PeftConfig`]): The configuration of the Peft model.
 
 
     **Attributes**:
-        - **base_model** ([`PreTrainedModel`]) -- The base transformer model used for Peft.
+        - **base_model** ([`~transformers.PreTrainedModel`]) -- The base transformer model used for Peft.
         - **peft_config** ([`PeftConfig`]) -- The configuration of the Peft model.
         - **modules_to_save** (`list` of `str`) -- The list of sub-module names to save when
         saving the model.
         - **prompt_encoder** ([`PromptEncoder`]) -- The prompt encoder used for Peft if
-        `isinstance(self.peft_config, PromptLearningConfig)`.
+        using [`PromptLearningConfig`].
         - **prompt_tokens** (`torch.Tensor`) -- The virtual prompt tokens used for Peft if
-        `isinstance(self.peft_config, PromptLearningConfig)`.
+        using [`PromptLearningConfig`].
         - **transformer_backbone_name** (`str`) -- The name of the transformer
-        backbone in the base model if `isinstance(self.peft_config, PromptLearningConfig)`.
+        backbone in the base model if using [`PromptLearningConfig`].
         - **word_embeddings** (`torch.nn.Embedding`) -- The word embeddings of the transformer backbone
-        in the base model if `isinstance(self.peft_config, PromptLearningConfig)`.
+        in the base model if using [`PromptLearningConfig`].
     """
 
-    def __init__(self, model, peft_config: PeftConfig):
+    def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
         super().__init__()
-        self.peft_config = peft_config
         self.base_model = model
         self.config = self.base_model.config
         self.modules_to_save = None
-        if isinstance(self.peft_config, PromptLearningConfig):
-            self._setup_prompt_encoder()
+        self.peft_config = {}
+        self.active_adapter = adapter_name
+        self.peft_type = peft_config.peft_type
+        self.base_model_torch_dtype = getattr(model, "dtype", None)
+        if not isinstance(peft_config, PromptLearningConfig):
+            self.peft_config[adapter_name] = peft_config
+            self.base_model = PEFT_TYPE_TO_MODEL_MAPPING[peft_config.peft_type](
+                self.base_model, self.peft_config, adapter_name
+            )
+            self.set_additional_trainable_modules(peft_config, adapter_name)
         else:
-            self.base_model = LoraModel(peft_config, model)
-        if getattr(self.peft_config, "modules_to_save", None) is not None:
-            self.modules_to_save = self.peft_config.modules_to_save
-            _set_trainable(self)
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+            self.add_adapter(adapter_name, peft_config)
 
     def save_pretrained(self, save_directory, **kwargs):
         r"""
-        Args:
         This function saves the adapter model and the adapter configuration files to a directory, so that it can be
-        re-loaded using the `LoraModel.from_pretrained` class method, and also used by the `LoraModel.push_to_hub`
+        reloaded using the [`LoraModel.from_pretrained`] class method, and also used by the [`LoraModel.push_to_hub`]
         method.
+
+        Args:
             save_directory (`str`):
                 Directory where the adapter model and configuration files will be saved (will be created if it does not
                 exist).
-            **kwargs:
+            kwargs (additional keyword arguments, *optional*):
                 Additional keyword arguments passed along to the `push_to_hub` method.
         """
         if os.path.isfile(save_directory):
             raise ValueError(f"Provided path ({save_directory}) should be a directory, not a file")
         os.makedirs(save_directory, exist_ok=True)
 
-        # save only the trainable weights
-        output_state_dict = get_peft_model_state_dict(self, kwargs.get("state_dict", None))
-        torch.save(output_state_dict, os.path.join(save_directory, WEIGHTS_NAME))
-
-        # save the config and change the inference mode to `True`
-        if self.peft_config.base_model_name_or_path is None:
-            self.peft_config.base_model_name_or_path = (
-                self.base_model.__dict__.get("name_or_path", None)
-                if isinstance(self.peft_config, PromptLearningConfig)
-                else self.base_model.model.__dict__.get("name_or_path", None)
-            )
-        inference_mode = self.peft_config.inference_mode
-        self.peft_config.inference_mode = True
-        self.peft_config.save_pretrained(save_directory)
-        self.peft_config.inference_mode = inference_mode
+        for adapter_name, peft_config in self.peft_config.items():
+            # save only the trainable weights
+            output_state_dict = get_peft_model_state_dict(
+                self, state_dict=kwargs.get("state_dict", None), adapter_name=adapter_name
+            )
+            output_dir = os.path.join(save_directory, adapter_name) if adapter_name != "default" else save_directory
+            os.makedirs(output_dir, exist_ok=True)
+            torch.save(output_state_dict, os.path.join(output_dir, WEIGHTS_NAME))
+
+            # save the config and change the inference mode to `True`
+            if peft_config.base_model_name_or_path is None:
+                peft_config.base_model_name_or_path = (
+                    self.base_model.__dict__.get("name_or_path", None)
+                    if isinstance(peft_config, PromptLearningConfig)
+                    else self.base_model.model.__dict__.get("name_or_path", None)
+                )
+            inference_mode = peft_config.inference_mode
+            peft_config.inference_mode = True
+            peft_config.save_pretrained(output_dir)
+            peft_config.inference_mode = inference_mode
 
     @classmethod
-    def from_pretrained(cls, model, model_id, **kwargs):
+    def from_pretrained(cls, model, model_id, adapter_name="default", is_trainable=False, **kwargs):
         r"""
+        Instantiate a [`LoraModel`] from a pretrained Lora configuration and weights.
+
         Args:
-        Instantiate a `LoraModel` from a pretrained Lora configuration and weights.
-            model (`transformers.PreTrainedModel`):
-                The model to be adapted. The model should be initialized with the `from_pretrained` method. from
-                `transformers` library.
-            model_id (`str`):
+            model ([`~transformers.PreTrainedModel`]):
+                The model to be adapted. The model should be initialized with the
+                [`~transformers.PreTrainedModel.from_pretrained`] method from the 🤗 Transformers library.
+            model_id (`str` or `os.PathLike`):
                 The name of the Lora configuration to use. Can be either:
-                    - A string, the `model id` of a Lora configuration hosted inside a model repo on
-                        huggingface Hub
-                    - A path to a directory containing a Lora configuration file saved using the
-                        `save_pretrained` method, e.g., ``./my_lora_config_directory/``.
+                    - A string, the `model id` of a Lora configuration hosted inside a model repo on the Hugging Face
+                      Hub.
+                    - A path to a directory containing a Lora configuration file saved using the `save_pretrained`
+                      method (`./my_lora_config_directory/`).
         """
         from .mapping import MODEL_TYPE_TO_PEFT_MODEL_MAPPING, PEFT_TYPE_TO_CONFIG_MAPPING
 
         # load the config
-        config = PEFT_TYPE_TO_CONFIG_MAPPING[PeftConfig.from_pretrained(model_id).peft_type].from_pretrained(model_id)
-
-        if getattr(model, "hf_device_map", None) is not None:
+        config = PEFT_TYPE_TO_CONFIG_MAPPING[
+            PeftConfig.from_pretrained(model_id, subfolder=kwargs.get("subfolder", None)).peft_type
+        ].from_pretrained(model_id, subfolder=kwargs.get("subfolder", None))
+
+        if (getattr(model, "hf_device_map", None) is not None) and len(
+            set(model.hf_device_map.values()).intersection({"cpu", "disk"})
+        ) > 0:
             remove_hook_from_submodules(model)
 
-        if config.task_type not in MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys():
-            model = cls(model, config)
+        if isinstance(config, PromptLearningConfig) and is_trainable:
+            raise ValueError("Cannot set a prompt learning adapter to trainable when loading pretrained adapter.")
         else:
-            model = MODEL_TYPE_TO_PEFT_MODEL_MAPPING[config.task_type](model, config)
+            config.inference_mode = not is_trainable
 
-        # load weights if any
-        if os.path.exists(os.path.join(model_id, WEIGHTS_NAME)):
-            filename = os.path.join(model_id, WEIGHTS_NAME)
+        if config.task_type not in MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys():
+            model = cls(model, config, adapter_name)
         else:
-            try:
-                filename = hf_hub_download(model_id, WEIGHTS_NAME)
-            except:  # noqa
-                raise ValueError(
-                    f"Can't find weights for {model_id} in {model_id} or in the Hugging Face Hub. "
-                    f"Please check that the file {WEIGHTS_NAME} is present at {model_id}."
-                )
-
-        adapters_weights = torch.load(
-            filename, map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        )
-        # load the weights into the model
-        model = set_peft_model_state_dict(model, adapters_weights)
-        if getattr(model, "hf_device_map", None) is not None:
-            device_map = kwargs.get("device_map", "auto")
-            max_memory = kwargs.get("max_memory", None)
-            no_split_module_classes = model._no_split_modules
-            if device_map != "sequential":
-                max_memory = get_balanced_memory(
-                    model,
-                    max_memory=max_memory,
-                    no_split_module_classes=no_split_module_classes,
-                    low_zero=(device_map == "balanced_low_0"),
-                )
-            if isinstance(device_map, str):
-                device_map = infer_auto_device_map(
-                    model, max_memory=max_memory, no_split_module_classes=no_split_module_classes
-                )
-            model = dispatch_model(model, device_map=device_map)
-            hook = AlignDevicesHook(io_same_device=True)
-            if model.peft_config.peft_type == PeftType.LORA:
-                add_hook_to_module(model.base_model.model, hook)
-            else:
-                remove_hook_from_submodules(model.prompt_encoder)
-                add_hook_to_module(model.base_model, hook)
+            model = MODEL_TYPE_TO_PEFT_MODEL_MAPPING[config.task_type](model, config, adapter_name)
+        model.load_adapter(model_id, adapter_name, **kwargs)
         return model
 
-    def _setup_prompt_encoder(self):
+    def _setup_prompt_encoder(self, adapter_name):
+        config = self.peft_config[adapter_name]
+        self.prompt_encoder = torch.nn.ModuleDict({})
+        self.prompt_tokens = {}
         transformer_backbone = None
         for name, module in self.base_model.named_children():
             for param in module.parameters():
                 param.requires_grad = False
             if isinstance(module, PreTrainedModel):
                 # Make sure to freeze Tranformers model
                 if transformer_backbone is None:
                     transformer_backbone = module
                     self.transformer_backbone_name = name
 
-        if self.peft_config.num_transformer_submodules is None:
-            self.peft_config.num_transformer_submodules = (
-                2 if self.peft_config.task_type == TaskType.SEQ_2_SEQ_LM else 1
-            )
+        if config.num_transformer_submodules is None:
+            config.num_transformer_submodules = 2 if config.task_type == TaskType.SEQ_2_SEQ_LM else 1
 
         for named_param, value in list(transformer_backbone.named_parameters()):
             if value.shape[0] == self.base_model.config.vocab_size:
                 self.word_embeddings = transformer_backbone.get_submodule(named_param.replace(".weight", ""))
                 break
 
-        if self.peft_config.peft_type == PeftType.PROMPT_TUNING:
-            prompt_encoder = PromptEmbedding(self.peft_config, self.word_embeddings)
-        elif self.peft_config.peft_type == PeftType.P_TUNING:
-            prompt_encoder = PromptEncoder(self.peft_config)
-        elif self.peft_config.peft_type == PeftType.PREFIX_TUNING:
-            prompt_encoder = PrefixEncoder(self.peft_config)
+        if config.peft_type == PeftType.PROMPT_TUNING:
+            prompt_encoder = PromptEmbedding(config, self.word_embeddings)
+        elif config.peft_type == PeftType.P_TUNING:
+            prompt_encoder = PromptEncoder(config)
+        elif config.peft_type == PeftType.PREFIX_TUNING:
+            prompt_encoder = PrefixEncoder(config)
         else:
             raise ValueError("Not supported")
-        self.prompt_encoder = prompt_encoder
-        self.prompt_tokens = torch.arange(
-            self.peft_config.num_virtual_tokens * self.peft_config.num_transformer_submodules
+        self.prompt_encoder.update(torch.nn.ModuleDict({adapter_name: prompt_encoder}))
+        self.prompt_tokens[adapter_name] = torch.arange(
+            config.num_virtual_tokens * config.num_transformer_submodules
         ).long()
 
-    def get_prompt_embedding_to_save(self):
+    def get_prompt_embedding_to_save(self, adapter_name):
         """
         Returns the prompt embedding to save when saving the model. Only applicable when `peft_config.peft_type !=
         PeftType.LORA`.
         """
-        prompt_tokens = self.prompt_tokens.unsqueeze(0).expand(1, -1).to(self.device)
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
-            prompt_tokens = prompt_tokens[:, : self.peft_config.num_virtual_tokens]
-        prompt_embeddings = self.prompt_encoder(prompt_tokens)
+        prompt_tokens = self.prompt_tokens[adapter_name].unsqueeze(0).expand(1, -1).to(self.device)
+        if self.peft_config[adapter_name].peft_type == PeftType.PREFIX_TUNING:
+            prompt_tokens = prompt_tokens[:, : self.peft_config[adapter_name].num_virtual_tokens]
+        prompt_embeddings = self.prompt_encoder[adapter_name](prompt_tokens)
         return prompt_embeddings[0].detach().cpu()
 
     def get_prompt(self, batch_size):
         """
         Returns the virtual prompts to use for Peft. Only applicable when `peft_config.peft_type != PeftType.LORA`.
         """
-        prompt_tokens = self.prompt_tokens.unsqueeze(0).expand(batch_size, -1).to(self.device)
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
-            prompt_tokens = prompt_tokens[:, : self.peft_config.num_virtual_tokens]
-            if self.peft_config.inference_mode:
-                past_key_values = self.prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
+        peft_config = self.active_peft_config
+        prompt_encoder = self.prompt_encoder[self.active_adapter]
+        prompt_tokens = self.prompt_tokens[self.active_adapter].unsqueeze(0).expand(batch_size, -1).to(self.device)
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
+            prompt_tokens = prompt_tokens[:, : peft_config.num_virtual_tokens]
+            if peft_config.inference_mode:
+                past_key_values = prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
             else:
-                past_key_values = self.prompt_encoder(prompt_tokens)
+                past_key_values = prompt_encoder(prompt_tokens)
             past_key_values = past_key_values.view(
                 batch_size,
-                self.peft_config.num_virtual_tokens,
-                self.peft_config.num_layers * 2,
-                self.peft_config.num_attention_heads,
-                self.peft_config.token_dim // self.peft_config.num_attention_heads,
+                peft_config.num_virtual_tokens,
+                peft_config.num_layers * 2,
+                peft_config.num_attention_heads,
+                peft_config.token_dim // peft_config.num_attention_heads,
             )
-            if self.peft_config.num_transformer_submodules == 2:
+            if peft_config.num_transformer_submodules == 2:
                 past_key_values = torch.cat([past_key_values, past_key_values], dim=2)
             past_key_values = past_key_values.permute([2, 0, 3, 1, 4]).split(
-                self.peft_config.num_transformer_submodules * 2
+                peft_config.num_transformer_submodules * 2
             )
             if TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING.get(self.config.model_type, None) is not None:
                 post_process_fn = TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING[self.config.model_type]
                 past_key_values = post_process_fn(past_key_values)
             return past_key_values
         else:
-            if self.peft_config.inference_mode:
-                prompts = self.prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
+            if peft_config.inference_mode:
+                prompts = prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
             else:
-                prompts = self.prompt_encoder(prompt_tokens)
+                prompts = prompt_encoder(prompt_tokens)
             return prompts
 
     def print_trainable_parameters(self):
         """
         Prints the number of trainable parameters in the model.
         """
         trainable_params = 0
@@ -295,120 +296,252 @@
         return self.get_base_model()(*args, **kwargs)
 
     @contextmanager
     def disable_adapter(self):
         """
         Disables the adapter module.
         """
-        if isinstance(self.peft_config, PromptLearningConfig):
-            old_forward = self.forward
-            self.forward = self.base_model.forward
-        else:
-            self.base_model.disable_adapter_layers()
-        yield
-        if isinstance(self.peft_config, PromptLearningConfig):
-            self.forward = old_forward
-        else:
-            self.base_model.enable_adapter_layers()
+        try:
+            if isinstance(self.peft_config, PromptLearningConfig):
+                old_forward = self.forward
+                self.forward = self.base_model.forward
+            else:
+                self.base_model.disable_adapter_layers()
+            yield
+        finally:
+            if isinstance(self.peft_config, PromptLearningConfig):
+                self.forward = old_forward
+            else:
+                self.base_model.enable_adapter_layers()
 
     def get_base_model(self):
         """
         Returns the base model.
         """
-        return self.base_model if isinstance(self.peft_config, PromptLearningConfig) else self.base_model.model
+        return self.base_model if isinstance(self.active_peft_config, PromptLearningConfig) else self.base_model.model
+
+    def add_adapter(self, adapter_name, peft_config):
+        if peft_config.peft_type != self.peft_type:
+            raise ValueError(
+                f"Cannot combine adapters with different peft types. "
+                f"Found {self.peft_type} and {peft_config.peft_type}."
+            )
+        self.peft_config[adapter_name] = peft_config
+        if isinstance(peft_config, PromptLearningConfig):
+            self._setup_prompt_encoder(adapter_name)
+        else:
+            self.base_model.add_adapter(adapter_name, peft_config)
+
+        self.set_additional_trainable_modules(peft_config, adapter_name)
+
+    def set_additional_trainable_modules(self, peft_config, adapter_name):
+        if getattr(peft_config, "modules_to_save", None) is not None:
+            if self.modules_to_save is None:
+                self.modules_to_save = set(peft_config.modules_to_save)
+            else:
+                self.modules_to_save.update(peft_config.modules_to_save)
+            _set_trainable(self, adapter_name)
+
+    def load_adapter(self, model_id, adapter_name, is_trainable=False, **kwargs):
+        from .mapping import PEFT_TYPE_TO_CONFIG_MAPPING
+
+        if adapter_name not in self.peft_config:
+            # load the config
+            peft_config = PEFT_TYPE_TO_CONFIG_MAPPING[
+                PeftConfig.from_pretrained(model_id, subfolder=kwargs.get("subfolder", None)).peft_type
+            ].from_pretrained(model_id, subfolder=kwargs.get("subfolder", None))
+            if isinstance(peft_config, PromptLearningConfig) and is_trainable:
+                raise ValueError("Cannot set a prompt learning adapter to trainable when loading pretrained adapter.")
+            else:
+                peft_config.inference_mode = not is_trainable
+            self.add_adapter(adapter_name, peft_config)
+
+        # load weights if any
+        path = os.path.join(model_id, kwargs["subfolder"]) if kwargs.get("subfolder", None) is not None else model_id
+
+        if os.path.exists(os.path.join(path, WEIGHTS_NAME)):
+            filename = os.path.join(path, WEIGHTS_NAME)
+        else:
+            try:
+                filename = hf_hub_download(model_id, WEIGHTS_NAME, subfolder=kwargs.get("subfolder", None))
+            except:  # noqa
+                raise ValueError(
+                    f"Can't find weights for {model_id} in {model_id} or in the Hugging Face Hub. "
+                    f"Please check that the file {WEIGHTS_NAME} is present at {model_id}."
+                )
+
+        adapters_weights = torch.load(
+            filename, map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        )
+        # load the weights into the model
+        set_peft_model_state_dict(self, adapters_weights, adapter_name=adapter_name)
+        if (
+            (getattr(self, "hf_device_map", None) is not None)
+            and (len(set(self.hf_device_map.values()).intersection({"cpu", "disk"})) > 0)
+            and len(self.peft_config) == 1
+        ):
+            device_map = kwargs.get("device_map", "auto")
+            max_memory = kwargs.get("max_memory", None)
+            offload_dir = kwargs.get("offload_folder", None)
+            offload_index = kwargs.get("offload_index", None)
+
+            dispatch_model_kwargs = {}
+            # Safety checker for previous `accelerate` versions
+            # `offload_index` was introduced in https://github.com/huggingface/accelerate/pull/873/
+            if "offload_index" in inspect.signature(dispatch_model).parameters:
+                dispatch_model_kwargs["offload_index"] = offload_index
+
+            no_split_module_classes = self._no_split_modules
+
+            if device_map != "sequential":
+                max_memory = get_balanced_memory(
+                    self,
+                    max_memory=max_memory,
+                    no_split_module_classes=no_split_module_classes,
+                    low_zero=(device_map == "balanced_low_0"),
+                )
+            if isinstance(device_map, str):
+                device_map = infer_auto_device_map(
+                    self, max_memory=max_memory, no_split_module_classes=no_split_module_classes
+                )
+            dispatch_model(
+                self,
+                device_map=device_map,
+                offload_dir=offload_dir,
+                **dispatch_model_kwargs,
+            )
+            hook = AlignDevicesHook(io_same_device=True)
+            if isinstance(self.peft_config[adapter_name], PromptLearningConfig):
+                remove_hook_from_submodules(self.prompt_encoder)
+            add_hook_to_module(self.get_base_model(), hook)
+
+        # Set model in evaluation mode to deactivate Dropout modules by default
+        self.eval()
+
+    def set_adapter(self, adapter_name):
+        """
+        Sets the active adapter.
+        """
+        if adapter_name not in self.peft_config:
+            raise ValueError(f"Adapter {adapter_name} not found.")
+        self.active_adapter = adapter_name
+        if not isinstance(self.peft_config[adapter_name], PromptLearningConfig):
+            self.base_model.set_adapter(adapter_name)
+        _set_adapter(self, adapter_name)
+
+    @property
+    def active_peft_config(self):
+        return self.peft_config[self.active_adapter]
 
 
 class PeftModelForSequenceClassification(PeftModel):
     """
     Peft model for sequence classification tasks.
 
     Args:
-        model ([`PreTrainedModel`]): Base transformer model
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
         peft_config ([`PeftConfig`]): Peft config.
 
     **Attributes**:
-        - **config** ([`PretrainedConfig`]) -- The configuration object of the base model.
+        - **config** ([`~transformers.PretrainedConfig`]) -- The configuration object of the base model.
         - **cls_layer_name** (`str`) -- The name of the classification layer.
 
-    Example::
+    Example:
 
-        >>> from transformers import AutoModelForSequenceClassification >>> from peft import
-        PeftModelForSequenceClassification, get_peft_config >>> config = {
-                'peft_type': 'PREFIX_TUNING', 'task_type': 'SEQ_CLS', 'inference_mode': False, 'num_virtual_tokens':
-                20, 'token_dim': 768, 'num_transformer_submodules': 1, 'num_attention_heads': 12, 'num_layers': 12,
-                'encoder_hidden_size': 768, 'prefix_projection': False, 'postprocess_past_key_value_function': None
-            }
-        >>> peft_config = get_peft_config(config) >>> model =
-        AutoModelForSequenceClassification.from_pretrained("bert-base-cased") >>> peft_model =
-        PeftModelForSequenceClassification(model, peft_config) >>> peft_model.print_trainable_parameters() trainable
-        params: 370178 || all params: 108680450 || trainable%: 0.3406113979101117
+        ```py
+        >>> from transformers import AutoModelForSequenceClassification
+        >>> from peft import PeftModelForSequenceClassification, get_peft_config
+
+        >>> config = {
+        ...     "peft_type": "PREFIX_TUNING",
+        ...     "task_type": "SEQ_CLS",
+        ...     "inference_mode": False,
+        ...     "num_virtual_tokens": 20,
+        ...     "token_dim": 768,
+        ...     "num_transformer_submodules": 1,
+        ...     "num_attention_heads": 12,
+        ...     "num_layers": 12,
+        ...     "encoder_hidden_size": 768,
+        ...     "prefix_projection": False,
+        ...     "postprocess_past_key_value_function": None,
+        ... }
+
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModelForSequenceClassification.from_pretrained("bert-base-cased")
+        >>> peft_model = PeftModelForSequenceClassification(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        trainable params: 370178 || all params: 108680450 || trainable%: 0.3406113979101117
+        ```
     """
 
-    def __init__(self, model, peft_config: PeftConfig):
-        super().__init__(model, peft_config)
-        self.modules_to_save = ["classifier", "score"]
+    def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
+        if self.modules_to_save is None:
+            self.modules_to_save = {"classifier", "score"}
+        else:
+            self.modules_to_save.update({"classifier", "score"})
 
         for name, _ in self.base_model.named_children():
             if any(module_name in name for module_name in self.modules_to_save):
                 self.cls_layer_name = name
                 break
 
         # to make sure classifier layer is trainable
-        _set_trainable(self)
+        _set_trainable(self, adapter_name)
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        if not isinstance(self.peft_config, PromptLearningConfig):
+        peft_config = self.active_peft_config
+        if not isinstance(peft_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, self.peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         kwargs.update(
             {
                 "attention_mask": attention_mask,
                 "labels": labels,
                 "output_attentions": output_attentions,
                 "output_hidden_states": output_hidden_states,
                 "return_dict": return_dict,
             }
         )
 
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
             return self._prefix_tuning_forward(input_ids=input_ids, **kwargs)
         else:
             if kwargs.get("token_type_ids", None) is not None:
                 kwargs["token_type_ids"] = torch.cat(
                     (
-                        torch.zeros(batch_size, self.peft_config.num_virtual_tokens).to(self.device),
+                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.device),
                         kwargs["token_type_ids"],
                     ),
                     dim=1,
                 ).long()
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             prompts = self.get_prompt(batch_size=batch_size)
@@ -486,66 +619,81 @@
                 hidden_states=outputs.hidden_states,
                 attentions=outputs.attentions,
             )
 
 
 class PeftModelForCausalLM(PeftModel):
     """
-    Peft model for Causal LM
+    Peft model for causal language modeling.
 
     Args:
-        model ([`PreTrainedModel`]): Base transformer model
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
         peft_config ([`PeftConfig`]): Peft config.
 
 
-    Example::
+    Example:
+
+        ```py
+        >>> from transformers import AutoModelForCausalLM
+        >>> from peft import PeftModelForCausalLM, get_peft_config
 
-        >>> from transformers import AutoModelForCausalLM >>> from peft import PeftModelForCausalLM, get_peft_config
         >>> config = {
-                'peft_type': 'PREFIX_TUNING', 'task_type': 'CAUSAL_LM', 'inference_mode': False, 'num_virtual_tokens':
-                20, 'token_dim': 1280, 'num_transformer_submodules': 1, 'num_attention_heads': 20, 'num_layers': 36,
-                'encoder_hidden_size': 1280, 'prefix_projection': False, 'postprocess_past_key_value_function': None
-            }
-        >>> peft_config = get_peft_config(config) >>> model = AutoModelForCausalLM.from_pretrained("gpt2-large") >>>
-        peft_model = PeftModelForCausalLM(model, peft_config) >>> peft_model.print_trainable_parameters() trainable
-        params: 1843200 || all params: 775873280 || trainable%: 0.23756456724479544
+        ...     "peft_type": "PREFIX_TUNING",
+        ...     "task_type": "CAUSAL_LM",
+        ...     "inference_mode": False,
+        ...     "num_virtual_tokens": 20,
+        ...     "token_dim": 1280,
+        ...     "num_transformer_submodules": 1,
+        ...     "num_attention_heads": 20,
+        ...     "num_layers": 36,
+        ...     "encoder_hidden_size": 1280,
+        ...     "prefix_projection": False,
+        ...     "postprocess_past_key_value_function": None,
+        ... }
+
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModelForCausalLM.from_pretrained("gpt2-large")
+        >>> peft_model = PeftModelForCausalLM(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        trainable params: 1843200 || all params: 775873280 || trainable%: 0.23756456724479544
+        ```
     """
 
-    def __init__(self, model, peft_config: PeftConfig):
-        super().__init__(model, peft_config)
+    def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
         self.base_model_prepare_inputs_for_generation = self.base_model.prepare_inputs_for_generation
-        self.base_model.prepare_inputs_for_generation = self.prepare_inputs_for_generation
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
-        if not isinstance(self.peft_config, PromptLearningConfig):
+        peft_config = self.active_peft_config
+        if not isinstance(peft_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, self.peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
 
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         if kwargs.get("token_type_ids", None) is not None:
             warnings.warn("Token type ids are not supported for parameter efficient tuning. Ignoring token type ids")
@@ -556,102 +704,155 @@
                 "labels": labels,
                 "output_attentions": output_attentions,
                 "output_hidden_states": output_hidden_states,
                 "return_dict": return_dict,
             }
         )
 
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
             past_key_values = self.get_prompt(batch_size)
             return self.base_model(input_ids=input_ids, past_key_values=past_key_values, **kwargs)
         else:
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             # concat prompt labels
             if labels is not None:
-                prefix_labels = torch.full((batch_size, self.peft_config.num_virtual_tokens), -100).to(self.device)
+                prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(self.device)
                 kwargs["labels"] = torch.cat((prefix_labels, labels), dim=1)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
             inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
             return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
 
     def generate(self, **kwargs):
-        if not isinstance(self.peft_config, PromptLearningConfig):
-            return self.base_model.generate(**kwargs)
+        peft_config = self.active_peft_config
+        self.base_model.prepare_inputs_for_generation = self.prepare_inputs_for_generation
+        try:
+            if not isinstance(peft_config, PromptLearningConfig):
+                outputs = self.base_model.generate(**kwargs)
+            else:
+                if "input_ids" not in kwargs:
+                    raise ValueError("input_ids must be provided for Peft model generation")
+                # For gpt2 models, we construct postion_ids on the fly by using attention mask, and position ids need to match input_shape.
+                # for prefix tuning, input shape is determined using `input_ids`. Thus we should not expand 'attention_mask' here
+                # for prompt tuning input_ids is not passed but a concatenated input_embeds is passed. Thus attention_mask needs to be of same size of num_virtual_tokens + input_ids
+                if kwargs.get("attention_mask", None) is not None and peft_config.peft_type in [
+                    PeftType.PROMPT_TUNING,
+                    PeftType.P_TUNING,
+                ]:
+                    # concat prompt attention mask
+                    prefix_attention_mask = torch.ones(
+                        kwargs["input_ids"].shape[0], peft_config.num_virtual_tokens
+                    ).to(kwargs["input_ids"].device)
+                    kwargs["attention_mask"] = torch.cat((prefix_attention_mask, kwargs["attention_mask"]), dim=1)
+
+                if kwargs.get("position_ids", None) is not None:
+                    warnings.warn(
+                        "Position ids are not supported for parameter efficient tuning. Ignoring position ids."
+                    )
+                    kwargs["position_ids"] = None
+                if kwargs.get("token_type_ids", None) is not None:
+                    warnings.warn(
+                        "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
+                    )
+                    kwargs["token_type_ids"] = None
+
+                outputs = self.base_model.generate(**kwargs)
+        except:
+            self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
+            raise
         else:
-            if "input_ids" not in kwargs:
-                raise ValueError("input_ids must be provided for Peft model generation")
-            if kwargs.get("attention_mask", None) is not None:
-                # concat prompt attention mask
-                prefix_attention_mask = torch.ones(
-                    kwargs["input_ids"].shape[0], self.peft_config.num_virtual_tokens
-                ).to(kwargs["input_ids"].device)
-                kwargs["attention_mask"] = torch.cat((prefix_attention_mask, kwargs["attention_mask"]), dim=1)
-
-            if kwargs.get("position_ids", None) is not None:
-                warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
-                kwargs["position_ids"] = None
-            if kwargs.get("token_type_ids", None) is not None:
-                warnings.warn(
-                    "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
-                )
-                kwargs["token_type_ids"] = None
-
-            return self.base_model.generate(**kwargs)
+            self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
+            return outputs
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
+        peft_config = self.active_peft_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
-        if isinstance(self.peft_config, PromptLearningConfig):
-            if model_kwargs["past_key_values"] is None and self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if isinstance(peft_config, PromptLearningConfig):
+            if peft_config.peft_type == PeftType.PREFIX_TUNING:
+                prefix_attention_mask = torch.ones(
+                    model_kwargs["input_ids"].shape[0], peft_config.num_virtual_tokens
+                ).to(model_kwargs["input_ids"].device)
+                model_kwargs["attention_mask"] = torch.cat(
+                    (prefix_attention_mask, model_kwargs["attention_mask"]), dim=1
+                )
+
+            if model_kwargs["past_key_values"] is None and peft_config.peft_type == PeftType.PREFIX_TUNING:
                 past_key_values = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0])
+
+                if self.base_model_torch_dtype is not None:
+                    # handle the case for Bloom where it outputs tuple of tuples
+                    if isinstance(past_key_values[0], tuple):
+                        past_key_values = tuple(
+                            tuple(
+                                past_key_value.to(self.base_model_torch_dtype)
+                                for past_key_value in past_key_value_tuple
+                            )
+                            for past_key_value_tuple in past_key_values
+                        )
+                    else:
+                        past_key_values = tuple(
+                            past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_values
+                        )
+
                 model_kwargs["past_key_values"] = past_key_values
             else:
                 if model_kwargs["past_key_values"] is None:
                     inputs_embeds = self.word_embeddings(model_kwargs["input_ids"])
                     prompts = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0])
                     prompts = prompts.to(inputs_embeds.dtype)
                     model_kwargs["inputs_embeds"] = torch.cat((prompts, inputs_embeds), dim=1)
                     model_kwargs["input_ids"] = None
 
         return model_kwargs
 
 
 class PeftModelForSeq2SeqLM(PeftModel):
     """
-    Peft model for Seq2Seq LM
+    Peft model for sequence-to-sequence language modeling.
 
     Args:
-        model ([`PreTrainedModel`]): Base transformer model
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
         peft_config ([`PeftConfig`]): Peft config.
 
 
-    Example::
+    Example:
+
+        ```py
+        >>> from transformers import AutoModelForSeq2SeqLM
+        >>> from peft import PeftModelForSeq2SeqLM, get_peft_config
 
-        >>> from transformers import AutoModelForSeq2SeqLM >>> from peft import PeftModelForSeq2SeqLM, get_peft_config
         >>> config = {
-                'peft_type': 'LORA', 'task_type': 'SEQ_2_SEQ_LM', 'inference_mode': False, 'r': 8, 'target_modules':
-                ['q', 'v'], 'lora_alpha': 32, 'lora_dropout': 0.1, 'merge_weights': False, 'fan_in_fan_out': False,
-                'enable_lora': None, 'bias': 'none'
-            }
-        >>> peft_config = get_peft_config(config) >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base") >>>
-        peft_model = PeftModelForSeq2SeqLM(model, peft_config) >>> peft_model.print_trainable_parameters() trainable
-        params: 884736 || all params: 223843584 || trainable%: 0.3952474242013566
+        ...     "peft_type": "LORA",
+        ...     "task_type": "SEQ_2_SEQ_LM",
+        ...     "inference_mode": False,
+        ...     "r": 8,
+        ...     "target_modules": ["q", "v"],
+        ...     "lora_alpha": 32,
+        ...     "lora_dropout": 0.1,
+        ...     "merge_weights": False,
+        ...     "fan_in_fan_out": False,
+        ...     "enable_lora": None,
+        ...     "bias": "none",
+        ... }
+
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base")
+        >>> peft_model = PeftModelForSeq2SeqLM(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        trainable params: 884736 || all params: 223843584 || trainable%: 0.3952474242013566
+        ```
     """
 
-    def __init__(self, model, peft_config: PeftConfig):
-        super().__init__(model, peft_config)
+    def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
         self.base_model_prepare_inputs_for_generation = self.base_model.prepare_inputs_for_generation
-        self.base_model.prepare_inputs_for_generation = self.prepare_inputs_for_generation
         self.base_model_prepare_encoder_decoder_kwargs_for_generation = (
             self.base_model._prepare_encoder_decoder_kwargs_for_generation
         )
-        self.base_model._prepare_encoder_decoder_kwargs_for_generation = (
-            self._prepare_encoder_decoder_kwargs_for_generation
-        )
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         inputs_embeds=None,
         decoder_input_ids=None,
@@ -659,15 +860,16 @@
         decoder_inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
-        if not isinstance(self.peft_config, PromptLearningConfig):
+        peft_config = self.active_peft_config
+        if not isinstance(peft_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 decoder_input_ids=decoder_input_ids,
                 decoder_attention_mask=decoder_attention_mask,
                 decoder_inputs_embeds=decoder_inputs_embeds,
@@ -677,15 +879,15 @@
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if decoder_attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, self.peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
             decoder_attention_mask = torch.cat((prefix_attention_mask, decoder_attention_mask), dim=1)
 
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         if kwargs.get("token_type_ids", None) is not None:
             warnings.warn("Token type ids are not supported for parameter efficient tuning. Ignoring token type ids")
@@ -697,15 +899,15 @@
                 "labels": labels,
                 "output_attentions": output_attentions,
                 "output_hidden_states": output_hidden_states,
                 "return_dict": return_dict,
             }
         )
 
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
             past_key_values = self.get_prompt(batch_size)
             return self.base_model(
                 input_ids=input_ids, decoder_input_ids=decoder_input_ids, past_key_values=past_key_values, **kwargs
             )
         else:
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
@@ -713,153 +915,206 @@
                 decoder_input_ids = shift_tokens_right(
                     labels, self.config.pad_token_id, self.config.decoder_start_token_id
                 )
                 decoder_inputs_embeds = self.word_embeddings(decoder_input_ids)
 
             if attention_mask is not None:
                 # concat prompt attention mask
-                prefix_attention_mask = torch.ones(batch_size, self.peft_config.num_virtual_tokens).to(self.device)
+                prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
                 kwargs["attention_mask"] = torch.cat((prefix_attention_mask, attention_mask), dim=1)
             # concat prompt labels
             if labels is not None:
-                if self.peft_config.num_transformer_submodules == 1:
+                if peft_config.num_transformer_submodules == 1:
                     kwargs["labels"] = labels
-                elif self.peft_config.num_transformer_submodules == 2:
-                    prefix_labels = torch.full((batch_size, self.peft_config.num_virtual_tokens), -100).to(self.device)
+                elif peft_config.num_transformer_submodules == 2:
+                    prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(self.device)
                     kwargs["labels"] = torch.cat((prefix_labels, labels), dim=1)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
-            inputs_embeds = torch.cat((prompts[:, : self.peft_config.num_virtual_tokens], inputs_embeds), dim=1)
-            if self.peft_config.num_transformer_submodules == 1:
+            inputs_embeds = torch.cat((prompts[:, : peft_config.num_virtual_tokens], inputs_embeds), dim=1)
+            if peft_config.num_transformer_submodules == 1:
                 return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
-            elif self.peft_config.num_transformer_submodules == 2:
+            elif peft_config.num_transformer_submodules == 2:
                 decoder_inputs_embeds = torch.cat(
-                    (prompts[:, self.peft_config.num_virtual_tokens :], decoder_inputs_embeds), dim=1
+                    (prompts[:, peft_config.num_virtual_tokens :], decoder_inputs_embeds), dim=1
                 )
                 return self.base_model(
                     inputs_embeds=inputs_embeds, decoder_inputs_embeds=decoder_inputs_embeds, **kwargs
                 )
 
     def generate(self, **kwargs):
-        if not isinstance(self.peft_config, PromptLearningConfig):
-            return self.base_model.generate(**kwargs)
-        else:
-            if "input_ids" not in kwargs:
-                raise ValueError("input_ids must be provided for Peft model generation")
-            if kwargs.get("position_ids", None) is not None:
-                warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
-                kwargs["position_ids"] = None
-            if kwargs.get("token_type_ids", None) is not None:
-                warnings.warn(
-                    "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
-                )
-                kwargs["token_type_ids"] = None
-
-            if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
-                return self.base_model.generate(**kwargs)
+        peft_config = self.active_peft_config
+        self.base_model.prepare_inputs_for_generation = self.prepare_inputs_for_generation
+        self.base_model._prepare_encoder_decoder_kwargs_for_generation = (
+            self._prepare_encoder_decoder_kwargs_for_generation
+        )
+        try:
+            if not isinstance(peft_config, PromptLearningConfig):
+                outputs = self.base_model.generate(**kwargs)
             else:
-                raise NotImplementedError
+                if "input_ids" not in kwargs:
+                    raise ValueError("input_ids must be provided for Peft model generation")
+                if kwargs.get("position_ids", None) is not None:
+                    warnings.warn(
+                        "Position ids are not supported for parameter efficient tuning. Ignoring position ids."
+                    )
+                    kwargs["position_ids"] = None
+                if kwargs.get("token_type_ids", None) is not None:
+                    warnings.warn(
+                        "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
+                    )
+                    kwargs["token_type_ids"] = None
+
+                if peft_config.peft_type == PeftType.PREFIX_TUNING:
+                    outputs = self.base_model.generate(**kwargs)
+                else:
+                    raise NotImplementedError
+        except:
+            self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
+            self.base_model._prepare_encoder_decoder_kwargs_for_generation = (
+                self.base_model_prepare_encoder_decoder_kwargs_for_generation
+            )
+            raise
+        else:
+            self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
+            self.base_model._prepare_encoder_decoder_kwargs_for_generation = (
+                self.base_model_prepare_encoder_decoder_kwargs_for_generation
+            )
+            return outputs
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
+        peft_config = self.active_peft_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
-        if model_kwargs["past_key_values"] is None and self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if model_kwargs["past_key_values"] is None and peft_config.peft_type == PeftType.PREFIX_TUNING:
             batch_size = model_kwargs["decoder_input_ids"].shape[0]
             past_key_values = self.get_prompt(batch_size)
+            if self.base_model_torch_dtype is not None:
+                # handle the case for Bloom where it outputs tuple of tuples
+                if isinstance(past_key_values[0], tuple):
+                    past_key_values = tuple(
+                        tuple(
+                            past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_value_tuple
+                        )
+                        for past_key_value_tuple in past_key_values
+                    )
+                else:
+                    past_key_values = tuple(
+                        past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_values
+                    )
             model_kwargs["past_key_values"] = past_key_values
+
         return model_kwargs
 
 
 class PeftModelForTokenClassification(PeftModel):
     """
-    Peft model for sequence classification tasks.
+    Peft model for token classification tasks.
 
     Args:
-        model ([`PreTrainedModel`]): Base transformer model
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
         peft_config ([`PeftConfig`]): Peft config.
 
     **Attributes**:
-        - **config** ([`PretrainedConfig`]) -- The configuration object of the base model.
+        - **config** ([`~transformers.PretrainedConfig`]) -- The configuration object of the base model.
         - **cls_layer_name** (`str`) -- The name of the classification layer.
 
-    Example::
+    Example:
 
-        >>> from transformers import AutoModelForSequenceClassification >>> from peft import
-        PeftModelForTokenClassification, get_peft_config >>> config = {
-                'peft_type': 'PREFIX_TUNING', 'task_type': 'TOKEN_CLS', 'inference_mode': False, 'num_virtual_tokens':
-                20, 'token_dim': 768, 'num_transformer_submodules': 1, 'num_attention_heads': 12, 'num_layers': 12,
-                'encoder_hidden_size': 768, 'prefix_projection': False, 'postprocess_past_key_value_function': None
-            }
-        >>> peft_config = get_peft_config(config) >>> model =
-        AutoModelForTokenClassification.from_pretrained("bert-base-cased") >>> peft_model =
-        PeftModelForTokenClassification(model, peft_config) >>> peft_model.print_trainable_parameters() trainable
-        params: 370178 || all params: 108680450 || trainable%: 0.3406113979101117
+        ```py
+        >>> from transformers import AutoModelForSequenceClassification
+        >>> from peft import PeftModelForTokenClassification, get_peft_config
+
+        >>> config = {
+        ...     "peft_type": "PREFIX_TUNING",
+        ...     "task_type": "TOKEN_CLS",
+        ...     "inference_mode": False,
+        ...     "num_virtual_tokens": 20,
+        ...     "token_dim": 768,
+        ...     "num_transformer_submodules": 1,
+        ...     "num_attention_heads": 12,
+        ...     "num_layers": 12,
+        ...     "encoder_hidden_size": 768,
+        ...     "prefix_projection": False,
+        ...     "postprocess_past_key_value_function": None,
+        ... }
+
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModelForTokenClassification.from_pretrained("bert-base-cased")
+        >>> peft_model = PeftModelForTokenClassification(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        trainable params: 370178 || all params: 108680450 || trainable%: 0.3406113979101117
+        ```
     """
 
-    def __init__(self, model, peft_config: PeftConfig):
-        super().__init__(model, peft_config)
-        self.modules_to_save = ["classifier", "score"]
+    def __init__(self, model, peft_config: PeftConfig = None, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
+        if self.modules_to_save is None:
+            self.modules_to_save = {"classifier", "score"}
+        else:
+            self.modules_to_save.update({"classifier", "score"})
 
         for name, _ in self.base_model.named_children():
             if any(module_name in name for module_name in self.modules_to_save):
                 self.cls_layer_name = name
                 break
 
         # to make sure classifier layer is trainable
-        _set_trainable(self)
+        _set_trainable(self, adapter_name)
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
+        peft_config = self.active_peft_config
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        if not isinstance(self.peft_config, PromptLearningConfig):
+        if not isinstance(peft_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, self.peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         kwargs.update(
             {
                 "attention_mask": attention_mask,
                 "labels": labels,
                 "output_attentions": output_attentions,
                 "output_hidden_states": output_hidden_states,
                 "return_dict": return_dict,
             }
         )
 
-        if self.peft_config.peft_type == PeftType.PREFIX_TUNING:
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
             return self._prefix_tuning_forward(input_ids=input_ids, **kwargs)
         else:
             if kwargs.get("token_type_ids", None) is not None:
                 kwargs["token_type_ids"] = torch.cat(
                     (
-                        torch.zeros(batch_size, self.peft_config.num_virtual_tokens).to(self.device),
+                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.device),
                         kwargs["token_type_ids"],
                     ),
                     dim=1,
                 ).long()
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             prompts = self.get_prompt(batch_size=batch_size)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `peft-0.2.0/src/peft/tuners/__init__.py` & `peft-0.3.0/src/peft/tuners/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,11 +13,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .adaption_prompt import AdaptionPromptConfig, AdaptionPromptModel
 from .lora import LoraConfig, LoraModel
+from .adalora import AdaLoraConfig, AdaLoraModel
 from .p_tuning import PromptEncoder, PromptEncoderConfig, PromptEncoderReparameterizationType
 from .prefix_tuning import PrefixEncoder, PrefixTuningConfig
 from .prompt_tuning import PromptEmbedding, PromptTuningConfig, PromptTuningInit
```

### Comparing `peft-0.2.0/src/peft/tuners/lora.py` & `peft-0.3.0/src/peft/tuners/lora.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,52 +8,54 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import importlib
 import math
 import re
 import warnings
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from typing import List, Optional, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from transformers.pytorch_utils import Conv1D
 
-from ..utils import PeftConfig, PeftType, transpose
-
-
-def is_bnb_available():
-    return importlib.util.find_spec("bitsandbytes") is not None
+from ..import_utils import is_bnb_available
+from ..utils import (
+    TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
+    ModulesToSaveWrapper,
+    PeftConfig,
+    PeftType,
+    _freeze_adapter,
+    _get_submodules,
+    transpose,
+)
 
 
 if is_bnb_available():
     import bitsandbytes as bnb
 
 
 @dataclass
 class LoraConfig(PeftConfig):
     """
-    This is the configuration class to store the configuration of a [`~peft.Lora`].
+    This is the configuration class to store the configuration of a [`LoraModel`].
 
     Args:
-        r (`int`): Lora attention dimension
+        r (`int`): Lora attention dimension.
         target_modules (`Union[List[str],str]`): The names of the modules to apply Lora to.
         lora_alpha (`float`): The alpha parameter for Lora scaling.
         lora_dropout (`float`): The dropout probability for Lora layers.
-        merge_weights (`bool`):
-            Whether to merge the weights of the Lora layers with the base transformer model in `eval` mode.
-        fan_in_fan_out (`bool`): Set this to True if the layer to replace stores weight like (fan_in, fan_out)
-        enable_lora ( `List[bool]`): Used with `lora.MergedLinear`.
+        fan_in_fan_out (`bool`): Set this to True if the layer to replace stores weight like (fan_in, fan_out).
+        For example, gpt-2 uses `Conv1D` which stores weights like (fan_in, fan_out) and hence this should be set to `True`.:
         bias (`str`): Bias type for Lora. Can be 'none', 'all' or 'lora_only'
         modules_to_save (`List[str]`):List of modules apart from LoRA layers to be set as trainable
             and saved in the final checkpoint.
     """
 
     r: int = field(default=8, metadata={"help": "Lora attention dimension"})
     target_modules: Optional[Union[List[str], str]] = field(
@@ -61,175 +63,337 @@
         metadata={
             "help": "List of module names or regex expression of the module names to replace with Lora."
             "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$' "
         },
     )
     lora_alpha: int = field(default=None, metadata={"help": "Lora alpha"})
     lora_dropout: float = field(default=None, metadata={"help": "Lora dropout"})
-    merge_weights: bool = field(
-        default=False, metadata={"help": "Merge weights of the original model and the Lora model"}
-    )
     fan_in_fan_out: bool = field(
         default=False,
         metadata={"help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"},
     )
-    enable_lora: Optional[List[bool]] = field(default=None, metadata={"help": "Used with `lora.MergedLinear`."})
     bias: str = field(default="none", metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"})
     modules_to_save: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
     )
+    init_lora_weights: bool = field(
+        default=True,
+        metadata={"help": "Whether to initialize the weights of the Lora layers."},
+    )
 
     def __post_init__(self):
         self.peft_type = PeftType.LORA
 
 
 class LoraModel(torch.nn.Module):
     """
     Creates Low Rank Adapter (Lora) model from a pretrained transformers model.
 
     Args:
-        model ([`transformers.PreTrainedModel`]): The model to be adapted.
+        model ([`~transformers.PreTrainedModel`]): The model to be adapted.
         config ([`LoraConfig`]): The configuration of the Lora model.
 
     Returns:
         `torch.nn.Module`: The Lora model.
 
-    Example::
+    Example:
 
-        >>> from transformers import AutoModelForSeq2SeqLM, LoraConfig >>> from peft import LoraModel, LoraConfig >>>
-        config = LoraConfig(
-            peft_type="LORA", task_type="SEQ_2_SEQ_LM", r=8, lora_alpha=32, target_modules=["q", "v"],
-            lora_dropout=0.01, )
-        >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base") >>> lora_model = LoraModel(config, model)
+        ```py
+        >>> from transformers import AutoModelForSeq2SeqLM, LoraConfig
+        >>> from peft import LoraModel, LoraConfig
+
+        >>> config = LoraConfig(
+        ...     peft_type="LORA",
+        ...     task_type="SEQ_2_SEQ_LM",
+        ...     r=8,
+        ...     lora_alpha=32,
+        ...     target_modules=["q", "v"],
+        ...     lora_dropout=0.01,
+        ... )
+
+        >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base")
+        >>> lora_model = LoraModel(config, model)
+        ```
+
+        ```py
+        >>> import transformers
+        >>> from peft import LoraConfig, PeftModel, get_peft_model, prepare_model_for_int8_training
+
+        >>> target_modules = ["q_proj", "k_proj", "v_proj", "out_proj", "fc_in", "fc_out", "wte"]
+        >>> config = LoraConfig(
+        ...     r=4, lora_alpha=16, target_modules=target_modules, lora_dropout=0.1, bias="none", task_type="CAUSAL_LM"
+        ... )
+
+        >>> model = transformers.GPTJForCausalLM.from_pretrained(
+        ...     "kakaobrain/kogpt",
+        ...     revision="KoGPT6B-ryan1.5b-float16",  # or float32 version: revision=KoGPT6B-ryan1.5b
+        ...     pad_token_id=tokenizer.eos_token_id,
+        ...     use_cache=False,
+        ...     device_map={"": rank},
+        ...     torch_dtype=torch.float16,
+        ...     load_in_8bit=True,
+        ... )
+        >>> model = prepare_model_for_int8_training(model)
+        >>> lora_model = get_peft_model(model, config)
+        ```
 
     **Attributes**:
-        - **model** ([`transformers.PreTrainedModel`]) -- The model to be adapted.
+        - **model** ([`~transformers.PreTrainedModel`]) -- The model to be adapted.
         - **peft_config** ([`LoraConfig`]): The configuration of the Lora model.
     """
 
-    def __init__(self, config, model):
+    def __init__(self, model, config, adapter_name):
         super().__init__()
-        self.peft_config = config
         self.model = model
-        self._find_and_replace()
-        mark_only_lora_as_trainable(self.model, self.peft_config.bias)
         self.forward = self.model.forward
+        self.peft_config = config
+        self.add_adapter(adapter_name, self.peft_config[adapter_name])
 
-    def _find_and_replace(self):
+    def add_adapter(self, adapter_name, config=None):
+        if config is not None:
+            model_config = self.model.config.to_dict() if hasattr(self.model.config, "to_dict") else self.model.config
+            config = self._prepare_lora_config(config, model_config)
+            self.peft_config[adapter_name] = config
+        self._find_and_replace(adapter_name)
+        if len(self.peft_config) > 1 and self.peft_config[adapter_name].bias != "none":
+            raise ValueError(
+                "LoraModel supports only 1 adapter with bias. When using multiple adapters, set bias to 'none' for all adapters."
+            )
+        mark_only_lora_as_trainable(self.model, self.peft_config[adapter_name].bias)
+        if self.peft_config[adapter_name].inference_mode:
+            _freeze_adapter(self.model, adapter_name)
+
+    def _find_and_replace(self, adapter_name):
+        lora_config = self.peft_config[adapter_name]
         loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
         if loaded_in_8bit and not is_bnb_available():
             raise ImportError(
                 "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
                 "You can install it with `pip install bitsandbytes`."
             )
         is_target_modules_in_base_model = False
         kwargs = {
-            "r": self.peft_config.r,
-            "lora_alpha": self.peft_config.lora_alpha,
-            "lora_dropout": self.peft_config.lora_dropout,
-            "fan_in_fan_out": self.peft_config.fan_in_fan_out,
-            "merge_weights": self.peft_config.merge_weights or self.peft_config.inference_mode,
+            "r": lora_config.r,
+            "lora_alpha": lora_config.lora_alpha,
+            "lora_dropout": lora_config.lora_dropout,
+            "fan_in_fan_out": lora_config.fan_in_fan_out,
+            "init_lora_weights": lora_config.init_lora_weights,
         }
         key_list = [key for key, _ in self.model.named_modules()]
         for key in key_list:
-            if isinstance(self.peft_config.target_modules, str):
-                target_module_found = re.fullmatch(self.peft_config.target_modules, key)
+            if isinstance(lora_config.target_modules, str):
+                target_module_found = re.fullmatch(lora_config.target_modules, key)
             else:
-                target_module_found = any(key.endswith(target_key) for target_key in self.peft_config.target_modules)
+                target_module_found = any(key.endswith(target_key) for target_key in lora_config.target_modules)
             if target_module_found:
                 if not is_target_modules_in_base_model:
                     is_target_modules_in_base_model = True
-                parent, target, target_name = self._get_submodules(key)
-                bias = target.bias is not None
-                if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
-                    kwargs.update(
-                        {
-                            "has_fp16_weights": target.state.has_fp16_weights,
-                            "memory_efficient_backward": target.state.memory_efficient_backward,
-                            "threshold": target.state.threshold,
-                            "index": target.index,
-                        }
+                parent, target, target_name = _get_submodules(self.model, key)
+                if hasattr(target, "bias"):
+                    bias = target.bias is not None
+
+                if isinstance(target, LoraLayer):
+                    target.update_layer(
+                        adapter_name,
+                        lora_config.r,
+                        lora_config.lora_alpha,
+                        lora_config.lora_dropout,
+                        lora_config.init_lora_weights,
                     )
-                    if self.peft_config.enable_lora is None:
-                        new_module = Linear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
-                    else:
-                        kwargs.update({"enable_lora": self.peft_config.enable_lora})
-                        new_module = MergedLinear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
-                elif isinstance(target, torch.nn.Linear) and self.peft_config.enable_lora is None:
-                    new_module = Linear(target.in_features, target.out_features, bias=bias, **kwargs)
-                elif self.peft_config.enable_lora is not None:
-                    kwargs.update({"enable_lora": self.peft_config.enable_lora})
-                    if isinstance(target, Conv1D):
-                        in_features, out_features = (
-                            target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
+                else:
+                    if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
+                        eightbit_kwargs = kwargs.copy()
+                        eightbit_kwargs.update(
+                            {
+                                "has_fp16_weights": target.state.has_fp16_weights,
+                                "memory_efficient_backward": target.state.memory_efficient_backward,
+                                "threshold": target.state.threshold,
+                                "index": target.index,
+                            }
+                        )
+                        new_module = Linear8bitLt(
+                            adapter_name, target.in_features, target.out_features, bias=bias, **eightbit_kwargs
                         )
+                    elif isinstance(target, torch.nn.Embedding):
+                        embedding_kwargs = kwargs.copy()
+                        embedding_kwargs.pop("fan_in_fan_out", None)
+                        in_features, out_features = target.num_embeddings, target.embedding_dim
+                        new_module = Embedding(adapter_name, in_features, out_features, **embedding_kwargs)
                     else:
-                        in_features, out_features = target.in_features, target.out_features
-                        if kwargs["fan_in_fan_out"]:
-                            warnings.warn(
-                                "fan_in_fan_out is set to True but the target module is not a Conv1D. "
-                                "Setting fan_in_fan_out to False."
+                        if isinstance(target, torch.nn.Linear):
+                            in_features, out_features = target.in_features, target.out_features
+                            if kwargs["fan_in_fan_out"]:
+                                warnings.warn(
+                                    "fan_in_fan_out is set to True but the target module is `torch.nn.Linear`. "
+                                    "Setting fan_in_fan_out to False."
+                                )
+                                kwargs["fan_in_fan_out"] = lora_config.fan_in_fan_out = False
+                        elif isinstance(target, Conv1D):
+                            in_features, out_features = (
+                                target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
                             )
-                            kwargs["fan_in_fan_out"] = False
-                    new_module = MergedLinear(in_features, out_features, bias=bias, **kwargs)
-                self._replace_module(parent, target_name, new_module, target)
+                            if not kwargs["fan_in_fan_out"]:
+                                warnings.warn(
+                                    "fan_in_fan_out is set to False but the target module is `Conv1D`. "
+                                    "Setting fan_in_fan_out to True."
+                                )
+                                kwargs["fan_in_fan_out"] = lora_config.fan_in_fan_out = True
+                        else:
+                            raise ValueError(
+                                f"Target module {target} is not supported. "
+                                f"Currently, only `torch.nn.Linear` and `Conv1D` are supported."
+                            )
+                        new_module = Linear(adapter_name, in_features, out_features, bias=bias, **kwargs)
+
+                    self._replace_module(parent, target_name, new_module, target)
         if not is_target_modules_in_base_model:
             raise ValueError(
-                f"Target modules {self.peft_config.target_modules} not found in the base model. "
+                f"Target modules {lora_config.target_modules} not found in the base model. "
                 f"Please check the target modules and try again."
             )
 
-    def _get_submodules(self, key):
-        parent = self.model.get_submodule(".".join(key.split(".")[:-1]))
-        target_name = key.split(".")[-1]
-        target = self.model.get_submodule(key)
-        return parent, target, target_name
-
     def _replace_module(self, parent_module, child_name, new_module, old_module):
         setattr(parent_module, child_name, new_module)
         new_module.weight = old_module.weight
-        if old_module.bias is not None:
-            new_module.bias = old_module.bias
+        if hasattr(old_module, "bias"):
+            if old_module.bias is not None:
+                new_module.bias = old_module.bias
+
         if getattr(old_module, "state", None) is not None:
             new_module.state = old_module.state
             new_module.to(old_module.weight.device)
 
+        # dispatch to correct device
+        for name, module in new_module.named_modules():
+            if "lora_" in name:
+                module.to(old_module.weight.device)
+
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
             return getattr(self.model, name)
 
-    @property
-    def modules_to_save(self):
-        return None
-
     def get_peft_config_as_dict(self, inference: bool = False):
-        config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self.peft_config).items()}
-        if inference:
-            config["inference_mode"] = True
+        config_dict = {}
+        for key, value in self.peft_config.items():
+            config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(value).items()}
+            if inference:
+                config["inference_mode"] = True
+        config_dict[key] = config
         return config
 
     def _set_adapter_layers(self, enabled=True):
         for module in self.model.modules():
             if isinstance(module, LoraLayer):
                 module.disable_adapters = False if enabled else True
 
     def enable_adapter_layers(self):
         self._set_adapter_layers(enabled=True)
 
     def disable_adapter_layers(self):
         self._set_adapter_layers(enabled=False)
 
+    def set_adapter(self, adapter_name):
+        for module in self.model.modules():
+            if isinstance(module, LoraLayer):
+                if module.merged:
+                    warnings.warn("Adapter cannot be set when the model is merged. Unmerging the model first.")
+                    module.unmerge()
+                module.active_adapter = adapter_name
+
+    def merge_adapter(self):
+        for module in self.model.modules():
+            if isinstance(module, LoraLayer):
+                module.merge()
+
+    def unmerge_adapter(self):
+        for module in self.model.modules():
+            if isinstance(module, LoraLayer):
+                module.unmerge()
+
+    @staticmethod
+    def _prepare_lora_config(peft_config, model_config):
+        if peft_config.target_modules is None:
+            if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING:
+                raise ValueError("Please specify `target_modules` in `peft_config`")
+            peft_config.target_modules = TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING[model_config["model_type"]]
+        if peft_config.inference_mode:
+            peft_config.merge_weights = True
+        return peft_config
+
+    def merge_and_unload(self):
+        r"""
+        This method merges the LoRa layers into the base model. This is needed if someone wants to use the base model
+        as a standalone model.
+        """
+        if getattr(self.config, "model_type", None) == "gpt2":
+            raise ValueError("GPT2 models are not supported for merging LORA layers")
+
+        if getattr(self.model, "is_loaded_in_8bit", False):
+            raise ValueError("Cannot merge LORA layers when the model is loaded in 8-bit mode")
+
+        key_list = [key for key, _ in self.model.named_modules() if "lora" not in key]
+        for key in key_list:
+            try:
+                parent, target, target_name = _get_submodules(self.model, key)
+            except AttributeError:
+                continue
+            if isinstance(target, LoraLayer):
+                bias = target.bias is not None
+                new_module = torch.nn.Linear(target.in_features, target.out_features, bias=bias)
+                target.merge()
+                self._replace_module(parent, target_name, new_module, target)
+
+            # save any additional trainable modules part of `modules_to_save`
+            if isinstance(target, ModulesToSaveWrapper):
+                setattr(parent, target_name, target.modules_to_save[target.active_adapter])
+
+        return self.model
+
+    def add_weighted_adapter(self, adapters, weights, adapter_name):
+        if len({self.peft_config[adapter].r for adapter in adapters}) != 1:
+            raise ValueError("All adapters must have the same r value")
+        self.peft_config[adapter_name] = self.peft_config[adapters[0]]
+        self.peft_config[adapter_name].lora_alpha = self.peft_config[adapters[0]].r
+        self._find_and_replace(adapter_name)
+        mark_only_lora_as_trainable(self.model, self.peft_config[adapter_name].bias)
+        _freeze_adapter(self.model, adapter_name)
+        key_list = [key for key, _ in self.model.named_modules() if "lora" not in key]
+        for key in key_list:
+            _, target, _ = _get_submodules(self.model, key)
+            if isinstance(target, LoraLayer):
+                if adapter_name in target.lora_A:
+                    target.lora_A[adapter_name].weight.data = target.lora_A[adapter_name].weight.data * 0.0
+                    target.lora_B[adapter_name].weight.data = target.lora_B[adapter_name].weight.data * 0.0
+                    for adapter, weight in zip(adapters, weights):
+                        if adapter not in target.lora_A:
+                            continue
+                        target.lora_A[adapter_name].weight.data += (
+                            target.lora_A[adapter].weight.data * weight * target.scaling[adapter]
+                        )
+                        target.lora_B[adapter_name].weight.data += target.lora_B[adapter].weight.data * weight
+
+                elif adapter_name in target.lora_embedding_A:
+                    target.lora_embedding_A[adapter_name].data = target.lora_embedding_A[adapter_name].data * 0.0
+                    target.lora_embedding_B[adapter_name].data = target.lora_embedding_B[adapter_name].data * 0.0
+                    for adapter, weight in zip(adapters, weights):
+                        if adapter not in target.lora_embedding_A:
+                            continue
+                        target.lora_embedding_A[adapter_name].data += (
+                            target.lora_embedding_A[adapter].data * weight * target.scaling[adapter]
+                        )
+                        target.lora_embedding_B[adapter_name].data += target.lora_embedding_B[adapter].data * weight
+
 
 # Below code is based on https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
 # and modified to work with PyTorch FSDP
 
 
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
@@ -255,220 +419,259 @@
     else:
         raise NotImplementedError
 
 
 class LoraLayer:
     def __init__(
         self,
-        r: int,
-        lora_alpha: int,
-        lora_dropout: float,
-        merge_weights: bool,
+        in_features: int,
+        out_features: int,
     ):
-        self.r = r
-        self.lora_alpha = lora_alpha
-        # Optional dropout
-        if lora_dropout > 0.0:
-            self.lora_dropout = nn.Dropout(p=lora_dropout)
-        else:
-            self.lora_dropout = lambda x: x
+        self.r = {}
+        self.lora_alpha = {}
+        self.scaling = {}
+        self.lora_dropout = nn.ModuleDict({})
+        self.lora_A = nn.ModuleDict({})
+        self.lora_B = nn.ModuleDict({})
+        # For Embedding layer
+        self.lora_embedding_A = nn.ParameterDict({})
+        self.lora_embedding_B = nn.ParameterDict({})
         # Mark the weight as unmerged
         self.merged = False
-        self.merge_weights = merge_weights
         self.disable_adapters = False
+        self.in_features = in_features
+        self.out_features = out_features
+
+    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights):
+        self.r[adapter_name] = r
+        self.lora_alpha[adapter_name] = lora_alpha
+        if lora_dropout > 0.0:
+            lora_dropout_layer = nn.Dropout(p=lora_dropout)
+        else:
+            lora_dropout_layer = nn.Identity()
+
+        self.lora_dropout.update(nn.ModuleDict({adapter_name: lora_dropout_layer}))
+        # Actual trainable parameters
+        if r > 0:
+            self.lora_A.update(nn.ModuleDict({adapter_name: nn.Linear(self.in_features, r, bias=False)}))
+            self.lora_B.update(nn.ModuleDict({adapter_name: nn.Linear(r, self.out_features, bias=False)}))
+            self.scaling[adapter_name] = lora_alpha / r
+        if init_lora_weights:
+            self.reset_lora_parameters(adapter_name)
+        self.to(self.weight.device)
+
+    def update_layer_embedding(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights):
+        self.r[adapter_name] = r
+        self.lora_alpha[adapter_name] = lora_alpha
+        if lora_dropout > 0.0:
+            lora_dropout_layer = nn.Dropout(p=lora_dropout)
+        else:
+            lora_dropout_layer = nn.Identity()
+
+        self.lora_dropout.update(nn.ModuleDict({adapter_name: lora_dropout_layer}))
+        # Actual trainable parameters
+        if r > 0:
+            self.lora_embedding_A.update(
+                nn.ParameterDict({adapter_name: nn.Parameter(self.weight.new_zeros((r, self.in_features)))})
+            )
+            self.lora_embedding_B.update(
+                nn.ParameterDict({adapter_name: nn.Parameter(self.weight.new_zeros((self.out_features, r)))})
+            )
+            self.scaling[adapter_name] = lora_alpha / r
+        if init_lora_weights:
+            self.reset_lora_parameters(adapter_name)
+        self.to(self.weight.device)
+
+    def reset_lora_parameters(self, adapter_name):
+        if adapter_name in self.lora_A.keys():
+            # initialize A the same way as the default for nn.Linear and B to zero
+            nn.init.kaiming_uniform_(self.lora_A[adapter_name].weight, a=math.sqrt(5))
+            nn.init.zeros_(self.lora_B[adapter_name].weight)
+        if adapter_name in self.lora_embedding_A.keys():
+            # initialize a the same way as the default for nn.linear and b to zero
+            nn.init.zeros_(self.lora_embedding_A[adapter_name])
+            nn.init.normal_(self.lora_embedding_B[adapter_name])
 
 
 class Linear(nn.Linear, LoraLayer):
     # Lora implemented in a dense layer
     def __init__(
         self,
+        adapter_name: str,
         in_features: int,
         out_features: int,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,  # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
-        merge_weights: bool = True,
         **kwargs,
     ):
+        init_lora_weights = kwargs.pop("init_lora_weights", True)
+
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
+        LoraLayer.__init__(self, in_features=in_features, out_features=out_features)
+        # Freezing the pre-trained weight matrix
+        self.weight.requires_grad = False
 
         self.fan_in_fan_out = fan_in_fan_out
-        # Actual trainable parameters
-        if r > 0:
-            self.lora_A = nn.Linear(in_features, r, bias=False)
-            self.lora_B = nn.Linear(r, out_features, bias=False)
-            self.scaling = self.lora_alpha / self.r
-            # Freezing the pre-trained weight matrix
-            self.weight.requires_grad = False
-        self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.T
 
-    def reset_parameters(self):
         nn.Linear.reset_parameters(self)
-        if hasattr(self, "lora_A"):
-            # initialize A the same way as the default for nn.Linear and B to zero
-            nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_B.weight)
+        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+        self.active_adapter = adapter_name
 
-    def train(self, mode: bool = True):
-        nn.Linear.train(self, mode)
-        self.lora_A.train(mode)
-        self.lora_B.train(mode)
-        if not mode and self.merge_weights and not self.merged:
-            # Merge the weights and mark it
-            if self.r > 0:
-                self.weight.data += (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
+    def merge(self):
+        if self.active_adapter not in self.lora_A.keys():
+            return
+        if self.merged:
+            warnings.warn("Already merged. Nothing to do.")
+            return
+        if self.r[self.active_adapter] > 0:
+            self.weight.data += (
+                transpose(
+                    self.lora_B[self.active_adapter].weight @ self.lora_A[self.active_adapter].weight,
+                    self.fan_in_fan_out,
                 )
+                * self.scaling[self.active_adapter]
+            )
             self.merged = True
-        elif self.merge_weights and self.merged:
-            # Make sure that the weights are not merged
-            if self.r > 0:
-                self.weight.data -= (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
+
+    def unmerge(self):
+        if self.active_adapter not in self.lora_A.keys():
+            return
+        if not self.merged:
+            warnings.warn("Already unmerged. Nothing to do.")
+            return
+        if self.r[self.active_adapter] > 0:
+            self.weight.data -= (
+                transpose(
+                    self.lora_B[self.active_adapter].weight @ self.lora_A[self.active_adapter].weight,
+                    self.fan_in_fan_out,
                 )
+                * self.scaling[self.active_adapter]
+            )
             self.merged = False
 
-    def eval(self):
-        nn.Linear.eval(self)
-        self.lora_A.eval()
-        self.lora_B.eval()
-
     def forward(self, x: torch.Tensor):
-        if self.disable_adapters:
-            if self.r > 0 and self.merged:
-                self.weight.data -= (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
-                )
-                self.merged = False
+        previous_dtype = x.dtype
+
+        if self.active_adapter not in self.lora_A.keys():
             return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-        elif self.r > 0 and not self.merged:
+        if self.disable_adapters:
+            if self.r[self.active_adapter] > 0 and self.merged:
+                self.unmerge()
             result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-            if self.r > 0:
-                result += self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
-            return result
+        elif self.r[self.active_adapter] > 0 and not self.merged:
+            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+
+            x = x.to(self.lora_A[self.active_adapter].weight.dtype)
+
+            result += (
+                self.lora_B[self.active_adapter](
+                    self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
+                )
+                * self.scaling[self.active_adapter]
+            )
         else:
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
 
+        result = result.to(previous_dtype)
 
-class MergedLinear(nn.Linear, LoraLayer):
-    # Lora implemented in a dense layer
+        return result
+
+
+class Embedding(nn.Embedding, LoraLayer):
+    # LoRA implemented in a Embedding layer
     def __init__(
         self,
-        in_features: int,
-        out_features: int,
+        adapter_name: str,
+        num_embeddings: int,
+        embedding_dim: int,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
-        enable_lora: List[bool] = [False],
-        fan_in_fan_out: bool = False,
-        merge_weights: bool = True,
         **kwargs,
     ):
-        nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
-        if out_features % len(enable_lora) != 0:
-            raise ValueError("The length of enable_lora must divide out_features")
-        self.enable_lora = enable_lora
-        self.fan_in_fan_out = fan_in_fan_out
-        # Actual trainable parameters
-        if r > 0 and any(enable_lora):
-            self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
-            self.lora_B = nn.Conv1d(
-                r * sum(enable_lora),
-                out_features // len(enable_lora) * sum(enable_lora),
-                kernel_size=1,
-                groups=2,
-                bias=False,
-            )
-            self.scaling = self.lora_alpha / self.r
-            # Freezing the pre-trained weight matrix
-            self.weight.requires_grad = False
-            # Compute the indices
-            self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
-            self.lora_ind[enable_lora, :] = True
-            self.lora_ind = self.lora_ind.view(-1)
-        self.reset_parameters()
-        if fan_in_fan_out:
-            self.weight.data = self.weight.data.T
+        init_lora_weights = kwargs.pop("init_lora_weights", True)
 
-    def reset_parameters(self):
-        nn.Linear.reset_parameters(self)
-        if hasattr(self, "lora_A"):
-            # initialize A the same way as the default for nn.Linear and B to zero
-            nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_B.weight)
+        nn.Embedding.__init__(self, num_embeddings, embedding_dim, **kwargs)
+        LoraLayer.__init__(self, in_features=num_embeddings, out_features=embedding_dim)
 
-    def zero_pad(self, x):
-        result = x.new_zeros((*x.shape[:-1], self.out_features))
-        result = result.view(-1, self.out_features)
-        result[:, self.lora_ind] = x.reshape(-1, self.out_features // len(self.enable_lora) * sum(self.enable_lora))
-        return result.view((*x.shape[:-1], self.out_features))
-
-    def train(self, mode: bool = True):
-        nn.Linear.train(self, mode)
-        self.lora_A.train(mode)
-        self.lora_B.train(mode)
-        if not mode and self.merge_weights and not self.merged:
-            # Merge the weights and mark it
-            if self.r > 0 and any(self.enable_lora):
-                delta_w = F.conv1d(
-                    self.lora_A.weight.data.unsqueeze(0),
-                    self.lora_B.weight.data.unsqueeze(-1),
-                    groups=sum(self.enable_lora),
-                ).squeeze(0)
-                self.weight.data += self.zero_pad(transpose(delta_w * self.scaling, self.fan_in_fan_out))
-            self.merged = True
-        elif self.merge_weights and self.merged:
-            # Make sure that the weights are not merged
-            if self.r > 0 and any(self.enable_lora):
-                delta_w = F.conv1d(
-                    self.lora_A.weight.data.unsqueeze(0),
-                    self.lora_B.weight.data.unsqueeze(-1),
-                    groups=sum(self.enable_lora),
-                ).squeeze(0)
-                self.weight.data -= self.zero_pad(transpose(delta_w * self.scaling, self.fan_in_fan_out))
+        self.weight.requires_grad = False
+
+        nn.Embedding.reset_parameters(self)
+        self.update_layer_embedding(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+        self.active_adapter = adapter_name
+
+    def unmerge(self, mode: bool = True):
+        if not self.merged:
+            warnings.warn("Already unmerged. Nothing to do.")
+            return
+        if self.r[self.active_adapter] > 0:
+            self.weight.data -= (
+                transpose(
+                    self.lora_embedding_B[self.active_adapter] @ self.lora_embedding_A[self.active_adapter], True
+                )
+                * self.scaling[self.active_adapter]
+            )
             self.merged = False
 
-    def eval(self):
-        nn.Linear.eval(self)
-        self.lora_A.eval()
-        self.lora_B.eval()
+    def merge(self):
+        if self.merged:
+            warnings.warn("Already merged. Nothing to do.")
+            return
+        if self.r[self.active_adapter] > 0:
+            self.weight.data += (
+                transpose(
+                    self.lora_embedding_B[self.active_adapter] @ self.lora_embedding_A[self.active_adapter], True
+                )
+                * self.scaling[self.active_adapter]
+            )
+            self.merged = True
 
     def forward(self, x: torch.Tensor):
         if self.disable_adapters:
-            if self.r > 0 and self.merged and any(self.enable_lora):
-                delta_w = F.conv1d(
-                    self.lora_A.weight.data.unsqueeze(0),
-                    self.lora_B.weight.data.unsqueeze(-1),
-                    groups=sum(self.enable_lora),
-                ).squeeze(0)
-                self.weight.data -= self.zero_pad(transpose(delta_w * self.scaling, self.fan_in_fan_out))
+            if self.r[self.active.adapter] > 0 and self.merged:
+                self.weight.data -= (
+                    transpose(
+                        self.lora_embedding_B[self.active_adapter].weight
+                        @ self.lora_embedding_A[self.active_adapter].weight,
+                        True,
+                    )
+                    * self.scaling[self.active_adapter]
+                )
                 self.merged = False
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-        elif self.merged:
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-        else:
-            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-            if self.r > 0:
-                after_A = self.lora_A(self.lora_dropout(x))
-                after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
-                result += self.zero_pad(after_B) * self.scaling
+            return nn.Embedding.forward(self, x)
+
+        elif self.r[self.active_adapter] > 0 and not self.merged:
+            result = nn.Embedding.forward(self, x)
+            if self.r[self.active_adapter] > 0:
+                after_A = F.embedding(
+                    x,
+                    self.lora_embedding_A[self.active_adapter].T,
+                    self.padding_idx,
+                    self.max_norm,
+                    self.norm_type,
+                    self.scale_grad_by_freq,
+                    self.sparse,
+                )
+                result += (after_A @ self.lora_embedding_B[self.active_adapter].T) * self.scaling[self.active_adapter]
             return result
+        else:
+            return nn.Embedding.forward(self, x)
 
 
 if is_bnb_available():
 
     class Linear8bitLt(bnb.nn.Linear8bitLt, LoraLayer):
         # Lora implemented in a dense layer
         def __init__(
             self,
+            adapter_name,
             in_features,
             out_features,
             r: int = 0,
             lora_alpha: int = 1,
             lora_dropout: float = 0.0,
             **kwargs,
         ):
@@ -478,119 +681,42 @@
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
                 memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
-            # Actual trainable parameters
-            if r > 0:
-                self.lora_A = nn.Linear(in_features, r, bias=False)
-                self.lora_B = nn.Linear(r, out_features, bias=False)
-                self.scaling = self.lora_alpha / self.r
-                # Freezing the pre-trained weight matrix
-                self.weight.requires_grad = False
-            self.reset_parameters()
-
-        def reset_parameters(self):
-            if hasattr(self, "lora_A"):
-                # initialize A the same way as the default for nn.Linear and B to zero
-                nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
-                nn.init.zeros_(self.lora_B.weight)
+            LoraLayer.__init__(self, in_features=in_features, out_features=out_features)
 
-        def forward(self, x: torch.Tensor):
-            result = super().forward(x)
-
-            if self.disable_adapters:
-                return result
-            elif self.r > 0:
-                if not torch.is_autocast_enabled():
-                    expected_dtype = result.dtype
-
-                    if x.dtype != torch.float32:
-                        x = x.float()
-                    output = self.lora_B(self.lora_A(self.lora_dropout(x))).to(expected_dtype) * self.scaling
-                    result += output
-                else:
-                    output = self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
-                    result += output
-            return result
+            # Freezing the pre-trained weight matrix
+            self.weight.requires_grad = False
 
-    class MergedLinear8bitLt(bnb.nn.Linear8bitLt, LoraLayer):
-        # Lora implemented in a dense layer
-        def __init__(
-            self,
-            in_features: int,
-            out_features: int,
-            r: int = 0,
-            lora_alpha: int = 1,
-            lora_dropout: float = 0.0,
-            enable_lora: List[bool] = [False],
-            **kwargs,
-        ):
-            bnb.nn.Linear8bitLt.__init__(
-                self,
-                in_features,
-                out_features,
-                bias=kwargs.get("bias", True),
-                has_fp16_weights=kwargs.get("has_fp16_weights", True),
-                memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
-                threshold=kwargs.get("threshold", 0.0),
-                index=kwargs.get("index", None),
-            )
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
-            if out_features % len(enable_lora) != 0:
-                raise ValueError("The length of enable_lora must divide out_features")
-            self.enable_lora = enable_lora
-            # Actual trainable parameters
-            if r > 0 and any(enable_lora):
-                self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
-                self.lora_B = nn.Conv1d(
-                    r * sum(enable_lora),
-                    out_features // len(enable_lora) * sum(enable_lora),
-                    kernel_size=1,
-                    groups=2,
-                    bias=False,
-                )
-                self.scaling = self.lora_alpha / self.r
-                # Freezing the pre-trained weight matrix
-                self.weight.requires_grad = False
-                # Compute the indices
-                self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
-                self.lora_ind[enable_lora, :] = True
-                self.lora_ind = self.lora_ind.view(-1)
-            self.reset_parameters()
-
-        def reset_parameters(self):
-            if hasattr(self, "lora_A"):
-                # initialize A the same way as the default for nn.Linear and B to zero
-                nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
-                nn.init.zeros_(self.lora_B.weight)
-
-        def zero_pad(self, x):
-            result = x.new_zeros((*x.shape[:-1], self.out_features))
-            result = result.view(-1, self.out_features)
-            result[:, self.lora_ind] = x.reshape(
-                -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
-            )
-            return result.view((*x.shape[:-1], self.out_features))
+            init_lora_weights = kwargs.pop("init_lora_weights", True)
+            self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+            self.active_adapter = adapter_name
 
         def forward(self, x: torch.Tensor):
             result = super().forward(x)
-            if self.disable_adapters:
+
+            if self.disable_adapters or self.active_adapter not in self.lora_A.keys():
                 return result
-            elif self.r > 0:
+            elif self.r[self.active_adapter] > 0:
                 if not torch.is_autocast_enabled():
                     expected_dtype = result.dtype
+
                     if x.dtype != torch.float32:
                         x = x.float()
-                    after_A = self.lora_A(self.lora_dropout(x))
-                    after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
-                    output = self.zero_pad(after_B).to(expected_dtype) * self.scaling
-                    result += output
+                    output = (
+                        self.lora_B[self.active_adapter](
+                            self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
+                        ).to(expected_dtype)
+                        * self.scaling[self.active_adapter]
+                    )
                 else:
-                    after_A = self.lora_A(self.lora_dropout(x))
-                    after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
-                    output = self.zero_pad(after_B) * self.scaling
-                    result += output
+                    output = (
+                        self.lora_B[self.active_adapter](
+                            self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
+                        )
+                        * self.scaling[self.active_adapter]
+                    )
+                result += output
             return result
```

### Comparing `peft-0.2.0/src/peft/tuners/p_tuning.py` & `peft-0.3.0/src/peft/tuners/p_tuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     MLP = "MLP"
     LSTM = "LSTM"
 
 
 @dataclass
 class PromptEncoderConfig(PromptLearningConfig):
     """
-    This is the configuration class to store the configuration of a [`~peft.PromptEncoder`].
+    This is the configuration class to store the configuration of a [`PromptEncoder`].
 
     Args:
-        encoder_reparameterization_type
-            (Union[[`PromptEncoderReparameterizationType`], `str`]): The type of reparameterization to use.
+        encoder_reparameterization_type (Union[[`PromptEncoderReparameterizationType`], `str`]):
+            The type of reparameterization to use.
         encoder_hidden_size (`int`): The hidden size of the prompt encoder.
         encoder_num_layers (`int`): The number of layers of the prompt encoder.
         encoder_dropout (`float`): The dropout probability of the prompt encoder.
     """
 
     encoder_reparameterization_type: Union[str, PromptEncoderReparameterizationType] = field(
         default=PromptEncoderReparameterizationType.MLP,
@@ -67,41 +67,52 @@
 class PromptEncoder(torch.nn.Module):
     """
     The prompt encoder network that is used to generate the virtual token embeddings for p-tuning.
 
     Args:
         config ([`PromptEncoderConfig`]): The configuration of the prompt encoder.
 
-    Example::
+    Example:
 
-        >>> from peft import PromptEncoder, PromptEncoderConfig >>> config = PromptEncoderConfig(
-                peft_type="P_TUNING", task_type="SEQ_2_SEQ_LM", num_virtual_tokens=20, token_dim=768,
-                num_transformer_submodules=1, num_attention_heads=12, num_layers=12,
-                encoder_reparameterization_type="MLP", encoder_hidden_size=768
-            )
-        >>> prompt_encoder = PromptEncoder(config)
+    ```py
+    >>> from peft import PromptEncoder, PromptEncoderConfig
+
+    >>> config = PromptEncoderConfig(
+    ...     peft_type="P_TUNING",
+    ...     task_type="SEQ_2_SEQ_LM",
+    ...     num_virtual_tokens=20,
+    ...     token_dim=768,
+    ...     num_transformer_submodules=1,
+    ...     num_attention_heads=12,
+    ...     num_layers=12,
+    ...     encoder_reparameterization_type="MLP",
+    ...     encoder_hidden_size=768,
+    ... )
+
+    >>> prompt_encoder = PromptEncoder(config)
+    ```
 
     **Attributes**:
-        - **embedding** ([`~torch.nn.Embedding`]) -- The embedding layer of the prompt encoder.
-        - **mlp_head** ([`~torch.nn.Sequential`]) -- The MLP head of the prompt encoder if `inference_mode=False`.
-        - **lstm_head** ([`~torch.nn.LSTM`]) -- The LSTM head of the prompt encoder if `inference_mode=False` and
+        - **embedding** (`torch.nn.Embedding`) -- The embedding layer of the prompt encoder.
+        - **mlp_head** (`torch.nn.Sequential`) -- The MLP head of the prompt encoder if `inference_mode=False`.
+        - **lstm_head** (`torch.nn.LSTM`) -- The LSTM head of the prompt encoder if `inference_mode=False` and
         `encoder_reparameterization_type="LSTM"`.
         - **token_dim** (`int`) -- The hidden embedding dimension of the base transformer model.
         - **input_size** (`int`) -- The input size of the prompt encoder.
         - **output_size** (`int`) -- The output size of the prompt encoder.
         - **hidden_size** (`int`) -- The hidden size of the prompt encoder.
         - **total_virtual_tokens** (`int`): The total number of virtual tokens of the
         prompt encoder.
-        - **encoder_type** (Union[[`PromptEncoderReparameterizationType`], `str`]):
-            The encoder type of the prompt encoder.
+        - **encoder_type** (Union[[`PromptEncoderReparameterizationType`], `str`]): The encoder type of the prompt
+          encoder.
 
 
-    Input shape: (batch_size, total_virtual_tokens)
+    Input shape: (`batch_size`, `total_virtual_tokens`)
 
-    Output shape: (batch_size, total_virtual_tokens, token_dim)
+    Output shape: (`batch_size`, `total_virtual_tokens`, `token_dim`)
     """
 
     def __init__(self, config):
         super().__init__()
         self.token_dim = config.token_dim
         self.input_size = self.token_dim
         self.output_size = self.token_dim
```

### Comparing `peft-0.2.0/src/peft/tuners/prefix_tuning.py` & `peft-0.3.0/src/peft/tuners/prefix_tuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from ..utils import PeftType, PromptLearningConfig
 
 
 @dataclass
 class PrefixTuningConfig(PromptLearningConfig):
     """
-    This is the configuration class to store the configuration of a [`~peft.PrefixEncoder`].
+    This is the configuration class to store the configuration of a [`PrefixEncoder`].
 
     Args:
         encoder_hidden_size (`int`): The hidden size of the prompt encoder.
         prefix_projection (`bool`): Whether to project the prefix embeddings.
     """
 
     encoder_hidden_size: int = field(
@@ -44,38 +44,46 @@
         self.peft_type = PeftType.PREFIX_TUNING
 
 
 # Based on https://github.com/THUDM/P-tuning-v2/blob/main/model/prefix_encoder.py
 # with some refactor
 class PrefixEncoder(torch.nn.Module):
     r"""
-    The torch.nn model to encode the prefix
+    The `torch.nn` model to encode the prefix.
 
     Args:
         config ([`PrefixTuningConfig`]): The configuration of the prefix encoder.
 
-    Example::
+    Example:
 
-        >>> from peft import PrefixEncoder, PrefixTuningConfig >>> config = PrefixTuningConfig(
-                peft_type="PREFIX_TUNING", task_type="SEQ_2_SEQ_LM", num_virtual_tokens=20, token_dim=768,
-                num_transformer_submodules=1, num_attention_heads=12, num_layers=12, encoder_hidden_size=768
-            )
-        >>> prefix_encoder = PrefixEncoder(config)
+    ```py
+    >>> from peft import PrefixEncoder, PrefixTuningConfig
 
+    >>> config = PrefixTuningConfig(
+    ...     peft_type="PREFIX_TUNING",
+    ...     task_type="SEQ_2_SEQ_LM",
+    ...     num_virtual_tokens=20,
+    ...     token_dim=768,
+    ...     num_transformer_submodules=1,
+    ...     num_attention_heads=12,
+    ...     num_layers=12,
+    ...     encoder_hidden_size=768,
+    ... )
+    >>> prefix_encoder = PrefixEncoder(config)
+    ```
 
     **Attributes**:
-        - **embedding** (`torch.nn.Embedding`) --
-            The embedding layer of the prefix encoder.
-        - **transform** (`torch.nn.Sequential`) -- The
-        two-layer MLP to transform the prefix embeddings if `prefix_projection` is `True`.
+        - **embedding** (`torch.nn.Embedding`) -- The embedding layer of the prefix encoder.
+        - **transform** (`torch.nn.Sequential`) -- The two-layer MLP to transform the prefix embeddings if
+          `prefix_projection` is `True`.
         - **prefix_projection** (`bool`) -- Whether to project the prefix embeddings.
 
-    Input shape: (batch_size, num_virtual_tokens)
+    Input shape: (`batch_size`, `num_virtual_tokens`)
 
-    Output shape: (batch_size, num_virtual_tokens, 2*layers*hidden)
+    Output shape: (`batch_size`, `num_virtual_tokens`, `2*layers*hidden`)
     """
 
     def __init__(self, config):
         super().__init__()
         self.prefix_projection = config.prefix_projection
         token_dim = config.token_dim
         num_layers = config.num_layers
```

### Comparing `peft-0.2.0/src/peft/tuners/prompt_tuning.py` & `peft-0.3.0/src/peft/tuners/prompt_tuning.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     TEXT = "TEXT"
     RANDOM = "RANDOM"
 
 
 @dataclass
 class PromptTuningConfig(PromptLearningConfig):
     """
-    This is the configuration class to store the configuration of a [`~peft.PromptEmbedding`].
+    This is the configuration class to store the configuration of a [`PromptEmbedding`].
 
     Args:
         prompt_tuning_init (Union[[`PromptTuningInit`], `str`]): The initialization of the prompt embedding.
-        prompt_tuning_init_text ( Optional[`str`]): The text to initialize the prompt embedding.
-            Only used if `prompt_tuning_init` is `TEXT`
-        tokenizer_name_or_path ( Optional[`str`]): The name or path of the tokenizer.
-            Only used if `prompt_tuning_init` is `TEXT`
+        prompt_tuning_init_text (`str`, *optional*):
+            The text to initialize the prompt embedding. Only used if `prompt_tuning_init` is `TEXT`.
+        tokenizer_name_or_path (`str`, *optional*):
+            The name or path of the tokenizer. Only used if `prompt_tuning_init` is `TEXT`.
     """
 
     prompt_tuning_init: Union[PromptTuningInit, str] = field(
         default=PromptTuningInit.RANDOM,
         metadata={"help": "How to initialize the prompt tuning parameters"},
     )
     prompt_tuning_init_text: Optional[str] = field(
@@ -67,31 +67,41 @@
     The model to encode virtual tokens into prompt embeddings.
 
     Args:
         config ([`PromptTuningConfig`]): The configuration of the prompt embedding.
         word_embeddings (`torch.nn.Module`): The word embeddings of the base transformer model.
 
     **Attributes**:
-        **embedding** (`torch.nn.Embedding`) -- The embedding layer of the prompt embedding.
+        - **embedding** (`torch.nn.Embedding`) -- The embedding layer of the prompt embedding.
 
-    Example::
+    Example:
 
-        >>> from peft import PromptEmbedding, PromptTuningConfig >>> config = PromptTuningConfig(
-                peft_type="PROMPT_TUNING", task_type="SEQ_2_SEQ_LM", num_virtual_tokens=20, token_dim=768,
-                num_transformer_submodules=1, num_attention_heads=12, num_layers=12, prompt_tuning_init="TEXT",
-                prompt_tuning_init_text="Predict if sentiment of this review is positive, negative or neutral",
-                tokenizer_name_or_path="t5-base",
-            )
-        >>> # t5_model.shared is the word embeddings of the base model >>> prompt_embedding = PromptEmbedding(config,
-        t5_model.shared)
+    ```py
+    >>> from peft import PromptEmbedding, PromptTuningConfig
 
+    >>> config = PromptTuningConfig(
+    ...     peft_type="PROMPT_TUNING",
+    ...     task_type="SEQ_2_SEQ_LM",
+    ...     num_virtual_tokens=20,
+    ...     token_dim=768,
+    ...     num_transformer_submodules=1,
+    ...     num_attention_heads=12,
+    ...     num_layers=12,
+    ...     prompt_tuning_init="TEXT",
+    ...     prompt_tuning_init_text="Predict if sentiment of this review is positive, negative or neutral",
+    ...     tokenizer_name_or_path="t5-base",
+    ... )
+
+    >>> # t5_model.shared is the word embeddings of the base model
+    >>> prompt_embedding = PromptEmbedding(config, t5_model.shared)
+    ```
 
-    Input Shape: (batch_size, total_virtual_tokens)
+    Input Shape: (`batch_size`, `total_virtual_tokens`)
 
-    Output Shape: (batch_size, total_virtual_tokens, token_dim)
+    Output Shape: (`batch_size`, `total_virtual_tokens`, `token_dim`)
     """
 
     def __init__(self, config, word_embeddings):
         super().__init__()
 
         total_virtual_tokens = config.num_virtual_tokens * config.num_transformer_submodules
         self.embedding = torch.nn.Embedding(total_virtual_tokens, config.token_dim)
```

### Comparing `peft-0.2.0/src/peft/utils/__init__.py` & `peft-0.3.0/src/peft/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .adapters_utils import CONFIG_NAME, WEIGHTS_NAME
 from .config import PeftConfig, PeftType, PromptLearningConfig, TaskType
 from .other import (
     TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
+    TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING,
+    CONFIG_NAME,
+    WEIGHTS_NAME,
     _set_trainable,
     bloom_model_postprocess_past_key_value,
     prepare_model_for_int8_training,
     shift_tokens_right,
     transpose,
+    _get_submodules,
+    _set_adapter,
+    _freeze_adapter,
+    ModulesToSaveWrapper,
 )
 from .save_and_load import get_peft_model_state_dict, set_peft_model_state_dict
```

### Comparing `peft-0.2.0/src/peft/utils/adapters_utils.py` & `peft-0.3.0/src/peft/import_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-WEIGHTS_NAME = "adapter_model.bin"
-CONFIG_NAME = "adapter_config.json"
+import importlib
 
-# TODO: add automapping and superclass here?
+
+def is_bnb_available():
+    return importlib.util.find_spec("bitsandbytes") is not None
```

### Comparing `peft-0.2.0/src/peft/utils/config.py` & `peft-0.3.0/src/peft/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,36 +17,38 @@
 import os
 from dataclasses import asdict, dataclass, field
 from typing import Optional, Union
 
 from huggingface_hub import hf_hub_download
 from transformers.utils import PushToHubMixin
 
-from .adapters_utils import CONFIG_NAME
+from .other import CONFIG_NAME
 
 
 class PeftType(str, enum.Enum):
     PROMPT_TUNING = "PROMPT_TUNING"
     P_TUNING = "P_TUNING"
     PREFIX_TUNING = "PREFIX_TUNING"
     LORA = "LORA"
+    ADALORA = "ADALORA"
+    ADAPTION_PROMPT = "ADAPTION_PROMPT"
 
 
 class TaskType(str, enum.Enum):
     SEQ_CLS = "SEQ_CLS"
     SEQ_2_SEQ_LM = "SEQ_2_SEQ_LM"
     CAUSAL_LM = "CAUSAL_LM"
     TOKEN_CLS = "TOKEN_CLS"
 
 
 @dataclass
 class PeftConfigMixin(PushToHubMixin):
     r"""
     This is the base configuration class for PEFT adapter models. It contains all the methods that are common to all
-    PEFT adapter models. This class inherits from `transformers.utils.PushToHubMixin` which contains the methods to
+    PEFT adapter models. This class inherits from [`~transformers.utils.PushToHubMixin`] which contains the methods to
     push your model to the Hub. The method `save_pretrained` will save the configuration of your adapter model in a
     directory. The method `from_pretrained` will load the configuration of your adapter model from a directory.
 
     Args:
         peft_type (Union[[`~peft.utils.config.PeftType`], `str`]): The type of Peft method to use.
     """
     peft_type: Optional[PeftType] = field(default=None, metadata={"help": "The type of PEFT model."})
@@ -61,16 +63,16 @@
     def save_pretrained(self, save_directory, **kwargs):
         r"""
         This method saves the configuration of your adapter model in a directory.
 
         Args:
             save_directory (`str`):
                 The directory where the configuration will be saved.
-            **kwargs:
-                Additional keyword arguments passed along to the `transformers.utils.PushToHubMixin.push_to_hub`
+            kwargs (additional keyword arguments, *optional*):
+                Additional keyword arguments passed along to the [`~transformers.utils.PushToHubMixin.push_to_hub`]
                 method.
         """
         if os.path.isfile(save_directory):
             raise AssertionError(f"Provided path ({save_directory}) should be a directory, not a file")
 
         os.makedirs(save_directory, exist_ok=True)
 
@@ -78,31 +80,36 @@
         output_path = os.path.join(save_directory, CONFIG_NAME)
 
         # save it
         with open(output_path, "w") as writer:
             writer.write(json.dumps(output_dict, indent=2, sort_keys=True))
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_name_or_path, **kwargs):
+    def from_pretrained(cls, pretrained_model_name_or_path, subfolder=None, **kwargs):
         r"""
         This method loads the configuration of your adapter model from a directory.
 
         Args:
             pretrained_model_name_or_path (`str`):
-                The directory or the hub-id where the configuration is saved.
-            **kwargs:
+                The directory or the Hub repository id where the configuration is saved.
+            kwargs (additional keyword arguments, *optional*):
                 Additional keyword arguments passed along to the child class initialization.
         """
-        if os.path.isfile(os.path.join(pretrained_model_name_or_path, CONFIG_NAME)):
-            config_file = os.path.join(pretrained_model_name_or_path, CONFIG_NAME)
+        path = (
+            os.path.join(pretrained_model_name_or_path, subfolder)
+            if subfolder is not None
+            else pretrained_model_name_or_path
+        )
+        if os.path.isfile(os.path.join(path, CONFIG_NAME)):
+            config_file = os.path.join(path, CONFIG_NAME)
         else:
             try:
-                config_file = hf_hub_download(pretrained_model_name_or_path, CONFIG_NAME)
+                config_file = hf_hub_download(pretrained_model_name_or_path, CONFIG_NAME, subfolder=subfolder)
             except Exception:
-                raise ValueError(f"Can't find config.json at '{pretrained_model_name_or_path}'")
+                raise ValueError(f"Can't find '{CONFIG_NAME}' at '{pretrained_model_name_or_path}'")
 
         loaded_attributes = cls.from_json_file(config_file)
 
         config = cls(**kwargs)
 
         for key, value in loaded_attributes.items():
             if hasattr(config, key):
@@ -124,15 +131,15 @@
 
         return json_object
 
 
 @dataclass
 class PeftConfig(PeftConfigMixin):
     """
-    This is the base configuration class to store the configuration of a :class:`~peft.PeftModel`.
+    This is the base configuration class to store the configuration of a [`PeftModel`].
 
     Args:
         peft_type (Union[[`~peft.utils.config.PeftType`], `str`]): The type of Peft method to use.
         task_type (Union[[`~peft.utils.config.TaskType`], `str`]): The type of task to perform.
         inference_mode (`bool`, defaults to `False`): Whether to use the Peft model in inference mode.
     """
 
@@ -141,16 +148,16 @@
     task_type: Union[str, TaskType] = field(default=None, metadata={"help": "Task type"})
     inference_mode: bool = field(default=False, metadata={"help": "Whether to use inference mode"})
 
 
 @dataclass
 class PromptLearningConfig(PeftConfig):
     """
-    This is the base configuration class to store the configuration of a Union[[`~peft.PrefixTuning`],
-    [`~peft.PromptEncoder`], [`~peft.PromptTuning`]].
+    This is the base configuration class to store the configuration of [`PrefixTuning`], [`PromptEncoder`], or
+    [`PromptTuning`].
 
     Args:
         num_virtual_tokens (`int`): The number of virtual tokens to use.
         token_dim (`int`): The hidden embedding dimension of the base transformer model.
         num_transformer_submodules (`int`): The number of transformer submodules in the base transformer model.
         num_attention_heads (`int`): The number of attention heads in the base transformer model.
         num_layers (`int`): The number of layers in the base transformer model.
```

### Comparing `peft-0.2.0/src/peft.egg-info/PKG-INFO` & `peft-0.3.0/src/peft.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peft
-Version: 0.2.0
+Version: 0.3.0
 Summary: Parameter-Efficient Fine-Tuning (PEFT)
 Home-page: https://github.com/huggingface/peft
 Author: The HuggingFace team
 Author-email: sourab@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: docs_specific
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
@@ -47,18 +48,19 @@
 
 Parameter-Efficient Fine-Tuning (PEFT) methods enable efficient adaptation of pre-trained language models (PLMs) to various downstream applications without fine-tuning all the model's parameters. Fine-tuning large-scale PLMs is often prohibitively costly. In this regard, PEFT methods only fine-tune a small number of (extra) model parameters, thereby greatly decreasing the computational and storage costs. Recent State-of-the-Art PEFT techniques achieve performance comparable to that of full fine-tuning. 
 
 Seamlessly integrated with 🤗 Accelerate for large scale models leveraging DeepSpeed and Big Model Inference. 
 
 Supported methods:
 
-1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2106.09685.pdf)
+1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
-3. P-Tuning: [GPT Understands, Too](https://arxiv.org/pdf/2103.10385.pdf)
-4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/pdf/2104.08691.pdf) 
+3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
+4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
+5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -86,38 +88,40 @@
 |   Model         | Full Finetuning | PEFT-LoRA PyTorch  | PEFT-LoRA DeepSpeed with CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | bigscience/T0_3B (3B params) | 47.14GB GPU / 2.96GB CPU  | 14.4GB GPU / 2.96GB CPU | 9.8GB GPU / 17.8GB CPU |
 | bigscience/mt0-xxl (12B params) | OOM GPU | 56GB GPU / 3GB CPU | 22GB GPU / 52GB CPU |
 | bigscience/bloomz-7b1 (7B params) | OOM GPU | 32GB GPU / 3.8GB CPU | 18.1GB GPU / 35GB CPU |
 
 Performance of PEFT-LoRA tuned [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) on [`ought/raft/twitter_complaints`](https://huggingface.co/datasets/ought/raft/viewer/twitter_complaints) leaderboard. 
-A point to note is that we didn't try to sequeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
+A point to note is that we didn't try to squeeze performance by playing around with input instruction templates, LoRA hyperparams and other training related hyperparams. Also, we didn't use the larger 13B [mt0-xxl](https://huggingface.co/bigscience/mt0-xxl) model.
 So, we are already seeing comparable performance to SoTA with parameter efficient tuning. Also, the final checkpoint size is just `19MB` in comparison to `11GB` size of the backbone [`bigscience/T0_3B`](https://huggingface.co/bigscience/T0_3B) model.
 
 |   Submission Name        | Accuracy |
 | --------- | ---- |
 | Human baseline (crowdsourced) |	0.897 |
 | Flan-T5 | 0.892 |
 | lora-t0-3b | 0.863 |
 
 **Therefore, we can see that performance comparable to SoTA is achievable by PEFT methods with consumer hardware such as 16GB and 24GB GPUs.**
 
+An insightful blogpost explaining the advantages of using PEFT for fine-tuning FlanT5-XXL: [https://www.philschmid.de/fine-tune-flan-t5-peft](https://www.philschmid.de/fine-tune-flan-t5-peft)
+
 ### Parameter Efficient Tuning of Diffusion Models
 
 GPU memory required by different settings during training is given below. The final checkpoint size is `8.8 MB`.
 
 Hardware: Single A100 80GB GPU with CPU RAM above 64GB
 
-|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpoitning  |
+|   Model         | Full Finetuning | PEFT-LoRA  | PEFT-LoRA with Gradient Checkpointing  |
 | --------- | ---- | ---- | ---- |
 | CompVis/stable-diffusion-v1-4 | 27.5GB GPU / 3.97GB CPU | 15.5GB GPU / 3.84GB CPU | 8.12GB GPU / 3.77GB CPU | 
 
 
 **Training**
-An example of using LoRA for parameter efficient dreambooth training is given in `~examples/lora_dreambooth/train_dreambooth.py`
+An example of using LoRA for parameter efficient dreambooth training is given in [`examples/lora_dreambooth/train_dreambooth.py`](examples/lora_dreambooth/train_dreambooth.py)
 
 ```bash
 export MODEL_NAME= "CompVis/stable-diffusion-v1-4" #"stabilityai/stable-diffusion-2-1"
 export INSTANCE_DIR="path-to-instance-images"
 export CLASS_DIR="path-to-class-images"
 export OUTPUT_DIR="path-to-save-model"
 
@@ -147,38 +151,41 @@
 ```
 
 Try out the 🤗 Gradio Space which should run seamlessly on a T4 instance:
 [smangrul/peft-lora-sd-dreambooth](https://huggingface.co/spaces/smangrul/peft-lora-sd-dreambooth).
 
 ![peft lora dreambooth gradio space](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/peft_lora_dreambooth_gradio_space.png)
 
+**NEW** ✨ Multi Adapter support and combining multiple LoRA adapters in a weighted combination 
+![peft lora dreambooth weighted adapter](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/peft/weighted_adapter_dreambooth_lora.png)
+
 ### Parameter Efficient Tuning of LLMs for RLHF components such as Ranker and Policy
-- Here is an exmaple in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) 
-- Example using PEFT for both reward model and policy [ToDo]
+- Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
+- Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
-- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
+- Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
 An example of using LoRA for the task of adapting `LayoutLMForTokenClassification` on `FUNSD` dataset is given in `~examples/token_classification/PEFT_LoRA_LayoutLMForTokenClassification_on_FUNSD.py`. We can observe that with only `0.62 %` of parameters being trainable, we achieve performance (F1 0.777) comparable to full finetuning (F1 0.786) (without any hyerparam tuning runs for extracting more performance), and the checkpoint of this is only `2.8MB`. Now, if there are `N` such datasets, just have these PEFT models one for each dataset and save a lot of storage without having to worry about the problem of catastrophic forgetting or overfitting of backbone/base model.
 
-Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset suing differenct PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
+Another example is fine-tuning [`roberta-large`](https://huggingface.co/roberta-large) on [`MRPC` GLUE](https://huggingface.co/datasets/glue/viewer/mrpc) dataset using different PEFT methods. The notebooks are given in `~examples/sequence_classification`. 
 
 
 ## PEFT + 🤗 Accelerate
 
-PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices etc during training.
+PEFT models work with 🤗 Accelerate out of the box. Use 🤗 Accelerate for Distributed training on various hardware such as GPUs, Apple Silicon devices, etc during training.
 Use 🤗 Accelerate for inferencing on consumer hardware with small resources.
 
 ### Example of PEFT model training using 🤗 Accelerate's DeepSpeed integration
 
 DeepSpeed version required `v0.8.0`. An example is provided in `~examples/conditional_generation/peft_lora_seq2seq_accelerate_ds_zero3_offload.py`. 
   a. First, run `accelerate config --config_file ds_zero3_cpu.yaml` and answer the questionnaire. 
   Below are the contents of the config file.
@@ -239,22 +246,24 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-| --------- | ---- | ---- | ---- | ----  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  |
-| Bloom          | ✅  | ✅  | ✅  | ✅  |
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B   | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
+|--------------| ---- | ---- | ---- | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ---- |
 | T5        | ✅   | ✅   | ✅   | ✅   |
 | BART      | ✅   | ✅   | ✅   | ✅   |
 
@@ -294,14 +303,20 @@
 ### Image Classification
 
 |   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
 | --------- | ---- | ---- | ---- | ----  |
 | ViT           | ✅  |   |   |   | 
 | Swin           | ✅  |   |   |   | 
 
+### Image to text (Multi-modal models)
+
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
+| --------- | ---- | ---- | ---- | ----  |
+| Blip-2           | ✅  |   |   |   | 
+
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
@@ -366,18 +381,21 @@
 
 2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
 
 3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
 `P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
 new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
 
+4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+
 ## Backlog:
-1. Explore and possibly integrate `(IA)^3`
-2. Add tests
-3. Add more use cases and examples
+- [x] Add tests
+- [x] Multi Adapter training and inference support
+- [x] Add more use cases and examples
+- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
```

