# Comparing `tmp/sdkit-1.0.84.tar.gz` & `tmp/sdkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-1.0.84.tar", last modified: Wed May  3 10:41:25 2023, max compression
+gzip compressed data, was "sdkit-1.0.9.tar", last modified: Mon Dec 26 06:53:41 2022, max compression
```

## Comparing `sdkit-1.0.84.tar` & `sdkit-1.0.9.tar`

### file list

```diff
@@ -1,80 +1,61 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:25.132047 sdkit-1.0.84/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.84/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.84/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-03 10:41:25.128045 sdkit-1.0.84/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.84/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-03 10:40:41.000000 sdkit-1.0.84/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:22.893859 sdkit-1.0.84/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3522 2023-04-22 10:04:42.000000 sdkit-1.0.84/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.130857 sdkit-1.0.84/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.84/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1141 2023-02-18 09:02:00.000000 sdkit-1.0.84/sdkit/filter/apply_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.84/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.84/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.228855 sdkit-1.0.84/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.84/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9810 2023-05-03 09:29:32.000000 sdkit-1.0.84/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.84/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.413587 sdkit-1.0.84/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.84/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.84/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3456 2023-04-29 08:59:57.000000 sdkit-1.0.84/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.84/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.507792 sdkit-1.0.84/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.84/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.84/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.602063 sdkit-1.0.84/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.84/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.882506 sdkit-1.0.84/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1687 2023-04-28 10:51:00.000000 sdkit-1.0.84/sdkit/models/model_loader/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.975361 sdkit-1.0.84/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3810 2023-04-28 10:50:59.000000 sdkit-1.0.84/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.84/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.84/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:24.122361 sdkit-1.0.84/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10893 2023-05-03 10:21:42.000000 sdkit-1.0.84/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.84/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10003 2023-05-03 09:32:43.000000 sdkit-1.0.84/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.84/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:24.320092 sdkit-1.0.84/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.84/sdkit/models/models_db/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:24.776047 sdkit-1.0.84/sdkit/models/models_db/configs/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.84/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.84/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.84/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.84/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.84/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.84/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:24.851047 sdkit-1.0.84/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.84/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:25.096048 sdkit-1.0.84/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-04-29 09:01:32.000000 sdkit-1.0.84/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.84/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.84/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.84/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-04-28 10:51:00.000000 sdkit-1.0.84/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.84/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6818 2023-05-03 10:35:44.000000 sdkit-1.0.84/sdkit/utils/memory_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-03 10:41:23.001862 sdkit-1.0.84/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-03 10:41:22.000000 sdkit-1.0.84/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2240 2023-05-03 10:41:22.000000 sdkit-1.0.84/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-03 10:41:22.000000 sdkit-1.0.84/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-03 10:41:22.000000 sdkit-1.0.84/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-03 10:41:22.000000 sdkit-1.0.84/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-03 10:41:25.134047 sdkit-1.0.84/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-03 10:25:33.000000 sdkit-1.0.84/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.901213 sdkit-1.0.9/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.9/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10561 2022-12-26 06:53:41.901213 sdkit-1.0.9/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9417 2022-12-25 12:59:22.000000 sdkit-1.0.9/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1202 2022-12-26 06:53:21.000000 sdkit-1.0.9/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:40.786016 sdkit-1.0.9/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1558 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:40.978753 sdkit-1.0.9/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1080 2022-12-23 17:45:58.000000 sdkit-1.0.9/sdkit/filter/apply_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      967 2022-12-24 15:54:42.000000 sdkit-1.0.9/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      348 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.053355 sdkit-1.0.9/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       54 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3797 2022-12-24 15:27:25.000000 sdkit-1.0.9/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2442 2022-12-24 14:19:36.000000 sdkit-1.0.9/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.155566 sdkit-1.0.9/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2258 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2493 2022-12-23 13:03:14.000000 sdkit-1.0.9/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1929 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.234088 sdkit-1.0.9/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      259 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5404 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.359482 sdkit-1.0.9/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1116 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/model_loader/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      551 2022-12-24 15:57:14.000000 sdkit-1.0.9/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.422375 sdkit-1.0.9/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1855 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4196 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1171 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.500383 sdkit-1.0.9/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4026 2022-12-25 11:34:33.000000 sdkit-1.0.9/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9418 2022-12-26 06:51:41.000000 sdkit-1.0.9/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1474 2022-12-24 16:01:04.000000 sdkit-1.0.9/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.656056 sdkit-1.0.9/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      688 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/models_db/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      483 2022-12-26 06:24:39.000000 sdkit-1.0.9/sdkit/models/models_db/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1286 2022-12-26 06:17:24.000000 sdkit-1.0.9/sdkit/models/models_db/print_quick_hashes.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      546 2022-12-26 06:24:50.000000 sdkit-1.0.9/sdkit/models/models_db/realesrgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9883 2022-12-26 06:40:39.000000 sdkit-1.0.9/sdkit/models/models_db/stable_diffusion.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      205 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.703314 sdkit-1.0.9/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1999 2022-12-26 04:43:58.000000 sdkit-1.0.9/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:41.881083 sdkit-1.0.9/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      805 2022-12-26 05:50:49.000000 sdkit-1.0.9/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      210 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/utils/device_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2638 2022-12-26 04:21:30.000000 sdkit-1.0.9/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1508 2022-12-26 06:25:26.000000 sdkit-1.0.9/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      986 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2082 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2194 2022-12-23 10:54:05.000000 sdkit-1.0.9/sdkit/utils/latent_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2022-12-26 06:53:40.883117 sdkit-1.0.9/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10561 2022-12-26 06:53:40.000000 sdkit-1.0.9/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1439 2022-12-26 06:53:40.000000 sdkit-1.0.9/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2022-12-26 06:53:40.000000 sdkit-1.0.9/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       85 2022-12-26 06:53:40.000000 sdkit-1.0.9/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2022-12-26 06:53:40.000000 sdkit-1.0.9/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2022-12-26 06:53:41.901213 sdkit-1.0.9/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      288 2022-12-23 10:54:05.000000 sdkit-1.0.9/setup.py
```

### Comparing `sdkit-1.0.84/LICENSE` & `sdkit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.84/PKG-INFO` & `sdkit-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.84
+Version: 1.0.9
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sdkit
 **sdkit** (**s**table **d**iffusion **kit**) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient.
 
@@ -24,27 +23,25 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
-Tested with Python 3.8. Supports Windows, Linux and Mac.
+Tested with Python 3.8.
 
-**Windows/Linux:**
-1. `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
+1. On Windows and Linux only: `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
 2. Run `pip install sdkit`
 
-**Mac:**
-1. Run `pip install sdkit`
+We don't support Mac yet, but we'd love to accept code contributions!
 
 # Example
 ### Local model
 A simple example for generating an image from a Stable Diffusion model file (already present on the disk):
 ```python
 import sdkit
 from sdkit.models import load_model
@@ -110,15 +107,15 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, multiple GPU support, gfpgan (fix faces), realesrgan (upscale), 14 samplers (including k-samplers), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
 📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
@@ -131,47 +128,50 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
-You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
+You can certainly use diffusers. `sdkit` is just a different attempt at a productive toolkit, so use `sdkit` if you find its features useful.
 
 `sdkit`:
-1. is a simple, lightweight toolkit for Stable Diffusion projects.
+1. is a fresh attempt at a simple, lightweight toolkit for Stable Diffusion projects.
 2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
-3. works with the popular `.ckpt` and `.safetensors` model format.
+3. works with the popular `.ckpt` and `.safetensors` model format (instead of only the diffusers format).
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
-8. includes 19 samplers (including k-samplers).
+8. includes 14 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
 
+This is not to say that `diffusers` doesn't do these. The easy-to-use API of `diffusers` is an inspiration for `sdkit`.
+
 # Who is using sdkit?
-* [Easy Diffusion (cmdr2 UI)](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
-* [aipromptstudio.com](https://aipromptstudio.com/)
+* [cmdr2 UI](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
 - CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
 - Seamless tiling.
 - Outpainting.
+- Mac support.
 - AMD support.
+- Allow other samplers for img2img (instead of only DDIM).
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
```

### Comparing `sdkit-1.0.84/README.md` & `sdkit-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
-Tested with Python 3.8. Supports Windows, Linux and Mac.
+Tested with Python 3.8.
 
-**Windows/Linux:**
-1. `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
+1. On Windows and Linux only: `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
 2. Run `pip install sdkit`
 
-**Mac:**
-1. Run `pip install sdkit`
+We don't support Mac yet, but we'd love to accept code contributions!
 
 # Example
 ### Local model
 A simple example for generating an image from a Stable Diffusion model file (already present on the disk):
 ```python
 import sdkit
 from sdkit.models import load_model
@@ -92,15 +90,15 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, multiple GPU support, gfpgan (fix faces), realesrgan (upscale), 14 samplers (including k-samplers), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
 📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
@@ -113,47 +111,50 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
-You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
+You can certainly use diffusers. `sdkit` is just a different attempt at a productive toolkit, so use `sdkit` if you find its features useful.
 
 `sdkit`:
-1. is a simple, lightweight toolkit for Stable Diffusion projects.
+1. is a fresh attempt at a simple, lightweight toolkit for Stable Diffusion projects.
 2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
-3. works with the popular `.ckpt` and `.safetensors` model format.
+3. works with the popular `.ckpt` and `.safetensors` model format (instead of only the diffusers format).
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
-8. includes 19 samplers (including k-samplers).
+8. includes 14 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
 
+This is not to say that `diffusers` doesn't do these. The easy-to-use API of `diffusers` is an inspiration for `sdkit`.
+
 # Who is using sdkit?
-* [Easy Diffusion (cmdr2 UI)](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
-* [aipromptstudio.com](https://aipromptstudio.com/)
+* [cmdr2 UI](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
 - CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
 - Seamless tiling.
 - Outpainting.
+- Mac support.
 - AMD support.
+- Allow other samplers for img2img (instead of only DDIM).
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
```

