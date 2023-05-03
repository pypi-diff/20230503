# Comparing `tmp/canvascli-0.5.1.tar.gz` & `tmp/canvascli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvascli-0.5.1.tar", last modified: Sat Oct  1 16:47:56 2022, max compression
+gzip compressed data, was "canvascli-0.6.0.tar", last modified: Wed May  3 19:01:14 2023, max compression
```

## Comparing `canvascli-0.5.1.tar` & `canvascli-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2022-10-01 16:47:56.425013 canvascli-0.5.1/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1069 2021-06-02 17:43:36.000000 canvascli-0.5.1/LICENSE
--rw-rw-r--   0 joel      (1000) joel      (1000)       52 2022-02-28 07:42:04.000000 canvascli-0.5.1/MANIFEST.in
--rw-rw-r--   0 joel      (1000) joel      (1000)     3988 2022-10-01 16:47:56.425013 canvascli-0.5.1/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3683 2022-07-26 08:38:27.000000 canvascli-0.5.1/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2022-10-01 16:47:56.425013 canvascli-0.5.1/canvascli/
--rw-rw-r--   0 joel      (1000) joel      (1000)       72 2022-03-02 16:22:02.000000 canvascli-0.5.1/canvascli/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    35173 2022-04-26 02:01:30.000000 canvascli-0.5.1/canvascli/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      497 2022-10-01 16:47:56.425013 canvascli-0.5.1/canvascli/_version.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    40191 2022-10-01 16:40:58.000000 canvascli-0.5.1/canvascli/main.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2022-10-01 16:47:56.425013 canvascli-0.5.1/canvascli.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)     3988 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       49 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/entry_points.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      128 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/requires.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       10 2022-10-01 16:47:56.000000 canvascli-0.5.1/canvascli.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      197 2022-10-01 16:47:56.425013 canvascli-0.5.1/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)      951 2022-07-26 08:38:27.000000 canvascli-0.5.1/setup.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    80044 2022-02-28 07:42:04.000000 canvascli-0.5.1/versioneer.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1069 2021-06-02 17:43:36.000000 canvascli-0.6.0/LICENSE
+-rw-rw-r--   0 joel      (1000) joel      (1000)       52 2022-02-28 07:42:04.000000 canvascli-0.6.0/MANIFEST.in
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-03 19:01:14.015461 canvascli-0.6.0/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3700 2023-04-09 23:39:09.000000 canvascli-0.6.0/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       72 2022-03-02 16:22:02.000000 canvascli-0.6.0/canvascli/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      497 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli/_version.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    61599 2023-04-24 15:51:31.000000 canvascli-0.6.0/canvascli/main.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli.egg-info/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      324 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)       49 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/entry_points.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      144 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/requires.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)       10 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      197 2023-05-03 19:01:14.015461 canvascli-0.6.0/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)      979 2023-04-12 21:40:16.000000 canvascli-0.6.0/setup.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    80044 2022-02-28 07:42:04.000000 canvascli-0.6.0/versioneer.py
```

### Comparing `canvascli-0.5.1/LICENSE` & `canvascli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canvascli-0.5.1/PKG-INFO` & `canvascli-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvascli
-Version: 0.5.1
+Version: 0.6.0
 Summary: A CLI to reformat and review Canvas grades
 Home-page: https://github.com/joelostblom/canvascli
 Author: Joel Ostblom
 Author-email: joelostblom@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,20 +29,17 @@
 ## Usage
 
 All `canvascli` functionality requires that you have [created an Canvas API access
 token](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-manage-API-access-tokens-as-an-instructor/ta-p/1177),
 so do that first if you don't have one already.
 
 > When running `canvascli`,
