# Comparing `tmp/je_editor-0.0.96.tar.gz` & `tmp/je_editor-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor-0.0.96.tar", last modified: Wed May  3 07:36:29 2023, max compression
+gzip compressed data, was "je_editor-0.0.97.tar", last modified: Wed May  3 08:35:39 2023, max compression
```

## Comparing `je_editor-0.0.96.tar` & `je_editor-0.0.97.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.142273 je_editor-0.0.96/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.96/LICENSE
--rw-rw-rw-   0        0        0     3093 2023-05-03 07:36:29.141083 je_editor-0.0.96/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.96/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.938235 je_editor-0.0.96/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.96/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.974867 je_editor-0.0.96/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.980379 je_editor-0.0.96/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.96/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.96/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.987380 je_editor-0.0.96/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.96/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.96/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.993378 je_editor-0.0.96/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.96/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     8064 2023-05-03 07:25:06.000000 je_editor-0.0.96/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.999657 je_editor-0.0.96/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.96/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.96/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.007662 je_editor-0.0.96/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.96/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.96/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.015662 je_editor-0.0.96/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.96/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.96/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.96/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.018668 je_editor-0.0.96/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.96/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.024662 je_editor-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.030666 je_editor-0.0.96/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.96/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.96/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.033662 je_editor-0.0.96/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.037661 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.043663 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.049924 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.055573 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.061592 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.069292 je_editor-0.0.96/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.96/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.96/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.96/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.074322 je_editor-0.0.96/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.96/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5956 2023-05-03 06:19:40.000000 je_editor-0.0.96/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.078325 je_editor-0.0.96/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.96/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.96/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.081734 je_editor-0.0.96/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.96/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.085734 je_editor-0.0.96/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.96/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.96/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.090740 je_editor-0.0.96/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.96/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.96/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.96/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.093737 je_editor-0.0.96/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.097734 je_editor-0.0.96/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.96/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.96/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.105761 je_editor-0.0.96/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.96/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.107920 je_editor-0.0.96/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.113257 je_editor-0.0.96/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.96/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.118653 je_editor-0.0.96/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.96/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.124681 je_editor-0.0.96/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.96/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.96/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.131083 je_editor-0.0.96/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:29.136080 je_editor-0.0.96/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.96/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.96/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:36:28.971588 je_editor-0.0.96/je_editor.egg-info/
--rw-rw-rw-   0        0        0     3093 2023-05-03 07:36:28.000000 je_editor-0.0.96/je_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3041 2023-05-03 07:36:28.000000 je_editor-0.0.96/je_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:36:28.000000 je_editor-0.0.96/je_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 07:36:28.000000 je_editor-0.0.96/je_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 07:36:28.000000 je_editor-0.0.96/je_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1144 2023-05-03 07:36:02.000000 je_editor-0.0.96/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 07:36:29.143283 je_editor-0.0.96/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.383363 je_editor-0.0.97/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.97/LICENSE
+-rw-rw-rw-   0        0        0     3093 2023-05-03 08:35:39.382116 je_editor-0.0.97/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.97/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.108801 je_editor-0.0.97/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.97/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.147415 je_editor-0.0.97/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.154816 je_editor-0.0.97/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.97/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.97/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.161829 je_editor-0.0.97/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.97/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.97/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.168830 je_editor-0.0.97/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.97/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     8200 2023-05-03 08:34:32.000000 je_editor-0.0.97/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.174872 je_editor-0.0.97/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.97/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.97/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.182923 je_editor-0.0.97/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.97/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.97/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.193832 je_editor-0.0.97/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.97/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.97/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.97/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.197933 je_editor-0.0.97/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.97/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.203836 je_editor-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.213707 je_editor-0.0.97/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.97/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.97/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.216706 je_editor-0.0.97/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.225763 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.231879 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.239875 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.246974 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.253211 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.264107 je_editor-0.0.97/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.97/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.97/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.97/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.273277 je_editor-0.0.97/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.97/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     6098 2023-05-03 08:34:32.000000 je_editor-0.0.97/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.281376 je_editor-0.0.97/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.97/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.97/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.285385 je_editor-0.0.97/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.97/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.291390 je_editor-0.0.97/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.97/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.97/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.298939 je_editor-0.0.97/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.97/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.97/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.97/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.302880 je_editor-0.0.97/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.310773 je_editor-0.0.97/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.97/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.97/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.329992 je_editor-0.0.97/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.97/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.334489 je_editor-0.0.97/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.344724 je_editor-0.0.97/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.97/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.354967 je_editor-0.0.97/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.97/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.363598 je_editor-0.0.97/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.97/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.97/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.370830 je_editor-0.0.97/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.379117 je_editor-0.0.97/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.97/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.97/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:35:39.143415 je_editor-0.0.97/je_editor.egg-info/
+-rw-rw-rw-   0        0        0     3093 2023-05-03 08:35:38.000000 je_editor-0.0.97/je_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3041 2023-05-03 08:35:39.000000 je_editor-0.0.97/je_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 08:35:38.000000 je_editor-0.0.97/je_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 08:35:38.000000 je_editor-0.0.97/je_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 08:35:38.000000 je_editor-0.0.97/je_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1144 2023-05-03 08:35:17.000000 je_editor-0.0.97/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 08:35:39.383363 je_editor-0.0.97/setup.cfg
```

### Comparing `je_editor-0.0.96/LICENSE` & `je_editor-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/PKG-INFO` & `je_editor-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor
-Version: 0.0.96
+Version: 0.0.97
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.96/README.md` & `je_editor-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/__init__.py` & `je_editor-0.0.97/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/__main__.py` & `je_editor-0.0.97/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor-0.0.97/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor-0.0.97/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor-0.0.97/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,35 @@
                 output_message = self.run_output_queue.get_nowait()
                 output_message = str(output_message).strip()
                 if output_message:
                     self.code_result.append(output_message)
         except queue.Empty:
             pass
         if self.process.returncode == 0:
