# Comparing `tmp/ricecooker-0.7.1.tar.gz` & `tmp/ricecooker-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ricecooker-0.7.1.tar", last modified: Wed Feb  1 00:56:22 2023, max compression
+gzip compressed data, was "dist/ricecooker-0.7.2.tar", last modified: Wed May  3 02:22:10 2023, max compression
```

## Comparing `ricecooker-0.7.1.tar` & `ricecooker-0.7.2.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2023-02-01 00:56:13.000000 ricecooker-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      348 2023-02-01 00:56:13.000000 ricecooker-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3325 2023-02-01 00:56:13.000000 ricecooker-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2506 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)    26802 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     1908 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_csv_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/chefs/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/chefs/fake_chef.py
--rw-r--r--   0 runner    (1001) docker     (116)     2552 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (116)    12165 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_pdfutils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5078 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_chef_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)     3078 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_links.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (116)    23858 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/
--rw-r--r--   0 runner    (1001) docker     (116)   114608 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (116)    37428 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg
--rw-r--r--   0 runner    (1001) docker     (116)     1929 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv
--rw-r--r--   0 runner    (1001) docker     (116)      488 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/Content.csv
--rw-r--r--   0 runner    (1001) docker     (116)      266 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/Channel.csv
--rw-r--r--   0 runner    (1001) docker     (116)      979 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/Exercises.csv
--rw-r--r--   0 runner    (1001) docker     (116)    19221 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (116)    19584 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (116)    23745 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_exercises.py
--rw-r--r--   0 runner    (1001) docker     (116)     3447 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (116)     2279 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     4046 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (116)    12965 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_videos.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/
--rw-r--r--   0 runner    (1001) docker     (116)     8924 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (116)     5244 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_web.py
--rw-r--r--   0 runner    (1001) docker     (116)     5117 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3056 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10156 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_videos.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (116)    49913 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/thumbnails/toowide.png
--rw-r--r--   0 runner    (1001) docker     (116)    63258 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/thumbnails/tootall.png
--rw-r--r--   0 runner    (1001) docker     (116)   142272 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/thumbnails/toosquare.png
--rw-r--r--   0 runner    (1001) docker     (116)   163118 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/thumbnails/BRAlogo1.png
--rw-r--r--   0 runner    (1001) docker     (116)    27648 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/Wilhelm_Scream.mp3
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/
--rw-r--r--   0 runner    (1001) docker     (116)   318539 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.epub
--rw-r--r--   0 runner    (1001) docker     (116)     7519 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.pdf
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.zip
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/
--rw-r--r--   0 runner    (1001) docker     (116)    22759 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/basic.srt
--rw-r--r--   0 runner    (1001) docker     (116)     1183 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/encapsulated.sami
--rw-r--r--   0 runner    (1001) docker     (116)      470 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/encapsulated.vtt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/not.txt
--rw-r--r--   0 runner    (1001) docker     (116)    20575 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/basic.vtt
--rw-r--r--   0 runner    (1001) docker     (116)      736 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/subtitles/empty.ttml
--rw-r--r--   0 runner    (1001) docker     (116)     1065 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/page_with_links.html
--rw-r--r--   0 runner    (1001) docker     (116)  5033338 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/kepub.epub
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/audio/
--rw-r--r--   0 runner    (1001) docker     (116)   764176 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/audio/file_example_MP3_700KB.mp3
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/assets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/assets/images/
--rw-r--r--   0 runner    (1001) docker     (116)       86 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/assets/images/copyright.txt
--rw-r--r--   0 runner    (1001) docker     (116)    15108 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/assets/css/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/assets/css/empty.css
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/assets/css/empty2.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/tests/media_utils/files/assets/js/
--rw-r--r--   0 runner    (1001) docker     (116)       60 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/assets/js/empty.js
--rw-r--r--   0 runner    (1001) docker     (116)      104 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/files/file_metadata.txt
--rw-r--r--   0 runner    (1001) docker     (116)    11697 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/media_utils/test_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (116)    15234 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (116)     9495 2023-02-01 00:56:13.000000 ricecooker-0.7.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    14115 2023-02-01 00:56:22.000000 ricecooker-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2242 2023-02-01 00:56:13.000000 ricecooker-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      487 2023-02-01 00:56:13.000000 ricecooker-0.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)      488 2023-02-01 00:56:22.000000 ricecooker-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker/classes/
--rw-r--r--   0 runner    (1001) docker     (116)    25149 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/classes/questions.py
--rw-r--r--   0 runner    (1001) docker     (116)    52445 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/classes/files.py
--rw-r--r--   0 runner    (1001) docker     (116)    61722 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/classes/nodes.py
--rw-r--r--   0 runner    (1001) docker     (116)     7384 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/classes/licenses.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7641 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    14047 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/commands.py
--rw-r--r--   0 runner    (1001) docker     (116)     2204 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    14074 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker/templates/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker/utils/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1240 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/kolibripreview.py
--rw-r--r--   0 runner    (1001) docker     (116)    16945 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/jsontrees.py
--rw-r--r--   0 runner    (1001) docker     (116)    15485 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/linecook.py
--rw-r--r--   0 runner    (1001) docker     (116)     4419 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/html_writer.py
--rw-r--r--   0 runner    (1001) docker     (116)    22252 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/youtube.py
--rw-r--r--   0 runner    (1001) docker     (116)    10204 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/thumbscropping.py
--rw-r--r--   0 runner    (1001) docker     (116)     8160 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/videos.py
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (116)     9076 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/libstudio.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    25289 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/corrections.py
--rw-r--r--   0 runner    (1001) docker     (116)      643 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7680 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (116)     1315 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (116)     1807 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (116)     1351 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/encodings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/browser.py
--rw-r--r--   0 runner    (1001) docker     (116)    37125 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)     9018 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2196 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (116)     9222 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (116)     6188 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10055 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (116)     3199 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/web.py
--rw-r--r--   0 runner    (1001) docker     (116)    41077 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     3148 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (116)    37099 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/chefs.py
--rw-r--r--   0 runner    (1001) docker     (116)      230 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker/managers/
--rw-r--r--   0 runner    (1001) docker     (116)    18134 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/managers/tree.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8758 2023-02-01 00:56:13.000000 ricecooker-0.7.1/ricecooker/managers/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)    21943 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/nodes.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (116)     7434 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/uploadprocess.md
--rw-r--r--   0 runner    (1001) docker     (116)     4499 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/corrections.md
--rw-r--r--   0 runner    (1001) docker     (116)     5571 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/kolibripreview.md
--rw-r--r--   0 runner    (1001) docker     (116)     5510 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/design_cli.md
--rw-r--r--   0 runner    (1001) docker     (116)     5486 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/ids.md
--rw-r--r--   0 runner    (1001) docker     (116)     2401 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/sushops.md
--rw-r--r--   0 runner    (1001) docker     (116)      252 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)    14760 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/htmlapps.md
--rw-r--r--   0 runner    (1001) docker     (116)    19873 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     6467 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)      947 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/index_api_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2716 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      311 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/index_utils.rst
--rw-r--r--   0 runner    (1001) docker     (116)     8008 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (116)      687 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (116)    10452 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/explanations.md
--rw-r--r--   0 runner    (1001) docker     (116)    13376 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1760 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/jiro.md
--rw-r--r--   0 runner    (1001) docker     (116)     4626 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (116)      207 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5073 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (116)      614 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (116)     7221 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/chefops.md
--rw-r--r--   0 runner    (1001) docker     (116)      298 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/404.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4007 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/parsing_html.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/figures/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/figures/HandBrake/
--rw-r--r--   0 runner    (1001) docker     (116)    48626 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/HandBrake/handbreake_audio_settings.png
--rw-r--r--   0 runner    (1001) docker     (116)   113089 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/HandBrake/handbrake_steps.png
--rw-r--r--   0 runner    (1001) docker     (116)    52981 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/HandBrake/handbreake_resizing_settings.png
--rw-r--r--   0 runner    (1001) docker     (116)   242328 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/HandBrake/handbreake_screenshot_video_settings.png
--rw-r--r--   0 runner    (1001) docker     (116)     9314 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/kolibri_logo.png
--rw-r--r--   0 runner    (1001) docker     (116)   144375 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/content_pipeline_diagram_with_highlight.png
--rw-r--r--   0 runner    (1001) docker     (116)   128604 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/content_pipeline_diagram.png
--rw-r--r--   0 runner    (1001) docker     (116)    39710 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/figures/ricecooker_domain.png
--rw-r--r--   0 runner    (1001) docker     (116)     5077 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/pdfutils.md
--rw-r--r--   0 runner    (1001) docker     (116)     5306 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/downloader.md
--rw-r--r--   0 runner    (1001) docker     (116)     7621 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (116)     3177 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/terminology.md
--rw-r--r--   0 runner    (1001) docker     (116)     4347 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/content_workflows.md
--rw-r--r--   0 runner    (1001) docker     (116)     2962 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/introduction.md
--rw-r--r--   0 runner    (1001) docker     (116)     7656 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/developer_workflows.md
--rw-r--r--   0 runner    (1001) docker     (116)     3407 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/reviewing_channels.md
--rw-r--r--   0 runner    (1001) docker     (116)      445 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/concepts/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/csv_metadata/
--rw-r--r--   0 runner    (1001) docker     (116)     5043 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/csv_metadata/csv_exercises.md
--rw-r--r--   0 runner    (1001) docker     (116)     1369 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/csv_metadata/csv_workflow.md
--rw-r--r--   0 runner    (1001) docker     (116)      279 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/csv_metadata/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      119 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/csv_metadata/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9709 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/files.md
--rw-r--r--   0 runner    (1001) docker     (116)     3511 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/exercises.md
--rw-r--r--   0 runner    (1001) docker     (116)     2485 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/languages.md
--rw-r--r--   0 runner    (1001) docker     (116)     6580 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/docs/community/
--rw-r--r--   0 runner    (1001) docker     (116)      381 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/community/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)    13551 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/video_compression.md
--rw-r--r--   0 runner    (1001) docker     (116)      856 2023-02-01 00:56:13.000000 ricecooker-0.7.1/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       11 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14115 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      444 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5320 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      105 2023-02-01 00:56:22.000000 ricecooker-0.7.1/ricecooker.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 02:21:59.000000 ricecooker-0.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 02:21:59.000000 ricecooker-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 02:21:59.000000 ricecooker-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-03 02:22:10.000000 ricecooker-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-03 02:21:59.000000 ricecooker-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/404.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/chefops.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/community/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/content_workflows.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/developer_workflows.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/reviewing_channels.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/terminology.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/csv_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/csv_exercises.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/csv_workflow.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/corrections.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/design_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/ids.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/kolibripreview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/sushops.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/uploadprocess.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/downloader.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/exercises.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/figures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/figures/HandBrake/
+-rw-r--r--   0 runner    (1001) docker     (123)   113089 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbrake_steps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48626 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_audio_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52981 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_resizing_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   242328 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_screenshot_video_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   128604 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/content_pipeline_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   144375 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/content_pipeline_diagram_with_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/kolibri_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39710 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/ricecooker_domain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/files.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/htmlapps.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index_api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/languages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/nodes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/parsing_html.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/pdfutils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/jiro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/video_compression.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37099 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/chefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52387 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25149 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/questions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/caching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25289 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37125 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/html_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/jsontrees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/kolibripreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/libstudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/linecook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41077 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/thumbscropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 02:22:10.000000 ricecooker-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-03 02:21:59.000000 ricecooker-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/chefs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/chefs/fake_chef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26802 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/Wilhelm_Scream.mp3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/empty.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/empty2.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/copyright.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/js/empty.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)   764176 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/audio/file_example_MP3_700KB.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/file_metadata.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/
+-rw-r--r--   0 runner    (1001) docker     (123)   318539 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.epub
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.zip
+-rw-r--r--   0 runner    (1001) docker     (123)  5033338 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/kepub.epub
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/page_with_links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.srt
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.vtt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/empty.ttml
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.sami
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.vtt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/not.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)   163118 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/BRAlogo1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142272 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/toosquare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63258 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/tootall.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/toowide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_chef_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_csv_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23745 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_exercises.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19221 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_pdfutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19584 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Channel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Content.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Exercises.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/
+-rw-r--r--   0 runner    (1001) docker     (123)    23858 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)   114608 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/.gitkeep
```

### Comparing `ricecooker-0.7.1/LICENSE` & `ricecooker-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/README.md` & `ricecooker-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_downloader.py` & `ricecooker-0.7.2/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/conftest.py` & `ricecooker-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_csv_metadata.py` & `ricecooker-0.7.2/tests/test_csv_metadata.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_youtube.py` & `ricecooker-0.7.2/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_requests.py` & `ricecooker-0.7.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_pdfutils.py` & `ricecooker-0.7.2/tests/test_pdfutils.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_chef_integration.py` & `ricecooker-0.7.2/tests/test_chef_integration.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_links.py` & `ricecooker-0.7.2/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png` & `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png` & `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg` & `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv` & `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/testchannels/csv_channel_with_exercises/Exercises.csv` & `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Exercises.csv`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_files.py` & `ricecooker-0.7.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_tree.py` & `ricecooker-0.7.2/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_exercises.py` & `ricecooker-0.7.2/tests/test_exercises.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_licenses.py` & `ricecooker-0.7.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_settings.py` & `ricecooker-0.7.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_argparse.py` & `ricecooker-0.7.2/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_videos.py` & `ricecooker-0.7.2/tests/test_videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_youtube.py` & `ricecooker-0.7.2/tests/media_utils/test_youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/README.md` & `ricecooker-0.7.2/tests/media_utils/README.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_web.py` & `ricecooker-0.7.2/tests/media_utils/test_web.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_subtitles.py` & `ricecooker-0.7.2/tests/media_utils/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_proxy.py` & `ricecooker-0.7.2/tests/media_utils/test_proxy.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_audio.py` & `ricecooker-0.7.2/tests/media_utils/test_audio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_videos.py` & `ricecooker-0.7.2/tests/media_utils/test_videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/thumbnails/toowide.png` & `ricecooker-0.7.2/tests/media_utils/files/thumbnails/toowide.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/thumbnails/tootall.png` & `ricecooker-0.7.2/tests/media_utils/files/thumbnails/tootall.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/thumbnails/toosquare.png` & `ricecooker-0.7.2/tests/media_utils/files/thumbnails/toosquare.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/thumbnails/BRAlogo1.png` & `ricecooker-0.7.2/tests/media_utils/files/thumbnails/BRAlogo1.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/Wilhelm_Scream.mp3` & `ricecooker-0.7.2/tests/media_utils/files/Wilhelm_Scream.mp3`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.epub` & `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.epub`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.pdf` & `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.pdf`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/generate_thumbnail/sample.zip` & `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.zip`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/subtitles/basic.srt` & `ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.srt`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/subtitles/encapsulated.sami` & `ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.sami`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/subtitles/basic.vtt` & `ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.vtt`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/subtitles/empty.ttml` & `ricecooker-0.7.2/tests/media_utils/files/subtitles/empty.ttml`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/page_with_links.html` & `ricecooker-0.7.2/tests/media_utils/files/page_with_links.html`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/kepub.epub` & `ricecooker-0.7.2/tests/media_utils/files/kepub.epub`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/audio/file_example_MP3_700KB.mp3` & `ricecooker-0.7.2/tests/media_utils/files/audio/file_example_MP3_700KB.mp3`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg` & `ricecooker-0.7.2/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/media_utils/test_thumbnails.py` & `ricecooker-0.7.2/tests/media_utils/test_thumbnails.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_thumbnails.py` & `ricecooker-0.7.2/tests/test_thumbnails.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/tests/test_data.py` & `ricecooker-0.7.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/PKG-INFO` & `ricecooker-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricecooker
-Version: 0.7.1
+Version: 0.7.2
 Summary: API for adding content to the Kolibri content curation server
 Home-page: https://github.com/learningequality/ricecooker
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT license
 Description: ricecooker
         ==========