### Comparing `sdkit-1.0.84/pyproject.toml` & `sdkit-1.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "1.0.84"
+version = "1.0.9"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!"
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: Microsoft :: Windows :: Windows 10",
 	"Operating System :: Microsoft :: Windows :: Windows 11",
 	"Operating System :: POSIX :: Linux",
-	"Operating System :: MacOS",
 ]
 keywords = ["stable diffusion", "ai", "art"]
 
 [project.urls]
 "Homepage" = "https://github.com/easydiffusion/sdkit"
 "Bug Tracker" = "https://github.com/easydiffusion/sdkit/issues"
-
-[tool.isort]
-profile = "black"
-
-[tool.black]
-line-length = 120
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
```

### Comparing `sdkit-1.0.84/sdkit/generate/prompt_parser.py` & `sdkit-1.0.9/sdkit/generate/prompt_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 import torch
 
 from sdkit.utils import log
 
-
 def get_cond_and_uncond(prompt, negative_prompt, batch_size, model):
     cond = parse_prompt(prompt, batch_size, model)
     uncond = parse_prompt(negative_prompt, batch_size, model)
 
     return cond, uncond
 
-
 def parse_prompt(prompt, batch_size, model):
     """
     Requires model to be on the device
     """
     empty_result = model.get_learned_conditioning(batch_size * [""])
     result = torch.zeros_like(empty_result)
     subprompts, weights = split_weighted_subprompts(prompt)
     weights_sum = sum(weights)
 
     for i, subprompt in enumerate(subprompts):
-        result = torch.add(
-            result, model.get_learned_conditioning(batch_size * [subprompt]), alpha=weights[i] / weights_sum
-        )
+        result = torch.add(result, model.get_learned_conditioning(batch_size * [subprompt]), alpha=weights[i] / weights_sum)
 
     if len(subprompts) == 0:
         result = empty_result
 
     return result
 
-
 def split_weighted_subprompts(text):
     """
-    grabs all text up to the first occurrence of ':'
+    grabs all text up to the first occurrence of ':' 
     uses the grabbed text as a sub-prompt, and takes the value following ':' as weight
     if ':' has no value defined, defaults to 1.0
     repeats until no text remaining
     """
     remaining = len(text)
     prompts = []
     weights = []
     while remaining > 0:
         if ":" in text:
-            idx = text.index(":")  # first occurrence from start
+            idx = text.index(":") # first occurrence from start
             # grab up to index as sub-prompt
             prompt = text[:idx]
             remaining -= idx
             # remove from main text
-            text = text[idx + 1 :]
-            # find value for weight
+            text = text[idx+1:]
+            # find value for weight 
             if " " in text:
-                idx = text.index(" ")  # first occurence
-            else:  # no space, read to end
+                idx = text.index(" ") # first occurence
+            else: # no space, read to end
                 idx = len(text)
             if idx != 0:
                 try:
                     weight = float(text[:idx])
-                except:  # couldn't treat as float
+                except: # couldn't treat as float
                     log.warn(f"Warning: '{text[:idx]}' is not a value, are you missing a space?")
                     weight = 1.0
-            else:  # no value found
+            else: # no value found
                 weight = 1.0
             # remove from main text
             remaining -= idx
-            text = text[idx + 1 :]
+            text = text[idx+1:]
             # append the sub-prompt and its weight
             prompts.append(prompt)
             weights.append(weight)
-        else:  # no : found
-            if len(text) > 0:  # there is still text though
+        else: # no : found
+            if len(text) > 0: # there is still text though
                 # take remainder as weight 1
                 prompts.append(text)
                 weights.append(1.0)
             remaining = 0
-    return prompts, weights
+    return prompts, weights
```

### Comparing `sdkit-1.0.84/sdkit/generate/sampler/default_samplers.py` & `sdkit-1.0.9/sdkit/generate/sampler/default_samplers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,63 @@
 import torch
+from torch import Tensor
+
 from ldm.models.diffusion.ddim import DDIMSampler
-from ldm.models.diffusion.dpm_solver import DPMSolverSampler
 from ldm.models.diffusion.plms import PLMSSampler
-from torch import Tensor
+from ldm.models.diffusion.dpm_solver import DPMSolverSampler
 
 from sdkit import Context
 
 samplers = {
-    "ddim": DDIMSampler,
-    "plms": PLMSSampler,
-    "dpm_solver_stability": DPMSolverSampler,
+    'ddim': DDIMSampler,
+    'plms': PLMSSampler,
+    'dpm_solver_stability': DPMSolverSampler,
 }
 
-
-def sample(
-    context: Context,
-    sampler_name: str = None,
-    noise: Tensor = None,
-    batch_size: int = 1,
-    shape: tuple = (),
-    steps: int = 50,
-    cond: Tensor = None,
-    uncond: Tensor = None,
-    guidance_scale: float = 0.8,
-    callback=None,
-    **kwargs,
-):
-    model = context.models["stable-diffusion"]
-    sample_fn = _sample_txt2img if "init_image_latent" not in kwargs else _sample_img2img
+def sample(context: Context, sampler_name:str=None, noise: Tensor=None, batch_size: int=1, shape: tuple=(), steps: int=50, cond: Tensor=None, uncond: Tensor=None, guidance_scale: float=0.8, callback=None, **kwargs):
+    model = context.models['stable-diffusion']
+    sample_fn = _sample_txt2img if 'init_image_latent' not in kwargs else _sample_img2img
 
     common_params = {
-        "S": steps,
-        "batch_size": batch_size,
-        "shape": shape,
-        "conditioning": cond,
-        "verbose": False,
-        "unconditional_guidance_scale": guidance_scale,
-        "unconditional_conditioning": uncond,
-        "eta": 0.0,
-        "img_callback": callback,
+        'S': steps,
+        'batch_size': batch_size,
+        'shape': shape,
+        'conditioning': cond,
+        'verbose': False,
+        'unconditional_guidance_scale': guidance_scale,
+        'unconditional_conditioning': uncond,
+        'eta': 0.,
+        'img_callback': callback,
     }
 
     samples, _ = sample_fn(model, sampler_name, noise, steps, batch_size, common_params.copy(), **kwargs)
     return samples
 
-
 def _sample_txt2img(model, sampler_name, noise, steps, batch_size, params, **kwargs):
     sampler = samplers[sampler_name](model)
-    params.update(
-        {
-            "x_T": noise,
-        }
-    )
+    params.update({
+        'x_T': noise,
+    })
 
     return sampler.sample(**params)
 
-
 def _sample_img2img(model, sampler_name, noise, steps, batch_size, params, **kwargs):
     sampler = DDIMSampler(model)
 
-    actual_inference_steps = int(steps * kwargs["prompt_strength"])
-    init_image_latent = kwargs["init_image_latent"]
-    mask = kwargs.get("mask")
-
-    sampler.make_schedule(ddim_num_steps=steps, ddim_eta=0.0, verbose=False)
-    z_enc = sampler.stochastic_encode(
-        init_image_latent, torch.tensor([actual_inference_steps] * batch_size).to(model.device), noise=noise
-    )
-
-    sampler.make_schedule = (
-        lambda **kwargs: kwargs
-    )  # we've already called this, don't call this again from within the sampler
-    sampler.ddim_timesteps = sampler.ddim_timesteps[:actual_inference_steps]
-
-    params.update(
-        {
-            "S": actual_inference_steps,
-            "x_T": z_enc,
-            "x0": init_image_latent if mask is not None else None,
-            "mask": mask,
-        }
-    )
+    actual_inference_steps = int(steps * kwargs['prompt_strength'])
+    init_image_latent = kwargs['init_image_latent']
+    mask = kwargs.get('mask')
 
-    return sampler.sample(**params)
+    sampler.make_schedule(ddim_num_steps=steps, ddim_eta=0., verbose=False)
+    z_enc = sampler.stochastic_encode(init_image_latent, torch.tensor([actual_inference_steps] * batch_size).to(model.device), noise=noise)
 
+    sampler.make_schedule = (lambda **kwargs: kwargs) # we've already called this, don't call this again from within the sampler
+    sampler.ddim_timesteps = sampler.ddim_timesteps[:actual_inference_steps]
 
-# fix the precision used for sampler buffers on M1/M2 Macs
-# based on the approach used in https://github.com/AUTOMATIC1111/stable-diffusion-webui/blob/master/modules/sd_hijack.py
-def register_buffer_mps_aware(self, name, attr):
-    if type(attr) == torch.Tensor:
-        model_device = torch.device(self.model.device)
-        is_mps_device = hasattr(torch.backends, "mps") and model_device == torch.device("mps")
-        if attr.device != model_device:
-            attr = attr.to(device=model_device, dtype=torch.float32 if is_mps_device else None)
-    setattr(self, name, attr)
-
+    params.update({
+        'S': actual_inference_steps,
+        'x_T': z_enc,
+        'x0': init_image_latent if mask is not None else None,
+        'mask': mask,
+    })
 
