# Comparing `tmp/wagtail_heroicons-0.1.2.tar.gz` & `tmp/wagtail_heroicons-0.1.3.tar.gz`

## Comparing `wagtail_heroicons-0.1.2.tar` & `wagtail_heroicons-0.1.3.tar`

### file list

```diff
@@ -1,479 +1,479 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/.flake8
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/apps.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/icons.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/py.typed
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/wagtail_hooks.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/academic-cap.svg
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/adjustments.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/annotation.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/archive.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-circle-down.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-circle-left.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-circle-right.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-circle-up.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-down.svg
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-left.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-down.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-left.svg
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-right.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-up.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-right.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-sm-down.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-sm-left.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-sm-right.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-sm-up.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrow-up.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/arrows-expand.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/at-symbol.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/backspace.svg
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/badge-check.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/ban.svg
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/beaker.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/bell.svg
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/book-open.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/bookmark-alt.svg
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/bookmark.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/briefcase.svg
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cake.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/calculator.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/calendar.svg
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/camera.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cash.svg
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chart-bar.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chart-pie.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chart-square-bar.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chat-alt-2.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chat-alt.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chat.svg
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/check-circle.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/check.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-double-down.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-double-left.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-double-right.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-double-up.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-down.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-left.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-right.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chevron-up.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chip.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/clipboard-check.svg
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/clipboard-copy.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/clipboard-list.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/clipboard.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/clock.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cloud-download.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cloud-upload.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cloud.svg
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/code.svg
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cog.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/collection.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/color-swatch.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/credit-card.svg
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cube-transparent.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cube.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-bangladeshi.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-dollar.svg
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-euro.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-pound.svg
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-rupee.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-yen.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cursor-click.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/database.svg
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/desktop-computer.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/device-mobile.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/device-tablet.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-add.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-download.svg
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-duplicate.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-remove.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-report.svg
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-search.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-text.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/dots-circle-horizontal.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/dots-horizontal.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/dots-vertical.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/download.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/duplicate.svg
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/emoji-happy.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/emoji-sad.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/exclamation-circle.svg
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/exclamation.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/external-link.svg
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/eye-off.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/eye.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/fast-forward.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/film.svg
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/filter.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/finger-print.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/fire.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/flag.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/folder-add.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/folder-download.svg
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/folder-open.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/folder-remove.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/folder.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/gift.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/globe-alt.svg
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/globe.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/hand.svg
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/hashtag.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/heart.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/home.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/identification.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/inbox-in.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/inbox.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/information-circle.svg
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/key.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/library.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/light-bulb.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/lightning-bolt.svg
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/link.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/location-marker.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/lock-closed.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/lock-open.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/login.svg
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/logout.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/mail-open.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/mail.svg
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/map.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/menu-alt-1.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/menu-alt-2.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/menu-alt-3.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/menu-alt-4.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/menu.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/microphone.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/minus-circle.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/minus-sm.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/minus.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/moon.svg
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/music-note.svg
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/newspaper.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/office-building.svg
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/paper-airplane.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/paper-clip.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/pause.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/pencil-alt.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/pencil.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-incoming.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-missed-call.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-outgoing.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone.svg
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/photograph.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/play.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/plus-circle.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/plus-sm.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/plus.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/presentation-chart-bar.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/presentation-chart-line.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/printer.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/puzzle.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/qrcode.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/question-mark-circle.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/receipt-refund.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/receipt-tax.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/refresh.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/reply.svg
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/rewind.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/rss.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/save-as.svg
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/save.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/scale.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/scissors.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/search-circle.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/search.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/selector.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/server.svg
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/share.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shield-check.svg
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shield-exclamation.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shopping-bag.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shopping-cart.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/sort-ascending.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/sort-descending.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/sparkles.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/speakerphone.svg
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/star.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/status-offline.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/status-online.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/stop.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/sun.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/support.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/switch-horizontal.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/switch-vertical.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/table.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/tag.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/template.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/terminal.svg
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/thumb-down.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/thumb-up.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/ticket.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/translate.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/trash.svg
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/trending-down.svg
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/trending-up.svg
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/truck.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/upload.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user-add.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user-circle.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user-group.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user-remove.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/users.svg
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/variable.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/video-camera.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-boards.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-grid-add.svg
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-grid.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-list.svg
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/volume-off.svg
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/volume-up.svg
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/wifi.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/x-circle.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/x.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/zoom-in.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/zoom-out.svg
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/academic-cap.svg
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/adjustments.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/annotation.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/archive.svg
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-circle-down.svg
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-circle-left.svg
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-circle-right.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-circle-up.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-down.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-left.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-down.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-left.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-right.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-up.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-right.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-sm-down.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-sm-left.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-sm-right.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-sm-up.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrow-up.svg
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrows-expand.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/at-symbol.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/backspace.svg
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/badge-check.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/ban.svg
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/beaker.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/bell.svg
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/book-open.svg
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/bookmark-alt.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/bookmark.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/briefcase.svg
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cake.svg
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/calculator.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/calendar.svg
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/camera.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cash.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chart-bar.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chart-pie.svg
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chart-square-bar.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chat-alt-2.svg
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chat-alt.svg
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chat.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/check-circle.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/check.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-down.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-left.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-right.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-up.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-down.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-left.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-right.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-up.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chip.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-check.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-copy.svg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-list.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clock.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cloud-download.svg
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cloud-upload.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cloud.svg
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/code.svg
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cog.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/collection.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/color-swatch.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/credit-card.svg
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cube-transparent.svg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cube.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-bangladeshi.svg
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-dollar.svg
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-euro.svg
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-pound.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-rupee.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-yen.svg
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cursor-click.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/database.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/desktop-computer.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/device-mobile.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/device-tablet.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-add.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-download.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-duplicate.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-remove.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-report.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-search.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-text.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/dots-circle-horizontal.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/dots-horizontal.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/dots-vertical.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/download.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/duplicate.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/emoji-happy.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/emoji-sad.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/exclamation-circle.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/exclamation.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/external-link.svg
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/eye-off.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/eye.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/fast-forward.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/film.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/filter.svg
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/finger-print.svg
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/fire.svg
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/flag.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/folder-add.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/folder-download.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/folder-open.svg
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/folder-remove.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/folder.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/gift.svg
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/globe-alt.svg
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/globe.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/hand.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/hashtag.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/heart.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/home.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/identification.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/inbox-in.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/inbox.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/information-circle.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/key.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/library.svg
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/light-bulb.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/lightning-bolt.svg
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/link.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/location-marker.svg
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/lock-closed.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/lock-open.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/login.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/logout.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/mail-open.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/mail.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/map.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/menu-alt-1.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/menu-alt-2.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/menu-alt-3.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/menu-alt-4.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/menu.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/microphone.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/minus-circle.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/minus-sm.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/minus.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/moon.svg
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/music-note.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/newspaper.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/office-building.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/paper-airplane.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/paper-clip.svg
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/pause.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/pencil-alt.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/pencil.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-incoming.svg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-missed-call.svg
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-outgoing.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/photograph.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/play.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/plus-circle.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/plus-sm.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/plus.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/presentation-chart-bar.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/presentation-chart-line.svg
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/printer.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/puzzle.svg
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/qrcode.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/question-mark-circle.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/receipt-refund.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/receipt-tax.svg
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/refresh.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/reply.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/rewind.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/rss.svg
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/save-as.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/save.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/scale.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/scissors.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/search-circle.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/search.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/selector.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/server.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/share.svg
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shield-check.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shield-exclamation.svg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shopping-bag.svg
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shopping-cart.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sort-ascending.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sort-descending.svg
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sparkles.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/speakerphone.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/star.svg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/status-offline.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/status-online.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/stop.svg
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sun.svg
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/support.svg
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/switch-horizontal.svg
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/switch-vertical.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/table.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/tag.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/template.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/terminal.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/thumb-down.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/thumb-up.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/ticket.svg
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/translate.svg
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/trash.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/trending-down.svg
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/trending-up.svg
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/truck.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/upload.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/user-add.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/user-circle.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/user-group.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/user-remove.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/user.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/users.svg
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/variable.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/video-camera.svg
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-boards.svg
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-grid-add.svg
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-grid.svg
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-list.svg
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/volume-off.svg
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/volume-up.svg
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/wifi.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/x-circle.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/x.svg
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/zoom-in.svg
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/zoom-out.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/tests/parser.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/tests/test_build.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/tests/test_icons.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/.gitignore
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/LICENSE
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/README.md
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/.flake8
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/apps.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/icons.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/py.typed
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/wagtail_hooks.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/academic-cap.svg
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/adjustments.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/annotation.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/archive.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-circle-down.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-circle-left.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-circle-right.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-circle-up.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-down.svg
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-left.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-down.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-left.svg
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-right.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-narrow-up.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-right.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-sm-down.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-sm-left.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-sm-right.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-sm-up.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrow-up.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/arrows-expand.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/at-symbol.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/backspace.svg
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/badge-check.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/ban.svg
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/beaker.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/bell.svg
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/book-open.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/bookmark-alt.svg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/bookmark.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/briefcase.svg
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cake.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/calculator.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/calendar.svg
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/camera.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cash.svg
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chart-bar.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chart-pie.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chart-square-bar.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chat-alt-2.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chat-alt.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chat.svg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/check-circle.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/check.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-double-down.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-double-left.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-double-right.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-double-up.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-down.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-left.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-right.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chevron-up.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chip.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/clipboard-check.svg
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/clipboard-copy.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/clipboard-list.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/clipboard.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/clock.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cloud-download.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cloud-upload.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cloud.svg
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/code.svg
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cog.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/collection.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/color-swatch.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/credit-card.svg
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cube-transparent.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cube.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-bangladeshi.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-dollar.svg
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-euro.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-pound.svg
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-rupee.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-yen.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cursor-click.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/database.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/desktop-computer.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/device-mobile.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/device-tablet.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-add.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-download.svg
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-duplicate.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-remove.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-report.svg
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-search.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-text.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/dots-circle-horizontal.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/dots-horizontal.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/dots-vertical.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/download.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/duplicate.svg
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/emoji-happy.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/emoji-sad.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/exclamation-circle.svg
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/exclamation.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/external-link.svg
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/eye-off.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/eye.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/fast-forward.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/film.svg
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/filter.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/finger-print.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/fire.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/flag.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/folder-add.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/folder-download.svg
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/folder-open.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/folder-remove.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/folder.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/gift.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/globe-alt.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/globe.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/hand.svg
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/hashtag.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/heart.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/home.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/identification.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/inbox-in.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/inbox.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/information-circle.svg
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/key.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/library.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/light-bulb.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/lightning-bolt.svg
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/link.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/location-marker.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/lock-closed.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/lock-open.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/login.svg
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/logout.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/mail-open.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/mail.svg
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/map.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/menu-alt-1.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/menu-alt-2.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/menu-alt-3.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/menu-alt-4.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/menu.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/microphone.svg
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/minus-circle.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/minus-sm.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/minus.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/moon.svg
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/music-note.svg
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/newspaper.svg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/office-building.svg
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/paper-airplane.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/paper-clip.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/pause.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/pencil-alt.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/pencil.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-incoming.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-missed-call.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-outgoing.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone.svg
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/photograph.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/play.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/plus-circle.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/plus-sm.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/plus.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/presentation-chart-bar.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/presentation-chart-line.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/printer.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/puzzle.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/qrcode.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/question-mark-circle.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/receipt-refund.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/receipt-tax.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/refresh.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/reply.svg
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/rewind.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/rss.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/save-as.svg
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/save.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/scale.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/scissors.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/search-circle.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/search.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/selector.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/server.svg
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/share.svg
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shield-check.svg
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shield-exclamation.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shopping-bag.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shopping-cart.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/sort-ascending.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/sort-descending.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/sparkles.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/speakerphone.svg
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/star.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/status-offline.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/status-online.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/stop.svg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/sun.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/support.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/switch-horizontal.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/switch-vertical.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/table.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/tag.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/template.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/terminal.svg
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/thumb-down.svg
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/thumb-up.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/ticket.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/translate.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/trash.svg
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/trending-down.svg
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/trending-up.svg
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/truck.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/upload.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user-add.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user-circle.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user-group.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user-remove.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/users.svg
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/variable.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/video-camera.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-boards.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-grid-add.svg
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-grid.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-list.svg
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/volume-off.svg
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/volume-up.svg
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/wifi.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/x-circle.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/x.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/zoom-in.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/zoom-out.svg
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/academic-cap.svg
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/adjustments.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/annotation.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/archive.svg
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-circle-down.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-circle-left.svg
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-circle-right.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-circle-up.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-down.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-left.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-down.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-left.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-right.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-narrow-up.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-right.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-sm-down.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-sm-left.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-sm-right.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-sm-up.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrow-up.svg
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrows-expand.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/at-symbol.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/backspace.svg
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/badge-check.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/ban.svg
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/beaker.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/bell.svg
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/book-open.svg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/bookmark-alt.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/bookmark.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/briefcase.svg
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cake.svg
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/calculator.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/calendar.svg
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/camera.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cash.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chart-bar.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chart-pie.svg
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chart-square-bar.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chat-alt-2.svg
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chat-alt.svg
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chat.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/check-circle.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/check.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-down.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-left.svg
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-right.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-up.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-down.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-left.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-right.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-up.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chip.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-check.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-copy.svg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-list.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clock.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cloud-download.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cloud-upload.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cloud.svg
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/code.svg
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cog.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/collection.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/color-swatch.svg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/credit-card.svg
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cube-transparent.svg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cube.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-bangladeshi.svg
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-dollar.svg
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-euro.svg
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-pound.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-rupee.svg
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-yen.svg
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cursor-click.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/database.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/desktop-computer.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/device-mobile.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/device-tablet.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-add.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-download.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-duplicate.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-remove.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-report.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-search.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-text.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/dots-circle-horizontal.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/dots-horizontal.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/dots-vertical.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/download.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/duplicate.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/emoji-happy.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/emoji-sad.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/exclamation-circle.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/exclamation.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/external-link.svg
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/eye-off.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/eye.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/fast-forward.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/film.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/filter.svg
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/finger-print.svg
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/fire.svg
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/flag.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/folder-add.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/folder-download.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/folder-open.svg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/folder-remove.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/folder.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/gift.svg
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/globe-alt.svg
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/globe.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/hand.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/hashtag.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/heart.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/home.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/identification.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/inbox-in.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/inbox.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/information-circle.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/key.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/library.svg
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/light-bulb.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/lightning-bolt.svg
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/link.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/location-marker.svg
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/lock-closed.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/lock-open.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/login.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/logout.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/mail-open.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/mail.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/map.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/menu-alt-1.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/menu-alt-2.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/menu-alt-3.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/menu-alt-4.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/menu.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/microphone.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/minus-circle.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/minus-sm.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/minus.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/moon.svg
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/music-note.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/newspaper.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/office-building.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/paper-airplane.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/paper-clip.svg
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/pause.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/pencil-alt.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/pencil.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-incoming.svg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-missed-call.svg
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-outgoing.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/photograph.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/play.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/plus-circle.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/plus-sm.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/plus.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/presentation-chart-bar.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/presentation-chart-line.svg
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/printer.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/puzzle.svg
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/qrcode.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/question-mark-circle.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/receipt-refund.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/receipt-tax.svg
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/refresh.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/reply.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/rewind.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/rss.svg
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/save-as.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/save.svg
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/scale.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/scissors.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/search-circle.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/search.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/selector.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/server.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/share.svg
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shield-check.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shield-exclamation.svg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shopping-bag.svg
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shopping-cart.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sort-ascending.svg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sort-descending.svg
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sparkles.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/speakerphone.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/star.svg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/status-offline.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/status-online.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/stop.svg
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sun.svg
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/support.svg
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/switch-horizontal.svg
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/switch-vertical.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/table.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/tag.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/template.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/terminal.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/thumb-down.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/thumb-up.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/ticket.svg
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/translate.svg
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/trash.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/trending-down.svg
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/trending-up.svg
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/truck.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/upload.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/user-add.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/user-circle.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/user-group.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/user-remove.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/user.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/users.svg
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/variable.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/video-camera.svg
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-boards.svg
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-grid-add.svg
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-grid.svg
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-list.svg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/volume-off.svg
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/volume-up.svg
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/wifi.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/x-circle.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/x.svg
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/zoom-in.svg
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/zoom-out.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/tests/parser.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/tests/test_build.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/tests/test_icons.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/README.md
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 wagtail_heroicons-0.1.3/PKG-INFO
```