@@ -260,14 +260,15 @@
         * First release on PyPI.
         
 Keywords: ricecooker
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Topic :: Education
-Requires-Python: >=3.6, <3.11
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
```

### Comparing `ricecooker-0.7.1/setup.py` & `ricecooker-0.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     "pytest>=3.0.2",
     "requests>=2.11.1",
     "le_utils>=0.1.26",
     "validators",  # TODO: check if this is necessary
     "requests_file",
     "beautifulsoup4>=4.6.3,<4.9.0",  # pinned to match versions in le-pycaption
     "selenium==3.0.1",
-    "youtube-dl>=2020.6.16.1",
-    "yt-dlp==2022.03.08.1",
+    "yt-dlp>=2023.3.4",
     "html5lib",
     "cachecontrol==0.12.0",
     "lockfile==0.12.2",  # TODO: check if this is necessary
     "css-html-js-minify==2.2.2",
     "mock==2.0.0",
     "pypdf2==1.26.0",
     "dictdiffer>=0.8.0",
@@ -56,23 +55,24 @@
         "console_scripts": [
             "corrections = ricecooker.utils.corrections:correctionsmain",
             "jiro = ricecooker.cli:main",
         ]
     },
     include_package_data=True,
     install_requires=requirements,
-    python_requires=">=3.6, <3.11",
+    python_requires=">=3.7, <3.11",
     license="MIT license",
     zip_safe=False,
     keywords="ricecooker",
     classifiers=[
         "Intended Audience :: Developers",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Natural Language :: English",
         "Topic :: Education",
     ],
     test_suite="tests",
 )