-DDIMSampler.register_buffer = register_buffer_mps_aware
-PLMSSampler.register_buffer = register_buffer_mps_aware
-DPMSolverSampler.register_buffer = register_buffer_mps_aware
+    return sampler.sample(**params)
```

### Comparing `sdkit-1.0.84/sdkit/generate/sampler/sampler_main.py` & `sdkit-1.0.9/sdkit/generate/sampler/sampler_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,44 @@
 import torch
 from torch import Tensor
 
 from sdkit import Context
 from sdkit.utils import log
 
-from . import default_samplers, k_samplers, unipc_samplers
+from . import default_samplers, k_samplers
 
-
-def make_samples(
-    context: Context,
-    sampler_name: str = None,
-    seed: int = 42,
-    batch_size: int = 1,
-    shape: tuple = (),
-    steps: int = 50,
-    cond: Tensor = None,
-    uncond: Tensor = None,
-    guidance_scale: float = 0.8,
-    callback=None,
-    **kwargs,
-):
+def make_samples(context: Context, sampler_name: str=None, seed: int=42, batch_size: int=1, shape: tuple=(), steps: int=50, cond: Tensor=None, uncond: Tensor=None, guidance_scale: float=0.8, callback=None, **kwargs):
     """
     Common args:
     * context: Context
     * sampler_name: str
     * seed: int
     * batch_size: int - number of images to generate in parallel
     * shape: tuple
     * steps: int - number of inference steps
     * cond: Tensor - conditioning from the prompt
     * uncond: Tensor - unconditional conditioning from the negative prompt
     * guidance_scale: float
     * callback: function - signature: `callback(x_samples: Tensor, i: int)`
 
     additional args for txt2img:
-
+    
     additional args for img2img:
     * init_image_latent: Tensor
     * mask: Tensor
     * prompt_strength: float - between 0 and 1. Use 0 to ignore the prompt entirely, or 1 to ignore the init image entirely
     """
     sampler_module = None
-    if sampler_name in default_samplers.samplers:
-        sampler_module = default_samplers
-    if sampler_name in k_samplers.samplers:
-        sampler_module = k_samplers
-    if sampler_name in unipc_samplers.samplers:
-        sampler_module = unipc_samplers
-    if sampler_module is None:
-        raise RuntimeError(f'Unknown sampler "{sampler_name}"!')
+    if sampler_name in default_samplers.samplers: sampler_module = default_samplers
+    if sampler_name in k_samplers.samplers: sampler_module = k_samplers
+    if sampler_module is None: raise RuntimeError(f'Unknown sampler "{sampler_name}"!')
 
     noise = make_some_noise(seed, batch_size, shape, context.device)
 
-    return sampler_module.sample(
-        context, sampler_name, noise, batch_size, shape, steps, cond, uncond, guidance_scale, callback, **kwargs
-    )
-
+    return sampler_module.sample(context, sampler_name, noise, batch_size, shape, steps, cond, uncond, guidance_scale, callback, **kwargs)
 
 def make_some_noise(seed, batch_size, shape, device):
     b1, b2, b3 = shape
     img_shape = (1, b1, b2, b3)
     tens = []
     log.info(f"seeds used = {[seed+s for s in range(batch_size)]}")
```

### Comparing `sdkit-1.0.84/sdkit/models/model_downloader.py` & `sdkit-1.0.9/sdkit/models/model_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,103 +1,95 @@
 import os
 from urllib.parse import urlparse
 
 from sdkit.utils import download_file, log
 
-
-def download_models(models: dict, download_base_dir: str = None, subdir_for_model_type=True):
-    """
+def download_models(models: dict, download_base_dir: str=None, subdir_for_model_type=True):
+    '''
     Downloads the requested models (and config files) based on the SDKit models database.
     Resumes incomplete downloads, and shows a progress bar.
 
     Args:
     * models: dict of {string: string or list}. Models to download of `model_type: model_ids`.
               E.g. `{'stable-diffusion': ['1.4', '1.5-inpainting'], 'gfpgan': '1.3'}`
               `model_ids` can be a single string, or a list of strings.
     * download_base_dir: str - base directory inside which the models are downloaded.
               Note: The actual download directorypath will include the `model_type` if `subdir_for_model_type` is `True`.
               If `download_base_dir` is `None`, it'll use the `~/.cache/sdkit` folder, where `~` is the home or user-folder.
     * subdir_for_model_type: bool - default True. Saves the downloaded model in a subdirectory (named with the model_type).
               For e.g. if `download_base_dir` is `D:\\models`, then a `stable-diffusion` type model is downloaded to
               `D:\\models\\stable-diffusion`, a `hypernetwork` type model is downloaded to `D:\\models\\hypernetwork` and so on.
-    """
+    '''
     for model_type, model_ids in models.items():
         model_ids = model_ids if isinstance(model_ids, list) else [model_ids]
 
         for model_id in model_ids:
             download_model(model_type, model_id, download_base_dir, subdir_for_model_type)
 
-
-def download_model(model_type: str, model_id: str, download_base_dir: str = None, subdir_for_model_type=True):
-    """
+def download_model(model_type: str, model_id: str, download_base_dir: str=None, subdir_for_model_type=True):
+    '''
     Downloads the requested model (and config file) based on the SDKit models database.
     Resumes incomplete downloads, and shows a progress bar.
 
     Args:
     * model_type: str
     * model_id: str
     * download_base_dir: str - base directory inside which the models are downloaded.
               Note: The actual download directory path will include the `model_type` if `subdir_for_model_type` is `True`.
               If `download_base_dir` is `None`, it'll use the `~/.cache/sdkit` folder, where `~` is the home or user-folder.
     * subdir_for_model_type: bool - default True. Saves the downloaded model in a subdirectory (named with the model_type).
               For e.g. if `download_base_dir` is `D:\\models`, then a `stable-diffusion` type model is downloaded to
               `D:\\models\\stable-diffusion`, a `hypernetwork` type model is downloaded to `D:\\models\\hypernetwork` and so on.
-    """
+    '''
     download_base_dir = get_actual_base_dir(model_type, download_base_dir, subdir_for_model_type)
     try:
-        model_url, model_file_name = get_url_and_filename(model_type, model_id, url_key="url")
-        config_url, config_file_name = get_url_and_filename(model_type, model_id, url_key="config_url")
+        model_url, model_file_name = get_url_and_filename(model_type, model_id, url_key='url')
+        config_url, config_file_name = get_url_and_filename(model_type, model_id, url_key='config_url')
 
         if model_url is None:
-            log.warn(f"No download url found for model {model_type} {model_id}")
+            log.warn(f'No download url found for model {model_type} {model_id}')
             return
 
-        os.makedirs(download_base_dir, exist_ok=True)
         out_path = os.path.join(download_base_dir, model_file_name)
         download_file(model_url, out_path)
 
         if config_url:
             out_path = os.path.join(download_base_dir, config_file_name)
             download_file(config_url, out_path)
     except Exception as e:
         log.exception(e)
 
-
-def resolve_downloaded_model_path(
-    model_type: str, model_id: str, download_base_dir: str = None, subdir_for_model_type=True
-):
-    """
+def resolve_downloaded_model_path(model_type: str, model_id: str, download_base_dir: str=None, subdir_for_model_type=True):
+    '''
     Gets the path to the downloaded model file. Returns `None` if a file doesn't exist at the calculated path.
 
     Args:
     * model_type: str
     * model_id: str
     * download_base_dir: str - base directory inside which the models are downloaded.
               Note: The actual download directory path will include the `model_type` if `subdir_for_model_type` is `True`.
               If `download_base_dir` is `None`, it'll use the `~/.cache/sdkit` folder, where `~` is the home or user-folder.
     * subdir_for_model_type: bool - default True. Saves the downloaded model in a subdirectory (named with the model_type).
               For e.g. if `download_base_dir` is `D:\\models`, then a `stable-diffusion` type model is downloaded to
               `D:\\models\\stable-diffusion`, a `hypernetwork` type model is downloaded to `D:\\models\\hypernetwork` and so on.
-    """
+    '''
     download_base_dir = get_actual_base_dir(model_type, download_base_dir, subdir_for_model_type)
-    _, file_name = get_url_and_filename(model_type, model_id, url_key="url")
+    _, file_name = get_url_and_filename(model_type, model_id, url_key='url')
     if file_name is None:
         return
 
     file_path = os.path.join(download_base_dir, file_name)
     return file_path if os.path.exists(file_path) else None
 
-
 def get_actual_base_dir(model_type, download_base_dir, subdir_for_model_type):
-    download_base_dir = os.path.join("~", ".cache", "sdkit") if download_base_dir is None else download_base_dir
+    download_base_dir = os.path.join('~', '.cache', 'sdkit') if download_base_dir is None else download_base_dir
     download_base_dir = os.path.join(download_base_dir, model_type) if subdir_for_model_type else download_base_dir
     return os.path.abspath(download_base_dir)
 
-
-def get_url_and_filename(model_type, model_id, url_key="url"):
+def get_url_and_filename(model_type, model_id, url_key='url'):
     from sdkit.models import get_model_info_from_db
 
     model_info = get_model_info_from_db(model_type=model_type, model_id=model_id)
     url = model_info.get(url_key)
     if url is None:
         return None, None
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/__init__.py` & `sdkit-1.0.9/sdkit/models/model_loader/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,36 @@
+from . import hypernetwork
+from . import stable_diffusion, gfpgan, realesrgan, vae
+
 from sdkit import Context
 from sdkit.utils import gc, log
 