### Comparing `wagtail_heroicons-0.1.2/CHANGELOG.md` & `wagtail_heroicons-0.1.3/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.3] - 2023-05-03
+
+### Fixed
+
+- Fixed a TypeError when attempting to use the package; the `Heroicon` dataclass was adding
+  a `Path` object to the list of icons in the  `register_icons` Wagtail hook instead of a 
+  string. Reported by @ReijerTheCoder in #40 and fixed in #41.
+
 ## [0.1.2] - 2023-04-21
 
 ### Changed
 
 - Add the MIT license and Refactoring UI Inc. copyright information to all SVG files.
 
 ## [0.1.1] - 2023-04-21
@@ -33,11 +41,12 @@
 
 - Build script:
   - Download Heroicons from NPM and copy to `templates` folder
   - Edit SVG files to add correct `id` attribute
   - Edit and build the icon registry in `icons.py`
 - Initial documentation
 
-[unreleased]: https://github.com/joshuadavidthomas/wagtail-heroicons/compare/v0.1.2...HEAD
+[unreleased]: https://github.com/joshuadavidthomas/wagtail-heroicons/compare/v0.1.3...HEAD
+[0.1.3]: https://github.com/joshuadavidthomas/wagtail-heroicons/releases/tag/v0.1.3
 [0.1.2]: https://github.com/joshuadavidthomas/wagtail-heroicons/releases/tag/v0.1.2
 [0.1.1]: https://github.com/joshuadavidthomas/wagtail-heroicons/releases/tag/v0.1.1
 [0.1.0]: https://github.com/joshuadavidthomas/wagtail-heroicons/releases/tag/v0.1.0
