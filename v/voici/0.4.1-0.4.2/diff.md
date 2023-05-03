# Comparing `tmp/voici-0.4.1.tar.gz` & `tmp/voici-0.4.2.tar.gz`

## Comparing `voici-0.4.1.tar` & `voici-0.4.2.tar`

### file list

```diff
@@ -1,189 +1,188 @@
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.1/.eslintignore
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.1/.eslintrc.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.1/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.1/.prettierrc
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 voici-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.1/RELEASE.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.1/environment.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.1/lerna.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.1/lint-staged.config.js
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.1/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.1/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.1/setup.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.1/tsconfigbase.json
--rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.1/yarn.lock
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.1/demo/environment.yml
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/iris.csv
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/voici.ipynb
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/widgets/bqplot.ipynb
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/widgets/ipycanvas.ipynb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.1/docs/changelog.md
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.1/docs/conf.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.1/docs/configuration.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.1/docs/contributing.md
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.1/docs/deploy.md
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.1/docs/environment.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.1/docs/index.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.1/docs/install.md
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.1/docs/voila-logo.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.1/scripts/bump-version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/package.json
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
--rw-r--r--   0        0        0   186883 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
--rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
--rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
--rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
--rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.1/voici/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.1/voici/__main__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.1/voici/_version.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.1/voici/addon.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 voici-0.4.1/voici/app.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 voici-0.4.1/voici/exporter.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.1/voici/tree_exporter.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/index.html
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1023.js
--rw-r--r--   0        0        0   599879 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1024.js
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/103.js
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1053.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1058.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1100.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1105.js
--rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1432.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1497.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1553.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1581.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1667.js
--rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1672.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1672.js.LICENSE.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1732.js
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1890.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1980.js
--rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2075.js
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2106.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2230.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2266.js
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2322.js
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2359.js
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2361.js
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2488.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2516.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2630.js
--rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2687.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/275.js
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2784.js
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2784.js.LICENSE.txt
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/286.js
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2950.js
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3008.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3086.js
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3251.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3256.js
--rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/330.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3305.js
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3312.js
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3316.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3316.js.LICENSE.txt
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3349.js
--rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/339.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3504.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3655.js
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3693.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3811.js
--rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3851.js
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3922.js
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4259.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4359.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4382.js
--rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/450.js
--rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4530.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4530.js.LICENSE.txt
--rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4875.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4896.js
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4939.js
--rw-r--r--   0        0        0   901522 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4963.js
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4963.js.LICENSE.txt
--rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4977.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5188.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5291.js
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/53.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5403.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5445.js
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5474.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5826.js
--rw-r--r--   0        0        0   104080 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5950.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5950.js.LICENSE.txt
--rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5952.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5952.js.LICENSE.txt
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/596.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5985.js
--rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6111.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6178.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6196.js
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6219.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6219.js.LICENSE.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6417.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6527.js
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6587.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6614.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6616.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6757.js
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6790.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6839.js
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6852.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6856.js
--rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6914.js
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6976.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7003.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7015.js
--rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7066.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/709.js
--rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/74.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7469.js
--rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7560.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7623.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7695.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7795.js
--rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8085.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8164.js
--rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8291.js
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8291.js.LICENSE.txt
--rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8316.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8316.js.LICENSE.txt
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/846.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/86.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8679.js
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8809.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8874.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9060.js
--rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9112.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9320.js
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9339.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9406.js
--rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9513.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9513.js.LICENSE.txt
--rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9727.js
--rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9757.js
--rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9780.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9807.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9817.js
--rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9900.js
--rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9988.js
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/service-worker-b2fb40a.js
--rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/treepage.js
--rw-r--r--   0        0        0    24220 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/voici.js
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.1/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.1/LICENSE
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 voici-0.4.1/README.md
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 voici-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.2/.eslintignore
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.2/.eslintrc.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.2/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.2/.prettierrc
+-rw-r--r--   0        0        0    14521 2020-02-02 00:00:00.000000 voici-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.2/RELEASE.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.2/environment.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.2/lerna.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.2/lint-staged.config.js
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.2/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.2/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.2/setup.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.2/tsconfigbase.json
+-rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.2/yarn.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.2/demo/environment.yml
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.2/demo/notebooks/iris.csv
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.2/demo/notebooks/voici.ipynb
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.2/demo/notebooks/widgets/bqplot.ipynb
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.2/demo/notebooks/widgets/ipycanvas.ipynb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.2/docs/changelog.md
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.2/docs/conf.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.2/docs/configuration.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.2/docs/contributing.md
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.2/docs/deploy.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.2/docs/environment.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.2/docs/index.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.2/docs/install.md
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.2/docs/voila-logo.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.2/scripts/bump-version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/package.json
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
+-rw-r--r--   0        0        0   219822 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
+-rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
+-rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.2/voici/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.2/voici/__main__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.2/voici/_version.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.2/voici/addon.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 voici-0.4.2/voici/app.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 voici-0.4.2/voici/exporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.2/voici/tree_exporter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/index.html
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1023.js
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/103.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1053.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1058.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1100.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1105.js
+-rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1432.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1497.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1553.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1581.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1667.js
+-rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1672.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1672.js.LICENSE.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1732.js
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1890.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/1980.js
+-rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2075.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2106.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2230.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2266.js
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2322.js
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2359.js
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2361.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2488.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2516.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2630.js
+-rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2687.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/275.js
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2784.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2784.js.LICENSE.txt
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/286.js
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/2950.js
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3008.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3086.js
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3251.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3256.js
+-rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/330.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3305.js
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3312.js
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3316.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3316.js.LICENSE.txt
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3349.js
+-rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/339.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3504.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3655.js
+-rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3693.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3811.js
+-rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3851.js
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/3922.js
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4259.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4359.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4382.js
+-rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/450.js
+-rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4530.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4530.js.LICENSE.txt
+-rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4875.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4896.js
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4939.js
+-rw-r--r--   0        0        0   901522 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4963.js
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4963.js.LICENSE.txt
+-rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/4977.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5188.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5291.js
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/53.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5403.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5445.js
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5474.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5826.js
+-rw-r--r--   0        0        0   104080 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5950.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5950.js.LICENSE.txt
+-rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5952.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5952.js.LICENSE.txt
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/596.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/5985.js
+-rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6111.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6178.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6196.js
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6219.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6219.js.LICENSE.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6417.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6527.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6587.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6614.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6616.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6757.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6790.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6839.js
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6852.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6856.js
+-rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6914.js
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/6976.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7003.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7015.js
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7066.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/709.js
+-rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/74.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7469.js
+-rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7560.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7623.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7695.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/7795.js
+-rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8085.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8164.js
+-rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8291.js
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8291.js.LICENSE.txt
+-rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8316.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8316.js.LICENSE.txt
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/846.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/86.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8679.js
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8809.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/8874.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9060.js
+-rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9112.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9320.js
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9339.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9406.js
+-rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9513.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9513.js.LICENSE.txt
+-rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9727.js
+-rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9757.js
+-rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9780.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9807.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9817.js
+-rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9900.js
+-rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/9988.js
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/service-worker-b2fb40a.js
+-rw-r--r--   0        0        0    23502 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/treepage.js
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 voici-0.4.2/voici/static/build/voici.js
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 voici-0.4.2/README.md
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 voici-0.4.2/PKG-INFO
```

