# Comparing `tmp/je_editor-0.0.94.tar.gz` & `tmp/je_editor-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor-0.0.94.tar", last modified: Wed May  3 05:47:26 2023, max compression
+gzip compressed data, was "je_editor-0.0.95.tar", last modified: Wed May  3 06:22:31 2023, max compression
```

## Comparing `je_editor-0.0.94.tar` & `je_editor-0.0.95.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.044849 je_editor-0.0.94/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.94/LICENSE
--rw-rw-rw-   0        0        0     3093 2023-05-03 05:47:26.042937 je_editor-0.0.94/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.94/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.801451 je_editor-0.0.94/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.94/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.839398 je_editor-0.0.94/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.847342 je_editor-0.0.94/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.94/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.94/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.853439 je_editor-0.0.94/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.94/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.94/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.860436 je_editor-0.0.94/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.94/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     8332 2023-05-03 04:53:30.000000 je_editor-0.0.94/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.867400 je_editor-0.0.94/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.94/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.94/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.874376 je_editor-0.0.94/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.94/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.94/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.885427 je_editor-0.0.94/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.94/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.94/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.94/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.889350 je_editor-0.0.94/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.94/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.896109 je_editor-0.0.94/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor-0.0.94/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.904195 je_editor-0.0.94/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.94/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.94/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.907113 je_editor-0.0.94/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.913979 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.920899 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.926533 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     4819 2023-05-03 05:41:42.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.933481 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.942518 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.953225 je_editor-0.0.94/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.94/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.94/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.94/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.959860 je_editor-0.0.94/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.94/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6068 2023-05-02 01:27:43.000000 je_editor-0.0.94/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.965731 je_editor-0.0.94/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.94/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.94/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.970729 je_editor-0.0.94/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.94/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.975727 je_editor-0.0.94/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.94/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.94/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.981910 je_editor-0.0.94/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.94/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.94/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.94/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.985931 je_editor-0.0.94/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.990875 je_editor-0.0.94/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.94/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.94/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.002548 je_editor-0.0.94/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.94/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.006423 je_editor-0.0.94/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.012770 je_editor-0.0.94/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.94/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.020771 je_editor-0.0.94/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.94/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.025805 je_editor-0.0.94/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.94/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.94/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.033574 je_editor-0.0.94/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:26.039847 je_editor-0.0.94/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.94/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.94/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:47:25.835351 je_editor-0.0.94/je_editor.egg-info/
--rw-rw-rw-   0        0        0     3093 2023-05-03 05:47:25.000000 je_editor-0.0.94/je_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3041 2023-05-03 05:47:25.000000 je_editor-0.0.94/je_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 05:47:25.000000 je_editor-0.0.94/je_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 05:47:25.000000 je_editor-0.0.94/je_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 05:47:25.000000 je_editor-0.0.94/je_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1144 2023-05-03 05:47:01.000000 je_editor-0.0.94/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 05:47:26.045925 je_editor-0.0.94/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.910199 je_editor-0.0.95/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor-0.0.95/LICENSE
+-rw-rw-rw-   0        0        0     3093 2023-05-03 06:22:31.909201 je_editor-0.0.95/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor-0.0.95/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.608117 je_editor-0.0.95/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor-0.0.95/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.648149 je_editor-0.0.95/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.655151 je_editor-0.0.95/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor-0.0.95/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor-0.0.95/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.662255 je_editor-0.0.95/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor-0.0.95/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor-0.0.95/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.670150 je_editor-0.0.95/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.95/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     8291 2023-05-03 06:10:36.000000 je_editor-0.0.95/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.676152 je_editor-0.0.95/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor-0.0.95/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor-0.0.95/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.684151 je_editor-0.0.95/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor-0.0.95/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor-0.0.95/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.700155 je_editor-0.0.95/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor-0.0.95/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor-0.0.95/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor-0.0.95/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.705160 je_editor-0.0.95/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor-0.0.95/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.712158 je_editor-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.722783 je_editor-0.0.95/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor-0.0.95/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor-0.0.95/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.726810 je_editor-0.0.95/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.738782 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.750788 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.758912 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.769899 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.777532 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.792915 je_editor-0.0.95/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor-0.0.95/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor-0.0.95/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor-0.0.95/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.802914 je_editor-0.0.95/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor-0.0.95/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     5956 2023-05-03 06:19:40.000000 je_editor-0.0.95/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.810867 je_editor-0.0.95/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor-0.0.95/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor-0.0.95/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.812887 je_editor-0.0.95/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor-0.0.95/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.821523 je_editor-0.0.95/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor-0.0.95/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor-0.0.95/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.829400 je_editor-0.0.95/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor-0.0.95/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor-0.0.95/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor-0.0.95/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.834407 je_editor-0.0.95/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.843175 je_editor-0.0.95/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor-0.0.95/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor-0.0.95/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.857196 je_editor-0.0.95/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor-0.0.95/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.862189 je_editor-0.0.95/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.871224 je_editor-0.0.95/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor-0.0.95/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.879287 je_editor-0.0.95/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor-0.0.95/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.889188 je_editor-0.0.95/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor-0.0.95/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor-0.0.95/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.896185 je_editor-0.0.95/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.906199 je_editor-0.0.95/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor-0.0.95/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor-0.0.95/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:22:31.643151 je_editor-0.0.95/je_editor.egg-info/
+-rw-rw-rw-   0        0        0     3093 2023-05-03 06:22:31.000000 je_editor-0.0.95/je_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3041 2023-05-03 06:22:31.000000 je_editor-0.0.95/je_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:22:31.000000 je_editor-0.0.95/je_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 06:22:31.000000 je_editor-0.0.95/je_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 06:22:31.000000 je_editor-0.0.95/je_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1144 2023-05-03 06:22:04.000000 je_editor-0.0.95/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 06:22:31.911198 je_editor-0.0.95/setup.cfg
```

### Comparing `je_editor-0.0.94/LICENSE` & `je_editor-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/PKG-INFO` & `je_editor-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor
-Version: 0.0.94
+Version: 0.0.95
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.94/README.md` & `je_editor-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/__init__.py` & `je_editor-0.0.95/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/__main__.py` & `je_editor-0.0.95/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor-0.0.95/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor-0.0.95/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor-0.0.95/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,15 @@
             exec_file = reformat_os_file_path
             # run program
             execute_program_list = [compiler_path, exec_file]
             self.process = subprocess.Popen(
                 execute_program_list,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
-                stdin=subprocess.PIPE,
-                shell=False
+                shell=True
             )
             self.still_run_program = True
             # program output message queue thread
             self.read_program_output_from_thread = Thread(
                 target=self.read_program_output_from_process,
                 daemon=True
             )