-from . import (
-    gfpgan,
-    hypernetwork,
-    lora,
-    nsfw_checker,
-    realesrgan,
-    stable_diffusion,
-    vae,
-)
-
 models = {
-    "stable-diffusion": stable_diffusion,
-    "gfpgan": gfpgan,
-    "realesrgan": realesrgan,
-    "vae": vae,
-    "hypernetwork": hypernetwork,
-    "nsfw_checker": nsfw_checker,
-    "lora": lora,
+    'stable-diffusion': stable_diffusion,
+    'gfpgan': gfpgan,
+    'realesrgan': realesrgan,
+    'vae': vae,
+    'hypernetwork': hypernetwork,
 }
 
-
 def load_model(context: Context, model_type: str, **kwargs):
-    if context.model_paths.get(model_type) is None and model_type != "nsfw_checker":
+    if context.model_paths.get(model_type) is None:
         return
 
     if model_type in context.models:
         unload_model(context, model_type)
 
-    log.info(f"loading {model_type} model from {context.model_paths.get(model_type)} to device: {context.device}")
+    log.info(f'loading {model_type} model from {context.model_paths.get(model_type)} to device: {context.device}')
 
     context.models[model_type] = models[model_type].load_model(context, **kwargs)
 
-    log.info(f"loaded {model_type} model from {context.model_paths.get(model_type)} to device: {context.device}")
-
-    # reload dependent models
-    if model_type == "stable-diffusion":
-        load_model(context, "vae")
-        load_model(context, "hypernetwork")
-        if "lora" in context.models and hasattr(context, "_last_lora_alpha"):
-            del context._last_lora_alpha
-        load_model(context, "lora")
-
+    log.info(f'loaded {model_type} model from {context.model_paths.get(model_type)} to device: {context.device}')
 
 def unload_model(context: Context, model_type: str, **kwargs):
     if model_type not in context.models:
         return
 
-    if context.test_diffusers:
-        models[model_type].unload_model(context)
-        del context.models[model_type]
-    else:
-        del context.models[model_type]
-        models[model_type].unload_model(context)
-
+    del context.models[model_type]
+    models[model_type].unload_model(context)
     gc(context)
 
-    log.info(f"unloaded {model_type} model from device: {context.device}")
+    log.info(f'unloaded {model_type} model from device: {context.device}')
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/gfpgan.py` & `sdkit-1.0.9/sdkit/models/model_loader/gfpgan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import torch
 from gfpgan import GFPGANer
 
 from sdkit import Context
 
-
 def load_model(context: Context, **kwargs):
-    model_path = context.model_paths.get("gfpgan")
+    model_path = context.model_paths.get('gfpgan')
 
     # hack for a bug in facexlib: https://github.com/xinntao/facexlib/pull/19/files
     from facexlib.detection import retinaface
-
     retinaface.device = torch.device(context.device)
 
-    return GFPGANer(
-        device=torch.device(context.device),
-        model_path=model_path,
-        upscale=1,
-        arch="clean",
-        channel_multiplier=2,
-        bg_upsampler=None,
-    )
-
+    return GFPGANer(device=torch.device(context.device), model_path=model_path, upscale=1, arch='clean', channel_multiplier=2, bg_upsampler=None)
 
 def unload_model(context: Context, **kwargs):
     pass
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-1.0.9/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,42 @@
 import traceback
 
 from sdkit import Context
-from sdkit.utils import load_tensor_file, log
-
+from sdkit.utils import log, load_tensor_file
 
 def load_model(context: Context, **kwargs):
     from .hypernetwork import HypernetworkModule, override_attention_context_kv
-
-    model_path = context.model_paths.get("hypernetwork")
+    model_path = context.model_paths.get('hypernetwork')
 
     try:
         state_dict = load_tensor_file(model_path)
 
-        layer_structure = state_dict.get("layer_structure", [1, 2, 1])
-        activation_func = state_dict.get("activation_func", None)
-        weight_init = state_dict.get("weight_initialization", "Normal")
-        add_layer_norm = state_dict.get("is_layer_norm", False)
-        use_dropout = state_dict.get("use_dropout", False)
-        activate_output = state_dict.get("activate_output", True)
-        last_layer_dropout = state_dict.get("last_layer_dropout", False)
+        layer_structure = state_dict.get('layer_structure', [1, 2, 1])
+        activation_func = state_dict.get('activation_func', None)
+        weight_init = state_dict.get('weight_initialization', 'Normal')
+        add_layer_norm = state_dict.get('is_layer_norm', False)
+        use_dropout = state_dict.get('use_dropout', False)
+        activate_output = state_dict.get('activate_output', True)
+        last_layer_dropout = state_dict.get('last_layer_dropout', False)
 
-        layers = {"hypernetwork_strength": 0}
+        layers = {'hypernetwork_strength': 0}
         for size, sd in state_dict.items():
             if type(size) == int:
                 layers[size] = (
-                    HypernetworkModule(
-                        size,
-                        sd[0],
-                        layer_structure,
-                        activation_func,
-                        weight_init,
-                        add_layer_norm,
-                        use_dropout,
-                        activate_output,
-                        last_layer_dropout=last_layer_dropout,
-                        model=layers,
-                        device=context.device,
-                    ),
-                    HypernetworkModule(
-                        size,
-                        sd[1],
-                        layer_structure,
-                        activation_func,
-                        weight_init,
-                        add_layer_norm,
-                        use_dropout,
-                        activate_output,
-                        last_layer_dropout=last_layer_dropout,
-                        model=layers,
-                        device=context.device,
-                    ),
+                    HypernetworkModule(size, sd[0], layer_structure, activation_func, weight_init, add_layer_norm,
+                                    use_dropout, activate_output, last_layer_dropout=last_layer_dropout,
+                                    model=layers, device=context.device),
+                    HypernetworkModule(size, sd[1], layer_structure, activation_func, weight_init, add_layer_norm,
+                                    use_dropout, activate_output, last_layer_dropout=last_layer_dropout,
+                                    model=layers, device=context.device),
                 )
 
         override_attention_context_kv(layers)
 
         return layers
     except:
         log.error(traceback.format_exc())
-        log.error(f"Could not load hypernetwork: {model_path}")
-
+        log.error(f'Could not load hypernetwork: {model_path}')
+        del context.models['hypernetwork']
 
 def unload_model(context: Context, **kwargs):
-    from .hypernetwork import override_attention_context_kv
-
-    override_attention_context_kv(None)
+    pass
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-1.0.9/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,107 +1,83 @@
 # Modified version, originally contributed by c0bra5 - https://github.com/cmdr2/stable-diffusion-ui/pull/619
 # which was a cut down version of https://github.com/AUTOMATIC1111/stable-diffusion-webui/blob/c9a2cfdf2a53d37c2de1908423e4f548088667ef/modules/hypernetworks/hypernetwork.py
 
 import inspect
-
 import torch
 
-
 class HypernetworkModule(torch.nn.Module):
     multiplier = 0.5
     activation_dict = {
         "linear": torch.nn.Identity,
         "relu": torch.nn.ReLU,
         "leakyrelu": torch.nn.LeakyReLU,
         "elu": torch.nn.ELU,
         "swish": torch.nn.Hardswish,
         "tanh": torch.nn.Tanh,
         "sigmoid": torch.nn.Sigmoid,
     }
-    activation_dict.update(
-        {
-            cls_name.lower(): cls_obj
-            for cls_name, cls_obj in inspect.getmembers(torch.nn.modules.activation)
-            if inspect.isclass(cls_obj) and cls_obj.__module__ == "torch.nn.modules.activation"
-        }
-    )
+    activation_dict.update({cls_name.lower(): cls_obj for cls_name, cls_obj in inspect.getmembers(torch.nn.modules.activation) if inspect.isclass(cls_obj) and cls_obj.__module__ == 'torch.nn.modules.activation'})
 
-    def __init__(
-        self,
-        dim,
-        state_dict=None,
-        layer_structure=None,
-        activation_func=None,
-        weight_init="Normal",
-        add_layer_norm=False,
-        use_dropout=False,
-        activate_output=False,
-        last_layer_dropout=False,
-        model=None,
-        device="cuda",
-    ):
+    def __init__(self, dim, state_dict=None, layer_structure=None, activation_func=None, weight_init='Normal',
+                 add_layer_norm=False, use_dropout=False, activate_output=False, last_layer_dropout=False, model=None, device='cuda'):
         super().__init__()
 
         self.model = model
 
         assert layer_structure is not None, "layer_structure must not be None"
         assert layer_structure[0] == 1, "Multiplier Sequence should start with size 1!"
         assert layer_structure[-1] == 1, "Multiplier Sequence should end with size 1!"
 
         linears = []
         for i in range(len(layer_structure) - 1):
+
             # Add a fully-connected layer
-            linears.append(torch.nn.Linear(int(dim * layer_structure[i]), int(dim * layer_structure[i + 1])))
+            linears.append(torch.nn.Linear(int(dim * layer_structure[i]), int(dim * layer_structure[i+1])))
 
             # Add an activation func except last layer