-you can either enter your Canvas token when prompted at the command line
+you can either paste your Canvas token when prompted at the command line
 (ideally using a password manager, e.g. [KeePassXC](https://keepassxc.org/)),
-or store it in an environment variable named `CANVAS_PAT`
-(if you are using GitBash's default terminal on Windows,
-you will not be able to paste into the terminal prompt
-and defining the environmental variable is required).
+or [store it in an environment variable](https://www.poftut.com/how-to-set-environment-variables-for-linux-windows-bsd-and-macosx/) named `CANVAS_PAT`.
 
 Typing `canvascli` at the command prompt will show the general help message
 including the available sub-commands.
 The most common use case
 is probably to prepare final grades for FSC submission,
 which you can do like so:
 
@@ -52,35 +49,40 @@
 
 This will save a CSV file in the current directory
 which can be uploaded to the FSC.
 The file should automatically be correctly formatted,
 but it is a good idea to double check
 in case there are unexpected changes
 to how UBC inputs course info on Canvas.
+
 `canvascli` drops students without a grade by default,
 and creates a few helpful visualizations of the final grades
 and assignment scores.
 Run `canvascli prepare-fsc-grades --help`
 to view all available options.
 
-If you don't know the Canvas id of your course,
+If you don't know the Canvas course id of your course,
 `canvascli` can check for you:
 
 ```shell
 canvascli show-courses
 ```
 
 This will output a table with all the courses
 your API token has access to.
 Run `canvascli show-courses --help`
 to view all available options.
 
-## Shell completion
+<details><summary>
+
+## Shell completion (optional, click to expand)
 
-If you want subcommands and options to complete when you press <kbd>TAB</kbd>
+</summary>
+
+If you want suggestions for subcommands and option flags when you press <kbd>TAB</kbd>
 you can download the corresponding completion file
 from the GitHub repository
 and source it in your terminal's configuration file.
 If you don't want to do this manually,
 you can run one of the following commands
 (don't forget to restart your shell afterwards).
 
@@ -103,14 +105,16 @@
 and note that you will only get shell completion after typing `cavascli`,
 not `canvascli.exe`.
 
 ```sh
 curl -Ss https://raw.githubusercontent.com/joelostblom/canvascli/main/canvascli-complete.bash > ~/.canvascli-complete.bash && echo ". ~/.canvascli-complete.bash" >> ~/.bashrc
 ```
 
+</details>
+
 ## Questions and contributing
 
 Questions and contributions are welcome!
 The best way to get in touch is to
 [open a new issue or discussion](https://github.com/joelostblom/canvascli/issues/new/choose).
 Remember to follow the [Code of Conduct](CODE_OF_CONDUCT.md)
 when you participate in this project.
```

### Comparing `canvascli-0.5.1/README.md` & `canvascli-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 ## Usage
 
 All `canvascli` functionality requires that you have [created an Canvas API access
 token](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-manage-API-access-tokens-as-an-instructor/ta-p/1177),
 so do that first if you don't have one already.
 
 > When running `canvascli`,
-you can either enter your Canvas token when prompted at the command line
+you can either paste your Canvas token when prompted at the command line
 (ideally using a password manager, e.g. [KeePassXC](https://keepassxc.org/)),
-or store it in an environment variable named `CANVAS_PAT`
-(if you are using GitBash's default terminal on Windows,
-you will not be able to paste into the terminal prompt
-and defining the environmental variable is required).
+or [store it in an environment variable](https://www.poftut.com/how-to-set-environment-variables-for-linux-windows-bsd-and-macosx/) named `CANVAS_PAT`.
 
 Typing `canvascli` at the command prompt will show the general help message
 including the available sub-commands.
 The most common use case
 is probably to prepare final grades for FSC submission,
 which you can do like so:
 
@@ -41,35 +38,40 @@
 
 This will save a CSV file in the current directory
 which can be uploaded to the FSC.
 The file should automatically be correctly formatted,
 but it is a good idea to double check
 in case there are unexpected changes
 to how UBC inputs course info on Canvas.
+
 `canvascli` drops students without a grade by default,
 and creates a few helpful visualizations of the final grades
 and assignment scores.
 Run `canvascli prepare-fsc-grades --help`
 to view all available options.
 
-If you don't know the Canvas id of your course,
+If you don't know the Canvas course id of your course,
 `canvascli` can check for you:
 
 ```shell
 canvascli show-courses
 ```
 
 This will output a table with all the courses
 your API token has access to.
 Run `canvascli show-courses --help`
 to view all available options.
 
-## Shell completion
+<details><summary>
+
+## Shell completion (optional, click to expand)
 
-If you want subcommands and options to complete when you press <kbd>TAB</kbd>
+</summary>
+
+If you want suggestions for subcommands and option flags when you press <kbd>TAB</kbd>
 you can download the corresponding completion file
 from the GitHub repository
 and source it in your terminal's configuration file.
 If you don't want to do this manually,
 you can run one of the following commands
 (don't forget to restart your shell afterwards).
 
@@ -92,14 +94,16 @@
 and note that you will only get shell completion after typing `cavascli`,
 not `canvascli.exe`.
 
 ```sh
 curl -Ss https://raw.githubusercontent.com/joelostblom/canvascli/main/canvascli-complete.bash > ~/.canvascli-complete.bash && echo ". ~/.canvascli-complete.bash" >> ~/.bashrc
 ```
 
+</details>
+
 ## Questions and contributing
 
 Questions and contributions are welcome!
 The best way to get in touch is to
 [open a new issue or discussion](https://github.com/joelostblom/canvascli/issues/new/choose).
 Remember to follow the [Code of Conduct](CODE_OF_CONDUCT.md)
 when you participate in this project.
```

### Comparing `canvascli-0.5.1/canvascli/main.py` & `canvascli-0.6.0/canvascli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import click
 import numpy as np
 import pandas as pd
 from appdirs import user_data_dir
 from canvasapi import Canvas
 from canvasapi.exceptions import InvalidAccessToken, Unauthorized
 from luddite import get_version_pypi
+from scipy import stats
 from tqdm import tqdm
 # Using https://github.com/biqqles/dataclassy instead of dataclasses from
 # stdlibto allow for dataclass inheritance when there are default values. Could
 # use a custom init but it gets messy and the advantage of using dataclasses is
 # lost. Dataclass inheritance might be fixed in 3.10
 # https://bugs.python.org/issue36077
 from dataclassy import dataclass
@@ -126,32 +127,38 @@
               ' and students that dropped the course after completing some work.'
               ' Default: 0')
 @click.option('--drop-na', default=True, help='Whether to drop students'
               ' that are missing info such as student number.'
               ' Useful for only removing test students. Default: True')
 @click.option('--open-chart', default=None, type=bool, help='Whether to open'
               ' the grade distribution chart automatically.'
-              ' Default: Ask at the end')
-@click.option('--filter-assignments', default='.*', type=str, help='Regex to filter'
-              ' which assignments are included in the visualization (case-sensitive).'
-              ' Does not affect the final grade calculation.'
-              ' Default: All (.*)')
+              ' Default: Ask unless specified')
+@click.option('--filter-assignments', default=None, type=str, help='Regex to filter'
+              ' which assignments are included in the assignment-specific visualizations'
+              ' (case-sensitive). Does not affect the calculation or visualization'
+              ' of the final grades. The special string "False" excludes all assignments. '
+              'Default: Ask unless specified')
+@click.option('--group-by', default=None, type=click.Choice(['Section', 'Grader']),
+              help='Variable to group the visualizations by. A separate box plot'
+              ' will be created for each group. Default: None (`Section` if there'
+              ' are multiple sections, otherwise `Grader` if there are multiple graders,'
+              ' otherwise nothing)')
 @click.option('--override-campus', default=None, help='Override the automatically'
               ' detected course campus in the CSV file with this text. Default: None')
 @click.option('--override-course', default=None, help='Override the automatically'
               ' detected course title in the CSV file with this text. Default: None')
 @click.option('--override-section', default=None, help='Override the automatically'
               ' detected course section in the CSV file with this text. Default: None')
 @click.option('--override-session', default=None, help='Override the automatically'
               ' detected course session in the CSV file with this text. Default: None')
 @click.option('--override-subject', default=None, help='Override the automatically'
               ' detected course subject in the CSV file with this text. Default: None')
 def prepare_fsc_grades(course_id, filename, api_url, student_status,
                        drop_students, drop_threshold, drop_na, open_chart,
-                       filter_assignments, override_campus, override_course,
+                       filter_assignments, group_by, override_campus, override_course,
                        override_section, override_session, override_subject):
     """Prepare course grades for FSC submission.
     \b
     Download grades from a canvas course and convert them to the format
     required by the FSC for submission of final grades.
 
     Grades are rounded to whole percentages and capped at 100.
@@ -167,27 +174,28 @@
         canvascli prepare_fsc_grades --course-id 53665
         \b
         # Give a custom file name and drop a specific student
         canvascli prepare_fsc_grades --course-id 53665 --drop-students "43659202"
     """
     fsc_grades = FscGrades(
         course_id, filename, api_url, student_status, drop_students,
-        drop_threshold, drop_na, open_chart, filter_assignments, override_campus,
+        drop_threshold, drop_na, open_chart, filter_assignments, group_by, override_campus,
         override_course, override_section, override_session, override_subject)
     fsc_grades.connect_to_canvas()
     fsc_grades.connect_to_course()
     fsc_grades.get_canvas_grades()
     fsc_grades.drop_student_entries()
     fsc_grades.convert_grades_to_fsc_format()
     if fsc_grades.fsc_grades.empty:
         click.echo('Did not find any assigned grades, exiting.')
     else:
         fsc_grades.save_fsc_grades_to_file()
-        fsc_grades.plot_assignment_scores()
         fsc_grades.plot_fsc_grade_distribution()
+        fsc_grades.plot_assignment_scores()
+        fsc_grades.layout_and_save_charts()
         fsc_grades.show_manual_grade_entry_note()
     return
 
 
 @cli.command()
 @click.option('--api-url', default='https://canvas.ubc.ca', help='Base canvas URL.'
               ' Default: https://canvas.ubc.ca')
@@ -302,14 +310,15 @@
     api_url: str
     student_status: str
     drop_students: str
     drop_threshold: int
     drop_na: bool
     open_chart: bool
     filter_assignments: str
+    group_by: str
     override_campus: str
     override_course: str
     override_section: str
     override_session: str
     override_subject: str
     unauthorized_course_access_msg: str = (
         '\nYour API token is not authorized to access course {}.'
@@ -329,46 +338,97 @@
         if self.filename is None:
             self.filename = (f'fsc-grades_{self.course.course_code.replace(" ", "-")}'
                              .replace('/', '-'))
         return
 
     def get_canvas_grades(self):
         """Download grades from a canvas course."""
-        click.echo('Downloading student grades...')
         enrollments = self.course.get_enrollments(
             type=['StudentEnrollment'], state=[self.student_status]
         )
         canvas_grades = defaultdict(list)
-        for enrollment in enrollments:
+
+        # We can't know the length of `enrollments` since it is an iterable,
+        # so this is the best progress bar we can get here
+        enrollments_progress_bar = tqdm(
+            enrollments,
+            unit=' students',
+            desc='Downloading student grades',
+            bar_format='{desc}... {n}{unit}'
+        )
+        for enrollment in enrollments_progress_bar:
             canvas_grades['User ID'].append(enrollment.user['id'])
-            canvas_grades['Student Number'].append(enrollment.user['sis_user_id'])
+
+            # `sis_user_id` is removed from concluded courses by Canvas
+            if hasattr(enrollment.user, 'sis_user_id'):
+                canvas_grades['Student Number'].append(enrollment.user['sis_user_id'])
+            else:
+                # A warning about this case is emitted further down
+                canvas_grades['Student Number'].append('N/A')
             surname, preferred_name = enrollment.user['sortable_name'].split(', ')
             canvas_grades['Surname'].append(surname)
             canvas_grades['Preferred Name'].append(preferred_name)
+            canvas_grades['Section'].append(enrollment.course_section_id)
+            # Unposted "current" is what matches what is seen on Canvas for a course in progress
+            # Unposted "final" deducts points for assignments without a grade
+            # (it treats them as if an explicit grade of `0` was given, which is undesirable)
+            canvas_grades['Unposted Percent Grade'].append(enrollment.grades['unposted_current_score'])
 
             # A warning message is later displayed for these students
             if 'override_score' in enrollment.grades:
                 canvas_grades['Percent Grade'].append(enrollment.grades['override_score'])
                 canvas_grades['override_final_score'].append(enrollment.grades['final_score'])
             else:
                 canvas_grades['Percent Grade'].append(enrollment.grades['final_score'])
                 canvas_grades['override_final_score'].append(0)
 
             # A warning message is later displayed for these students
+            # Need to check for "final unposted" here rather than "current unposted"
             if 'unposted_final_score' in enrollment.grades:
-                canvas_grades['Unposted Percent Grade'].append(enrollment.grades['unposted_final_score'])
+                canvas_grades['Unposted Final Grade'].append(enrollment.grades['unposted_final_score'])
                 if enrollment.grades['unposted_final_score'] != enrollment.grades['final_score']:
                     canvas_grades['different_unposted_score'].append(True)
                 else:
                     canvas_grades['different_unposted_score'].append(False)
+            else:
+                canvas_grades['Unposted Final Grade'].append(pd.NA)
+                canvas_grades['different_unposted_score'].append(False)
 
         self.canvas_grades = pd.DataFrame(canvas_grades)
+
+        # Warn about missing student numbers
+        if (pd.DataFrame(canvas_grades)['Student Number'] == 'N/A').any():
+            click.secho('\nWARNING', fg='red', bold=True)
+            click.echo(
+                'Could not find students numbers for at least one student.'
+                '\nThis does not impact the visualizations,'
+                '\nbut you must add student numbers manually'
+                '\nbefore uploading the CSV file to the FSC.'
+                '\nThis could happen because your course has concluded'
+                '\nor because it includes a test student account.\n'
+            )
+
+        # Extract course section IDs for each students
+        # We are relying on the same extraction pattern as for the FSC grades,
+        # which LT hub mentioned should be safe to extract from the
+        # canvas course code (for UBC courses in general).
+        # There is no override for the individual student 
+        # which should be safe.
+        # Originally there was a check to verify that the course section is a number
+        # but it turns out some courses don't use numbers for the sections
+        section_ids_and_names = {
+            section.id: section.name.split()[2]
+            for section in self.course.get_sections()
+        }
+        self.canvas_grades['Section'] = (
+            self.canvas_grades['Section'].map(section_ids_and_names)
+        )
+
         different_unposted_score = self.canvas_grades.pop('different_unposted_score')
         override_final_score = self.canvas_grades.pop('override_final_score')
-
         # Display a note that some student grade are manually overridden
         if override_final_score.sum() > 0:
             click.secho('\nNOTE', fg='yellow', bold=True)
             click.echo(
                 'You have used the "Overide" column on Canvas'
                 '\nto change the final score for the following students:\n'
             )
@@ -384,36 +444,39 @@
                         index=False
                     )
                 )
             click.echo()
 
         # Warn about students with unposted grades that change their final scores
         if different_unposted_score.sum() > 0:
+            students_with_unposted_score = self.canvas_grades.query(
+                '@different_unposted_score == True'
+            # Dropping the unposted percent grade to not cause confusion by showing two "unposted" columns
+            ).drop(
+                columns='Unposted Percent Grade'
+            )
+
             click.secho('\nWARNING', fg='red', bold=True)
             click.echo(
                 'Remember to post all assignments on Canvas'
                 '\nbefore creating the CSV-file to upload to the FSC.'
                 '\nThere are currently unposted Canvas assignments'
-            )
-            students_with_unposted_score = self.canvas_grades.query(
-                '@different_unposted_score == True'
+                '\nthat would change the final score of '
+                + click.style(f'{students_with_unposted_score.shape[0]} students.', bold=True)
             )
             if students_with_unposted_score.shape[0] > 10:
-                click.echo(
-                    'that would change the final score of '
-                    + click.style(f'{students_with_unposted_score.shape[0]} students.', bold=True)
-                )
-                click.echo('Showing the first 10 here:\n')
-                click.echo(students_with_unposted_score[:10].to_markdown(index=False))
+                click.echo('Showing the first 10 in the table below:\n')
             else:
-                click.echo(
-                    'that would change the final score of the following '
-                    + click.style(f'{students_with_unposted_score.shape[0]} students:\n', bold=True)
-                )
-                click.echo(students_with_unposted_score.to_markdown(index=False))
+                click.echo('Showing these students in the table below:\n')
+            # Indexing up until the first 10 works even if there are fewer than 10 entries
+            click.echo(students_with_unposted_score[:10].to_markdown(index=False))
+            click.echo('')
+        # The unposted "final" grade is only needed for the comparison above
+        # For everyhting else, we use the unposted "current" grade
+        self.canvas_grades = self.canvas_grades.drop(columns='Unposted Final Grade')
         return
 
     def drop_student_entries(self):
         """Drop unwanted students entries such as test students and dropouts."""
         # Drop students under the grade thresholds
         # Test accounts and students who dropped the course often have a grade of zero
         dropped_students = self.canvas_grades.query(
@@ -453,43 +516,71 @@
                 f'Dropping {dropped_students.shape[0]}'
                 f" {'students' if dropped_students.shape[0] > 1 else 'student'}"
                 f' with missing information, a grade <= {self.drop_threshold},'
                 '\nor that was explicitly dropped by student number:\n'
             )
             click.echo(dropped_students.to_markdown(index=False))
             click.echo()
+
+        # It seems like students can be registered for multiple sections
+        if self.canvas_grades.duplicated(subset='User ID').sum() > 0:
+            click.secho('WARNING', fg='red', bold=True)
+            click.echo(
+                'The following students are enrolled in multiple sections.'
+                '\nOnly the first occurrence will be kept.'
+            )
+            click.echo(
+                self.canvas_grades[
+                    self.canvas_grades['User ID']
+                    .duplicated(keep=False)
+                ]
+                .drop(columns='Unposted Percent Grade')
+                .to_markdown(index=False)
+            )
+            click.echo()
+            self.canvas_grades = self.canvas_grades.drop_duplicates(subset='User ID')
+
         return
 
     def convert_grades_to_fsc_format(self):
         """Convert grades to FSC format."""
-        # Extract FSC info from canvas
+        self.campus = 'UBC'
         # LT hub mentioned that these fields should be safe to extract from the
         # canvas course code (for UBC courses in general), but there is an override
         # option just in case
-        self.campus = 'UBC'
-        self.subject, self.course_name, self.section, self.session = self.course.course_code.split()
+        # Some course codes include multiple sessions in the name,
+        # which is why we are doing this split in two steps and dropping everything
+        # from index 2 to -2 since the session is already extracted for each student elsewhere
+        subject_coursename_session = self.course.course_code.split()
+        self.subject, self.course_name = subject_coursename_session[:2]
+        self.session = subject_coursename_session[-1]
+
         if self.override_campus is not None:
             self.campus = self.override_campus
         if self.override_course is not None:
             self.course_name = self.override_course
         if self.override_section is not None:
             self.section = self.override_section
         if self.override_session is not None:
             self.session = self.override_session
+        else:
+            # Remove the session number suffix for the automatically extracted value
+            # since this only exists on Canvas but not FSC.
+            # Don't remove anything if a manual value is provided
+            self.session = self.session[:-1]
         if self.override_subject is not None:
             self.subject = self.override_subject
-        # Add FSC info to the dataframe, standing and standing reason are
+        # Add FSC info to the dataframe; standing and standing reason are
         # blank by default and filled out manually when needed
         self.fsc_grades = self.canvas_grades.copy()
-        additional_fsc_fields = ['Campus', 'Course', 'Section', 'Session', 'Subject',
-                      'Standing', 'Standing Reason']
-        # Remove the session number which is only present on Canvas but not FSC
-        self.session = self.session[:-1]
+        additional_fsc_fields = [
+            'Campus', 'Course', 'Session', 'Subject','Standing', 'Standing Reason'
+        ]
         self.fsc_grades[additional_fsc_fields] = (
-            self.campus, self.course_name, self.section, self.session, self.subject, '', '')
+            self.campus, self.course_name, self.session, self.subject, '', '')
 
         # Round to whole percentage format since FSC requires that
         # Using Decimal to always round up .5 instead of rounding to even,
         # which is the default in numpy but could seem unfair to individual students.
         # The Decimal type is not json serializable (issue for altair) so changing to int.
         self.fsc_grades['Exact Percent Grade'] = self.fsc_grades['Percent Grade']
         self.fsc_grades['Percent Grade'] = self.fsc_grades['Percent Grade'].apply(
@@ -514,367 +605,723 @@
             self.filename + '.csv',
             index=False
         )
         click.secho(f'Grades saved to {self.filename}.csv.', bold=True, fg='green')
         return
 
     def plot_assignment_scores(self):
-        assignment_regex = re.compile(self.filter_assignments)
-        assignments = [
-            a for a in self.course.get_assignments()
-            if a.published
-              and a.points_possible is not None
-              and a.points_possible > 0
-              and assignment_regex.search(a.name)
-        ]
+        # Prompt the user if they want to show assignments,
+        # since it takes time to download them and makes the chart more noisy
+        # Only show if `filter_assignments` is not already set to a string,
+        # which indicates that the user already knows they want to include assignments
+        if self.filter_assignments == 'False' or (
+            not isinstance(self.filter_assignments, str)
+            and not click.confirm('Download and plot assignment scores?', default=True)
+        ):
+            # Adding empty charts since there are concated charts later
+            # that rely on the existence of these charts
+            self.assignment_distributions = alt.Chart().mark_point(opacity=0)
+            self.assignment_scores = alt.Chart().mark_point(opacity=0)
+        else:
+            # If we get here it means that the user has selected "Yes" in the prompt,
+            # but not specified a string, so include all assignments
+            if self.filter_assignments is None:
+                self.filter_assignments = ''
+            assignment_regex = re.compile(self.filter_assignments)
+            assignments = [
+                a for a in self.course.get_assignments()
+                if (
+                    a.published
+                    and a.points_possible is not None
+                    and a.points_possible > 0
+                    and a.graded_submissions_exist
+                    and assignment_regex.search(a.name)
+                )
+            ]
 
-        assert assignments, (
-            'No assignment names matched'
-            f' the provided regular expression "{self.filter_assignments}"'
-        )
-        assignment_scores_dfs = []
-        click.echo("Downloading assignment scores...")
-        assignment_progress_bar = tqdm(assignments)
-        for assignment in assignment_progress_bar:
-            assignment_progress_bar.set_description(assignment.name)
-            submissions = assignment.get_submissions()
-            assignment_scores = defaultdict(list)
-            for submission in submissions:
-                assignment_scores['User ID'].append(submission.user_id)
-                assignment_scores['Grader ID'].append(submission.grader_id)
-                assignment_scores['Score'].append(
-                    100 * submission.score / assignment.points_possible
-                    if submission.score is not None else None
-                )
-                assignment_scores['Assignment'].append(assignment.name)
-            assignment_scores_dfs.append(pd.DataFrame(assignment_scores))
-        # fillna required on pandas >=1.4.0 due to https://github.com/pandas-dev/pandas/issues/46922
-        assignment_score_df = pd.concat(assignment_scores_dfs, ignore_index=True).fillna(np.nan)
-        # Sometime a negative number is returned for the grader,
-        # which does not make sense, maybe from gradescope?
-        assignment_score_df.loc[assignment_score_df['Grader ID'] < 0, 'Grader ID']  = pd.NA
-
-        user_ids_and_names = {
-            user.id: [user.name, user.sis_user_id]
-            for user in self.course.get_users()
-        }
-        user_ids_and_names_df = pd.DataFrame.from_dict(
-            user_ids_and_names, orient='index', columns=['Name', 'Student Number']
-        )
-        assignment_score_df['Grader'] = assignment_score_df['Grader ID'].map(user_ids_and_names_df['Name'])
-        assignment_score_df['Student'] = assignment_score_df['User ID'].map(user_ids_and_names_df['Name'])
-        assignment_score_df['Student Number'] = assignment_score_df['User ID'].map(
-            user_ids_and_names_df['Student Number']
-        )
-
-        # Using `round` instead of `Decimal` here
-        # since the latter can't deal with a df with a single `None`
-        # and because this is just to show on the assignment scores,
-        # so it does not have to be fairly rounded like the final FSC grades.
-        assignment_score_df['Score'] = assignment_score_df['Score'].round(2)
-        # self.canvas has had dropped students removed at this point
-        # so we can use it to drop from the assignment score as well
-        assignment_score_df = assignment_score_df.query(
-            '`User ID` in @self.canvas_grades["User ID"]'
-        ).copy()
-
-        grader_order = assignment_score_df.groupby(
-            'Grader'
-        )['Score'].mean().sort_values().index.tolist()
-        # assignment_order is only needed because VL does not support maintaining
-        # the orignal order for facets https://github.com/vega/vega-lite/issues/6221
-        assignment_order = assignment_score_df['Assignment'].unique().tolist()
-        height = max(80, len(grader_order) * 20)
+            # Raise error so that it is clear to the user what happens
+            # when the regex does not match any assignments
+            if not assignments:
+                raise click.ClickException(
+                    click.style(
+                        'No assignment names matched the provided regular expression: '
+                        f'"{self.filter_assignments}". Aborting...',
+                        bold=True,
+                        fg='red'
+                    )
+                )
+
+            assignment_scores_dfs = []
+            click.echo("Downloading assignment scores...")
+            assignment_progress_bar = tqdm(assignments)
+            for assignment in assignment_progress_bar:
+                assignment_progress_bar.set_description(assignment.name)
+                submissions = assignment.get_submissions()
+                assignment_scores = defaultdict(list)
+                for submission in submissions:
+                    assignment_scores['User ID'].append(submission.user_id)
+                    assignment_scores['Grader ID'].append(submission.grader_id)
+                    assignment_scores['Score'].append(
+                        100 * submission.score / assignment.points_possible
+                        if submission.score is not None else None
+                    )
+                    assignment_scores['Assignment'].append(assignment.name)
+                assignment_scores_dfs.append(pd.DataFrame(assignment_scores))
+            # fillna required on pandas >=1.4.0 due to https://github.com/pandas-dev/pandas/issues/46922
+            assignment_score_df = pd.concat(assignment_scores_dfs, ignore_index=True).fillna(np.nan)
+            # Sometime a negative number is returned for the grader,
+            # which does not make sense, maybe from gradescope?
+            assignment_score_df.loc[assignment_score_df['Grader ID'] < 0, 'Grader ID']  = pd.NA
+            user_ids_and_names = {
+                user.id: [user.name, user.sis_user_id if hasattr(user, 'sis_user_id') else 'N/A']
+                for user in self.course.get_users()
+            }
+            user_ids_and_names_df = pd.DataFrame.from_dict(
+                user_ids_and_names, orient='index', columns=['Name', 'Student Number']
+            )
+            assignment_score_df['Grader'] = assignment_score_df['Grader ID'].map(
+                user_ids_and_names_df['Name']
+            )
+            assignment_score_df['Name'] = assignment_score_df['User ID'].map(
+                user_ids_and_names_df['Name']
+            )
+            assignment_score_df['Student Number'] = assignment_score_df['User ID'].map(
+                user_ids_and_names_df['Student Number']
+            )
+            # The section number cannot be extracted via `get_users()`
+            assignment_score_df['Section'] = (
+                assignment_score_df['User ID'].map(
+                    self.canvas_grades.set_index('User ID')['Section']
+                )
+            )
+
+            # Using `round` instead of `Decimal` here
+            # since the latter can't deal with a df with a single `None`
+            # and because this is just to show on the assignment scores,
+            # so it does not have to be fairly rounded like the final FSC grades.
+            assignment_score_df['Score'] = assignment_score_df['Score'].round(2)
+            # self.canvas has had dropped students removed at this point
+            # so we can use it to drop from the assignment score as well
+            assignment_score_df = assignment_score_df.query(
+                '`User ID` in @self.canvas_grades["User ID"]'
+            ).copy()
+
+            # Plot scores for individual assignments
+            # Start by figuring out how many groups there are to set chart height
+            # and in what order to sort
+            if self.group_by is None:
+                if assignment_score_df['Section'].nunique() > 1:
+                    self.group_by = 'Section'
+                elif assignment_score_df['Grader'].nunique() > 1:
+                    self.group_by = 'Grader'
+            height = 80
+            # If group_by is set either manually or automatically above
+            if self.group_by is not None:
+                if self.group_by == 'Section':
+                    self.group_order = self.section_order
+                elif self.group_by == 'Grader':
+                    self.group_order = (
+                        assignment_score_df
+                        .groupby(self.group_by)
+                        ['Score']
+                        .median()
+                        .sort_values()
+                        .index.tolist()
+                    )
+                # Min height=80 for histograms to look nice
+                # 20 is the default step size for categorical scale
+                height = max(height, len(self.group_order) * 20)
+
+            # assignment_order is only needed because VL does not support maintaining
+            # the orignal order for facets https://github.com/vega/vega-lite/issues/6221
+            assignment_order = assignment_score_df['Assignment'].unique().tolist()
+
+            # Constant range 50 - 100 by default
+            # Since this is also used for the scale/axis domain for the boxplots
+            # we need to make sure that the boxplots and bins use the same min value;
+            # a power of 5 works for this since the bin step is 5 so we floor the min value to the closest 5
+            bin_extent = (
+                min(
+                    50,
+                    (assignment_score_df['Score'].min() // 5) * 5
+                ),
+                100
+            )
 
-        assignment_central_tendencies = alt.Chart(
+            boxplot_base = alt.Chart(
                 assignment_score_df
-            ).transform_aggregate(
-                Mean='mean(Score)',
-                Median='median(Score)',
-            ).transform_fold(
-                fold=['Mean', 'Median'],
-                as_=['Type', 'Percent Grade']
-            ).mark_point(
-            size=65,
-            shape='diamond',
-            fill='white'
-        ).encode(
-            x='Percent Grade:Q',
-            y=alt.value(height-6),  # -6 to get the bottom of the marker on the axis line
-            color=alt.Color(
-                'Type:N',
-                title='',
-                scale=alt.Scale(range=['coral', 'rebeccapurple']),
-                legend=None
-            ),
-            tooltip=['Type:N', alt.Tooltip('Percent Grade:Q', format='.3g')]
-        )
+            ).mark_boxplot(outliers={'opacity': 0}, median={'color': 'black'}).encode(
+                alt.X('Score', scale=alt.Scale(zero=False)).scale(domain=bin_extent, nice=False),
+                y=alt.value(height + 10),
+            )
+            boxplots = alt.layer(
+                boxplot_base,
+                boxplot_base.mark_point(size=30, shape='diamond', filled=True).encode(
+                    alt.X('mean(Score)', scale=alt.Scale(zero=False)),
+                    color=alt.value('#353535')
+                ),
+                boxplot_base.transform_aggregate(
+                    min="min(Score)",
+                    max="max(Score)",
+                    mean="mean(Score)",
+                    median="median(Score)",
+                    q1="q1(Score)",
+                    q3="q3(Score)",
+                    count="count()",
+                # Without setting the height here the tooltip region is too narrow,
+                # and the height of the boxplot chart does not matter as it does for the overall grades boxplot,
+                # not sure why it's different.
+                ).mark_bar(opacity=0, height=20).encode(
+                    x='q1:Q',
+                    x2='q3:Q',
+                    tooltip=alt.Tooltip(
+                        ['min:Q', 'q1:Q', 'mean:Q', 'median:Q', 'q3:Q', 'max:Q', 'count:Q'],
+                        format='.1f'
+                    )
+                )
+            )
 
-        # Min height=80 for histograms to look nice
-        # 20 is the default step size for categorical scale
-        self.assignment_distributions = alt.hconcat((
-            alt.Chart(
-                assignment_score_df,
-                height=height,
-            ).mark_bar().encode(
-                x=alt.X('Score', bin=alt.Bin(step=5)),
-                y=alt.Y('count()', title='Student Count'),
-            ) + assignment_central_tendencies
-            ).facet(
-                title=alt.TitleParams(
-                    'Assignment Score Distributions',
-                    subtitle=['Hover over the points to see the exact mean and median score.', ''],
-                    anchor='middle',
-                    dx=25
+            histograms = alt.layer(
+                alt.Chart(
+                    assignment_score_df,
+                    height=height,
+                    width=355
+                ).mark_bar().encode(
+                    x=alt.X('Score', bin=alt.Bin(extent=bin_extent, step=2.5), axis=alt.Axis(offset=20)),
+                    y=alt.Y('count()', title='Student Count'),
                 ),
-                facet=alt.Facet('Assignment', title='', sort=assignment_order),
-                columns=1
-            ), alt.Chart(
-                assignment_score_df.reset_index(),
-                height=height + 2,
-            ).mark_boxplot(median={'color': 'black'}).encode(
-                x=alt.X('Score', scale=alt.Scale(zero=False)),
-                y=alt.Y('Grader:N', sort=grader_order, title='', axis=alt.Axis(orient='right')),
-                color=alt.Color('Grader:N', sort=grader_order, legend=None)
+                boxplots,
             ).facet(
-                title=alt.TitleParams(
-                    'Comparison Between Graders',
-                    subtitle=['Hover over the box for detailed grader info.', ''],
-                    anchor='middle',
-                    dx=-40
+                title=alt.Title(
+                    'Assignment Score Distributions',
+                    subtitle=[
+                        'Hover over the box to view exact summary statistics.',
+                        'The "--filter-assignment" option controls what is shown here.'
+                    ],
+                    anchor='start',
+                    dx=35,
+                    dy=-5
                 ),
-                facet=alt.Facet('Assignment', title='', sort=assignment_order),
+                facet=alt.Facet('Assignment', title='', sort=assignment_order, header=alt.Header(labelPadding=0)),
                 columns=1
-            ).resolve_scale(
-                y='independent',  # Don't use the same y-axis ticks for each faceted boxplot
-            ),
-            spacing=60
-        ).resolve_scale(
-            color='independent'  # Don't use the mean/median color range for the boxplot
-        )
+            ).resolve_axis(
+                x='independent'
+            )
 
-        # Plot assignment scores
-        assignment_score_df['Assignment scores stdev'] = assignment_score_df['User ID'].map(
-            assignment_score_df.groupby('User ID')['Score'].std()
-        )
-        self.hover = alt.selection_single(
-            fields=['User ID'], on='mouseover', nearest=True, empty='none'
-        )
-        base = alt.Chart(
+            if self.group_by is not None:
+                boxplot_base = alt.Chart(
+                    assignment_score_df.reset_index(),
+                    height=height + 20,
+                ).mark_boxplot(median={'color': 'black'}).encode(  # TODO increase thickness and switch from black in new altair version
+                    alt.X('Score', scale=alt.Scale(zero=False, domain=bin_extent, nice=False)),
+                    alt.Y(
+                        f'{self.group_by}:N',
+                        sort=self.group_order,
+                        title='',
+                        axis=alt.Axis(orient='right')
+                    ),
+                    alt.Color(
+                        f'{self.group_by}:N',
+                        sort=self.group_order[::-1],  # Reverse so that the highest value closest to the axis gets the most important color
+                        legend=None,
+                        scale=alt.Scale(range=self.colorscheme_groups)
+                    )
+                )
+                boxplots = alt.layer(
+                    boxplot_base,
+                    boxplot_base.mark_point(size=30, shape='diamond', filled=True).encode(
+                        alt.X('mean(Score)', scale=alt.Scale(zero=False)),
+                        color=alt.value('#353535')
+                    ),
+                    boxplot_base.transform_aggregate(
+                        min="min(Score)",
+                        max="max(Score)",
+                        mean="mean(Score)",
+                        median="median(Score)",
+                        q1="q1(Score)",
+                        q3="q3(Score)",
+                        count="count()",
+                        groupby=[f'{self.group_by}']
+                    ).mark_bar(opacity=0).encode(
+                        x='q1:Q',
+                        x2='q3:Q',
+                        tooltip=alt.Tooltip(
+                            ['min:Q', 'q1:Q', 'mean:Q', 'median:Q', 'q3:Q', 'max:Q', 'count:Q'],
+                            format='.1f'
+                        )
+                    )
+                ).facet(
+                    title=alt.Title(
+                        f'Comparison Between {self.group_by}s',
+                        subtitle=[
+                            'Hover over the box to view exact summary statistics.',
+                            'The "--group-by" option controls what is shown here.'
+                        ],
+                        anchor='start',
+                        dy=-5
+                    ),
+                    facet=alt.Facet('Assignment', title='', sort=assignment_order, header=alt.Header(labelPadding=0)),
+                    columns=1
+                ).resolve_scale(
+                    y='independent' if self.group_by == 'Grader' else 'shared'
+                ).resolve_axis(
+                    x='independent'
+                )
+
+                self.assignment_distributions = alt.hconcat(
+                    histograms,
+                    boxplots,
+                    spacing=100
+                ).resolve_scale(
+                    color='independent'  # Don't use the mean/median color range for the boxplot
+                )
+            else:
+                self.assignment_distributions = histograms
+
+            # Plot assignment scores
+            assignment_score_df['Assignment scores stdev'] = assignment_score_df['User ID'].map(
+                assignment_score_df.groupby('User ID')['Score'].std()
+            )
+            base = alt.Chart(
                 assignment_score_df,
-                title=alt.TitleParams(
+                title=alt.Title(
                     'Student Assignment Scores',
                     subtitle=[
                         'Hover near a point to highlight a line.',
                         'Hover directly over a point to view student info.',
-                        'Click the three dots button to the right to save this entire page.',
+                        'Click the "..." button to the right to save this page as PNG/SVG.',
                     ],
-                    anchor='middle',
-                    dx=25
+                    anchor='start',
+                    dx=40
                 ),
             ).mark_point(opacity=0).encode(
-            y=alt.Y('Score', scale=alt.Scale(zero=False), title='Assignment Score (%)'),
-            detail='User ID',
-            x=alt.X('Assignment', title='', sort=assignment_order),
-            # Having the tooltip here instead of in the transformed chart
-            # makes it work with nearest,
-            # but significantly slows down the higlighting of the line
-            # tooltip=['Student', 'Student Number', 'Score'],
-        )
-        width = min(1000, max(400, 80 * assignment_score_df['Assignment'].nunique()))
-        self.assignment_scores = (
-            base.add_selection(
-                self.hover
-            ) + base.mark_line(opacity=0.5, interpolate='monotone').encode(
-                color=alt.Color(
-                    'Assignment scores stdev',
-                    scale=alt.Scale(scheme='cividis', reverse=True),
-                    title=['Stdev between', 'Assignments']
-                )
-            ) + (base.mark_line(size=3, interpolate='monotone', color='maroon')
-            + base.mark_circle(size=70, color='maroon', opacity=1).encode(
-                tooltip=['Student', 'Student Number', 'Score'],
-                )
+                y=alt.Y('Score', scale=alt.Scale(zero=False), title='Assignment Score (%)'),
+                detail='User ID',
+                x=alt.X('Assignment', title='', sort=assignment_order),
+                # Having the tooltip here instead of in the transformed chart
+                # makes it work with nearest,
+                # but significantly slows down the higlighting of the line
+                tooltip=['Name', 'Student Number', 'Score'],
             ).transform_filter(
-                self.hover
-            )).properties(
-                width=width,
-                height=280,
-            ).interactive()
-        return
+                alt.expr.test(alt.expr.regexp(self.search_input, 'i'), alt.datum.Name)
+            )
+            width = min(1000, max(400, 80 * assignment_score_df['Assignment'].nunique()))
+            self.assignment_scores = (
+                base.add_params(
+                    self.hover
+                ) + base.mark_line(opacity=0.5, interpolate='monotone').encode(
+                    color=alt.Color(
+                        'Assignment scores stdev',
+                        scale=alt.Scale(scheme='cividis', reverse=True),
+                        title=['Stdev between', 'Assignments']
+                    )
+                ) + (base.mark_line(size=3, interpolate='monotone', color='maroon')
+                + base.mark_circle(size=70, color='maroon', opacity=1).encode(
+                    # tooltip=['Name', 'Student Number', 'Score'],
+                    )
+                ).transform_filter(
+                    self.hover
+                )).properties(
+                    width=width,
+                    height=280,
+                ).interactive()
+            return
 
     def plot_fsc_grade_distribution(self):
+
+        def _compute_violin_cloud(series):
+            """Create a violin-shaped point cloud.
+
+            Compute the KDE and then place each point
+            at a random position within the bounds of the KDE at that location.
+            """
+
+            # TODO include a scaling parameter so that few points renders a more compressed violin
+
+            # The KDE needs at least 3 unique points to be computed
+            if series.nunique() < 3:
+                return pd.Series([0] * series.shape[0])
+            # NAs are not supported in SciPy's density calculation
+            na_series = series[series.isna()]
+            no_na_series = series.dropna()
+            no_na_sorted_series = no_na_series.sort_values()
+
+            # Compute the density function of the data
+            dens = stats.gaussian_kde(no_na_series)
+            # Compute the density value for each data point
+            pdf = dens(no_na_sorted_series)
+            # Normalize the y-range so that the aces domain can be set predictably
+            pdf = (pdf - pdf.min()) / (pdf.max() - pdf.min())
+
+            # Randomly jitter points within 0 and the upper bond of the probability density function
+            violin_cloud = np.empty(pdf.shape[0])
+            for i in range(pdf.shape[0]):
+                violin_cloud[i] = np.random.uniform(0, pdf[i])
+            # To create a symmetric density/violin, we make every second point negative
+            # Distributing every other point like this is also more likely to preserve the shape of the violin
+            violin_cloud[::2] = violin_cloud[::2] * -1
+            # Sorting by index makes it possible to merge with another df in the same order as the original one,
+            # even if the index labels might differ
+            return pd.concat([pd.Series(violin_cloud, index=no_na_sorted_series.index), na_series]).sort_index()
+
         # Prepare dataframe for filtering via Altair selection elements
         # First the rounded and raw scores are melted together separately for posted and unposted scores
         # Then they are merged into one frame and the posted and unposted score are melted together
         self.fsc_grades_for_viz = pd.merge(
             # Frame 1
             self.fsc_grades.rename(
                 columns={
                     'Unposted Percent Grade': 'FSC Rounded',
-                    'Unposted Exact Percent Grade': 'Exact'
+                    'Unposted Exact Percent Grade': 'Exact Percent'
                 }
-            # Combine the rounded and raw *unposted* scores 
+            ).assign(
+                # Computing the percentile based score on the rounded percent and with the "max" method
+                # is more lenient/beneficial for students
+                # since they get the max percentile value of everyone with the same score.
+                # This also seems more fair since the FSC rounded percentage
+                # is their actual final grade in the course.
+                Percentile=lambda df: df['FSC Rounded'].rank(pct=True, method='max').round(2) * 100
+            # Combine the rounded and raw *unposted* scores
             ).melt(
-                id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID'],
-                value_vars=['FSC Rounded', 'Exact'],
+                id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID', 'Section', 'Percentile'],
+                value_vars=['FSC Rounded', 'Exact Percent'],
                 value_name='Unposted Grade',
                 var_name='Percent Type'
             ),
             # Frame 2
             self.fsc_grades.rename(
                 columns={
                     'Percent Grade': 'FSC Rounded',
-                    'Exact Percent Grade': 'Exact'
+                    'Exact Percent Grade': 'Exact Percent'
                 }
-            # Combine the rounded and raw *posted* scores 
+            # Combine the rounded and raw *posted* scores
             ).melt(
-                id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID'],
-                value_vars=['FSC Rounded', 'Exact'],
+                id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID', 'Section'],
+                value_vars=['FSC Rounded', 'Exact Percent'],
                 value_name='Posted Grade',
                 var_name='Percent Type'
             )
         # Combine the posted and unposted scores
         ).melt(
-            id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID', 'Percent Type'],
+            id_vars=['Preferred Name', 'Surname', 'Student Number', 'User ID', 'Percent Type', 'Section', 'Percentile'],
             value_vars=['Unposted Grade', 'Posted Grade'],
             value_name='Percent Grade',
             var_name='Grade Status'
-        )
+        # This sorting of values is required to line up the points with the violin cloud below
+        ).sort_values(['User ID', 'Grade Status', 'Percent Type', 'Percent Grade'])
+
+        # This sorting of values and the index reset is required to line up the violin cloud with the df above
+        self.fsc_grades_for_viz['violin_cloud'] = self.fsc_grades.sort_values(
+            ['User ID', 'Percent Grade']
+        ).reset_index()[[
+            'Exact Percent Grade',
+            'Percent Grade',
+            'Unposted Exact Percent Grade',
+            'Unposted Percent Grade',
+        ]].apply(
+            _compute_violin_cloud
+        ).stack(
+            dropna=False
+        ).to_numpy()
 
         # Set up selection elements
         grade_status_dropdown = alt.binding_select(
             options=['Posted Grade', 'Unposted Grade'],
-            name='Grade Status '
+            name=' '
         )
-        grade_status_selection = alt.selection_single(
+        self.grade_status_selection = alt.selection_point(
             fields=['Grade Status'],
             bind=grade_status_dropdown,
-            init={'Grade Status': 'Unposted Grade'}
+            value=[{'Grade Status': 'Unposted Grade'}]
         )
         percent_type_dropdown = alt.binding_select(
-            options=['FSC Rounded', 'Exact'],
-            name='Percent Type '
+            options=['FSC Rounded', 'Exact Percent'],
+            name=' '
         )
-        percent_type_selection = alt.selection_single(
+        self.percent_type_selection = alt.selection_point(
             fields=['Percent Type'],
             bind=percent_type_dropdown,
-            init={'Percent Type': 'Exact'}
+            value=[{'Percent Type': 'Exact Percent'}]
+        )
+        self.search_input = alt.param(
+            value='',
+            bind=alt.binding(
+                input='search',
+                placeholder="Search name",
+                name=' ',
+            )
         )
 
-        # Plot distribution
-        hist = alt.Chart(self.fsc_grades_for_viz, height=200).mark_bar().encode(
-            alt.X('Percent Grade', bin=alt.Bin(step=5), title='', axis=alt.Axis(labels=False)),
+        # Plot overall grade distribution
+
+        # Constant range 50 - 100 by default
+        # Since this is also used for the scale/axis domain for the boxplots
+        # we need to make sure that the boxplots and bins use the same min value;
+        # a power of 5 works for this since the bin step is 5 so we floor the min value to the closest 5
+        bin_extent = (
+            min(
+                50,
+                (
+                    self.fsc_grades_for_viz.query(
+                        '`Grade Status` == "Unposted Grade"'
+                    )['Percent Grade'].min()
+                    // 5
+                ) * 5
+            ),
+            100
+        )
+        axis_values = list(range(int(bin_extent[0]), int(bin_extent[1]) + 1, 5))
+        self.hist = alt.Chart(self.fsc_grades_for_viz, height=180, width=355).mark_bar().encode(
+            alt.X('Percent Grade', bin=alt.Bin(extent=bin_extent, step=2.5), title='', axis=alt.Axis(labels=False, values=axis_values)),
             alt.Y('count()', title='Student Count')
         )
 
+        # Plot box
+        box_base = alt.Chart(
+            self.fsc_grades_for_viz,
+            height=20
+        # The opacity setting makes sure that the scale is lined up with the hisotrgams
+        # while not showing outliers
+        ).mark_boxplot(outliers={'opacity': 0}, median={'color': 'black'}).encode(
+            alt.X('Percent Grade', title='Final Percent Grade')
+                .scale(domain=bin_extent, nice=False)
+                .axis(values=axis_values),
+            y=alt.value(10)
+        )
+        self.box = alt.layer(
+            box_base,
+            box_base.mark_point(size=25, shape='diamond', filled=True).encode(
+                alt.X('mean(Percent Grade)', scale=alt.Scale(zero=False)),
+                color=alt.value('#353535')
+            ),
+            # Transparent tooltip box
+            box_base.transform_aggregate(
+                min="min(Percent Grade)",
+                max="max(Percent Grade)",
+                mean="mean(Percent Grade)",
+                median="median(Percent Grade)",
+                q1="q1(Percent Grade)",
+                q3="q3(Percent Grade)",
+                count="count()",
+            ).mark_bar(opacity=0).encode(
+                x='q1:Q',
+                x2='q3:Q',
+                tooltip=alt.Tooltip(
+                    ['min:Q', 'q1:Q', 'mean:Q', 'median:Q', 'q3:Q', 'max:Q', 'count:Q'],
+                    format='.1f'
+                )
+            )
+        )
+
         # Plot all observations
-        strip = alt.Chart(self.fsc_grades_for_viz, height=70).mark_point(
+        self.strip = alt.Chart(self.fsc_grades_for_viz, height=70).mark_point(
             size=20
         ).transform_calculate(
-            # Generate Gaussian jitter with a Box-Muller transform
-            jitter='sqrt(-2*log(random()))*cos(2*PI*random())',
             Name='datum["Preferred Name"] + " " + datum["Surname"]'
         ).encode(
-            alt.X('Percent Grade',
-                title='Final Percent Grade',
+            alt.X(
+                'Percent Grade',
+                title='',
+                axis=alt.Axis(
+                    labels=False,
+                    ticks=False,
+                    domain=False,
+                    values=axis_values
+                ),
                 scale=alt.Scale(
                     zero=False,
                     nice=False,
-                    padding=5
                 )
             ),
-            alt.Y('jitter:Q',
-                scale=alt.Scale(padding=2),
+            alt.Y(
+                'violin_cloud',
+                scale=alt.Scale(padding=5, domain=(-1, 1)),
                 axis=alt.Axis(
                     domain=False,
                     title='',
                     labels=False,
                     ticks=False,
                     grid=False
                 )
             ),
-            alt.Tooltip(['Name:N', 'Student Number', 'Percent Grade']),
+            alt.Tooltip(['Name:N', 'Student Number', 'Percent Grade', 'Percentile']),
         )
 
-        strip_overlay = strip.mark_circle(size=80, opacity=1).encode(
+        self.hover = alt.selection_point(
+            fields=['User ID'], on='mouseover', nearest=True, empty=False, clear='mouseout'
+        )
+        self.strip_overlay = self.strip.mark_circle(size=80, opacity=1).encode(
             color=alt.value('maroon')
         ).transform_filter(
             self.hover
         )
 
-        # Plot central tendencies
-        central_tendencies = alt.Chart(
-                self.fsc_grades_for_viz
-            ).transform_aggregate(
-                Mean='mean(Percent Grade)',
-                Median='median(Percent Grade)',
-            ).transform_fold(
-                fold=['Mean', 'Median'],
-                as_=['Type', 'Percent Grade']
-            ).transform_calculate(
-                y='-3.05',
-            ).mark_point(
-            size=65,
-            shape='diamond'
-        ).encode(
-            x='Percent Grade:Q',
-            y='y:Q',
-            color=alt.Color(
-                'Type:N',
-                title='',
-                scale=alt.Scale(range=['coral', 'rebeccapurple']),
-                legend=alt.Legend(legendY=300, legendX=295, orient='none', columns=2)
-            ),
-            tooltip=['Type:N', alt.Tooltip('Percent Grade:Q', format='.3g')]
-        )
+        # This is set regardless of how many sections there are since it would be used if group-by is 'Grader' as well
+        self.colorscheme_groups = [
+        # Tableau without the first blue
+        # since I already use that for all sections togethter
+             '#f58518',
+             '#e45756',
+             '#72b7b2',
+             '#54a24b',
+             '#eeca3b',
+             '#b279a2',
+             '#ff9da6',
+             '#9d755d',
+             '#bab0ac'
+        ]
 
+        # In case "Section" is explicitly passed to group-by
+        # although there is only one section
+        self.section_order = (
+            self.fsc_grades_for_viz
+            .query('`Percent Type` == "Exact Percent" & `Grade Status` == "Unposted Grade"')
+            .groupby('Section')
+            ['Percent Grade']
+            .median()
+            .sort_values()
+            .index.tolist()
+        )
+        # Compare sections if there are more than one (or explicitily specified)
+        if self.group_by is None:
+            if self.fsc_grades_for_viz['Section'].nunique() > 1:
+                self.group_by = 'Section'
+        if self.group_by == 'Section':
+            title_sections = alt.Title(
+                text=['', 'Comparison Between Sections'],
+                anchor='start'
+            )
+
+            box_base_sections = alt.Chart(
+                self.fsc_grades_for_viz,
+                title=title_sections
+            # The opacity setting makes sure that the scale is lined up with the hisotrgams
+            # while not showing outliers
+            ).mark_boxplot(outliers={'opacity': 0}, median={'color': 'black'}).encode(
+                alt.X('Percent Grade', title='Final Percent Grade')
+                    .scale(domain=bin_extent, nice=False)
+                    .axis(values=axis_values),
+                alt.Y(
+                    'Section:N',
+                    sort=self.section_order,
+                    title='',
+                    axis=alt.Axis(orient='right')
+                ),
+                alt.Color(
+                    'Section:N',
+                    sort=self.section_order[::-1],  # Reverse so that the highest value closest to the axis gets the most important color
+                    legend=None,
+                    scale=alt.Scale(range=self.colorscheme_groups)
+                )
+            )
+            self.box_sections = alt.layer(
+                box_base_sections,
+                box_base_sections.mark_point(size=25, shape='diamond', filled=True).encode(
+                    alt.X('mean(Percent Grade)', scale=alt.Scale(zero=False)),
+                    alt.Y(
+                        'Section:N',
+                        sort=self.section_order,
+                        title='',
+                        axis=alt.Axis(orient='right')
+                    ),
+                    color=alt.value('#353535')
+                ),
+                # Transparent tooltip box
+                box_base_sections.transform_aggregate(
+                    min="min(Percent Grade)",
+                    max="max(Percent Grade)",
+                    mean="mean(Percent Grade)",
+                    median="median(Percent Grade)",
+                    q1="q1(Percent Grade)",
+                    q3="q3(Percent Grade)",
+                    count="count()",
+                    groupby=['Section']
+                ).mark_bar(opacity=0).encode(
+                    x='q1:Q',
+                    x2='q3:Q',
+                    tooltip=alt.Tooltip(
+                        ['min:Q', 'q1:Q', 'mean:Q', 'median:Q', 'q3:Q', 'max:Q', 'count:Q'],
+                        format='.1f'
+                    )
+                )
+            )
+        return
+
+    def layout_and_save_charts(self):
         # Add instructions
-        title = alt.TitleParams(
-            text=f'Final Grade Distribution {self.subject} {self.course_name}',
+        title = alt.Title(
+            text=f'Grade Distribution {self.subject} {self.course_name}',
             subtitle=[
-                'Hover near a point to highlight it and view student info.',
-                'Zoom with the mouse wheel and double click to reset the view.',
-                'Changes in the dropdown menus below only affect this chart'
+                'Hover near a point to view student info.',
+                'Hover over the box to view exact summary statistics.',
+                'Changes in the dropdown menus below only affect this chart',
+                '',
+                ''
             ],
-            anchor='middle',
-            dx=25
+            anchor='start',
+            dx=35
         )
 
         # Concatenate, add filters, and save the chart
         chart_filename = self.filename + '.html'
-        alt.vconcat((alt.vconcat(
-            hist,
-            # strip on top so that individual observations are always visible
-            strip.add_selection(self.hover).interactive() + strip_overlay + central_tendencies,
-            spacing=0
-        ).properties(
-            title=title
-        ).resolve_scale(
-            x='shared'
-        ).transform_filter(
-                percent_type_selection & grade_status_selection
-        ).add_selection(
-            percent_type_selection, grade_status_selection
-        ) | self.assignment_scores), self.assignment_distributions, spacing=60
+        alt.vconcat(
+            alt.hconcat(
+                alt.vconcat(
+                    self.hist.add_params(
+                        self.percent_type_selection,
+                        self.grade_status_selection,
+                        self.search_input
+                    ),
+                    self.strip.add_params(self.hover).transform_filter(
+                        alt.expr.test(alt.expr.regexp(self.search_input, 'i'), alt.datum.Name)
+                    ).interactive() + self.strip_overlay,
+                    # x='shared' is required here for the `axis_values` to set the x-ticks correctly
+                    # Without it, the ticks do not line up with the histogram ticks
+                    alt.vconcat(
+                        self.box,
+                        self.box_sections
+                    ).resolve_scale(x='shared') if hasattr(self, 'box_sections') else self.box,
+                    spacing=0
+                ).properties(
+                    title=title
+                ).resolve_scale(
+                    x='shared'
+                ).transform_filter(
+                    self.percent_type_selection & self.grade_status_selection
+                ),
+                self.assignment_scores,
+                spacing=50
+            ),
+            self.assignment_distributions,
+            spacing=40
         ).resolve_scale(
             color='independent'
+        ).configure_view(
+            stroke=None
         ).save(
             chart_filename
         )
         # The label names are styled in serif by default for some reason
         with open(chart_filename, 'a') as chart_file:
             chart_file.write(
                 '\n<style>'
                 '\n    form.vega-bindings {'
                 '\n        font-family: sans-serif;'
                 '\n        font-size: 12px;'
                 '\n        position: absolute;'
-                '\n        left: 60px;'
-                '\n        top: 395px;'
+                '\n        opacity: 0.75;'
+                '\n        display: flex;'
+                '\n        gap: 5px;'
+                # This could be more left when there are only two digits in the y-axis,
+                # but then it looks weird with three digits
+                '\n        left: 35px;'
+                '\n        top: 65px;'
+                '\n    }'
+                '\n    input[type="search"] {'
+                '\n        width: 120px;'
                 '\n    }'
                 '\n</style>'
             )
         click.secho(f'Grade distribution chart saved to {chart_filename}.', bold=True, fg='green')
         if self.open_chart or self.open_chart is None and click.confirm(
                 'Open grade distribution chart?', default=True):
             click.launch(chart_filename)
```

### Comparing `canvascli-0.5.1/canvascli.egg-info/PKG-INFO` & `canvascli-0.6.0/canvascli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvascli
-Version: 0.5.1
+Version: 0.6.0
 Summary: A CLI to reformat and review Canvas grades
 Home-page: https://github.com/joelostblom/canvascli
 Author: Joel Ostblom
 Author-email: joelostblom@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,20 +29,17 @@
 ## Usage
 
 All `canvascli` functionality requires that you have [created an Canvas API access
 token](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-manage-API-access-tokens-as-an-instructor/ta-p/1177),
 so do that first if you don't have one already.
 
 > When running `canvascli`,
-you can either enter your Canvas token when prompted at the command line
+you can either paste your Canvas token when prompted at the command line
 (ideally using a password manager, e.g. [KeePassXC](https://keepassxc.org/)),
-or store it in an environment variable named `CANVAS_PAT`
-(if you are using GitBash's default terminal on Windows,
-you will not be able to paste into the terminal prompt
-and defining the environmental variable is required).
+or [store it in an environment variable](https://www.poftut.com/how-to-set-environment-variables-for-linux-windows-bsd-and-macosx/) named `CANVAS_PAT`.
 
 Typing `canvascli` at the command prompt will show the general help message
 including the available sub-commands.
 The most common use case
 is probably to prepare final grades for FSC submission,
 which you can do like so:
 
@@ -52,35 +49,40 @@
 
 This will save a CSV file in the current directory
 which can be uploaded to the FSC.
 The file should automatically be correctly formatted,
 but it is a good idea to double check
 in case there are unexpected changes
 to how UBC inputs course info on Canvas.
+
 `canvascli` drops students without a grade by default,
 and creates a few helpful visualizations of the final grades
 and assignment scores.
 Run `canvascli prepare-fsc-grades --help`
 to view all available options.
 
-If you don't know the Canvas id of your course,
+If you don't know the Canvas course id of your course,
 `canvascli` can check for you:
 
 ```shell
 canvascli show-courses
 ```
 
 This will output a table with all the courses
 your API token has access to.
 Run `canvascli show-courses --help`
 to view all available options.
 
-## Shell completion
+<details><summary>
+
+## Shell completion (optional, click to expand)
 
-If you want subcommands and options to complete when you press <kbd>TAB</kbd>
+</summary>
+
+If you want suggestions for subcommands and option flags when you press <kbd>TAB</kbd>
 you can download the corresponding completion file
 from the GitHub repository
 and source it in your terminal's configuration file.
 If you don't want to do this manually,
 you can run one of the following commands
 (don't forget to restart your shell afterwards).
 
@@ -103,14 +105,16 @@
 and note that you will only get shell completion after typing `cavascli`,
 not `canvascli.exe`.
 
 ```sh
 curl -Ss https://raw.githubusercontent.com/joelostblom/canvascli/main/canvascli-complete.bash > ~/.canvascli-complete.bash && echo ". ~/.canvascli-complete.bash" >> ~/.bashrc
 ```
 
+</details>
+
 ## Questions and contributing
 
 Questions and contributions are welcome!
 The best way to get in touch is to
 [open a new issue or discussion](https://github.com/joelostblom/canvascli/issues/new/choose).
 Remember to follow the [Code of Conduct](CODE_OF_CONDUCT.md)
 when you participate in this project.
```

### Comparing `canvascli-0.5.1/setup.py` & `canvascli-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,24 @@
     url='https://github.com/joelostblom/canvascli',
 
     python_requires='>=3.8',
     py_modules=['canvascli'],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        'altair>=4.2.0',
+        'altair>=5.0.0rc1',
         'canvasapi>=2.1.0',
         'click>=8.0.0',
         'pandas>=1.1.0',
         'tabulate>=0.8.3',
         'dataclassy>=0.10',
         'luddite>=1.0',
         'appdirs>=1.0',
-        'tqdm>=4.40'
+        'tqdm>=4.40',
+        'scipy>=1.4.0',
     ],
     entry_points={
         'console_scripts': [
             'canvascli = canvascli.main:cli',
         ],
     },
 )
```

### Comparing `canvascli-0.5.1/versioneer.py` & `canvascli-0.6.0/versioneer.py`

 * *Files identical despite different names*