+            self.timer.stop()
             self.exit_program()
         elif self.process.returncode is not None:
-            self.exit_program()
             self.timer.stop()
+            self.exit_program()
         if self.still_run_program:
             # poll return code
             self.process.poll()
 
     # exit program change run flag to false and clean read thread and queue and process
     def exit_program(self):
         self.still_run_program = False
         if self.read_program_output_from_thread is not None:
             self.read_program_output_from_thread = None
         if self.read_program_error_output_from_thread is not None:
             self.read_program_error_output_from_thread = None
         self.print_and_clear_queue()
         if self.process is not None:
             self.process.terminate()
+            print(f"Program exit with code {self.process.returncode}")
+            self.process = None
 
     def print_and_clear_queue(self):
         try:
             for std_output in iter(self.run_output_queue.get_nowait, None):
                 std_output = str(std_output).strip()
                 if std_output:
                     self.code_result.append(std_output)
```

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/code_result/code_record.py` & `je_editor-0.0.97/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor-0.0.97/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor-0.0.97/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor-0.0.97/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py` & `je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor-0.0.97/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor-0.0.97/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor-0.0.97/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor-0.0.97/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,32 +91,35 @@
                 output_message = self.run_output_queue.get_nowait()
                 output_message = str(output_message).strip()
                 if output_message:
                     self.code_result.append(output_message)
         except queue.Empty:
             pass
         if self.process.returncode == 0:
+            self.timer.stop()
             self.exit_program()
         elif self.process.returncode is not None:
-            self.exit_program()
             self.timer.stop()
+            self.exit_program()
         if self.still_run_shell:
             # poll return code
             self.process.poll()
 
     # exit program change run flag to false and clean read thread and queue and process
     def exit_program(self):
         self.still_run_shell = False
         if self.read_program_output_from_thread is not None:
             self.read_program_output_from_thread = None
         if self.read_program_error_output_from_thread is not None:
             self.read_program_error_output_from_thread = None
         self.print_and_clear_queue()
         if self.process is not None:
             self.process.terminate()
+            print(f"Shell command exit with code {self.process.returncode}")
+            self.process = None
 
     def print_and_clear_queue(self):
         try:
             for std_output in iter(self.run_output_queue.get_nowait, None):
                 std_output = str(std_output).strip()
                 if std_output:
                     self.code_result.append(std_output)
```

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor-0.0.97/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor-0.0.97/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor-0.0.97/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/encodings/python_encodings.py` & `je_editor-0.0.97/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/exception/exception_tags.py` & `je_editor-0.0.97/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/file/open/open_file.py` & `je_editor-0.0.97/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/file/save/save_file.py` & `je_editor-0.0.97/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/json/json_file.py` & `je_editor-0.0.97/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/json_format/json_process.py` & `je_editor-0.0.97/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor-0.0.97/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/je_editor.egg-info/PKG-INFO` & `je_editor-0.0.97/je_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor
-Version: 0.0.96
+Version: 0.0.97
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.96/je_editor.egg-info/SOURCES.txt` & `je_editor-0.0.97/je_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.96/pyproject.toml` & `je_editor-0.0.97/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor"
-version = "0.0.96"
+version = "0.0.97"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