-            if (
-                activation_func == "linear"
-                or activation_func is None
-                or (i >= len(layer_structure) - 2 and not activate_output)
-            ):
+            if activation_func == "linear" or activation_func is None or (i >= len(layer_structure) - 2 and not activate_output):
                 pass
             elif activation_func in self.activation_dict:
                 linears.append(self.activation_dict[activation_func]())
             else:
-                raise RuntimeError(f"hypernetwork uses an unsupported activation function: {activation_func}")
+                raise RuntimeError(f'hypernetwork uses an unsupported activation function: {activation_func}')
 
             # Add layer normalization
             if add_layer_norm:
-                linears.append(torch.nn.LayerNorm(int(dim * layer_structure[i + 1])))
+                linears.append(torch.nn.LayerNorm(int(dim * layer_structure[i+1])))
 
             # Add dropout except last layer
             if use_dropout and (i < len(layer_structure) - 3 or last_layer_dropout and i < len(layer_structure) - 2):
                 linears.append(torch.nn.Dropout(p=0.3))
 
         self.linear = torch.nn.Sequential(*linears)
 
         self.fix_old_state_dict(state_dict)
         self.load_state_dict(state_dict)
 
         self.to(device)
 
     def fix_old_state_dict(self, state_dict):
         changes = {
-            "linear1.bias": "linear.0.bias",
-            "linear1.weight": "linear.0.weight",
-            "linear2.bias": "linear.1.bias",
-            "linear2.weight": "linear.1.weight",
+            'linear1.bias': 'linear.0.bias',
+            'linear1.weight': 'linear.0.weight',
+            'linear2.bias': 'linear.1.bias',
+            'linear2.weight': 'linear.1.weight',
         }
 
         for fr, to in changes.items():
             x = state_dict.get(fr, None)
             if x is None:
                 continue
 
             del state_dict[fr]
             state_dict[to] = x
 
     def forward(self, x: torch.Tensor):
-        return x + self.linear(x) * self.model["hypernetwork_strength"]
-
+        return x + self.linear(x) * self.model['hypernetwork_strength']
 
 def apply_hypernetwork(hypernetwork, attention_context, layer=None):
     hypernetwork_layers = hypernetwork.get(attention_context.shape[2], None)
 
     if hypernetwork_layers is None:
         return attention_context, attention_context
 
@@ -109,18 +85,16 @@
         layer.hyper_k = hypernetwork_layers[0]
         layer.hyper_v = hypernetwork_layers[1]
 
     attention_context_k = hypernetwork_layers[0](attention_context)
     attention_context_v = hypernetwork_layers[1](attention_context)
     return attention_context_k, attention_context_v
 
-
 def override_attention_context_kv(hypernetwork_model):
     import sdkit.models.model_loader.stable_diffusion.optimizations as sd_model_optimizer
-
     def get_context_kv(attention_context):
         if hypernetwork_model is None:
             return attention_context, attention_context
         else:
             return apply_hypernetwork(hypernetwork_model, attention_context)
 
     sd_model_optimizer.get_context_kv = get_context_kv
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/realesrgan.py` & `sdkit-1.0.9/sdkit/models/model_loader/realesrgan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,31 @@
-import os
-
 import torch
+import os
 from basicsr.archs.rrdbnet_arch import RRDBNet
 from realesrgan import RealESRGANer
 
 from sdkit import Context
 
-
 def load_model(context: Context, **kwargs):
-    model_path = context.model_paths.get("realesrgan")
+    model_path = context.model_paths.get('realesrgan')
 
     RealESRGAN_models = {
-        "RealESRGAN_x4plus": RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4),
-        "RealESRGAN_x4plus_anime_6B": RRDBNet(
-            num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4
-        ),
+        'RealESRGAN_x4plus': RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4),
+        'RealESRGAN_x4plus_anime_6B': RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4)
     }
 
     model_to_use = os.path.basename(model_path)
     model_to_use, _ = os.path.splitext(model_to_use)
     model_to_use = RealESRGAN_models[model_to_use]
 
-    half = context.half_precision
-    model = RealESRGANer(
-        device=torch.device(context.device),
-        scale=4,
-        model_path=model_path,
-        model=model_to_use,
-        pre_pad=0,
-        half=half,
-        tile=256,
-    )
-    if "cuda" not in context.device:
-        model.model.to(context.device)
+    if context.device == 'cpu':
+        model = RealESRGANer(device=torch.device(context.device), scale=2, model_path=model_path, model=model_to_use, pre_pad=0, half=False) # cpu does not support half
+        model.model.to('cpu')
+    else:
+        model = RealESRGANer(device=torch.device(context.device), scale=2, model_path=model_path, model=model_to_use, pre_pad=0, half=context.half_precision)
 
     model.model.name = model_to_use
 
     return model
 
-
 def unload_model(context: Context, **kwargs):
     pass
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-1.0.9/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,254 +1,218 @@
-import math
-
 import torch
-from einops import rearrange
-from ldm.util import default
 from torch import einsum
+import math
+from ldm.util import default
+from einops import rearrange
 
 from sdkit import Context
 from sdkit.utils import log
 
-
 def send_to_device(context: Context, model):
     """
     Sends the model to the device, based on the VRAM optimizations set in
     `context.vram_optimizations`.
 
     Please see the documentation for `diffusionkit.types.Context.vram_optimizations`
     for a summary of the logic used for VRAM optimizations
     """
-    if len(context.vram_optimizations) == 0 or context.device == "cpu":
-        log.info("No VRAM optimizations being applied")
+    log.info(f'VRAM Optimizations: {context.vram_optimizations}')
+    if len(context.vram_optimizations) == 0 or context.device == 'cpu':
         model.to(context.device)
         model.cond_stage_model.device = context.device
         return
 
-    log.info(f"VRAM Optimizations: {context.vram_optimizations}")
-
     # based on the approach at https://github.com/AUTOMATIC1111/stable-diffusion-webui/blob/master/modules/lowvram.py
     # the idea is to keep only one module in the GPU at a time, depending on the desired optimization level
     # using torch's `register_forward_pre_hook()` hook
 
+    is_sd2_model = hasattr(model.cond_stage_model, 'model')
+    cond_transformer = model.cond_stage_model.model if is_sd2_model else model.cond_stage_model.transformer
+
     context.module_in_gpu = None
 
-    def move_to_gpu(module, _):
-        """
-        This hook ensures that only this module is in the GPU. It moves the
-        other module back to the CPU before loading itself to the GPU.
-        """
-        if module == context.module_in_gpu:
-            return
-
-        if context.module_in_gpu is not None:
-            context.module_in_gpu.to("cpu")
-            log.debug(
-                f"moved {getattr(context.module_in_gpu, 'log_name', context.module_in_gpu.__class__.__name__)} to cpu"
-            )
-
-        module.to(context.device)
-        if module == model.cond_stage_model:
-            module.device = context.device
-        context.module_in_gpu = module
-        log.debug(
-            f"moved {getattr(context.module_in_gpu, 'log_name', context.module_in_gpu.__class__.__name__)} to GPU"
-        )
+    def make_move_to_gpu_hook(module_name):
+        def move_to_gpu(module, _):
+            """
+            This hook ensures that only this module is in the GPU. It moves the
+            other module back to the CPU before loading itself to the GPU.
+            """
+            module = model.cond_stage_model if module == cond_transformer else module
+            if module == context.module_in_gpu:
+                return
+
+            if context.module_in_gpu is not None:
+                context.module_in_gpu.to('cpu')
+                log.debug(f'moved {module_name} to cpu')
+
+            module.to(context.device)
+            if module == model.cond_stage_model: module.device = context.device
+            context.module_in_gpu = module
+            log.debug(f'moved {module_name} to GPU')
+        return move_to_gpu
+
+    def wrap_fs_fn(fn, module_name):
+        move_to_gpu = make_move_to_gpu_hook(module_name)
 
-    def wrap_fs_fn(fn, model_to_move):
         def wrap(x):
-            move_to_gpu(model_to_move, None)
+            move_to_gpu(model.first_stage_model, None)
             return fn(x)
-
         return wrap
 
-    if (
-        "KEEP_FS_AND_CS_IN_CPU" in context.vram_optimizations
-        or "KEEP_ENTIRE_MODEL_IN_CPU" in context.vram_optimizations
-    ):
+    if 'KEEP_FS_AND_CS_IN_CPU' in context.vram_optimizations or 'KEEP_ENTIRE_MODEL_IN_CPU' in context.vram_optimizations:
+        if is_sd2_model: model.cond_stage_model.transformer = model.cond_stage_model.model
+
         # move the FS, CS and the main model to CPU. And send only the overall reference to the correct device
-        tmp = model.cond_stage_model, model.first_stage_model, model.model
-        model.cond_stage_model, model.first_stage_model, model.model = (None,) * 3
+        tmp = model.cond_stage_model.transformer, model.first_stage_model, model.model
+        model.cond_stage_model.transformer, model.first_stage_model, model.model = (None,) * 3
         model.to(context.device)
-        model.cond_stage_model, model.first_stage_model, model.model = tmp
+        model.cond_stage_model.transformer, model.first_stage_model, model.model = tmp
 
         # set forward_pre_hook (a feature of torch NN module) to move each module to the GPU only when required