### Comparing `voici-0.4.1/.eslintrc.js` & `voici-0.4.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/CHANGELOG.md` & `voici-0.4.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.2
+
+([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.4.1...3af43dac56a9f9e26d6a2161e0b0cdbd1573949a))
+
+### Bugs fixed
+
+- Fix outputs DOM structure [#74](https://github.com/voila-dashboards/voici/pull/74) ([@martinRenou](https://github.com/martinRenou))
+- Remove custom styling [#71](https://github.com/voila-dashboards/voici/pull/71) ([@martinRenou](https://github.com/martinRenou))
+- Fix version printing [#72](https://github.com/voila-dashboards/voici/pull/72) ([@martinRenou](https://github.com/martinRenou))
+
+### Documentation improvements
+
+- Update WIP comment [#73](https://github.com/voila-dashboards/voici/pull/73) ([@martinRenou](https://github.com/martinRenou))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-21&to=2023-05-03&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-04-21..2023-05-03&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-04-21..2023-05-03&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.4.1
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.4.0...417746aff5b4f3faa7b254e8c516a46e59a67155))
 
 ### Enhancements made
 
 - Add missing `react-dom` module to Webpack shared scope [#67](https://github.com/voila-dashboards/voici/pull/67) ([@trungleduc](https://github.com/trungleduc))
@@ -16,16 +38,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-18&to=2023-04-21&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-04-18..2023-04-21&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-04-18..2023-04-21&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-04-18..2023-04-21&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.4.0
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/v0.3.3...3fb43ef1d143a3e78939e7e35d293cda01d58867))
 
 ### Enhancements made
 
 - Update CLI [#65](https://github.com/voila-dashboards/voici/pull/65) ([@trungleduc](https://github.com/trungleduc))
```

### Comparing `voici-0.4.1/CONTRIBUTING.md` & `voici-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/RELEASE.md` & `voici-0.4.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/lint-staged.config.js` & `voici-0.4.2/lint-staged.config.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/package.json` & `voici-0.4.2/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/tsconfigbase.json` & `voici-0.4.2/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/yarn.lock` & `voici-0.4.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/demo/notebooks/iris.csv` & `voici-0.4.2/demo/notebooks/iris.csv`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/demo/notebooks/voici.ipynb` & `voici-0.4.2/demo/notebooks/voici.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/demo/notebooks/widgets/bqplot.ipynb` & `voici-0.4.2/demo/notebooks/widgets/bqplot.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/demo/notebooks/widgets/ipycanvas.ipynb` & `voici-0.4.2/demo/notebooks/widgets/ipycanvas.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/conf.py` & `voici-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/configuration.md` & `voici-0.4.2/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/deploy.md` & `voici-0.4.2/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/index.md` & `voici-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/install.md` & `voici-0.4.2/docs/install.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/docs/voila-logo.svg` & `voici-0.4.2/docs/voila-logo.svg`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/scripts/bump-version.py` & `voici-0.4.2/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/package.json` & `voici-0.4.2/ui-tests/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/yarn.lock` & `voici-0.4.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts` & `voici-0.4.2/ui-tests/tests/voici.test.ts`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png` & `voici-0.4.2/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/_version.py` & `voici-0.4.2/voici/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `voici-0.4.1/voici/addon.py` & `voici-0.4.2/voici/addon.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/app.py` & `voici-0.4.2/voici/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     LiteServeApp,
     LiteStatusApp,
     ManagedApp,
     lite_aliases,
 )
 from traitlets import default
 
+from ._version import __version__
+
 voici_aliases = dict(
     **lite_aliases,
     show_tracebacks="VoilaConfiguration.show_tracebacks",
     strip_sources="VoilaConfiguration.strip_sources",
     template="VoilaConfiguration.template",
     theme="VoilaConfiguration.theme",
 )
@@ -87,14 +89,16 @@
 
     pass
 
 
 class VoiciApp(LiteApp):
     """build ready-to-serve (or -publish) Voici sites"""
 
+    version = __version__
+
     __sub_apps = dict(
         # special apps
         list=VoiciListApp,
         # task apps
         status=VoiciStatusApp,
         init=VoiciInitApp,
         build=VoiciBuildApp,
```

### Comparing `voici-0.4.1/voici/exporter.py` & `voici-0.4.2/voici/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "include_output_prompt": not self.exclude_output_prompt,
             "no_prompt": self.exclude_input_prompt and self.exclude_output_prompt,
         }
 
         def notebook_execute(nb, kernel_id):
             return ""
 
-        page_config = self.update_page_config(nb, self.page_config)
+        page_config = self.update_page_config(nb, resources, self.page_config)
 
         # align the base url with the one used in the resources
         # this is because the base Voila template expects the base_url to be in the resources here:
         # https://github.com/voila-dashboards/voila/blob/0f4cc5360ff387eeaf7e647cee712b2ce08d573a/share/jupyter/voila/templates/lab/index.html.j2#L81
         # TODO: investigate whether there is something to do in Voila to avoid this
         base_url = page_config["baseUrl"]
         resources["base_url"] = base_url
@@ -116,13 +116,21 @@
             yield output
 
     def _init_resources(self, resources):
         # Not calling Voila's _init_resources, because we want to embed static
         # assets like CSS and theming instead of serving them from the server
         return super(VoilaExporter, self)._init_resources(resources)
 
-    def update_page_config(self, nb, page_config):
+    def update_page_config(self, nb, resources, page_config):
         page_config_copy = deepcopy(page_config)
 
         page_config_copy["notebookSrc"] = nb
 
+        # We need to forward some Jinja configuration options to the frontend rendering logic
+        page_config_copy["include_output"] = resources["global_content_filter"][
+            "include_output"
+        ]
+        page_config_copy["include_output_prompt"] = resources["global_content_filter"][
+            "include_output_prompt"
+        ]
+
         return page_config_copy
```

### Comparing `voici-0.4.1/voici/tree_exporter.py` & `voici-0.4.2/voici/tree_exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1023.js` & `voici-0.4.2/voici/static/build/1023.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/103.js` & `voici-0.4.2/voici/static/build/103.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1053.js` & `voici-0.4.2/voici/static/build/1053.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1058.js` & `voici-0.4.2/voici/static/build/1058.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1100.js` & `voici-0.4.2/voici/static/build/1100.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1105.js` & `voici-0.4.2/voici/static/build/1105.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1432.js` & `voici-0.4.2/voici/static/build/1432.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1553.js` & `voici-0.4.2/voici/static/build/1553.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1581.js` & `voici-0.4.2/voici/static/build/1581.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1667.js` & `voici-0.4.2/voici/static/build/1667.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1672.js` & `voici-0.4.2/voici/static/build/1672.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1770.js` & `voici-0.4.2/voici/static/build/1770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1890.js` & `voici-0.4.2/voici/static/build/1890.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/1980.js` & `voici-0.4.2/voici/static/build/1980.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2075.js` & `voici-0.4.2/voici/static/build/2075.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2106.js` & `voici-0.4.2/voici/static/build/2106.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2230.js` & `voici-0.4.2/voici/static/build/2230.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2322.js` & `voici-0.4.2/voici/static/build/2322.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2359.js` & `voici-0.4.2/voici/static/build/2359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2361.js` & `voici-0.4.2/voici/static/build/2361.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2488.js` & `voici-0.4.2/voici/static/build/2488.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2630.js` & `voici-0.4.2/voici/static/build/2630.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2687.js` & `voici-0.4.2/voici/static/build/2687.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/275.js` & `voici-0.4.2/voici/static/build/275.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2784.js` & `voici-0.4.2/voici/static/build/2784.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/286.js` & `voici-0.4.2/voici/static/build/286.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/2950.js` & `voici-0.4.2/voici/static/build/2950.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3008.js` & `voici-0.4.2/voici/static/build/3008.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3086.js` & `voici-0.4.2/voici/static/build/3086.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3251.js` & `voici-0.4.2/voici/static/build/3251.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3256.js` & `voici-0.4.2/voici/static/build/3256.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/330.js` & `voici-0.4.2/voici/static/build/330.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3305.js` & `voici-0.4.2/voici/static/build/3305.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3312.js` & `voici-0.4.2/voici/static/build/3312.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3316.js` & `voici-0.4.2/voici/static/build/3316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3316.js.LICENSE.txt` & `voici-0.4.2/voici/static/build/3316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3349.js` & `voici-0.4.2/voici/static/build/3349.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/339.js` & `voici-0.4.2/voici/static/build/339.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3504.js` & `voici-0.4.2/voici/static/build/3504.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3655.js` & `voici-0.4.2/voici/static/build/3655.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3693.js` & `voici-0.4.2/voici/static/build/3693.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3811.js` & `voici-0.4.2/voici/static/build/3811.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3851.js` & `voici-0.4.2/voici/static/build/3851.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/3922.js` & `voici-0.4.2/voici/static/build/3922.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4259.js` & `voici-0.4.2/voici/static/build/4259.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4359.js` & `voici-0.4.2/voici/static/build/4359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4382.js` & `voici-0.4.2/voici/static/build/4382.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/450.js` & `voici-0.4.2/voici/static/build/450.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4530.js` & `voici-0.4.2/voici/static/build/4530.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4875.js` & `voici-0.4.2/voici/static/build/4875.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4896.js` & `voici-0.4.2/voici/static/build/4896.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4939.js` & `voici-0.4.2/voici/static/build/4939.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4963.js` & `voici-0.4.2/voici/static/build/4963.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4963.js.LICENSE.txt` & `voici-0.4.2/voici/static/build/4963.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/4977.js` & `voici-0.4.2/voici/static/build/4977.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5188.js` & `voici-0.4.2/voici/static/build/5188.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5291.js` & `voici-0.4.2/voici/static/build/5291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/53.js` & `voici-0.4.2/voici/static/build/53.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5403.js` & `voici-0.4.2/voici/static/build/5403.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5445.js` & `voici-0.4.2/voici/static/build/5445.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5474.js` & `voici-0.4.2/voici/static/build/6852.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [5474], {
+    [6852], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.1",
+                version: "0.4.2",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -93,37 +93,36 @@
                     watch: 'tsc-watch --onSuccess "webpack --mode=development"'
                 },
                 publishConfig: {
                     access: "public"
                 }
             }
         },