```

### Comparing `ricecooker-0.7.1/ricecooker/classes/questions.py` & `ricecooker-0.7.2/ricecooker/classes/questions.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/classes/files.py` & `ricecooker-0.7.2/ricecooker/classes/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import zipfile
 from contextlib import contextmanager
 from functools import partial
 from urllib.parse import urlparse
 from xml.etree import ElementTree
 
 import filetype
-import youtube_dl
+import yt_dlp
 from cachecontrol.caches.file_cache import FileCache
 from le_utils.constants import exercises
 from le_utils.constants import file_formats
 from le_utils.constants import format_presets
 from le_utils.constants import languages
 from PIL import Image
 from PIL import UnidentifiedImageError
@@ -429,35 +429,33 @@
         os.remove(outtmpl_path)
     if os.path.exists(destination_path):
         os.remove(destination_path)
 
     # Download the web_url which can be either a video or subtitles
     if not config.USEPROXY:
         # Connect to YouTube directly
-        with youtube_dl.YoutubeDL(download_settings) as ydl:
+        with yt_dlp.YoutubeDL(download_settings) as ydl:
             ydl.download([web_url])
             if not os.path.exists(destination_path):
-                raise youtube_dl.utils.DownloadError("Failed to download " + web_url)
+                raise yt_dlp.utils.DownloadError("Failed to download " + web_url)
     else:
         # Connect to YouTube via an HTTP proxy
         yt_resource = YouTubeResource(web_url, useproxy=True, options=download_settings)
         result1 = yt_resource.get_resource_info()
         if result1 is None:
