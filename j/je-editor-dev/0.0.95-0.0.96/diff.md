# Comparing `tmp/je_editor_dev-0.0.95.tar.gz` & `tmp/je_editor_dev-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.95.tar", last modified: Wed May  3 06:24:43 2023, max compression
+gzip compressed data, was "je_editor_dev-0.0.96.tar", last modified: Wed May  3 07:33:32 2023, max compression
```

## Comparing `je_editor_dev-0.0.95.tar` & `je_editor_dev-0.0.96.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.979900 je_editor_dev-0.0.95/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/LICENSE
--rw-rw-rw-   0        0        0     3097 2023-05-03 06:24:43.978951 je_editor_dev-0.0.95/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.95/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.757226 je_editor_dev-0.0.95/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.95/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.760229 je_editor_dev-0.0.95/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.765238 je_editor_dev-0.0.95/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.773227 je_editor_dev-0.0.95/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.780244 je_editor_dev-0.0.95/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     8291 2023-05-03 06:10:36.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.786719 je_editor_dev-0.0.95/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.792794 je_editor_dev-0.0.95/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.802876 je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.805804 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.811838 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.817842 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.820819 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.826811 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.832872 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.837841 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.844194 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.850510 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.859064 je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.867207 je_editor_dev-0.0.95/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5956 2023-05-03 06:19:40.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.872681 je_editor_dev-0.0.95/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.876125 je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.881160 je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.887204 je_editor_dev-0.0.95/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor_dev-0.0.95/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.95/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.890677 je_editor_dev-0.0.95/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.896274 je_editor_dev-0.0.95/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.95/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.95/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.905210 je_editor_dev-0.0.95/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.95/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.908529 je_editor_dev-0.0.95/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.914480 je_editor_dev-0.0.95/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.95/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.920652 je_editor_dev-0.0.95/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.95/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.927676 je_editor_dev-0.0.95/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.95/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.95/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.933628 je_editor_dev-0.0.95/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.939915 je_editor_dev-0.0.95/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.95/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.95/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:24:43.974953 je_editor_dev-0.0.95/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     3097 2023-05-03 06:24:43.000000 je_editor_dev-0.0.95/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-05-03 06:24:43.000000 je_editor_dev-0.0.95/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:24:43.000000 je_editor_dev-0.0.95/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 06:24:43.000000 je_editor_dev-0.0.95/je_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 06:24:43.000000 je_editor_dev-0.0.95/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1134 2023-05-03 06:24:17.000000 je_editor_dev-0.0.95/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 06:24:43.979900 je_editor_dev-0.0.95/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.216787 je_editor_dev-0.0.96/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/LICENSE
+-rw-rw-rw-   0        0        0     3097 2023-05-03 07:33:32.215824 je_editor_dev-0.0.96/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.96/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.951336 je_editor_dev-0.0.96/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.96/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.955343 je_editor_dev-0.0.96/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.962442 je_editor_dev-0.0.96/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.969347 je_editor_dev-0.0.96/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.978436 je_editor_dev-0.0.96/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     8064 2023-05-03 07:25:06.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.985343 je_editor_dev-0.0.96/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:31.993348 je_editor_dev-0.0.96/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.003223 je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.006250 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.012227 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7136 2023-05-03 05:07:29.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.019232 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.024325 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.032337 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.040298 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.048919 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     4825 2023-05-03 06:18:10.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.058246 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.066291 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.078297 je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.086760 je_editor_dev-0.0.96/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     5956 2023-05-03 06:19:40.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.093759 je_editor_dev-0.0.96/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.098762 je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.104815 je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.109814 je_editor_dev-0.0.96/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-02 08:30:57.000000 je_editor_dev-0.0.96/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.96/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.113990 je_editor_dev-0.0.96/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.120994 je_editor_dev-0.0.96/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.96/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.96/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.131007 je_editor_dev-0.0.96/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.96/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.134216 je_editor_dev-0.0.96/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.141225 je_editor_dev-0.0.96/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.96/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.148764 je_editor_dev-0.0.96/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.96/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.155731 je_editor_dev-0.0.96/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.96/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.96/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.163735 je_editor_dev-0.0.96/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.170842 je_editor_dev-0.0.96/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.96/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.96/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:32.209735 je_editor_dev-0.0.96/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     3097 2023-05-03 07:33:31.000000 je_editor_dev-0.0.96/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-05-03 07:33:31.000000 je_editor_dev-0.0.96/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:33:31.000000 je_editor_dev-0.0.96/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 07:33:31.000000 je_editor_dev-0.0.96/je_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 07:33:31.000000 je_editor_dev-0.0.96/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1134 2023-05-03 07:33:07.000000 je_editor_dev-0.0.96/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:33:32.217826 je_editor_dev-0.0.96/setup.cfg
```

### Comparing `je_editor_dev-0.0.95/LICENSE` & `je_editor_dev-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/PKG-INFO` & `je_editor_dev-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor_dev
-Version: 0.0.95
+Version: 0.0.96
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.95/README.md` & `je_editor_dev-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/__init__.py` & `je_editor_dev-0.0.96/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/__main__.py` & `je_editor_dev-0.0.96/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,28 +60,26 @@
             reformat_os_file_path = os.path.abspath(exec_file_name)
             # detect file is exist
             try:
                 if not Path(exec_file_name).exists():
                     raise JEditorExecException(file_not_fond_error)
             except OSError as error:
                 raise JEditorExecException(error)