-        model.first_stage_model.log_name = "model.first_stage_model"
-        model.first_stage_model.register_forward_pre_hook(move_to_gpu)
-        model.first_stage_model.encode = wrap_fs_fn(model.first_stage_model.encode, model.first_stage_model)
-        model.first_stage_model.decode = wrap_fs_fn(model.first_stage_model.decode, model.first_stage_model)
-
-        model.cond_stage_model.log_name = "model.cond_stage_model"
-        model.cond_stage_model.register_forward_pre_hook(move_to_gpu)
-        model.cond_stage_model.forward = wrap_fs_fn(model.cond_stage_model.forward, model.cond_stage_model)
-
-    if (
-        "KEEP_ENTIRE_MODEL_IN_CPU" in context.vram_optimizations
-    ):  # apply the same approach, but to the individual blocks in model
+        model.cond_stage_model.transformer.register_forward_pre_hook(make_move_to_gpu_hook('model.cond_stage_model.transformer'))
+        model.first_stage_model.register_forward_pre_hook(make_move_to_gpu_hook('model.first_stage_model'))
+        model.first_stage_model.encode = wrap_fs_fn(model.first_stage_model.encode, 'model.first_stage_model.encode')
+        model.first_stage_model.decode = wrap_fs_fn(model.first_stage_model.decode, 'model.first_stage_model.decode')
+
+        if is_sd2_model:
+            model.cond_stage_model.model = model.cond_stage_model.transformer
+            del model.cond_stage_model.transformer
+
+    if 'KEEP_ENTIRE_MODEL_IN_CPU' in context.vram_optimizations: # apply the same approach, but to the individual blocks in model
         d = model.model.diffusion_model
 
         tmp = d.input_blocks, d.middle_block, d.output_blocks, d.time_embed
         d.input_blocks, d.middle_block, d.output_blocks, d.time_embed = (None,) * 4
         model.model.to(context.device)
         d.input_blocks, d.middle_block, d.output_blocks, d.time_embed = tmp
 
-        d.time_embed.log_name = "model.model.diffusion_model.time_embed"
-        d.time_embed.register_forward_pre_hook(move_to_gpu)
-
-        for i, block in enumerate(d.input_blocks):
-            block.log_name = f"model.model.diffusion_model.input_blocks[{i}]"
-            block.register_forward_pre_hook(move_to_gpu)
-
-        d.middle_block.log_name = "model.model.diffusion_model.middle_block"
-        d.middle_block.register_forward_pre_hook(move_to_gpu)
-
-        for i, block in enumerate(d.output_blocks):
-            block.log_name = f"model.model.diffusion_model.output_blocks[{i}]"
-            block.register_forward_pre_hook(move_to_gpu)
+        d.time_embed.register_forward_pre_hook(make_move_to_gpu_hook('model.model.diffusion_model.time_embed'))
+        for block in d.input_blocks: block.register_forward_pre_hook(make_move_to_gpu_hook('model.model.diffusion_model.input_blocks'))
+        d.middle_block.register_forward_pre_hook(make_move_to_gpu_hook('model.model.diffusion_model.middle_block'))
+        for block in d.output_blocks: block.register_forward_pre_hook(make_move_to_gpu_hook('model.model.diffusion_model.output_blocks'))
     else:
         model.model.to(context.device)
 
-    if (
-        "KEEP_ENTIRE_MODEL_IN_CPU" not in context.vram_optimizations
-        and "KEEP_FS_AND_CS_IN_CPU" not in context.vram_optimizations
-    ):
-        model.to(context.device)
-        model.cond_stage_model.device = context.device
-
-
 def get_context_kv(attention_context):
     return attention_context, attention_context
 
-
 # modified version of https://github.com/Doggettx/stable-diffusion/blob/main/ldm/modules/attention.py#L170
 # faster iterations/sec than the default SD implementation, and consumes far less VRAM
 # On a 3060 12 GB (with the sd-v1-4.ckpt model):
 # - without this code, the standard SD sampler runs at 4.5 it/sec, and consumes ~6.6 GB of VRAM
 # - using this code makes the sampler run at 5.6 to 5.9 it/sec, and consume ~3.6 GB of VRAM on lower-end PCs, and ~4.9 GB on higher-end PCs
-def make_attn_forward(context: Context, attn_precision="fp16"):
+def make_attn_forward(context: Context, attn_precision='fp16'):
     app_context = context
 
     def get_steps(q, k):
-        if context.device == "cpu" or "SET_ATTENTION_STEP_TO_2" in context.vram_optimizations:
+        if context.device == 'cpu':
             return 2
-        elif "SET_ATTENTION_STEP_TO_4" in context.vram_optimizations:
-            return 4  # use for balanced
-        elif "SET_ATTENTION_STEP_TO_6" in context.vram_optimizations:
-            return 6
-        elif "SET_ATTENTION_STEP_TO_8" in context.vram_optimizations:
-            return 8
-        elif "SET_ATTENTION_STEP_TO_16" in context.vram_optimizations:
-            return 16
-        elif "SET_ATTENTION_STEP_TO_24" in context.vram_optimizations:
-            return 24  # use for low
+        elif 'SET_ATTENTION_STEP_TO_4' in context.vram_optimizations:
+            return 4
 
         # figure out the available memory
         stats = torch.cuda.memory_stats(q.device)
-        mem_active = stats["active_bytes.all.current"]
-        mem_reserved = stats["reserved_bytes.all.current"]
+        mem_active = stats['active_bytes.all.current']
+        mem_reserved = stats['reserved_bytes.all.current']
         mem_free_cuda, _ = torch.cuda.mem_get_info(torch.cuda.current_device())
         mem_free_torch = mem_reserved - mem_active
         mem_free_total = mem_free_cuda + mem_free_torch
 
         # figure out the required memory
-        gb = 1024**3
+        gb = 1024 ** 3
         tensor_size = q.shape[0] * q.shape[1] * k.shape[1] * q.element_size()
         modifier = 3 if q.element_size() == 2 else 2.5
         mem_required = tensor_size * modifier
 
         steps = 1
         if mem_required > mem_free_total:
             steps = 2 ** (math.ceil(math.log(mem_required / mem_free_total, 2)))
 
         if steps > 64:
             max_res = math.floor(math.sqrt(math.sqrt(mem_free_total / 2.5)) / 8) * 64
-            raise RuntimeError(
-                f"Not enough memory, use lower resolution (max approx. {max_res}x{max_res}). "
-                f"Need: {mem_required / 64 / gb:0.1f} GB free, Have:{mem_free_total / gb:0.1f} GB free"
-            )
+            raise RuntimeError(f'Not enough memory, use lower resolution (max approx. {max_res}x{max_res}). '
+                            f'Need: {mem_required / 64 / gb:0.1f} GB free, Have:{mem_free_total / gb:0.1f} GB free')
 
         return steps
 
     def forward(self, x, context=None, mask=None):
         h = self.heads
 
         q_in = self.to_q(x)
         context = default(context, x)
         context_k, context_v = get_context_kv(context)
         k_in = self.to_k(context_k)
         v_in = self.to_v(context_v)
         k_in *= self.scale
         del context, x
 
-        q, k, v = map(lambda t: rearrange(t, "b n (h d) -> (b h) n d", h=h), (q_in, k_in, v_in))
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> (b h) n d', h=h), (q_in, k_in, v_in))
         del q_in, k_in, v_in
 
-        autocast_device = "cpu" if app_context.device == "cpu" else "cuda"  # doesn't accept (or need) 'cuda:N'
+        autocast_device = 'cpu' if app_context.device == 'cpu' else 'cuda' # doesn't accept (or need) 'cuda:N'
 
         r1 = torch.zeros(q.shape[0], q.shape[1], v.shape[2], device=q.device, dtype=q.dtype)
         steps = get_steps(q, k)
         slice_size = q.shape[1] // steps if (q.shape[1] % steps) == 0 else q.shape[1]
         for i in range(0, q.shape[1], slice_size):
             end = i + slice_size
             if attn_precision == "fp32":
                 with torch.autocast(enabled=False, device_type=autocast_device):
-                    q, k = q.float(), k.float()
-                    s1 = einsum("b i d, b j d -> b i j", q[:, i:end], k)
+                    q_fp, k_fp = q[:, i:end].float(), k.float()
+                    s1 = einsum('b i d, b j d -> b i j', q_fp, k_fp)
             else:
-                s1 = einsum("b i d, b j d -> b i j", q[:, i:end], k)
+                s1 = einsum('b i d, b j d -> b i j', q[:, i:end], k)
 
             s2 = s1.softmax(dim=-1, dtype=q.dtype)
             del s1
 
-            r1[:, i:end] = einsum("b i j, b j d -> b i d", s2, v)
+            r1[:, i:end] = einsum('b i j, b j d -> b i d', s2, v)
             del s2
 
         del q, k, v
 
-        r2 = rearrange(r1, "(b h) n d -> b n (h d)", h=h)
+        r2 = rearrange(r1, '(b h) n d -> b n (h d)', h=h)
         del r1
 
         return self.to_out(r2)
 
     return forward
 
-
 def print_model_size_breakdown(model):
     """
     Useful debugging function for analyzing the memory usage of a model
     """
 
     def mb(n_bytes):
         return int(n_bytes / float(10**6))
 
     log.info(f"precision: {model.dtype}")
 
     # model
     size_input, size_middle, size_output = 0, 0, 0
     for key, val in model.model.diffusion_model.state_dict().items():
         s = val.element_size() * val.nelement()
-        if "input" in key:
+        if 'input' in key:
             size_input += s