-            raise youtube_dl.utils.DownloadError("Failed to get resource info")
+            raise yt_dlp.utils.DownloadError("Failed to get resource info")
         download_settings["writethumbnail"] = False  # overwrite default behaviour
         if file_format == file_formats.VTT:
             # We need to use the proxy when downloading subtitles
             result2 = yt_resource.download(options=download_settings, useproxy=True)
         else:
             # For video files we can skip the proxy for faster download speed
             result2 = yt_resource.download(options=download_settings)
         if result2 is None or not os.path.exists(destination_path):
-            raise youtube_dl.utils.DownloadError(
-                "Failed to download resource " + web_url
-            )
+            raise yt_dlp.utils.DownloadError("Failed to download resource " + web_url)
 
     # Write file to local storage
     filename = copy_file_to_storage(destination_path, ext=file_format)
 
     FILECACHE.set(key, bytes(filename, "utf-8"))
     return filename
 
@@ -929,15 +927,15 @@
                 config.LOGGER.info("\t--- Compressed {}".format(self.filename))
             if self.filename and config.get_storage_path(self.filename):
                 self.duration = extract_duration_of_media(
                     config.get_storage_path(self.filename),
                     extract_path_ext(self.filename),
                 )
 
-        except (youtube_dl.utils.DownloadError, VideoCompressionError) as err:
+        except (yt_dlp.utils.DownloadError, VideoCompressionError) as err:
             self.filename = None
             self.error = str(err)
             config.FAILED_FILES.append(self)
 
         return self.filename
 
 