```

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/code_result/code_record.py` & `je_editor-0.0.95/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor-0.0.95/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor-0.0.95/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor-0.0.95/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py` & `je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,8 +101,8 @@
         message_box.setText("Venv already exists")
         message_box.exec()
 
 
 def activate_venv(activate_command: str, path: str):
     activate_path = Path(os.getcwd() + path)
     print(activate_command + str(activate_path))
-    shell_manager.exec_shell(activate_command + str(activate_path))
+    shell_manager.exec_shell(activate_command + " " + str(activate_path))
```

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor-0.0.95/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor-0.0.95/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor-0.0.95/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor-0.0.95/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,19 @@
         """
         :param shell_command: shell command will run
         :return: if error return result and True else return result and False
         """
         try:
             self.exit_program()
             self.code_result.setPlainText("")
-            # run shell command
-            args = shlex.split(shell_command)
             self.process = subprocess.Popen(
-                args,
+                shell_command,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
-                stdin=subprocess.PIPE,
-                shell=False,
+                shell=True,
             )
             self.still_run_shell = True
             # program output message queue thread
             self.read_program_output_from_thread = Thread(
                 target=self.read_program_output_from_process,
                 daemon=True
             )
```

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor-0.0.95/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor-0.0.95/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor-0.0.95/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/encodings/python_encodings.py` & `je_editor-0.0.95/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/exception/exception_tags.py` & `je_editor-0.0.95/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/file/open/open_file.py` & `je_editor-0.0.95/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/file/save/save_file.py` & `je_editor-0.0.95/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/json/json_file.py` & `je_editor-0.0.95/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/json_format/json_process.py` & `je_editor-0.0.95/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor-0.0.95/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/je_editor.egg-info/PKG-INFO` & `je_editor-0.0.95/je_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor
-Version: 0.0.94
+Version: 0.0.95
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor-0.0.94/je_editor.egg-info/SOURCES.txt` & `je_editor-0.0.95/je_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.94/pyproject.toml` & `je_editor-0.0.95/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor"
-version = "0.0.94"
+version = "0.0.95"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