-        65474: (e, t, n) => {
+        46852: (e, t, n) => {
             "use strict";
-            n.r(t), n(71024), n(24627);
+            n.r(t);
             var i = n(59110),
                 a = n(94456),
-                r = n(7631),
                 o = n(22312),
-                s = n(75238),
-                l = n(73198),
-                u = n(40049),
-                c = n(12299),
-                d = n(35918),
-                p = n(92233),
-                g = n(42051);
-            const m = n(27693),
-                h = "application/vnd.jupyter.widget-view+json";
-            class f extends s.JupyterFrontEnd {
+                r = n(75238),
+                s = n(73198),
+                l = n(40049),
+                u = n(12299),
+                c = n(35918),
+                d = n(92233),
+                p = n(42051);
+            const g = n(27693),
+                m = "application/vnd.jupyter.widget-view+json";
+            class h extends r.JupyterFrontEnd {
                 constructor(e) {
                     var t;
                     if (super(Object.assign(Object.assign({}, e), {
                             shell: null !== (t = e.shell) && void 0 !== t ? t : new o.VoilaShell
-                        })), this.name = "Voici", this.namespace = this.name, this.version = m.version, this._widgetManagerPromise = new p.PromiseDelegate, e.mimeExtensions)
-                        for (const t of (0, s.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
+                        })), this.name = "Voici", this.namespace = this.name, this.version = g.version, this._widgetManagerPromise = new d.PromiseDelegate, e.mimeExtensions)
+                        for (const t of (0, r.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
                     this._kernelspecs = e.kernelspecs, this._serviceManager = e.serviceManager
                 }
                 get widgetManagerPromise() {
                     return this._widgetManagerPromise
                 }
                 get paths() {
                     return {
@@ -169,201 +168,188 @@
                     }))
                 }
                 async renderWidgets() {
                     var e, t, n;
                     const a = this._serviceManager;
                     if (!a) return void console.error("Missing service manager");
                     await a.ready;
-                    const r = a.sessions;
-                    await r.ready;
-                    const o = new u.NotebookModel;
-                    o.fromString(i.PageConfig.getOption("notebookSrc"));
-                    let s = o.metadata.get("kernelspec");
+                    const o = a.sessions;
+                    await o.ready;
+                    const r = new l.NotebookModel;
+                    r.fromString(i.PageConfig.getOption("notebookSrc"));
+                    let s = r.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
-                    const l = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
+                    const d = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
                     let p;
-                    if (!l) return void console.error("No kernel available");
-                    if (s.name in l) console.log(`${s.name} kernel is available!`), p = l[s.name];
+                    if (!d) return void console.error("No kernel available");
+                    if (s.name in d) console.log(`${s.name} kernel is available!`), p = d[s.name];
                     else
-                        for (const e in l)
-                            if (s.language === (null === (n = l[e]) || void 0 === n ? void 0 : n.language)) {
-                                console.log(`${s.name} kernel is not available, fallback to using ${l[e].name}`), p = l[e];
+                        for (const e in d)
+                            if (s.language === (null === (n = d[e]) || void 0 === n ? void 0 : n.language)) {
+                                console.log(`${s.name} kernel is not available, fallback to using ${d[e].name}`), p = d[e];
                                 break
                             } if (!p) return void console.error(`No kernel available for ${s.language}`);
-                    const g = await r.startNew({
+                    const g = await o.startNew({
                             name: "",
                             path: "",
                             type: "notebook",
                             kernel: p
                         }),
-                        m = g.kernel;
-                    m ? m.connectionStatusChanged.connect((async (e, t) => {
+                        h = g.kernel;
+                    h ? h.connectionStatusChanged.connect((async (e, t) => {
                         if ("connected" === t) {
                             window.update_loading_text(0, 0, "Starting up kernel...");
-                            const e = new c.RenderMimeRegistry({
-                                    initialFactories: c.standardRendererFactories
+                            const e = new u.RenderMimeRegistry({
+                                    initialFactories: u.standardRendererFactories
                                 }),
-                                t = new d.KernelWidgetManager(m, e);
-                            if (e.removeMimeType(h), e.addFactory({
+                                t = new c.KernelWidgetManager(h, e);
+                            if (e.removeMimeType(m), e.addFactory({
                                     safe: !1,
-                                    mimeTypes: [h],
-                                    createRenderer: e => new d.WidgetRenderer(e, t)
+                                    mimeTypes: [m],
+                                    createRenderer: e => new c.WidgetRenderer(e, t)
                                 }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            m.statusChanged.connect((async (t, i) => {
+                            h.statusChanged.connect((async (t, i) => {
                                 n || "idle" !== i || (n = !0, await b.executeCells({
-                                    source: o,
+                                    source: r,
                                     rendermime: e,
                                     kernel: g.kernel
                                 }))
                             }))
                         }
                     })) : console.error("Can not start kernel")
                 }
             }
             var b;
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
-                        source: i,
-                        rendermime: a,
+                        source: a,
+                        rendermime: o,
                         kernel: r
-                    } = e, o = i.cells.length;
-                    for (let e = 0; e < o; e++) {
-                        const s = i.cells.get(e);
-                        if (window.update_loading_text(e + 1, o, null), "code" !== s.type) {
-                            e === o - 1 && window.display_cells();
+                    } = e, l = a.cells.length;
+                    for (let e = 0; e < l; e++) {
+                        const u = a.cells.get(e);
+                        if (window.update_loading_text(e + 1, l, null), "code" !== u.type) {
+                            e === l - 1 && window.display_cells();
                             continue
                         }
-                        const u = new l.OutputAreaModel({
-                                trusted: !0
-                            }),
-                            c = new l.SimplifiedOutputArea({
-                                model: u,
-                                rendermime: a
-                            });
-                        c.future = r.requestExecute({
-                            code: s.value.text
-                        }), await c.future.done;
-                        const d = document.querySelector(`[cell-index="${e+1}"]`);
-                        if (d && c.node.childNodes.length > 0) {
-                            null === (t = d.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
+                        const c = new s.OutputAreaModel({
+                            trusted: !0
+                        });
+                        let d;
+                        d = "true" === i.PageConfig.getOption("include_output_prompt") ? new s.OutputArea({
+                            model: c,
+                            rendermime: o
+                        }) : new s.SimplifiedOutputArea({
+                            model: c,
+                            rendermime: o
+                        }), d.future = r.requestExecute({
+                            code: u.value.text
+                        }), await d.future.done;
+                        const g = document.querySelector(`[cell-index="${e+1}"]`);
+                        if (g && i.PageConfig.getOption("include_output") && d.node.childNodes.length > 0) {
+                            null === (t = g.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
-                            e.classList.add("jp-Cell-outputWrapper"), null === (n = d.lastElementChild) || void 0 === n || n.appendChild(e), c.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), g.Widget.attach(c, e)
+                            e.classList.add("jp-Cell-outputWrapper");
+                            const i = document.createElement("div");
+                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = g.lastElementChild) || void 0 === n || n.appendChild(e), d.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), p.Widget.attach(d, e)
                         }
-                        e === o - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
+                        e === l - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
                     }
                 }
             }(b || (b = {}));
-            var w = n(67651),
+            var f = n(67651),
                 y = n(37782);
-            const v = {
-                    id: "@voila-dashboards/voici:widget-manager",
-                    autoStart: !0,
-                    provides: w.IJupyterWidgetRegistry,
-                    activate: async e => {
-                        if (!(e instanceof f)) throw Error("The Voici Widget Manager plugin must be activated in a VoilaApp");
-                        const t = e.widgetManagerPromise;
-                        return {
-                            registerWidget: async e => {
-                                (await t.promise).register(e)
-                            }
-                        }
-                    }
-                },
-                j = {
-                    id: "@voila-dashboards/voici:theme-manager",
-                    autoStart: !0,
-                    optional: [y.IThemeManager],
-                    activate: (e, t) => {
-                        if (!t) return;
-                        const n = window.location.search,
-                            a = new URLSearchParams(n).get("theme"),
-                            r = i.PageConfig.getOption("jpThemeName");
-                        let o = a ? decodeURIComponent(a) : r;
-                        o = o || "light", "dark" !== o && "JupyterLab Dark" !== o || (o = "JupyterLab Dark"), "light" !== o && "JupyterLab Light" !== o || (o = "JupyterLab Light"), t.themeChanged.connect((() => {
-                            t.theme !== o && t.setTheme(o)
-                        }))
-                    }
-                },
-                P = [o.pathsPlugin, o.translatorPlugin, v, j];
-            async function k(e, t) {
+            f.IJupyterWidgetRegistry;
+            const w = {
+                id: "@voila-dashboards/voici:theme-manager",
+                autoStart: !0,
+                optional: [y.IThemeManager],
+                activate: (e, t) => {
+                    if (!t) return;
+                    const n = window.location.search,
+                        a = new URLSearchParams(n).get("theme"),
+                        o = i.PageConfig.getOption("jpThemeName");
+                    let r = a ? decodeURIComponent(a) : o;
+                    r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
+                        t.theme !== r && t.setTheme(r)
+                    }))
+                }
+            };
+            async function v(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
 
-            function* C(e, t) {
+            function* j(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
                 const a = Array.isArray(n) ? n : [n];
                 for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            const O = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                x = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+            o.pathsPlugin, o.translatorPlugin;
+            const P = [n.e(7531).then(n.t.bind(n, 7531, 23))],
+                C = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), P],
-                    t = [n(84632), n(70851)],
-                    s = JSON.parse(i.PageConfig.getOption("federated_extensions")),
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), o.translatorPlugin, o.pathsPlugin, w],
+                    t = [],
+                    r = JSON.parse(i.PageConfig.getOption("federated_extensions")),
+                    s = [],
                     l = [],
                     u = [],
-                    c = [],
-                    d = [],
-                    p = await Promise.allSettled(s.map((async e => (await async function(e, t) {
+                    c = await Promise.allSettled(r.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
                             }))
                         }(e), await n.I("default");
                         const i = window._JUPYTERLAB[t];
                         await i.init(n.S.default)
                     }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
-                Object.entries(p).forEach((([e, t]) => {
+                Object.entries(c).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
-                    n.liteExtension ? d.push(k(n.name, n.extension)) : (n.extension && l.push(k(n.name, n.extension)), n.mimeExtension && u.push(k(n.name, n.mimeExtension)), n.style && c.push(k(n.name, n.style)))
-                })), (await Promise.allSettled(l)).forEach((t => {
+                    n.extension && s.push(v(n.name, n.extension)), n.mimeExtension && l.push(v(n.name, n.mimeExtension)), n.style && u.push(v(n.name, n.style))
+                })), (await Promise.allSettled(s)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of C(t.value, x)) e.push(n);
+                        for (const n of j(t.value, C)) e.push(n);
                     else console.error(t.reason)
-                })), (await Promise.allSettled(u)).forEach((e => {
+                })), (await Promise.allSettled(l)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of C(e.value, x)) t.push(n);
+                        for (const n of j(e.value, C)) t.push(n);
                     else console.error(e.reason)
-                })), (await Promise.allSettled(c)).filter((({
+                })), (await Promise.allSettled(u)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
-                const g = [];
-                (await Promise.all(O)).forEach((e => {
-                    for (const t of C(e, x)) g.push(t)
-                })), (await Promise.allSettled(d)).forEach((e => {
-                    if ("fulfilled" === e.status)
-                        for (const t of C(e.value, x)) g.push(t);
-                    else console.error(e.reason)
+                const d = [];
+                (await Promise.all(P)).forEach((e => {
+                    for (const t of j(e, C)) d.push(t)
                 }));
-                const m = new a.JupyterLiteServer({
+                const p = new a.JupyterLiteServer({
                     shell: null
                 });
-                m.registerPluginModules(g), await m.start();
-                const h = await m.resolveRequiredService(r.IKernelSpecs),
-                    b = m.serviceManager,
-                    w = new f({
-                        serviceManager: b,
-                        kernelspecs: h,
-                        mimeExtensions: t,
+                p.registerPluginModules(d), await p.start();
+                const g = p.serviceManager,
+                    m = new h({
+                        serviceManager: g,
                         shell: new o.VoilaShell
                     });
-                w.registerPluginModules(e), await w.start(), await w.renderWidgets(), window.jupyterapp = w
+                m.registerPluginModules(e), m.started.then((() => {
+                    const e = document.getElementById("voila-tree-main");
+                    e && (e.style.display = "unset")
+                })), m.start()
             }))
         }
     }
 ]);
```

### Comparing `voici-0.4.1/voici/static/build/5826.js` & `voici-0.4.2/voici/static/build/5826.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5950.js` & `voici-0.4.2/voici/static/build/5950.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5952.js` & `voici-0.4.2/voici/static/build/5952.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/596.js` & `voici-0.4.2/voici/static/build/596.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/5985.js` & `voici-0.4.2/voici/static/build/5985.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6111.js` & `voici-0.4.2/voici/static/build/6111.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6178.js` & `voici-0.4.2/voici/static/build/6178.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6196.js` & `voici-0.4.2/voici/static/build/6196.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6219.js` & `voici-0.4.2/voici/static/build/6219.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6219.js.LICENSE.txt` & `voici-0.4.2/voici/static/build/6219.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6527.js` & `voici-0.4.2/voici/static/build/6527.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6614.js` & `voici-0.4.2/voici/static/build/6614.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6616.js` & `voici-0.4.2/voici/static/build/6616.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6757.js` & `voici-0.4.2/voici/static/build/6757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6770.js` & `voici-0.4.2/voici/static/build/6770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6790.js` & `voici-0.4.2/voici/static/build/6790.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6839.js` & `voici-0.4.2/voici/static/build/6839.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6852.js` & `voici-0.4.2/voici/static/build/5474.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [6852], {
+    [5474], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.1",
+                version: "0.4.2",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -93,36 +93,37 @@
                     watch: 'tsc-watch --onSuccess "webpack --mode=development"'
                 },
                 publishConfig: {
                     access: "public"
                 }
             }
         },
-        46852: (e, t, n) => {
+        65474: (e, t, n) => {
             "use strict";
-            n.r(t), n(71024);
+            n.r(t), n(24627);
             var i = n(59110),
                 a = n(94456),
-                r = n(22312),
-                o = n(75238),
-                s = n(73198),
-                l = n(40049),
-                u = n(12299),
-                c = n(35918),
-                d = n(92233),
-                p = n(42051);
-            const g = n(27693),
-                m = "application/vnd.jupyter.widget-view+json";
-            class h extends o.JupyterFrontEnd {
+                r = n(7631),
+                o = n(22312),
+                s = n(75238),
+                l = n(73198),
+                u = n(40049),
+                c = n(12299),
+                d = n(35918),
+                p = n(92233),
+                g = n(42051);
+            const m = n(27693),
+                h = "application/vnd.jupyter.widget-view+json";
+            class f extends s.JupyterFrontEnd {
                 constructor(e) {
                     var t;
                     if (super(Object.assign(Object.assign({}, e), {
-                            shell: null !== (t = e.shell) && void 0 !== t ? t : new r.VoilaShell
-                        })), this.name = "Voici", this.namespace = this.name, this.version = g.version, this._widgetManagerPromise = new d.PromiseDelegate, e.mimeExtensions)
-                        for (const t of (0, o.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
+                            shell: null !== (t = e.shell) && void 0 !== t ? t : new o.VoilaShell
+                        })), this.name = "Voici", this.namespace = this.name, this.version = m.version, this._widgetManagerPromise = new p.PromiseDelegate, e.mimeExtensions)
+                        for (const t of (0, s.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
                     this._kernelspecs = e.kernelspecs, this._serviceManager = e.serviceManager
                 }
                 get widgetManagerPromise() {
                     return this._widgetManagerPromise
                 }
                 get paths() {
                     return {
@@ -170,52 +171,52 @@
                 async renderWidgets() {
                     var e, t, n;
                     const a = this._serviceManager;
                     if (!a) return void console.error("Missing service manager");
                     await a.ready;
                     const r = a.sessions;
                     await r.ready;
-                    const o = new l.NotebookModel;
+                    const o = new u.NotebookModel;
                     o.fromString(i.PageConfig.getOption("notebookSrc"));
                     let s = o.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
-                    const d = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
+                    const l = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
                     let p;
-                    if (!d) return void console.error("No kernel available");
-                    if (s.name in d) console.log(`${s.name} kernel is available!`), p = d[s.name];
+                    if (!l) return void console.error("No kernel available");
+                    if (s.name in l) console.log(`${s.name} kernel is available!`), p = l[s.name];
                     else
-                        for (const e in d)
-                            if (s.language === (null === (n = d[e]) || void 0 === n ? void 0 : n.language)) {
-                                console.log(`${s.name} kernel is not available, fallback to using ${d[e].name}`), p = d[e];
+                        for (const e in l)
+                            if (s.language === (null === (n = l[e]) || void 0 === n ? void 0 : n.language)) {
+                                console.log(`${s.name} kernel is not available, fallback to using ${l[e].name}`), p = l[e];
                                 break
                             } if (!p) return void console.error(`No kernel available for ${s.language}`);
                     const g = await r.startNew({
                             name: "",
                             path: "",
                             type: "notebook",
                             kernel: p
                         }),
-                        h = g.kernel;
-                    h ? h.connectionStatusChanged.connect((async (e, t) => {
+                        m = g.kernel;
+                    m ? m.connectionStatusChanged.connect((async (e, t) => {
                         if ("connected" === t) {
                             window.update_loading_text(0, 0, "Starting up kernel...");
-                            const e = new u.RenderMimeRegistry({
-                                    initialFactories: u.standardRendererFactories
+                            const e = new c.RenderMimeRegistry({
+                                    initialFactories: c.standardRendererFactories
                                 }),
-                                t = new c.KernelWidgetManager(h, e);
-                            if (e.removeMimeType(m), e.addFactory({
+                                t = new d.KernelWidgetManager(m, e);
+                            if (e.removeMimeType(h), e.addFactory({
                                     safe: !1,
-                                    mimeTypes: [m],
-                                    createRenderer: e => new c.WidgetRenderer(e, t)
+                                    mimeTypes: [h],
+                                    createRenderer: e => new d.WidgetRenderer(e, t)
                                 }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            h.statusChanged.connect((async (t, i) => {
+                            m.statusChanged.connect((async (t, i) => {
                                 n || "idle" !== i || (n = !0, await b.executeCells({
                                     source: o,
                                     rendermime: e,
                                     kernel: g.kernel
                                 }))
                             }))
                         }
@@ -223,128 +224,151 @@
                 }
             }
             var b;
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
-                        source: i,
-                        rendermime: a,
-                        kernel: r
-                    } = e, o = i.cells.length;
-                    for (let e = 0; e < o; e++) {
-                        const l = i.cells.get(e);
-                        if (window.update_loading_text(e + 1, o, null), "code" !== l.type) {
-                            e === o - 1 && window.display_cells();
+                        source: a,
+                        rendermime: r,
+                        kernel: o
+                    } = e, s = a.cells.length;
+                    for (let e = 0; e < s; e++) {
+                        const u = a.cells.get(e);
+                        if (window.update_loading_text(e + 1, s, null), "code" !== u.type) {
+                            e === s - 1 && window.display_cells();
                             continue
                         }
-                        const u = new s.OutputAreaModel({
-                                trusted: !0
-                            }),
-                            c = new s.SimplifiedOutputArea({
-                                model: u,
-                                rendermime: a
-                            });
-                        c.future = r.requestExecute({
-                            code: l.value.text
-                        }), await c.future.done;
-                        const d = document.querySelector(`[cell-index="${e+1}"]`);
-                        if (d && c.node.childNodes.length > 0) {
-                            null === (t = d.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
+                        const c = new l.OutputAreaModel({
+                            trusted: !0
+                        });
+                        let d;
+                        d = "true" === i.PageConfig.getOption("include_output_prompt") ? new l.OutputArea({
+                            model: c,
+                            rendermime: r
+                        }) : new l.SimplifiedOutputArea({
+                            model: c,
+                            rendermime: r
+                        }), d.future = o.requestExecute({
+                            code: u.value.text
+                        }), await d.future.done;
+                        const p = document.querySelector(`[cell-index="${e+1}"]`);
+                        if (p && i.PageConfig.getOption("include_output") && d.node.childNodes.length > 0) {
+                            null === (t = p.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
-                            e.classList.add("jp-Cell-outputWrapper"), null === (n = d.lastElementChild) || void 0 === n || n.appendChild(e), c.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), p.Widget.attach(c, e)
+                            e.classList.add("jp-Cell-outputWrapper");
+                            const i = document.createElement("div");
+                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = p.lastElementChild) || void 0 === n || n.appendChild(e), d.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), g.Widget.attach(d, e)
                         }
-                        e === o - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
+                        e === s - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
                     }
                 }
             }(b || (b = {}));
-            var f = n(67651),
+            var w = n(67651),
                 y = n(37782);
-            f.IJupyterWidgetRegistry;
-            const w = {
-                id: "@voila-dashboards/voici:theme-manager",
-                autoStart: !0,
-                optional: [y.IThemeManager],
-                activate: (e, t) => {
-                    if (!t) return;
-                    const n = window.location.search,
-                        a = new URLSearchParams(n).get("theme"),
-                        r = i.PageConfig.getOption("jpThemeName");
-                    let o = a ? decodeURIComponent(a) : r;
-                    o = o || "light", "dark" !== o && "JupyterLab Dark" !== o || (o = "JupyterLab Dark"), "light" !== o && "JupyterLab Light" !== o || (o = "JupyterLab Light"), t.themeChanged.connect((() => {
-                        t.theme !== o && t.setTheme(o)
-                    }))
-                }
-            };
-            async function v(e, t) {
+            const v = {
+                    id: "@voila-dashboards/voici:widget-manager",
+                    autoStart: !0,
+                    provides: w.IJupyterWidgetRegistry,
+                    activate: async e => {
+                        if (!(e instanceof f)) throw Error("The Voici Widget Manager plugin must be activated in a VoilaApp");
+                        const t = e.widgetManagerPromise;
+                        return {
+                            registerWidget: async e => {
+                                (await t.promise).register(e)
+                            }
+                        }
+                    }
+                },
+                j = {
+                    id: "@voila-dashboards/voici:theme-manager",
+                    autoStart: !0,
+                    optional: [y.IThemeManager],
+                    activate: (e, t) => {
+                        if (!t) return;
+                        const n = window.location.search,
+                            a = new URLSearchParams(n).get("theme"),
+                            r = i.PageConfig.getOption("jpThemeName");
+                        let o = a ? decodeURIComponent(a) : r;
+                        o = o || "light", "dark" !== o && "JupyterLab Dark" !== o || (o = "JupyterLab Dark"), "light" !== o && "JupyterLab Light" !== o || (o = "JupyterLab Light"), t.themeChanged.connect((() => {
+                            t.theme !== o && t.setTheme(o)
+                        }))
+                    }
+                },
+                P = [o.pathsPlugin, o.translatorPlugin, v, j];
+            async function C(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
 
-            function* P(e, t) {
+            function* k(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
                 const a = Array.isArray(n) ? n : [n];
                 for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            r.pathsPlugin, r.translatorPlugin;
-            const j = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                C = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+            const O = [n.e(7531).then(n.t.bind(n, 7531, 23))],
+                x = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), r.translatorPlugin, r.pathsPlugin, w],
-                    t = [],
-                    o = JSON.parse(i.PageConfig.getOption("federated_extensions")),
-                    s = [],
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), P],
+                    t = [n(84632), n(70851)],
+                    s = JSON.parse(i.PageConfig.getOption("federated_extensions")),
                     l = [],
                     u = [],
-                    c = await Promise.allSettled(o.map((async e => (await async function(e, t) {
+                    c = [],
+                    d = [],
+                    p = await Promise.allSettled(s.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
                             }))
                         }(e), await n.I("default");
                         const i = window._JUPYTERLAB[t];
                         await i.init(n.S.default)
                     }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
-                Object.entries(c).forEach((([e, t]) => {
+                Object.entries(p).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
-                    n.extension && s.push(v(n.name, n.extension)), n.mimeExtension && l.push(v(n.name, n.mimeExtension)), n.style && u.push(v(n.name, n.style))
-                })), (await Promise.allSettled(s)).forEach((t => {
+                    n.liteExtension ? d.push(C(n.name, n.extension)) : (n.extension && l.push(C(n.name, n.extension)), n.mimeExtension && u.push(C(n.name, n.mimeExtension)), n.style && c.push(C(n.name, n.style)))
+                })), (await Promise.allSettled(l)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of P(t.value, C)) e.push(n);
+                        for (const n of k(t.value, x)) e.push(n);
                     else console.error(t.reason)
-                })), (await Promise.allSettled(l)).forEach((e => {
+                })), (await Promise.allSettled(u)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of P(e.value, C)) t.push(n);
+                        for (const n of k(e.value, x)) t.push(n);
                     else console.error(e.reason)
-                })), (await Promise.allSettled(u)).filter((({
+                })), (await Promise.allSettled(c)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
-                const d = [];
-                (await Promise.all(j)).forEach((e => {
-                    for (const t of P(e, C)) d.push(t)
+                const g = [];
+                (await Promise.all(O)).forEach((e => {
+                    for (const t of k(e, x)) g.push(t)
+                })), (await Promise.allSettled(d)).forEach((e => {
+                    if ("fulfilled" === e.status)
+                        for (const t of k(e.value, x)) g.push(t);
+                    else console.error(e.reason)
                 }));
-                const p = new a.JupyterLiteServer({
+                const m = new a.JupyterLiteServer({
                     shell: null
                 });
-                p.registerPluginModules(d), await p.start();
-                const g = p.serviceManager,
-                    m = new h({
-                        serviceManager: g,
-                        shell: new r.VoilaShell
+                m.registerPluginModules(g), await m.start();
+                const h = await m.resolveRequiredService(r.IKernelSpecs),
+                    b = m.serviceManager,
+                    w = new f({
+                        serviceManager: b,
+                        kernelspecs: h,
+                        mimeExtensions: t,
+                        shell: new o.VoilaShell
                     });
-                m.registerPluginModules(e), m.started.then((() => {
-                    const e = document.getElementById("voila-tree-main");
-                    e && (e.style.display = "unset")
-                })), m.start()
+                w.registerPluginModules(e), await w.start(), await w.renderWidgets(), window.jupyterapp = w
             }))
         }
     }
 ]);
```

### Comparing `voici-0.4.1/voici/static/build/6856.js` & `voici-0.4.2/voici/static/build/6856.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6914.js` & `voici-0.4.2/voici/static/build/6914.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/6976.js` & `voici-0.4.2/voici/static/build/6976.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7003.js` & `voici-0.4.2/voici/static/build/7003.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7015.js` & `voici-0.4.2/voici/static/build/7015.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7066.js` & `voici-0.4.2/voici/static/build/7066.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/709.js` & `voici-0.4.2/voici/static/build/709.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/74.js` & `voici-0.4.2/voici/static/build/74.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7469.js` & `voici-0.4.2/voici/static/build/7469.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7560.js` & `voici-0.4.2/voici/static/build/7560.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7623.js` & `voici-0.4.2/voici/static/build/7623.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7695.js` & `voici-0.4.2/voici/static/build/7695.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/7795.js` & `voici-0.4.2/voici/static/build/7795.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8085.js` & `voici-0.4.2/voici/static/build/8085.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8164.js` & `voici-0.4.2/voici/static/build/8164.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8291.js` & `voici-0.4.2/voici/static/build/8291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8316.js` & `voici-0.4.2/voici/static/build/8316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8316.js.LICENSE.txt` & `voici-0.4.2/voici/static/build/8316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/846.js` & `voici-0.4.2/voici/static/build/846.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/86.js` & `voici-0.4.2/voici/static/build/86.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8809.js` & `voici-0.4.2/voici/static/build/8809.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/8874.js` & `voici-0.4.2/voici/static/build/8874.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9060.js` & `voici-0.4.2/voici/static/build/9060.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9112.js` & `voici-0.4.2/voici/static/build/9112.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9339.js` & `voici-0.4.2/voici/static/build/9339.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9406.js` & `voici-0.4.2/voici/static/build/9406.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9513.js` & `voici-0.4.2/voici/static/build/9513.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9727.js` & `voici-0.4.2/voici/static/build/9727.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9757.js` & `voici-0.4.2/voici/static/build/9757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9780.js` & `voici-0.4.2/voici/static/build/9780.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9807.js` & `voici-0.4.2/voici/static/build/9807.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9900.js` & `voici-0.4.2/voici/static/build/9900.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/9988.js` & `voici-0.4.2/voici/static/build/9988.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/service-worker-b2fb40a.js` & `voici-0.4.2/voici/static/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/voici/static/build/treepage.js` & `voici-0.4.2/voici/static/build/treepage.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 var _JUPYTERLAB;
 (() => {
     var e, t, l, r, a, n, o, i, u, s, m, p, h, d = {
             60392: (e, t, l) => {
                 "use strict";
-                Promise.all([l.e(1024), l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(5918), l.e(8987), l.e(6852)]).then(l.bind(l, 46852))
+                Promise.all([l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(5918), l.e(8987), l.e(6852)]).then(l.bind(l, 46852))
             },
             68444: (e, t, l) => {
                 l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
```

### Comparing `voici-0.4.1/voici/static/build/voici.js` & `voici-0.4.2/voici/static/build/voici.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 var _JUPYTERLAB;
 (() => {
     var e, t, l, r, a, n, o, i, u, s, m, h, p, d = {
             37559: (e, t, l) => {
                 "use strict";
-                Promise.all([l.e(1024), l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(4627), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(5474)]).then(l.bind(l, 65474))
+                Promise.all([l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(4627), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(5474)]).then(l.bind(l, 65474))
             },
             68444: (e, t, l) => {
                 l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
```

### Comparing `voici-0.4.1/LICENSE` & `voici-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/README.md` & `voici-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Voici
 
 ![Github Actions Status](https://github.com/voila-dashboards/voici/actions/workflows/main.yml/badge.svg)
 [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge-launch.svg)](https://voici.readthedocs.io/en/latest/_static/lite)
 [![Documentation Status](https://readthedocs.org/projects/voici/badge/?version=latest)](https://voici.readthedocs.io/en/latest/?badge=latest)
 
-🚧 **WARNING: Voici is still a work in progress and should not be used for production workloads.** 🚧
+🚧 **WARNING: Voici is in early preview** 🚧
 
 Voici is a tool for generating static dashboards from Jupyter Notebooks. It can be used as a drop-in replacement for [Voilà](https://github.com/voila-dashboards/voila) and it has the same commands and supports most of Voila's configuration options.
 
 Unlike Voila, which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
 
 This is made possible thanks to the amazing work done in the [JupyterLite project](https://github.com/jupyterlite/jupyterlite).
```

### Comparing `voici-0.4.1/pyproject.toml` & `voici-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voici-0.4.1/PKG-INFO` & `voici-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voici
-Version: 0.4.1
+Version: 0.4.2
 Summary: Voici turns Jupyter notebooks into static web applications
 Project-URL: Homepage, https://github.com/voila-dashboards/voici
 Author: Voila Development Team
 License: BSD License
         
         Copyright (c) 2018 Voilà contributors.
         All rights reserved.
@@ -63,15 +63,15 @@
 
 # Voici
 
 ![Github Actions Status](https://github.com/voila-dashboards/voici/actions/workflows/main.yml/badge.svg)
 [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge-launch.svg)](https://voici.readthedocs.io/en/latest/_static/lite)
 [![Documentation Status](https://readthedocs.org/projects/voici/badge/?version=latest)](https://voici.readthedocs.io/en/latest/?badge=latest)
 
-🚧 **WARNING: Voici is still a work in progress and should not be used for production workloads.** 🚧
+🚧 **WARNING: Voici is in early preview** 🚧
 
 Voici is a tool for generating static dashboards from Jupyter Notebooks. It can be used as a drop-in replacement for [Voilà](https://github.com/voila-dashboards/voila) and it has the same commands and supports most of Voila's configuration options.
 
 Unlike Voila, which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
 
 This is made possible thanks to the amazing work done in the [JupyterLite project](https://github.com/jupyterlite/jupyterlite).
```