-        elif "middle" in key:
+        elif 'middle' in key:
             size_middle += s
-        elif "output" in key:
+        elif 'output' in key:
             size_output += s
 
-    log.info(
-        f"model.diffusion_model (input, middle, output blocks): {mb(size_input)} Mb, {mb(size_middle)} Mb, {mb(size_output)} Mb"
-    )
-    log.info(f"model.diffusion_model (total): {mb(size_input + size_middle + size_output)} Mb")
+    log.info(f'model.diffusion_model (input, middle, output blocks): {mb(size_input)} Mb, {mb(size_middle)} Mb, {mb(size_output)} Mb')
+    log.info(f'model.diffusion_model (total): {mb(size_input + size_middle + size_output)} Mb')
 
     # modelFS
     sizeFS = 0
     for _, val in model.first_stage_model.state_dict().items():
         sizeFS += val.element_size() * val.nelement()
 
-    log.info(f"model.first_stage_model: {mb(sizeFS)} Mb")
+    log.info(f'model.first_stage_model: {mb(sizeFS)} Mb')
 
     # modelCS
     sizeCS = 0
     for _, val in model.cond_stage_model.state_dict().items():
         sizeCS += val.element_size() * val.nelement()
 
-    log.info(f"model.cond_stage_model: {mb(sizeCS)} Mb")
+    log.info(f'model.cond_stage_model: {mb(sizeCS)} Mb')
 
-    log.info(f"model (TOTAL): {mb(size_input + size_middle + size_output + sizeFS + sizeCS)} Mb")
+    log.info(f'model (TOTAL): {mb(size_input + size_middle + size_output + sizeFS + sizeCS)} Mb')
```

### Comparing `sdkit-1.0.84/sdkit/models/model_loader/vae.py` & `sdkit-1.0.9/sdkit/models/model_loader/vae.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,49 @@
 import os
-import tempfile
 import traceback
+import tempfile
 
 from sdkit import Context
-from sdkit.utils import load_tensor_file, log
+from sdkit.utils import log, load_tensor_file
 
 """
 The VAE model overwrites the state_dict of model.first_stage_model.
 
 We keep a copy of the original first-stage state_dict when a SD model is loaded,
 and restore that copy if the custom VAE is unloaded.
 """
 
-
 def load_model(context: Context, **kwargs):
-    vae_model_path = context.model_paths.get("vae")
+    vae_model_path = context.model_paths.get('vae')
 
     try:
         vae = load_tensor_file(vae_model_path)
-        vae = vae["state_dict"]
-
-        if context.test_diffusers:
-            from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
-                convert_ldm_vae_checkpoint,
-                create_vae_diffusers_config,
-            )
-
-            # the ckpt converter requires the VAE dict in the original SD style
-            vae_converted = {}
-            for key, value in vae.items():
-                vae_converted["first_stage_model." + key] = value
-
-            vae = vae_converted
-
-            model = context.models["stable-diffusion"]
-            m = model["default"]
-            image_size = m.vae.sample_size
-
-            original_config = model["config"]
-            vae_config = create_vae_diffusers_config(original_config, image_size=image_size)
-            vae_dict = convert_ldm_vae_checkpoint(vae, vae_config)
-
-            log.info("Loading diffusers vae")
-        else:
-            vae_dict = {k: v for k, v in vae.items() if k[0:4] != "loss"}
-
+        vae_dict = {k: v for k, v in vae["state_dict"].items() if k[0:4] != "loss"}
         if context.half_precision:
             for key in vae_dict.keys():
                 vae_dict[key] = vae_dict[key].half()
 
         _set_vae(context, vae_dict)
 
         del vae_dict
-        return {}  # we don't need to access this again
+        return {} # we don't need to access this again
     except:
         log.error(traceback.format_exc())
-        log.error(f"Could not load VAE: {vae_model_path}")
-
+        log.error(f'Could not load VAE: {vae_model_path}')
 
 def move_model_to_cpu(context: Context):
     pass
 
-
 def unload_model(context: Context, **kwargs):
     base_vae = _get_base_model_vae(context)
     _set_vae(context, base_vae)
 
-
 def _set_vae(context: Context, vae: dict):
-    if "stable-diffusion" not in context.models:
+    if 'stable-diffusion' not in context.models:
         return
 
-    model = context.models["stable-diffusion"]
-
-    if context.test_diffusers:
-        m = model["default"]
-        m.vae.load_state_dict(vae, strict=False)
-    else:
-        model.first_stage_model.load_state_dict(vae, strict=False)
-
+    model = context.models['stable-diffusion']
+    model.first_stage_model.load_state_dict(vae, strict=False)
 
 def _get_base_model_vae(context: Context):
-    base_vae = os.path.join(tempfile.gettempdir(), "sd-base-vae.safetensors")
+    base_vae = os.path.join(tempfile.gettempdir(), 'sd-base-vae.safetensors')
     return load_tensor_file(base_vae)
```

### Comparing `sdkit-1.0.84/sdkit/train/merge_models.py` & `sdkit-1.0.9/sdkit/train/merge_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,51 @@
 # loosely inspired by https://github.com/lodimasq/batch-checkpoint-merger/blob/master/batch_checkpoint_merger/main.py#L71
 
-from sdkit.utils import load_tensor_file, log, save_tensor_file
-
+from sdkit.utils import load_tensor_file, save_tensor_file
 
 def merge_models(model0_path: str, model1_path: str, ratio: float, out_path: str, use_fp16=True):
-    """
+    '''
     Merges (using weighted sum) and writes to the `out_path`.
 
     * model0, model1 - the first and second model files to be merged
     * ratio - the ratio of the second model. 1 means only the second model will be used.
               0 means only the first model will be used.
-    """
+    '''
 
-    log.info(f"[cyan]Merge models:[/cyan] Merging {model0_path} and {model1_path}, ratio {ratio}")
     merged = merge_two_models(model0_path, model1_path, ratio, use_fp16)
-
-    log.info(f"[cyan]Merge models:[/cyan] ... saving as {out_path}")
-
-    if out_path.lower().endswith(".safetensors"):
-        # elldrethSOg4060Mix_v10.ckpt contains a state_dict key among all the tensors, but safetensors
-        # assumes that all entries are tensors, not dicts => remove the key
-        if "state_dict" in merged:
-            del merged["state_dict"]
-        save_tensor_file(merged, out_path)
-    else:
-        save_tensor_file({"state_dict": merged}, out_path)
-
+    save_tensor_file(merged, out_path)
 
 # do this pair-wise, to avoid having to load all the models into memory
 def merge_two_models(model0, model1, alpha, use_fp16=True):
-    """
+    '''
     Returns a tensor containing the merged model. Uses weighted-sum.
 
     * model0, model1 - the first and second model files to be merged
     * alpha - a float between [0, 1]. 0 means only model0 will be used, 1 means only model1.
-
+    
     If model0 is a tensor, then model0 will be over-written with the merged data,
     and the same model0 reference will be returned.
-    """
+    '''
 
     model0_file = load_tensor_file(model0) if isinstance(model0, str) else model0
     model1_file = load_tensor_file(model1) if isinstance(model1, str) else model1
 
-    model0 = model0_file["state_dict"] if "state_dict" in model0_file else model0_file
-    model1 = model1_file["state_dict"] if "state_dict" in model1_file else model1_file
+    model0 = model0_file['state_dict'] if 'state_dict' in model0_file else model0_file
+    model1 = model1_file['state_dict'] if 'state_dict' in model1_file else model1_file
 
     # common weights
     for key in model0.keys():
-        if "model" in key and key in model1:
+        if 'model' in key and key in model1:
             model0[key] = (1 - alpha) * model0[key] + alpha * model1[key]
 
     for key in model1.keys():
-        if "model" in key and key not in model0:
+        if 'model' in key and key not in model1:
             model0[key] = model1[key]
 
-    if use_fp16:
-        for key, val in model0.items():
-            if "model" in key:
-                model0[key] = val.half()
-
     # unload model1 from memory
     del model1
 
+    if use_fp16:
+        for key, val in model0.items():
+            model0[key] = val.half()
+
     return model0
```

### Comparing `sdkit-1.0.84/sdkit/utils/hash_utils.py` & `sdkit-1.0.9/sdkit/utils/hash_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,50 @@
-import hashlib
 import os
-
+import hashlib
 import requests
 
-
 def hash_url_quick(url):
-    from sdkit.utils import log
-
-    log.debug(f"hashing url: {url}")
-
     def get_size():
         res = requests.get(url, stream=True)
-        size = int(res.headers["content-length"])  # fail loudly if the url doesn't return a content-length header
-        log.debug(f"total size: {size}")
-        return size
+        return int(res.headers['content-length']) # fail loudly if the url doesn't return a content-length header
 
     def read_bytes(offset: int, count: int):
         res = requests.get(url, headers={"Range": f"bytes={offset}-{offset+count-1}"})
-        log.debug(f"read byte range. offset: {offset}, count: {count}, actual count: {len(res.content)}")
         return res.content
 
     return compute_quick_hash(
         total_size_fn=get_size,
         read_bytes_fn=read_bytes,
     )
 
-
 def hash_file_quick(file_path):
-    from sdkit.utils import log
-
-    log.debug(f"hashing file: {file_path}")
-
-    def get_size():
-        size = os.path.getsize(file_path)
-        log.debug(f"total size: {size}")
-        return size
-
     def read_bytes(offset: int, count: int):
-        with open(file_path, "rb") as f:
+        with open(file_path, 'rb') as f:
             f.seek(offset)
             bytes = f.read(count)
-            log.debug(f"read byte range. offset: {offset}, count: {count}, actual count: {len(bytes)}")
             return bytes
 
     return compute_quick_hash(
-        total_size_fn=get_size,
+        total_size_fn=lambda: os.path.getsize(file_path),
         read_bytes_fn=read_bytes,
     )
 
-
 def compute_quick_hash(total_size_fn, read_bytes_fn):
-    """
+    '''
     quick-hash logic:
     - read 64k chunks from the start, middle and end, and hash them
     - start offset: 1 MB
     - middle offset: 0
     - end offset: -1 MB
 
     Do not use if the file size is less than 3 MB
-    """
+    '''
     total_size = total_size_fn()
 
