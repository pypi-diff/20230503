# Comparing `tmp/je_editor-0.0.91.tar.gz` & `tmp/je_editor-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor-0.0.91.tar", last modified: Tue May  2 08:44:30 2023, max compression
+gzip compressed data, was "je_editor-0.0.92.tar", last modified: Wed May  3 01:48:20 2023, max compression
```

## Comparing `je_editor-0.0.91.tar` & `je_editor-0.0.92.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.782937 je_editor-0.0.91/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.91/LICENSE
--rw-rw-rw-   0        0        0     3093 2023-05-02 08:44:30.781937 je_editor-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.559089 je_editor-0.0.91/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.91/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.595321 je_editor-0.0.91/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.601418 je_editor-0.0.91/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.91/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.91/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.606437 je_editor-0.0.91/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.91/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.91/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.611436 je_editor-0.0.91/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.91/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     7371 2023-05-02 01:27:43.000000 je_editor-0.0.91/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.618748 je_editor-0.0.91/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.91/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.91/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.624748 je_editor-0.0.91/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.91/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.91/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.633838 je_editor-0.0.91/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.91/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.91/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.91/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.636760 je_editor-0.0.91/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.91/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.641799 je_editor-0.0.91/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7028 2023-05-02 08:42:44.000000 je_editor-0.0.91/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.652194 je_editor-0.0.91/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.91/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.91/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.655281 je_editor-0.0.91/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.660283 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.666470 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.672469 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-05-02 03:17:22.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.678473 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.684467 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4141 2023-05-02 03:15:20.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.693466 je_editor-0.0.91/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.91/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.91/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.91/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.699468 je_editor-0.0.91/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.91/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6068 2023-05-02 01:27:43.000000 je_editor-0.0.91/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.705559 je_editor-0.0.91/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.91/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.91/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.708501 je_editor-0.0.91/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.91/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.716504 je_editor-0.0.91/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.91/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.91/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.722560 je_editor-0.0.91/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.91/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.91/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.91/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.725563 je_editor-0.0.91/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.730467 je_editor-0.0.91/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.91/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.91/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.741556 je_editor-0.0.91/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.91/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.744593 je_editor-0.0.91/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.751599 je_editor-0.0.91/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.91/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.757595 je_editor-0.0.91/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.91/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.763155 je_editor-0.0.91/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.91/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.91/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.772928 je_editor-0.0.91/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.777935 je_editor-0.0.91/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.91/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.91/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:44:30.592835 je_editor-0.0.91/je_editor.egg-info/
--rw-rw-rw-   0        0        0     3093 2023-05-02 08:44:30.000000 je_editor-0.0.91/je_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3041 2023-05-02 08:44:30.000000 je_editor-0.0.91/je_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 08:44:30.000000 je_editor-0.0.91/je_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-02 08:44:30.000000 je_editor-0.0.91/je_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 08:44:30.000000 je_editor-0.0.91/je_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1144 2023-05-02 08:44:08.000000 je_editor-0.0.91/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 08:44:30.783936 je_editor-0.0.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.958152 je_editor-0.0.92/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.92/LICENSE
+-rw-rw-rw-   0        0        0     3093 2023-05-03 01:48:20.957150 je_editor-0.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.92/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.756276 je_editor-0.0.92/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.92/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.783326 je_editor-0.0.92/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.788327 je_editor-0.0.92/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.92/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.92/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.793327 je_editor-0.0.92/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.92/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.92/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.798372 je_editor-0.0.92/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.92/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     7371 2023-05-02 01:27:43.000000 je_editor-0.0.92/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.803393 je_editor-0.0.92/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.92/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.92/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.808241 je_editor-0.0.92/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.92/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.92/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.818767 je_editor-0.0.92/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.92/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.92/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.92/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.821767 je_editor-0.0.92/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.92/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.825766 je_editor-0.0.92/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7028 2023-05-02 08:42:44.000000 je_editor-0.0.92/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.831766 je_editor-0.0.92/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.92/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.92/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.833769 je_editor-0.0.92/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.838767 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.845766 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.850765 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     1228 2023-05-02 03:17:22.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.857186 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.862165 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4141 2023-05-02 03:15:20.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.870463 je_editor-0.0.92/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.92/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.92/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.92/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.877468 je_editor-0.0.92/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.92/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     6068 2023-05-02 01:27:43.000000 je_editor-0.0.92/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.882467 je_editor-0.0.92/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.92/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.92/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.885468 je_editor-0.0.92/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.92/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.891508 je_editor-0.0.92/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.92/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.92/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.897509 je_editor-0.0.92/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.92/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.92/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.92/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.899510 je_editor-0.0.92/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.905563 je_editor-0.0.92/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.92/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.92/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.917050 je_editor-0.0.92/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.92/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.920150 je_editor-0.0.92/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.926146 je_editor-0.0.92/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.92/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.934145 je_editor-0.0.92/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.92/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.940149 je_editor-0.0.92/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.92/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.92/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.947147 je_editor-0.0.92/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.954147 je_editor-0.0.92/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.92/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.92/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:20.780349 je_editor-0.0.92/je_editor.egg-info/
+-rw-rw-rw-   0        0        0     3093 2023-05-03 01:48:20.000000 je_editor-0.0.92/je_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3041 2023-05-03 01:48:20.000000 je_editor-0.0.92/je_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:48:20.000000 je_editor-0.0.92/je_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 01:48:20.000000 je_editor-0.0.92/je_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 01:48:20.000000 je_editor-0.0.92/je_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1144 2023-05-03 01:48:00.000000 je_editor-0.0.92/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:48:20.959147 je_editor-0.0.92/setup.cfg
```

### Comparing `je_editor-0.0.91/LICENSE` & `je_editor-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/PKG-INFO` & `je_editor-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor
-Version: 0.0.91
+Version: 0.0.92
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.91/README.md` & `je_editor-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/__init__.py` & `je_editor-0.0.92/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/__main__.py` & `je_editor-0.0.92/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor-0.0.92/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor-0.0.92/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor-0.0.92/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/code_result/code_record.py` & `je_editor-0.0.92/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor-0.0.92/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor-0.0.92/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor-0.0.92/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor-0.0.92/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py` & `je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor-0.0.92/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor-0.0.92/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor-0.0.92/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor-0.0.92/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor-0.0.92/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor-0.0.92/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor-0.0.92/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/encodings/python_encodings.py` & `je_editor-0.0.92/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/exception/exception_tags.py` & `je_editor-0.0.92/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/file/open/open_file.py` & `je_editor-0.0.92/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/file/save/save_file.py` & `je_editor-0.0.92/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/json/json_file.py` & `je_editor-0.0.92/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/json_format/json_process.py` & `je_editor-0.0.92/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor-0.0.92/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/je_editor.egg-info/PKG-INFO` & `je_editor-0.0.92/je_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor
-Version: 0.0.91
+Version: 0.0.92
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.91/je_editor.egg-info/SOURCES.txt` & `je_editor-0.0.92/je_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.91/pyproject.toml` & `je_editor-0.0.92/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