@@ -1005,15 +1003,15 @@
         return self.preset or format_presets.VIDEO_SUBTITLE
 
     def process_file(self):
         try:
             self.filename = self.download_subtitle()
             config.LOGGER.info("\t--- Downloaded subtitle {}".format(self.filename))
             return self.filename
-        except (FileNotFoundError, youtube_dl.utils.DownloadError):
+        except (FileNotFoundError, yt_dlp.utils.DownloadError):
             self.error = str(
                 "Subtitle with langauge {} is not available for {}".format(
                     self.language, self.youtube_url
                 )
             )
             config.FAILED_FILES.append(self)
```

### Comparing `ricecooker-0.7.1/ricecooker/classes/nodes.py` & `ricecooker-0.7.2/ricecooker/classes/nodes.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/classes/licenses.py` & `ricecooker-0.7.2/ricecooker/classes/licenses.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/cli.py` & `ricecooker-0.7.2/ricecooker/cli.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/commands.py` & `ricecooker-0.7.2/ricecooker/commands.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/exceptions.py` & `ricecooker-0.7.2/ricecooker/exceptions.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/config.py` & `ricecooker-0.7.2/ricecooker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 FAILED_FILES = []
 
 # Session for downloading files
 DOWNLOAD_SESSION = requests.Session()
 DOWNLOAD_SESSION.mount("file://", FileAdapter())
 