```

### Comparing `wagtail_heroicons-0.1.2/.github/workflows/release.yml` & `wagtail_heroicons-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/.github/workflows/test.yml` & `wagtail_heroicons-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/icons.py` & `wagtail_heroicons-0.1.3/wagtail_heroicons/icons.py`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/academic-cap.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/academic-cap.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/badge-check.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/badge-check.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/beaker.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/beaker.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/bell.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/bell.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/book-open.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/book-open.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/briefcase.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/briefcase.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cake.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cake.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/camera.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/camera.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/chart-bar.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/chart-bar.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/cog.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/cog.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/color-swatch.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/color-swatch.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/currency-dollar.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/currency-dollar.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/document-duplicate.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/document-duplicate.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/eye-off.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/eye-off.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/eye.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/eye.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/finger-print.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/finger-print.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/fire.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/fire.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/globe.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/globe.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/identification.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/identification.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/inbox-in.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/inbox-in.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/inbox.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/inbox.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/light-bulb.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/light-bulb.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/location-marker.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/location-marker.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/mail-open.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/mail-open.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-incoming.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-missed-call.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-missed-call.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone-outgoing.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/phone.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/phone.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/play.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/play.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/printer.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/printer.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/puzzle.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/puzzle.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/qrcode.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/qrcode.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/share.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/share.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shield-check.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shield-check.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/shield-exclamation.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/shield-exclamation.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/speakerphone.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/speakerphone.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/star.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/star.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/status-offline.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/status-offline.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/template.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/template.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/thumb-down.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/thumb-down.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/thumb-up.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/thumb-up.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/truck.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/truck.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/user-group.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/user-group.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/variable.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/variable.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-boards.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-boards.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-grid-add.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-grid-add.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/view-grid.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/view-grid.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/volume-off.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/volume-off.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/outline/volume-up.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/outline/volume-up.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/academic-cap.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/academic-cap.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/adjustments.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/adjustments.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/arrows-expand.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/arrows-expand.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/backspace.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/backspace.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/badge-check.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/badge-check.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/beaker.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/beaker.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/briefcase.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/briefcase.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cake.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cake.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/calculator.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/calculator.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-down.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-down.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-left.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-left.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-right.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-right.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chevron-double-up.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chevron-double-up.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/chip.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/chip.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-check.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-check.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-copy.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-copy.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/clipboard-list.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/clipboard-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cloud-download.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cloud-download.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/code.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/code.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cog.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cog.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cube-transparent.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cube-transparent.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cube.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cube.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-dollar.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-dollar.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-euro.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-euro.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-rupee.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-rupee.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/currency-yen.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/currency-yen.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/cursor-click.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/cursor-click.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/database.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/database.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-download.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-download.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-report.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-report.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/document-search.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/document-search.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/exclamation.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/exclamation.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/eye-off.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/eye-off.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/finger-print.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/finger-print.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/fire.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/fire.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/gift.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/gift.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/globe-alt.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/globe-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/globe.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/globe.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/hashtag.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/identification.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/identification.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/inbox-in.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/inbox-in.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/library.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/library.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/light-bulb.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/light-bulb.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/link.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/link.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/mail-open.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/mail-open.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-incoming.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-missed-call.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-missed-call.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/phone-outgoing.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/presentation-chart-bar.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/presentation-chart-bar.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/presentation-chart-line.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/presentation-chart-line.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/puzzle.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/puzzle.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/qrcode.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/qrcode.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/receipt-refund.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/receipt-refund.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/receipt-tax.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/receipt-tax.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/refresh.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/refresh.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/save-as.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/save-as.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/scale.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/scale.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/scissors.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/scissors.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/selector.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/selector.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shield-check.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shield-check.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shield-exclamation.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shield-exclamation.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/shopping-cart.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/shopping-cart.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sparkles.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sparkles.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/star.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/star.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/status-offline.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/status-offline.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/status-online.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/status-online.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/sun.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/sun.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/support.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/support.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/terminal.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/terminal.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/translate.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/translate.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/truck.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/truck.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/variable.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/variable.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-grid-add.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-grid-add.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/view-grid.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/view-grid.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/volume-off.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/volume-off.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/volume-up.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/volume-up.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/wifi.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/wifi.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/x-circle.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/x-circle.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/zoom-in.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/wagtail_heroicons/templates/heroicons/solid/zoom-out.svg` & `wagtail_heroicons-0.1.3/wagtail_heroicons/templates/heroicons/solid/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/tests/test_build.py` & `wagtail_heroicons-0.1.3/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/.gitignore` & `wagtail_heroicons-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/LICENSE` & `wagtail_heroicons-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/README.md` & `wagtail_heroicons-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/pyproject.toml` & `wagtail_heroicons-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail_heroicons-0.1.2/PKG-INFO` & `wagtail_heroicons-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-heroicons
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add Heroicons to your Wagtail site
 Project-URL: Homepage, https://github.com/joshuadavidthomas/wagtail-heroicons
 Project-URL: Issues, https://github.com/joshuadavidthomas/wagtail-heroicons/issues
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_swfvx0vc_/tmpu_mmdy4p_TarContainer/0/478", line 66, column 91: CDATA terminal not found*

 * *File "/tmp/diffoscope_swfvx0vc_/tmpu_mmdy4p_TarContainer/0/478", line 66, column 91: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-heroicons Version: 0.1.2 Summary: Add
+Metadata-Version: 2.1 Name: wagtail-heroicons Version: 0.1.3 Summary: Add
 Heroicons to your Wagtail site Project-URL: Homepage, https://github.com/
 joshuadavidthomas/wagtail-heroicons Project-URL: Issues, https://github.com/
 joshuadavidthomas/wagtail-heroicons/issues Author-email: Josh Thomas
 joshthomas.dev> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: Wagtail Classifier:
 Framework :: Wagtail :: 2 Classifier: Framework :: Wagtail :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

