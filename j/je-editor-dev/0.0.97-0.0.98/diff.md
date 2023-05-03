# Comparing `tmp/je_editor_dev-0.0.97.tar.gz` & `tmp/je_editor_dev-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.97.tar", last modified: Wed May  3 08:39:47 2023, max compression
+gzip compressed data, was "je_editor_dev-0.0.98.tar", last modified: Wed May  3 09:48:13 2023, max compression
```

## Comparing `je_editor_dev-0.0.97.tar` & `je_editor_dev-0.0.98.tar`

### file list

```diff
@@ -1,106 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.715822 je_editor_dev-0.0.97/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/LICENSE
--rw-rw-rw-   0        0        0     3097 2023-05-03 08:39:47.713763 je_editor_dev-0.0.97/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.97/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.429603 je_editor_dev-0.0.97/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.97/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.433725 je_editor_dev-0.0.97/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.442684 je_editor_dev-0.0.97/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.450383 je_editor_dev-0.0.97/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.457374 je_editor_dev-0.0.97/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     8200 2023-05-03 08:34:32.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.464398 je_editor_dev-0.0.97/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.472435 je_editor_dev-0.0.97/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.482377 je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.485375 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.491449 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.499383 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.503484 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.510377 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.518550 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.525487 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.534558 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.541528 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.552623 je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.558536 je_editor_dev-0.0.97/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6098 2023-05-03 08:34:32.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.568523 je_editor_dev-0.0.97/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.574523 je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.582682 je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.589643 je_editor_dev-0.0.97/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor_dev-0.0.97/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.97/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.594647 je_editor_dev-0.0.97/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.603058 je_editor_dev-0.0.97/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.97/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.97/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.614564 je_editor_dev-0.0.97/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.97/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.618601 je_editor_dev-0.0.97/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.644860 je_editor_dev-0.0.97/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.97/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.654258 je_editor_dev-0.0.97/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.97/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.662390 je_editor_dev-0.0.97/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.97/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.97/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.669405 je_editor_dev-0.0.97/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.677730 je_editor_dev-0.0.97/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.97/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.97/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:39:47.709762 je_editor_dev-0.0.97/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     3097 2023-05-03 08:39:47.000000 je_editor_dev-0.0.97/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-05-03 08:39:47.000000 je_editor_dev-0.0.97/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 08:39:47.000000 je_editor_dev-0.0.97/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 08:39:47.000000 je_editor_dev-0.0.97/je_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 08:39:47.000000 je_editor_dev-0.0.97/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1134 2023-05-03 08:39:26.000000 je_editor_dev-0.0.97/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 08:39:47.716822 je_editor_dev-0.0.97/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.970224 je_editor_dev-0.0.98/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/LICENSE
+-rw-rw-rw-   0        0        0     3097 2023-05-03 09:48:13.969221 je_editor_dev-0.0.98/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.98/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.700687 je_editor_dev-0.0.98/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.98/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.705692 je_editor_dev-0.0.98/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.712717 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.736865 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.743976 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     7891 2023-05-03 09:43:32.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.752139 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.757148 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.768159 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.771154 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.778212 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7183 2023-05-03 09:19:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.785169 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.789356 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.796363 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.804369 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.812362 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-03 09:35:31.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.820361 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.828365 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1317 2023-05-03 09:36:21.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.839357 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:33:51.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-05-03 09:46:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/build_venv_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.853389 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.861360 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     6278 2023-05-03 09:33:27.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.870356 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.875737 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.880810 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.885813 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-05-03 09:19:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.98/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.890697 je_editor_dev-0.0.98/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.896711 je_editor_dev-0.0.98/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.98/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.98/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.904707 je_editor_dev-0.0.98/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.98/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.908340 je_editor_dev-0.0.98/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.912773 je_editor_dev-0.0.98/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.917772 je_editor_dev-0.0.98/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.98/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.924775 je_editor_dev-0.0.98/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.98/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.98/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.929296 je_editor_dev-0.0.98/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.933316 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.966230 je_editor_dev-0.0.98/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     3097 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1134 2023-05-03 09:47:47.000000 je_editor_dev-0.0.98/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:48:13.971227 je_editor_dev-0.0.98/setup.cfg
```

### Comparing `je_editor_dev-0.0.97/LICENSE` & `je_editor_dev-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/PKG-INFO` & `je_editor_dev-0.0.98/je_editor_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je_editor_dev
-Version: 0.0.97
+Name: je-editor-dev
+Version: 0.0.98
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.97/README.md` & `je_editor_dev-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/__init__.py` & `je_editor_dev-0.0.98/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/__main__.py` & `je_editor_dev-0.0.98/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,25 +72,20 @@
                 compiler_path = shutil.which(
                     cmd="python3",
                     path=str(venv_path)
                 )
             else:
                 compiler_path = shutil.which(cmd="python3")
             if compiler_path is None:
