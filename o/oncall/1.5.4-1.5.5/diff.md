# Comparing `tmp/oncall-1.5.4.tar.gz` & `tmp/oncall-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oncall-1.5.4.tar", last modified: Tue Apr  4 15:07:00 2023, max compression
+gzip compressed data, was "oncall-1.5.5.tar", last modified: Wed May  3 19:40:17 2023, max compression
```

## Comparing `oncall-1.5.4.tar` & `oncall-1.5.5.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.441066 oncall-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-04 15:06:48.000000 oncall-1.5.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-04 15:06:48.000000 oncall-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-04 15:06:48.000000 oncall-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-04 15:06:48.000000 oncall-1.5.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-04 15:07:00.441066 oncall-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-04 15:06:48.000000 oncall-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:07:00.441066 oncall-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-04 15:06:48.000000 oncall-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.421064 oncall-1.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.425065 oncall-1.5.4/src/oncall/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.425065 oncall-1.5.4/src/oncall/api/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/api/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/bonus_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/event_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/event_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/event_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/events_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical_key_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical_key_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical_key_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/ical_key_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/iris_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/notification_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/populate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/public_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/roster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/roster_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/roster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/roster_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/rosters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/service_oncall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/service_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_iris_escalate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_oncall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/team_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8062 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/upcoming_shifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_pinned_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_pinned_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/user_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/api/v0/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/auth/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/modules/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/modules/ldap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/auth/modules/ldap_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/build_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/notifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2120 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/run_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/bin/user_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/doc_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/iris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/messengers/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/messengers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/messengers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/messengers/iris_messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/messengers/rocketchat_messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/messengers/teams_messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/metrics/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/metrics/influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/metrics/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.433065 oncall-1.5.4/src/oncall/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/notifier/reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/notifier/user_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.437066 oncall-1.5.4/src/oncall/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/scheduler/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/scheduler/no-skip-matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/scheduler/round-robin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/sphinx_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.437066 oncall-1.5.4/src/oncall/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.421064 oncall-1.5.4/src/oncall/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.437066 oncall-1.5.4/src/oncall/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/css/incalendar.css
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/css/loginsplash.css
--rw-r--r--   0 runner    (1001) docker     (123)    43949 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/css/oncall.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.437066 oncall-1.5.4/src/oncall/ui/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   476120 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/fonts/Source-Sans-Pro.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.437066 oncall-1.5.4/src/oncall/ui/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/chevron-bottom.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/headshot-blank.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/inbug.png
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/oncall_logo_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/images/oncall_logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.441066 oncall-1.5.4/src/oncall/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    64520 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/handlebars-4.0.12.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    82802 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/incalendar.js
--rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    79882 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/loginsplash.js
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/moment-timezone.js
--rw-r--r--   0 runner    (1001) docker     (123)   178745 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/moment-tz-data-full.js
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/moment-tz-data.js
--rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/moment.js
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/navigo.js
--rw-r--r--   0 runner    (1001) docker     (123)   136032 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/oncall.js
--rw-r--r--   0 runner    (1001) docker     (123)    96224 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/static/js/typeahead.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.441066 oncall-1.5.4/src/oncall/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    22629 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    87643 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/ui/templates/loginsplash.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.441066 oncall-1.5.4/src/oncall/user_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/user_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/user_sync/ldap_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/user_sync/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-04 15:06:48.000000 oncall-1.5.4/src/oncall/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.425065 oncall-1.5.4/src/oncall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 15:07:00.000000 oncall-1.5.4/src/oncall.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:07:00.441066 oncall-1.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-04 15:06:48.000000 oncall-1.5.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-04 15:06:48.000000 oncall-1.5.4/test/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-04-04 15:06:48.000000 oncall-1.5.4/test/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.877219 oncall-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 19:40:06.000000 oncall-1.5.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-03 19:40:06.000000 oncall-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 19:40:06.000000 oncall-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-05-03 19:40:06.000000 oncall-1.5.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 19:40:17.873219 oncall-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-03 19:40:06.000000 oncall-1.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:40:17.877219 oncall-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-03 19:40:06.000000 oncall-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.861219 oncall-1.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.861219 oncall-1.5.5/src/oncall/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.865219 oncall-1.5.5/src/oncall/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/bonus_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/event_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/event_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/event_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/events_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical_key_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical_key_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical_key_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/ical_key_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/iris_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/notification_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/populate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/public_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/roster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/roster_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/roster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/roster_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/rosters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/service_oncall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/service_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_iris_escalate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_oncall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/team_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8493 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/upcoming_shifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_pinned_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_pinned_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/user_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/api/v0/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/auth/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/modules/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/modules/ldap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/auth/modules/ldap_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/build_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/notifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2120 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/bin/user_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/doc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/iris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/messengers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/messengers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/messengers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/messengers/iris_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/messengers/rocketchat_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/messengers/teams_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/metrics/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/metrics/influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/metrics/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/notifier/reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/notifier/user_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/scheduler/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/scheduler/no-skip-matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/scheduler/round-robin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/sphinx_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.861219 oncall-1.5.5/src/oncall/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/css/incalendar.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/css/loginsplash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    43949 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/css/oncall.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.869219 oncall-1.5.5/src/oncall/ui/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   476120 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/fonts/Source-Sans-Pro.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.873219 oncall-1.5.5/src/oncall/ui/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/chevron-bottom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/headshot-blank.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/inbug.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/oncall_logo_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/images/oncall_logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.873219 oncall-1.5.5/src/oncall/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64520 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/handlebars-4.0.12.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82802 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/incalendar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    79882 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/loginsplash.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/moment-timezone.js
+-rw-r--r--   0 runner    (1001) docker     (123)   178745 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/moment-tz-data-full.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/moment-tz-data.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/moment.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/navigo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136032 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/oncall.js
+-rw-r--r--   0 runner    (1001) docker     (123)    96224 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/static/js/typeahead.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.873219 oncall-1.5.5/src/oncall/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    22629 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    87643 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/ui/templates/loginsplash.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.873219 oncall-1.5.5/src/oncall/user_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/user_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/user_sync/ldap_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/user_sync/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-03 19:40:06.000000 oncall-1.5.5/src/oncall/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.865219 oncall-1.5.5/src/oncall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:40:17.000000 oncall-1.5.5/src/oncall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:40:17.873219 oncall-1.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-03 19:40:06.000000 oncall-1.5.5/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-03 19:40:06.000000 oncall-1.5.5/test/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-03 19:40:06.000000 oncall-1.5.5/test/test_scheduler.py
```

### Comparing `oncall-1.5.4/LICENSE` & `oncall-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/NOTICE` & `oncall-1.5.5/NOTICE`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/PKG-INFO` & `oncall-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oncall
-Version: 1.5.4
+Version: 1.5.5
 Summary: Oncall is a calendar tool designed for scheduling and managing on-call shifts
 Home-page: https://github.com/linkedin/oncall
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `oncall-1.5.4/README.md` & `oncall-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/setup.py` & `oncall-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/__init__.py` & `oncall-1.5.5/src/oncall/api/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/audit.py` & `oncall-1.5.5/src/oncall/api/v0/audit.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/bonus_events.py` & `oncall-1.5.5/src/oncall/api/v0/bonus_events.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/event.py` & `oncall-1.5.5/src/oncall/api/v0/event.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/event_link.py` & `oncall-1.5.5/src/oncall/api/v0/event_link.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/event_override.py` & `oncall-1.5.5/src/oncall/api/v0/event_override.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/event_swap.py` & `oncall-1.5.5/src/oncall/api/v0/event_swap.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/events.py` & `oncall-1.5.5/src/oncall/api/v0/events.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/events_link.py` & `oncall-1.5.5/src/oncall/api/v0/events_link.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical.py` & `oncall-1.5.5/src/oncall/api/v0/ical.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical_key.py` & `oncall-1.5.5/src/oncall/api/v0/ical_key.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical_key_detail.py` & `oncall-1.5.5/src/oncall/api/v0/ical_key_detail.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical_key_requester.py` & `oncall-1.5.5/src/oncall/api/v0/ical_key_requester.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical_key_team.py` & `oncall-1.5.5/src/oncall/api/v0/ical_key_team.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/ical_key_user.py` & `oncall-1.5.5/src/oncall/api/v0/ical_key_user.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/modes.py` & `oncall-1.5.5/src/oncall/api/v0/modes.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/notification_types.py` & `oncall-1.5.5/src/oncall/api/v0/notification_types.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/notifications.py` & `oncall-1.5.5/src/oncall/api/v0/notifications.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/populate.py` & `oncall-1.5.5/src/oncall/api/v0/populate.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/preview.py` & `oncall-1.5.5/src/oncall/api/v0/preview.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/public_ical.py` & `oncall-1.5.5/src/oncall/api/v0/public_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/role.py` & `oncall-1.5.5/src/oncall/api/v0/role.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/roles.py` & `oncall-1.5.5/src/oncall/api/v0/roles.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/roster.py` & `oncall-1.5.5/src/oncall/api/v0/roster.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/roster_suggest.py` & `oncall-1.5.5/src/oncall/api/v0/roster_suggest.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/roster_user.py` & `oncall-1.5.5/src/oncall/api/v0/roster_user.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/roster_users.py` & `oncall-1.5.5/src/oncall/api/v0/roster_users.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/rosters.py` & `oncall-1.5.5/src/oncall/api/v0/rosters.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/schedule.py` & `oncall-1.5.5/src/oncall/api/v0/schedule.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/schedules.py` & `oncall-1.5.5/src/oncall/api/v0/schedules.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/search.py` & `oncall-1.5.5/src/oncall/api/v0/search.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/service.py` & `oncall-1.5.5/src/oncall/api/v0/service.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/service_oncall.py` & `oncall-1.5.5/src/oncall/api/v0/service_oncall.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/service_teams.py` & `oncall-1.5.5/src/oncall/api/v0/service_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/services.py` & `oncall-1.5.5/src/oncall/api/v0/services.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team.py` & `oncall-1.5.5/src/oncall/api/v0/team.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_admin.py` & `oncall-1.5.5/src/oncall/api/v0/team_admin.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_admins.py` & `oncall-1.5.5/src/oncall/api/v0/team_admins.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_changes.py` & `oncall-1.5.5/src/oncall/api/v0/team_changes.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_ical.py` & `oncall-1.5.5/src/oncall/api/v0/team_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_iris_escalate.py` & `oncall-1.5.5/src/oncall/api/v0/team_iris_escalate.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_oncall.py` & `oncall-1.5.5/src/oncall/api/v0/team_oncall.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_service.py` & `oncall-1.5.5/src/oncall/api/v0/team_service.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_services.py` & `oncall-1.5.5/src/oncall/api/v0/team_services.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_subscription.py` & `oncall-1.5.5/src/oncall/api/v0/team_subscription.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_subscriptions.py` & `oncall-1.5.5/src/oncall/api/v0/team_subscriptions.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_summary.py` & `oncall-1.5.5/src/oncall/api/v0/team_summary.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_user.py` & `oncall-1.5.5/src/oncall/api/v0/team_user.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/team_users.py` & `oncall-1.5.5/src/oncall/api/v0/team_users.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/teams.py` & `oncall-1.5.5/src/oncall/api/v0/teams.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,30 +125,28 @@
 
         {
             "name": "team-foo",
             "scheduling_timezone": "US/Pacific",
             "email": "team-foo@example.com",
             "slack_channel": "#team-foo",
             "slack_channel_notifications": "#team-foo-alerts",
+            "admin": "user_foo"
         }
 
     **Example response:**
 
     .. sourcecode:: http
 
         HTTP/1.1 201 Created
         Content-Type: application/json
 
     :statuscode 201: Successful create
     :statuscode 400: Error in creating team. Possible errors: API key auth not allowed, invalid attributes, missing required attributes
     :statuscode 422: Duplicate team name
     '''
-    if 'user' not in req.context:
-        # ban API auth because we don't know who to set as team admin
-        raise HTTPBadRequest('invalid login', 'API key auth is not allowed for team creation')
 
     data = load_json_body(req)
     if not data.get('name'):
         raise HTTPBadRequest('', 'name attribute missing from request')
     if not data.get('scheduling_timezone'):
         raise HTTPBadRequest('', 'scheduling_timezone attribute missing from request')
     team_name = unquote(data['name']).strip()
@@ -177,14 +175,24 @@
     if iris_plan is not None and iris.client is not None:
         plan_resp = iris.client.get(iris.client.url + 'plans?name=%s&active=1' % iris_plan)
         if plan_resp.status_code != 200 or plan_resp.json() == []:
             raise HTTPBadRequest('invalid iris escalation plan', 'no iris plan named %s exists' % iris_plan)
 
     connection = db.connect()
     cursor = connection.cursor()
+    # if team creation request is coming from api use the username from the admin field in lieu of the user context var
+    if 'user' not in req.context:
+        if not data.get('admin'):
+            raise HTTPBadRequest('invalid admin', 'API requests must specify a team admin username in the admin field')
+        user = data.get('admin')
+        cursor.execute('''SELECT `id` FROM `user` WHERE `name` = %s LIMIT 1''', (user, ))
+        if cursor.rowcount == 0:
+            raise HTTPBadRequest('invalid admin', 'admin username %s was not found in db' % user)
+        req.context['user'] = user
+
     try:
         cursor.execute('''INSERT INTO `team` (`name`, `slack_channel`, `slack_channel_notifications`, `email`, `scheduling_timezone`,
                                               `iris_plan`, `iris_enabled`, `override_phone_number`)
                           VALUES (%s, %s, %s, %s, %s, %s, %s, %s)''',
                        (team_name, slack, slack_notifications, email, scheduling_timezone, iris_plan, iris_enabled, override_number))
 
         team_id = cursor.lastrowid
```

### Comparing `oncall-1.5.4/src/oncall/api/v0/upcoming_shifts.py` & `oncall-1.5.5/src/oncall/api/v0/upcoming_shifts.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user.py` & `oncall-1.5.5/src/oncall/api/v0/user.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_ical.py` & `oncall-1.5.5/src/oncall/api/v0/user_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_notification.py` & `oncall-1.5.5/src/oncall/api/v0/user_notification.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_notifications.py` & `oncall-1.5.5/src/oncall/api/v0/user_notifications.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_pinned_team.py` & `oncall-1.5.5/src/oncall/api/v0/user_pinned_team.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_pinned_teams.py` & `oncall-1.5.5/src/oncall/api/v0/user_pinned_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/user_teams.py` & `oncall-1.5.5/src/oncall/api/v0/user_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/api/v0/users.py` & `oncall-1.5.5/src/oncall/api/v0/users.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/app.py` & `oncall-1.5.5/src/oncall/app.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/auth/__init__.py` & `oncall-1.5.5/src/oncall/auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,20 +150,27 @@
         cursor = connection.cursor()
         cursor.execute('SELECT `key` FROM `application` WHERE `name` = %s', app_name)
         if cursor.rowcount > 0:
             api_key = cursor.fetchone()[0].encode('utf-8')
             cursor.close()
             connection.close()
             window = int(time.time()) // 5
+            long_window = int(time.time()) // 30
             if is_client_digest_valid(client_digest, api_key, window, method, path, body):
                 req.context['app'] = app_name
                 return
             elif is_client_digest_valid(client_digest, api_key, window - 1, method, path, body):
                 req.context['app'] = app_name
                 return
+            elif is_client_digest_valid(client_digest, api_key, long_window, method, path, body):
+                req.context['app'] = app_name
+                return
+            elif is_client_digest_valid(client_digest, api_key, long_window - 1, method, path, body):
+                req.context['app'] = app_name
+                return
             else:
                 raise HTTPUnauthorized('Authentication failure', 'Wrong digest', '')
         else:
             cursor.close()
             connection.close()
             raise HTTPUnauthorized('Authentication failure', 'Application not found', '')
```

### Comparing `oncall-1.5.4/src/oncall/auth/login.py` & `oncall-1.5.5/src/oncall/auth/login.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/auth/modules/ldap_example.py` & `oncall-1.5.5/src/oncall/auth/modules/ldap_example.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/auth/modules/ldap_import.py` & `oncall-1.5.5/src/oncall/auth/modules/ldap_import.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/bin/notifier.py` & `oncall-1.5.5/src/oncall/bin/notifier.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/bin/run_server.py` & `oncall-1.5.5/src/oncall/bin/run_server.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/bin/scheduler.py` & `oncall-1.5.5/src/oncall/bin/scheduler.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/bin/user_sync.py` & `oncall-1.5.5/src/oncall/bin/user_sync.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/constants.py` & `oncall-1.5.5/src/oncall/constants.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/db.py` & `oncall-1.5.5/src/oncall/db.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/doc_helper.py` & `oncall-1.5.5/src/oncall/doc_helper.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/healthcheck.py` & `oncall-1.5.5/src/oncall/healthcheck.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/messengers/__init__.py` & `oncall-1.5.5/src/oncall/messengers/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/messengers/iris_messenger.py` & `oncall-1.5.5/src/oncall/messengers/iris_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/messengers/rocketchat_messenger.py` & `oncall-1.5.5/src/oncall/messengers/rocketchat_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/messengers/teams_messenger.py` & `oncall-1.5.5/src/oncall/messengers/teams_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/metrics/__init__.py` & `oncall-1.5.5/src/oncall/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/metrics/dummy.py` & `oncall-1.5.5/src/oncall/metrics/dummy.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/metrics/influx.py` & `oncall-1.5.5/src/oncall/metrics/influx.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/metrics/prometheus.py` & `oncall-1.5.5/src/oncall/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/notifier/reminder.py` & `oncall-1.5.5/src/oncall/notifier/reminder.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/notifier/user_validator.py` & `oncall-1.5.5/src/oncall/notifier/user_validator.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/scheduler/default.py` & `oncall-1.5.5/src/oncall/scheduler/default.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/scheduler/round-robin.py` & `oncall-1.5.5/src/oncall/scheduler/round-robin.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/sphinx_extension.py` & `oncall-1.5.5/src/oncall/sphinx_extension.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/__init__.py` & `oncall-1.5.5/src/oncall/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/css/bootstrap.min.css` & `oncall-1.5.5/src/oncall/ui/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/css/incalendar.css` & `oncall-1.5.5/src/oncall/ui/static/css/incalendar.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/css/jquery.dataTables.min.css` & `oncall-1.5.5/src/oncall/ui/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/css/loginsplash.css` & `oncall-1.5.5/src/oncall/ui/static/css/loginsplash.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/css/oncall.css` & `oncall-1.5.5/src/oncall/ui/static/css/oncall.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/fonts/Source-Sans-Pro.css` & `oncall-1.5.5/src/oncall/ui/static/fonts/Source-Sans-Pro.css`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/images/favicon.png` & `oncall-1.5.5/src/oncall/ui/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/images/headshot-blank.jpg` & `oncall-1.5.5/src/oncall/ui/static/images/headshot-blank.jpg`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/images/oncall_logo_blue.png` & `oncall-1.5.5/src/oncall/ui/static/images/oncall_logo_blue.png`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/images/oncall_logo_white.png` & `oncall-1.5.5/src/oncall/ui/static/images/oncall_logo_white.png`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/bootstrap.min.js` & `oncall-1.5.5/src/oncall/ui/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/handlebars-4.0.12.min.js` & `oncall-1.5.5/src/oncall/ui/static/js/handlebars-4.0.12.min.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/incalendar.js` & `oncall-1.5.5/src/oncall/ui/static/js/incalendar.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/jquery-3.3.1.min.js` & `oncall-1.5.5/src/oncall/ui/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/jquery.dataTables.min.js` & `oncall-1.5.5/src/oncall/ui/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/loginsplash.js` & `oncall-1.5.5/src/oncall/ui/static/js/loginsplash.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/moment-timezone.js` & `oncall-1.5.5/src/oncall/ui/static/js/moment-timezone.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/moment-tz-data-full.js` & `oncall-1.5.5/src/oncall/ui/static/js/moment-tz-data-full.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/moment-tz-data.js` & `oncall-1.5.5/src/oncall/ui/static/js/moment-tz-data.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/moment.js` & `oncall-1.5.5/src/oncall/ui/static/js/moment.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/navigo.js` & `oncall-1.5.5/src/oncall/ui/static/js/navigo.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/oncall.js` & `oncall-1.5.5/src/oncall/ui/static/js/oncall.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/static/js/typeahead.js` & `oncall-1.5.5/src/oncall/ui/static/js/typeahead.js`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/templates/base.html` & `oncall-1.5.5/src/oncall/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/templates/index.html` & `oncall-1.5.5/src/oncall/ui/templates/index.html`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/ui/templates/loginsplash.html` & `oncall-1.5.5/src/oncall/ui/templates/loginsplash.html`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/user_sync/ldap_sync.py` & `oncall-1.5.5/src/oncall/user_sync/ldap_sync.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/user_sync/slack.py` & `oncall-1.5.5/src/oncall/user_sync/slack.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall/utils.py` & `oncall-1.5.5/src/oncall/utils.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/src/oncall.egg-info/PKG-INFO` & `oncall-1.5.5/src/oncall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oncall
-Version: 1.5.4
+Version: 1.5.5
 Summary: Oncall is a calendar tool designed for scheduling and managing on-call shifts
 Home-page: https://github.com/linkedin/oncall
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `oncall-1.5.4/src/oncall.egg-info/SOURCES.txt` & `oncall-1.5.5/src/oncall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/test/test_auth.py` & `oncall-1.5.5/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/test/test_notifier.py` & `oncall-1.5.5/test/test_notifier.py`

 * *Files identical despite different names*

### Comparing `oncall-1.5.4/test/test_scheduler.py` & `oncall-1.5.5/test/test_scheduler.py`

 * *Files identical despite different names*