-            compiler_path = shutil.which(self.program_language)
-            if compiler_path is None and self.program_language == "python":
-                if sys.platform in ["win32", "cygwin", "msys"]:
-                    venv_path = Path(os.getcwd() + "/venv/Scripts")
-                else:
-                    venv_path = Path(os.getcwd() + "/venv/bin")
-                if venv_path.is_dir() and venv_path.exists():
-                    compiler_path = shutil.which(
-                        cmd="python3",
-                        path=str(venv_path)
-                    )
-                else:
-                    compiler_path = shutil.which(cmd="python3")
-            elif compiler_path is None and self.program_language == "python3":
+            if sys.platform in ["win32", "cygwin", "msys"]:
+                venv_path = Path(os.getcwd() + "/venv/Scripts")
+            else:
+                venv_path = Path(os.getcwd() + "/venv/bin")
+            if venv_path.is_dir() and venv_path.exists():
+                compiler_path = shutil.which(
+                    cmd="python3",
+                    path=str(venv_path)
+                )
+            else:
+                compiler_path = shutil.which(cmd="python3")
+            if compiler_path is None:
                 if sys.platform in ["win32", "cygwin", "msys"]:
                     venv_path = Path(os.getcwd() + "/venv/Scripts")
                 else:
                     venv_path = Path(os.getcwd() + "/venv/bin")
                 if venv_path.is_dir() and venv_path.exists():
                     compiler_path = shutil.which(
                         cmd="python",
```

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/code_result/code_record.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor_dev-0.0.96/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/encodings/python_encodings.py` & `je_editor_dev-0.0.96/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/exception/exception_tags.py` & `je_editor_dev-0.0.96/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/file/open/open_file.py` & `je_editor_dev-0.0.96/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/file/save/save_file.py` & `je_editor_dev-0.0.96/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/json/json_file.py` & `je_editor_dev-0.0.96/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/json_format/json_process.py` & `je_editor_dev-0.0.96/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor_dev-0.0.96/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/je_editor_dev.egg-info/PKG-INFO` & `je_editor_dev-0.0.96/je_editor_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor-dev
-Version: 0.0.95
+Version: 0.0.96
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.95/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.96/je_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.95/pyproject.toml` & `je_editor_dev-0.0.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor_dev"
-version = "0.0.95"
+version = "0.0.96"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