-# Environment variable indicating we should use a proxy for youtube_dl downloads
+# Environment variable indicating we should use a proxy for yt_dlp downloads
 USEPROXY = False
 USEPROXY = (
     True
     if os.getenv("USEPROXY") is not None or os.getenv("PROXY_LIST") is not None
     else False
 )
```

### Comparing `ricecooker-0.7.1/ricecooker/utils/kolibripreview.py` & `ricecooker-0.7.2/ricecooker/utils/kolibripreview.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/jsontrees.py` & `ricecooker-0.7.2/ricecooker/utils/jsontrees.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,29 +51,29 @@
 ################################################################################
 
 
 def read_tree_from_json(srcpath):
     """
     Load ricecooker json tree data from json file at `srcpath`.
     """
-    with open(srcpath) as infile:
+    with open(srcpath, encoding="utf-8") as infile:
         json_tree = json.load(infile)
         if json_tree is None:
             raise ValueError("Could not find ricecooker json tree")
     return json_tree
 
 
 def write_tree_to_json_tree(destpath, json_tree):
     """
     Save contents of `json_tree` (dict) to json file at `destpath`.
     """
     parent_dir, _ = os.path.split(destpath)
     if not os.path.exists(parent_dir):
         os.makedirs(parent_dir, exist_ok=True)
-    with open(destpath, "w", encoding="utf8") as json_file:
+    with open(destpath, "w", encoding="utf-8") as json_file:
         json.dump(json_tree, json_file, indent=2, ensure_ascii=False)
 
 
 # CONSTRUCT CHANNEL FROM RICECOOKER JSON TREE
 ################################################################################