-    if total_size < 0x300000:
-        all_bytes = read_bytes_fn(offset=0, count=total_size)
-        return hash_bytes(all_bytes)
-    else:
-        start_bytes = read_bytes_fn(offset=0x100000, count=0x10000)
-        middle_bytes = read_bytes_fn(offset=int(total_size / 2), count=0x10000)
-        end_bytes = read_bytes_fn(offset=total_size - 0x100000, count=0x10000)
-
-        return hash_bytes(start_bytes + middle_bytes + end_bytes)
+    start_bytes = read_bytes_fn(offset=0x100000, count=0x10000)
+    middle_bytes = read_bytes_fn(offset=int(total_size/2), count=0x10000)
+    end_bytes = read_bytes_fn(offset=total_size - 0x100000, count=0x10000)
 
+    return hash_bytes(start_bytes + middle_bytes + end_bytes)
 
 def hash_bytes(bytes):
     return hashlib.sha256(bytes).hexdigest()
```

### Comparing `sdkit-1.0.84/sdkit/utils/http_utils.py` & `sdkit-1.0.9/sdkit/utils/http_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-import os
-from shutil import copyfileobj
-
 import requests
+import os
 from tqdm import tqdm
-
+from shutil import copyfileobj
 
 def download_file(url: str, out_path: str):
-    """
+    '''
     Features:
     * Downloads large files (without storing them in memory)
     * Resumes downloads from the bytes it has downloaded already
     * Shows a progress bar
 
     The remote server needs to support the `Range` header, for resume to work.
-    """
+    '''
     from sdkit.utils import log
 
     start_offset = 0 if not os.path.exists(out_path) else os.path.getsize(out_path)
-    res = requests.get(url, stream=True)
-    if not res.ok:
-        return
-    total_bytes = int(res.headers.get("Content-Length", "0"))
-
-    res = requests.get(url, stream=True, headers={"Range": f"bytes={start_offset}-", "Accept-Encoding": "identity"})
-    if not res.ok:
-        return
-
-    write_mode = "wb" if start_offset == 0 else "ab"
+    res = requests.get(url, stream=True, headers={'Range': f'bytes={start_offset}-', 'Accept-Encoding': 'identity'})
+    total_bytes = int(res.headers.get('Content-Length', '0'))
+    write_mode = 'wb' if start_offset == 0 else 'ab'
 
-    log.info(f"Downloading {url} to {out_path}")
-    with open(out_path, write_mode) as f, tqdm.wrapattr(
-        res.raw, "read", initial=start_offset, total=total_bytes, desc="Downloading", colour="green"
-    ) as res_stream:
+    log.info(f'Downloading {url} to {out_path}')
+    with open(out_path, write_mode) as f, tqdm.wrapattr(res.raw, 'read', initial=start_offset, total=total_bytes, desc='Downloading', colour='green') as res_stream:
         copyfileobj(res_stream, f)
```

### Comparing `sdkit-1.0.84/sdkit/utils/image_utils.py` & `sdkit-1.0.9/sdkit/utils/image_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,56 @@
+import numpy as np
+import cv2
+from skimage import exposure
 import base64
-import re
 from io import BytesIO
-
-import cv2
-import numpy as np
 from PIL import Image
-from skimage import exposure
-
 
 # https://stackoverflow.com/a/61114178
-def img_to_base64_str(img, output_format="PNG", output_quality=75, output_lossless=False):
-    buffered = img_to_buffer(img, output_format, output_quality=output_quality, output_lossless=output_lossless)
+def img_to_base64_str(img, output_format="PNG", output_quality=75):
+    buffered = img_to_buffer(img, output_format, output_quality=output_quality)
     return buffer_to_base64_str(buffered, output_format)
 
-
-def img_to_buffer(img, output_format="PNG", output_quality=75, output_lossless=False):
+def img_to_buffer(img, output_format="PNG", output_quality=75):
     buffered = BytesIO()
-    if output_format.upper() == "PNG":
-        img.save(buffered, format=output_format)
-    elif output_format.upper() == "WEBP":
-        img.save(buffered, format=output_format, quality=output_quality, lossless=output_lossless)
-    else:
+    if output_format.upper() == "JPEG":
         img.save(buffered, format=output_format, quality=output_quality)
+    else:
+        img.save(buffered, format=output_format)
     buffered.seek(0)
     return buffered
 
-
 def buffer_to_base64_str(buffered, output_format="PNG"):
     buffered.seek(0)
     img_byte = buffered.getvalue()
-    mime_type = f"image/{output_format.lower()}"
+    mime_type = "image/png" if output_format.lower() == "png" else "image/jpeg"
     img_str = f"data:{mime_type};base64," + base64.b64encode(img_byte).decode()
     return img_str
 
-
 def base64_str_to_buffer(img_str):
-    img_str = re.sub(r"^data:image/[a-z]+;base64,", "", img_str)
+    mime_type = "image/png" if img_str.startswith("data:image/png;") else "image/jpeg"
+    img_str = img_str[len(f"data:{mime_type};base64,"):]
     data = base64.b64decode(img_str)
     buffered = BytesIO(data)
     return buffered
 
-
 def base64_str_to_img(img_str):
     buffered = base64_str_to_buffer(img_str)
     img = Image.open(buffered)
     return img
 
-
-def resize_img(img: Image, desired_width, desired_height, clamp_to_64=False):
+def resize_img(img: Image, desired_width, desired_height):
     w, h = img.size
 
     if desired_width is not None and desired_height is not None:
         w, h = desired_width, desired_height
 
-    if clamp_to_64:
-        w, h = map(lambda x: x - x % 64, (w, h))  # resize to integer multiple of 64
+    w, h = map(lambda x: x - x % 64, (w, h))  # resize to integer multiple of 64
 
     return img.resize((w, h), resample=Image.Resampling.LANCZOS)
 
-
 def apply_color_profile(orig_image: Image, image_to_modify: Image):
     reference = cv2.cvtColor(np.asarray(orig_image), cv2.COLOR_RGB2LAB)
     image_to_modify = cv2.cvtColor(np.asarray(image_to_modify), cv2.COLOR_RGB2LAB)
     matched = exposure.match_histograms(image_to_modify, reference, channel_axis=2)
 
     return Image.fromarray(cv2.cvtColor(matched, cv2.COLOR_LAB2RGB).astype("uint8"))
```

### Comparing `sdkit-1.0.84/sdkit.egg-info/PKG-INFO` & `sdkit-1.0.9/sdkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.84
+Version: 1.0.9
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sdkit
 **sdkit** (**s**table **d**iffusion **kit**) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient.
 
@@ -24,27 +23,25 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
-Tested with Python 3.8. Supports Windows, Linux and Mac.
+Tested with Python 3.8.
 
-**Windows/Linux:**
-1. `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
+1. On Windows and Linux only: `pip install torch torchvision --extra-index-url https://download.pytorch.org/whl/cu116`
 2. Run `pip install sdkit`
 
-**Mac:**
-1. Run `pip install sdkit`
+We don't support Mac yet, but we'd love to accept code contributions!
 
 # Example
 ### Local model
 A simple example for generating an image from a Stable Diffusion model file (already present on the disk):
 ```python
 import sdkit
 from sdkit.models import load_model
@@ -110,15 +107,15 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, multiple GPU support, gfpgan (fix faces), realesrgan (upscale), 14 samplers (including k-samplers), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
 📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
@@ -131,47 +128,50 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
-You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
+You can certainly use diffusers. `sdkit` is just a different attempt at a productive toolkit, so use `sdkit` if you find its features useful.
 
 `sdkit`:
-1. is a simple, lightweight toolkit for Stable Diffusion projects.
+1. is a fresh attempt at a simple, lightweight toolkit for Stable Diffusion projects.
 2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
-3. works with the popular `.ckpt` and `.safetensors` model format.
+3. works with the popular `.ckpt` and `.safetensors` model format (instead of only the diffusers format).
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
-8. includes 19 samplers (including k-samplers).
+8. includes 14 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
 
+This is not to say that `diffusers` doesn't do these. The easy-to-use API of `diffusers` is an inspiration for `sdkit`.
+
 # Who is using sdkit?
-* [Easy Diffusion (cmdr2 UI)](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
-* [aipromptstudio.com](https://aipromptstudio.com/)
+* [cmdr2 UI](https://github.com/cmdr2/stable-diffusion-ui) for Stable Diffusion.
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
 - CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
 - Seamless tiling.
 - Outpainting.
+- Mac support.
 - AMD support.
+- Allow other samplers for img2img (instead of only DDIM).
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
```