-                if sys.platform in ["win32", "cygwin", "msys"]:
-                    venv_path = Path(os.getcwd() + "/venv/Scripts")
-                else:
-                    venv_path = Path(os.getcwd() + "/venv/bin")
-                if venv_path.is_dir() and venv_path.exists():
-                    compiler_path = shutil.which(
-                        cmd="python",
-                        path=str(venv_path)
-                    )
-                else:
-                    compiler_path = shutil.which(cmd="python")
+                compiler_path = shutil.which(
+                    cmd="python",
+                    path=str(venv_path)
+                )
+            else:
+                compiler_path = shutil.which(cmd="python")
             if compiler_path is None:
                 raise JEditorExecException(compiler_not_found_error)
             exec_file = reformat_os_file_path
             # run program
             execute_program_list = [compiler_path, exec_file]
             self.process = subprocess.Popen(
                 execute_program_list,
```

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/code_result/code_record.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 class EditorMain(QMainWindow):
 
     def __init__(self):
         super(EditorMain, self).__init__()
         # Windows setup
         self.id = "JEditor"
+        # Venv
+        self.venv_path = None
         if sys.platform in ["win32", "cygwin", "msys"]:
             from ctypes import windll
             windll.shell32.SetCurrentProcessExplicitAppUserModelID(self.id)
         # set python buffered
         os.environ["PYTHONUNBUFFERED"] = "1"
         # Auto save thread
         self.auto_save_thread = None
```

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from PySide6.QtWidgets import QMainWindow, QMenuBar
 
 from je_editor.pyside_ui.menu.menu_bar.check_style_menu.build_check_style_menu import set_check_menu
 from je_editor.pyside_ui.menu.menu_bar.file_menu.build_file_menu import set_file_menu
 from je_editor.pyside_ui.menu.menu_bar.help_menu.build_help_menu import set_help_menu
 from je_editor.pyside_ui.menu.menu_bar.run_menu.build_run_menu import set_run_menu
+from je_editor.pyside_ui.menu.menu_bar.venv_menu.build_venv_menu import set_venv_menu
 
 
 def set_menu_bar(ui_we_want_to_set: QMainWindow):
     # set menu
     ui_we_want_to_set.menu = QMenuBar()
     ui_we_want_to_set.file_menu = ui_we_want_to_set.menu.addMenu("File")
     ui_we_want_to_set.run_menu = ui_we_want_to_set.menu.addMenu("Run")
     ui_we_want_to_set.text_menu = ui_we_want_to_set.menu.addMenu("Text")
     ui_we_want_to_set.check_menu = ui_we_want_to_set.menu.addMenu("Check Code Style")
     ui_we_want_to_set.help_menu = ui_we_want_to_set.menu.addMenu("Help")
+    ui_we_want_to_set.venv_menu = ui_we_want_to_set.menu.addMenu("Venv")
     ui_we_want_to_set.setMenuBar(ui_we_want_to_set.menu)
     set_file_menu(ui_we_want_to_set)
     set_run_menu(ui_we_want_to_set)
     set_check_menu(ui_we_want_to_set)
     set_help_menu(ui_we_want_to_set)
+    set_venv_menu(ui_we_want_to_set)
```

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import queue
 import shlex
 import subprocess
+import sys
 from threading import Thread
 
 from PySide6.QtCore import QTimer
 from PySide6.QtWidgets import QMainWindow, QTextEdit
 
 from je_editor.pyside_ui.colors.global_color import error_color, output_color
 from je_editor.utils.exception.exception_tags import je_editor_init_error
@@ -36,24 +37,28 @@
 
     def later_init(self):
         if self.main_window is not None:
             self.code_result: QTextEdit = self.main_window.code_result
         else:
             raise JEditorException(je_editor_init_error)
 
-    def exec_shell(self, shell_command: str):
+    def exec_shell(self, shell_command: [str, list]):
         """
         :param shell_command: shell command will run
         :return: if error return result and True else return result and False
         """
         try:
             self.exit_program()
             self.code_result.setPlainText("")
+            if sys.platform in ["win32", "cygwin", "msys"]:
+                args = shell_command
+            else:
+                args = shlex.split(shell_command)
             self.process = subprocess.Popen(
-                shell_command,
+                args,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 shell=True,
             )
             self.still_run_shell = True
             # program output message queue thread
             self.read_program_output_from_thread = Thread(
```

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from je_editor.utils.json.json_file import read_json
 from je_editor.utils.json.json_file import write_json
 
 user_setting_dict = {
     "font": "Lato",
     "font_size": 12,
     "encoding": "utf-8",
-    "last_file": None
+    "last_file": None,
 }
 
 
 def write_user_setting():
     user_setting_file = Path(getcwd() + "/user_setting.json")
     write_json(str(user_setting_file), user_setting_dict)
```

### Comparing `je_editor_dev-0.0.97/je_editor/utils/encodings/python_encodings.py` & `je_editor_dev-0.0.98/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/exception/exception_tags.py` & `je_editor_dev-0.0.98/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/file/open/open_file.py` & `je_editor_dev-0.0.98/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/file/save/save_file.py` & `je_editor_dev-0.0.98/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/json/json_file.py` & `je_editor_dev-0.0.98/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/json_format/json_process.py` & `je_editor_dev-0.0.98/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor_dev-0.0.98/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.97/je_editor_dev.egg-info/PKG-INFO` & `je_editor_dev-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je-editor-dev
-Version: 0.0.97
+Name: je_editor_dev
+Version: 0.0.98
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.97/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.98/je_editor_dev.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
 je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
 je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
 je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
 je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
 je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
 je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+je_editor/pyside_ui/menu/menu_bar/venv_menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/venv_menu/build_venv_menu.py
 je_editor/pyside_ui/search_ui/__init__.py
 je_editor/pyside_ui/search_ui/search_error_box.py
 je_editor/pyside_ui/search_ui/search_text_box.py
 je_editor/pyside_ui/shell_process/__init__.py
 je_editor/pyside_ui/shell_process/shell_exec.py
 je_editor/pyside_ui/syntax/__init__.py
 je_editor/pyside_ui/syntax/python_syntax.py
```

### Comparing `je_editor_dev-0.0.97/pyproject.toml` & `je_editor_dev-0.0.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor_dev"
-version = "0.0.97"
+version = "0.0.98"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