```

### Comparing `ricecooker-0.7.1/ricecooker/utils/linecook.py` & `ricecooker-0.7.2/ricecooker/utils/linecook.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/html_writer.py` & `ricecooker-0.7.2/ricecooker/utils/html_writer.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/youtube.py` & `ricecooker-0.7.2/ricecooker/utils/youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/thumbscropping.py` & `ricecooker-0.7.2/ricecooker/utils/thumbscropping.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/videos.py` & `ricecooker-0.7.2/ricecooker/utils/videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/tokens.py` & `ricecooker-0.7.2/ricecooker/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/libstudio.py` & `ricecooker-0.7.2/ricecooker/utils/libstudio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/corrections.py` & `ricecooker-0.7.2/ricecooker/utils/corrections.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/utils.py` & `ricecooker-0.7.2/ricecooker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/images.py` & `ricecooker-0.7.2/ricecooker/utils/images.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/paths.py` & `ricecooker-0.7.2/ricecooker/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/caching.py` & `ricecooker-0.7.2/ricecooker/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/encodings.py` & `ricecooker-0.7.2/ricecooker/utils/encodings.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/browser.py` & `ricecooker-0.7.2/ricecooker/utils/browser.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/downloader.py` & `ricecooker-0.7.2/ricecooker/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/pdf.py` & `ricecooker-0.7.2/ricecooker/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/audio.py` & `ricecooker-0.7.2/ricecooker/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/subtitles.py` & `ricecooker-0.7.2/ricecooker/utils/subtitles.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/proxy.py` & `ricecooker-0.7.2/ricecooker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/html.py` & `ricecooker-0.7.2/ricecooker/utils/html.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/web.py` & `ricecooker-0.7.2/ricecooker/utils/web.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/metadata_provider.py` & `ricecooker-0.7.2/ricecooker/utils/metadata_provider.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/utils/zip.py` & `ricecooker-0.7.2/ricecooker/utils/zip.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/chefs.py` & `ricecooker-0.7.2/ricecooker/chefs.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/managers/tree.py` & `ricecooker-0.7.2/ricecooker/managers/tree.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker/managers/progress.py` & `ricecooker-0.7.2/ricecooker/managers/progress.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/nodes.md` & `ricecooker-0.7.2/docs/nodes.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/uploadprocess.md` & `ricecooker-0.7.2/docs/developer/uploadprocess.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/corrections.md` & `ricecooker-0.7.2/docs/developer/corrections.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/kolibripreview.md` & `ricecooker-0.7.2/docs/developer/kolibripreview.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/design_cli.md` & `ricecooker-0.7.2/docs/developer/design_cli.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/ids.md` & `ricecooker-0.7.2/docs/developer/ids.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/developer/sushops.md` & `ricecooker-0.7.2/docs/developer/sushops.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/htmlapps.md` & `ricecooker-0.7.2/docs/htmlapps.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/conf.py` & `ricecooker-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/make.bat` & `ricecooker-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/index_api_reference.rst` & `ricecooker-0.7.2/docs/index_api_reference.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/examples/index.rst` & `ricecooker-0.7.2/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/history.rst` & `ricecooker-0.7.2/docs/history.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/tutorial/quickstart.rst` & `ricecooker-0.7.2/docs/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/tutorial/explanations.md` & `ricecooker-0.7.2/docs/tutorial/explanations.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/tutorial/gettingstarted.rst` & `ricecooker-0.7.2/docs/tutorial/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/tutorial/jiro.md` & `ricecooker-0.7.2/docs/tutorial/jiro.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/tutorial/tutorial.rst` & `ricecooker-0.7.2/docs/tutorial/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/installation.md` & `ricecooker-0.7.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/usage.md` & `ricecooker-0.7.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/chefops.md` & `ricecooker-0.7.2/docs/chefops.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/parsing_html.md` & `ricecooker-0.7.2/docs/parsing_html.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/HandBrake/handbreake_audio_settings.png` & `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_audio_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/HandBrake/handbrake_steps.png` & `ricecooker-0.7.2/docs/figures/HandBrake/handbrake_steps.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/HandBrake/handbreake_resizing_settings.png` & `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_resizing_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/HandBrake/handbreake_screenshot_video_settings.png` & `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_screenshot_video_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/kolibri_logo.png` & `ricecooker-0.7.2/docs/figures/kolibri_logo.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/content_pipeline_diagram_with_highlight.png` & `ricecooker-0.7.2/docs/figures/content_pipeline_diagram_with_highlight.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/content_pipeline_diagram.png` & `ricecooker-0.7.2/docs/figures/content_pipeline_diagram.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/figures/ricecooker_domain.png` & `ricecooker-0.7.2/docs/figures/ricecooker_domain.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/pdfutils.md` & `ricecooker-0.7.2/docs/pdfutils.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/downloader.md` & `ricecooker-0.7.2/docs/downloader.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/Makefile` & `ricecooker-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/concepts/terminology.md` & `ricecooker-0.7.2/docs/concepts/terminology.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/concepts/content_workflows.md` & `ricecooker-0.7.2/docs/concepts/content_workflows.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/concepts/introduction.md` & `ricecooker-0.7.2/docs/concepts/introduction.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/concepts/developer_workflows.md` & `ricecooker-0.7.2/docs/concepts/developer_workflows.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/concepts/reviewing_channels.md` & `ricecooker-0.7.2/docs/concepts/reviewing_channels.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/csv_metadata/csv_exercises.md` & `ricecooker-0.7.2/docs/csv_metadata/csv_exercises.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/csv_metadata/csv_workflow.md` & `ricecooker-0.7.2/docs/csv_metadata/csv_workflow.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/files.md` & `ricecooker-0.7.2/docs/files.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/exercises.md` & `ricecooker-0.7.2/docs/exercises.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/languages.md` & `ricecooker-0.7.2/docs/languages.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/index.rst` & `ricecooker-0.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/video_compression.md` & `ricecooker-0.7.2/docs/video_compression.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/docs/README.rst` & `ricecooker-0.7.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.1/ricecooker.egg-info/PKG-INFO` & `ricecooker-0.7.2/ricecooker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricecooker
-Version: 0.7.1
+Version: 0.7.2
 Summary: API for adding content to the Kolibri content curation server
 Home-page: https://github.com/learningequality/ricecooker
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT license
 Description: ricecooker
         ==========
@@ -260,14 +260,15 @@
         * First release on PyPI.
         
 Keywords: ricecooker
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Topic :: Education
-Requires-Python: >=3.6, <3.11
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
```

### Comparing `ricecooker-0.7.1/ricecooker.egg-info/SOURCES.txt` & `ricecooker-0.7.2/ricecooker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

