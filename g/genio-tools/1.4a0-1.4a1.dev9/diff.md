# Comparing `tmp/genio_tools-1.4a0-py3-none-any.whl.zip` & `tmp/genio_tools-1.4a1.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,27 @@
-Zip file size: 19874 bytes, number of entries: 22
--rw-rw-r--  2.0 unx      428 b- defN 23-May-03 11:13 aiot/__init__.py
+Zip file size: 24685 bytes, number of entries: 25
+-rw-rw-r--  2.0 unx      570 b- defN 23-May-03 12:11 aiot/__init__.py
 -rw-rw-r--  2.0 unx     1088 b- defN 23-May-03 11:13 aiot/app.py
--rw-rw-r--  2.0 unx     3640 b- defN 23-May-03 11:13 aiot/board.py
+-rw-rw-r--  2.0 unx     4953 b- defN 23-May-03 12:11 aiot/board.py
+-rw-rw-r--  2.0 unx     1973 b- defN 23-May-03 12:11 aiot/boardcontrol_linux.py
+-rw-rw-r--  2.0 unx     2472 b- defN 23-May-03 12:11 aiot/boardcontrol_win.py
 -rw-rw-r--  2.0 unx     2460 b- defN 23-May-03 09:03 aiot/bootrom.py
 -rw-rw-r--  2.0 unx     3402 b- defN 23-May-03 09:03 aiot/config.py
 -rw-rw-r--  2.0 unx     4040 b- defN 23-May-03 09:03 aiot/efuse.py
 -rw-rw-r--  2.0 unx     1306 b- defN 23-May-03 09:03 aiot/fastboot.py
--rw-rw-r--  2.0 unx     6682 b- defN 23-May-03 11:13 aiot/flash.py
+-rw-rw-r--  2.0 unx     9131 b- defN 23-May-03 12:11 aiot/flash.py
 -rw-rw-r--  2.0 unx     1377 b- defN 23-May-03 09:03 aiot/ftdi.py
+-rw-rw-r--  2.0 unx     3861 b- defN 23-May-03 12:11 aiot/ftdi_win.py
 -rw-rw-r--  2.0 unx      800 b- defN 23-May-03 09:03 aiot/rpmb.py
--rw-rw-r--  2.0 unx     2665 b- defN 23-May-03 11:13 aiot/ubootenv.py
--rw-rw-r--  2.0 unx      157 b- defN 23-May-03 11:22 aiot/version.py
+-rw-rw-r--  2.0 unx     2665 b- defN 23-May-03 11:27 aiot/ubootenv.py
+-rw-rw-r--  2.0 unx      170 b- defN 23-May-03 12:12 aiot/version.py
 -rw-rw-r--  2.0 unx      126 b- defN 23-May-03 09:03 aiot/image/__init__.py
--rw-rw-r--  2.0 unx     2526 b- defN 23-May-03 11:13 aiot/image/android.py
--rw-rw-r--  2.0 unx     6736 b- defN 23-May-03 11:13 aiot/image/ubuntu.py
--rw-rw-r--  2.0 unx     9043 b- defN 23-May-03 11:13 aiot/image/yocto.py
--rw-rw-r--  2.0 unx     1091 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      873 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx      334 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1660 b- defN 23-May-03 11:22 genio_tools-1.4a0.dist-info/RECORD
-22 files, 50531 bytes uncompressed, 17238 bytes compressed:  65.9%
+-rw-rw-r--  2.0 unx     2406 b- defN 23-May-03 11:27 aiot/image/android.py
+-rw-rw-r--  2.0 unx     6736 b- defN 23-May-03 11:27 aiot/image/ubuntu.py
+-rw-rw-r--  2.0 unx     9127 b- defN 23-May-03 11:27 aiot/image/yocto.py
+-rw-rw-r--  2.0 unx     1091 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      931 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      334 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1927 b- defN 23-May-03 12:12 genio_tools-1.4a1.dev9.dist-info/RECORD
+25 files, 63043 bytes uncompressed, 21629 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -3,14 +3,20 @@
 
 Filename: aiot/app.py
 Comment: 
 
 Filename: aiot/board.py
 Comment: 
 
+Filename: aiot/boardcontrol_linux.py
+Comment: 
+
+Filename: aiot/boardcontrol_win.py
+Comment: 
+
 Filename: aiot/bootrom.py
 Comment: 
 
 Filename: aiot/config.py
 Comment: 
 
 Filename: aiot/efuse.py
@@ -21,14 +27,17 @@
 
 Filename: aiot/flash.py
 Comment: 
 
 Filename: aiot/ftdi.py
 Comment: 
 
+Filename: aiot/ftdi_win.py
+Comment: 
+
 Filename: aiot/rpmb.py
 Comment: 
 
 Filename: aiot/ubootenv.py
 Comment: 
 
 Filename: aiot/version.py
@@ -42,26 +51,26 @@
 
 Filename: aiot/image/ubuntu.py
 Comment: 
 
 Filename: aiot/image/yocto.py
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/LICENSE
+Filename: genio_tools-1.4a1.dev9.dist-info/LICENSE
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/METADATA
+Filename: genio_tools-1.4a1.dev9.dist-info/METADATA
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/WHEEL
+Filename: genio_tools-1.4a1.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/entry_points.txt
+Filename: genio_tools-1.4a1.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/top_level.txt
+Filename: genio_tools-1.4a1.dev9.dist-info/top_level.txt
 Comment: 
 
-Filename: genio_tools-1.4a0.dist-info/RECORD
+Filename: genio_tools-1.4a1.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiot/__init__.py

```diff
@@ -8,9 +8,12 @@
 from aiot.config import Config
 from aiot.fastboot import Fastboot
 from aiot.flash import Flash
 from aiot.ubootenv import UBootEnv
 from aiot.version import version
 
 if platform.system() == 'Linux':
-    from aiot.board import BoardControl
+    from aiot.boardcontrol_linux import BoardControl
     from aiot.ftdi import FtdiControl
+elif platform.system() == 'Windows':
+    from aiot.boardcontrol_win import BoardControl
+    from aiot.ftdi_win import FtdiControl
```

## aiot/board.py

```diff
@@ -1,120 +1,131 @@
 # SPDX-License-Identifier: MIT
 # Copyright 2020 (c) BayLibre, SAS
 # Author: Fabien Parent <fparent@baylibre.com>
 
 import logging
-import gpiod
+import platform
 import sys
 import time
-
 import aiot
 
-class BoardControl:
-    GPIO_LOW = 0
-    GPIO_HIGH = 1
-
-    def __init__(self, reset_gpio, dl_gpio, pwr_gpio, chip_id = None):
-        chip = self.get_gpiochip(chip_id)
-
-        config = gpiod.line_request()
-        config.consumer = "aiot-board"
-        config.request_type = gpiod.line_request.DIRECTION_OUTPUT
-
-        self.reset_gpio = chip.get_line(reset_gpio)
-        self.dl_gpio = chip.get_line(dl_gpio)
-        self.pwr_gpio = chip.get_line(pwr_gpio)
-
-        self.reset_gpio.request(config)
-        self.dl_gpio.request(config)
-        self.pwr_gpio.request(config)
-
-        self.logger = logging.getLogger('aiot')
-
-    def get_gpiochip(self, chip_id = None):
-        known_devices = []
-        logger = logging.getLogger('aiot')
-
-        if chip_id is not None:
-            return gpiod.chip(chip_id)
+app_description = f"""
+    AIoT board control version {aiot.version}
 
-        for chip in gpiod.chip_iter():
-            if chip.label == 'ftdi-cbus':
-                known_devices.append(chip)
+    This tool is used to control MediaTek Genio and Pumpkin boards thorugh
+    the FTDI serial chip connected to UART0 on the board.
 
-        if len(known_devices) == 0:
-            raise RuntimeError("No 'ftdi-cbus' device found")
+    WARNING: This tool cannot be used with all the boards. Please
+    refer to the board documentation to check whether this tool
+    can be used.
 
-        if len(known_devices) > 1:
-            raise RuntimeError("Several 'ftdi-cbus' device found")
+    To use this board, you need to connect to the port labeled as
+    UART0 on the Genio or Pumpkin boards. It is usually a micro-USB port.
 
-        return known_devices[0]
+    Example Usage
+    -------------
 
-    def _set_gpio(self, gpio, value):
-        try:
-            gpio.set_value(value)
-        except PermissionError:
-            self.logger.error("FTDI chip not configured")
+    `aiot-board list`
+        shows the SERIAL of all the connected FTDI chips
 
-    def reset(self):
-        self.reset_gpio.set_value(BoardControl.GPIO_HIGH)
-        self.reset_gpio.set_value(BoardControl.GPIO_LOW)
+    `aiot-board -s SERIAL program-ftdi`
+        must be called at least once to properly program the FTDI chip of the Genio/Pumpkin
+        board to use the "reset", "download" and "power" commands.
 
-    def download_mode_boot(self):
-        self.dl_gpio.set_value(BoardControl.GPIO_HIGH)
-        self.reset()
-        self.dl_gpio.set_value(BoardControl.GPIO_LOW)
+        On some boards, you might have to change the GPIO configurations ("--gpio-reset" and others) according to board design.
+        If there is only one FTDI chip connected, the "-s SERIAL" option could be omitted.
 
-    def power(self):
-        self.pwr_gpio.set_value(BoardControl.GPIO_HIGH)
-        time.sleep(1)
-        self.pwr_gpio.set_value(BoardControl.GPIO_LOW)
+    `aiot-board -s SERIAL program-ftdi --ftdi-serial NEW_SERIAL`
+        can be used to update the SERIAL of a given FTDI chip.
 
+    `aiot-board -s SERIAL reset`
+        would hard reset the Genio or Pumpkin board
 
+    `aiot-board -s SERIAL download`
+        would hard reset the Genio or Pumpkin board and put it into download mode, for subsequent
+        image flashing process.
 
-app_description = """
-    AIoT board control
+    If there is only one FTDI chip connected, the "-s SERIAL" option could be omitted.
+"""
 
-    This tool is used to control MediaTek boards.
+def do_board_command(args):
+    board = aiot.BoardControl(args.gpio_reset, args.gpio_download,
+                              args.gpio_power, args.gpio_chip,
+                              serial = args.serial)
 
-    WARNING: This tool cannot be used with all the boards. Please
-    refer to the board documentation to check whether this tool
-    can be used.
-"""
+    if args.command == 'reset':
+        board.reset()
+    elif args.command == 'download':
+        board.download_mode_boot()
+    elif args.command == 'power':
+        board.power()
 
 def main():
     app = aiot.App(description=app_description)
     parser = app.parser
     logger = app.logger
 
-    parser.add_argument('command', type=str,
-        choices=['reset', 'download', 'power', 'program-ftdi'])
-    parser.add_argument('-c', '--gpio-chip', type=int, help='GPIOChip device')
-    parser.add_argument('-r', '--gpio-reset', type=int, default=1,
-        help='GPIO to use to reset the SoC')
-    parser.add_argument('-d', '--gpio-download', type=int, default=2,
-        help='GPIO to use to put the SoC in download mode (KPCOL0 pin)')
-    parser.add_argument('-p', '--gpio-power', type=int, default=0,
-        help='GPIO to use to power on the SoC')
-    parser.add_argument('--ftdi-product-name', type=str, default='undefined')
+    if platform.system() == 'Windows':
+        parser.add_argument('-s', '--serial',
+                            type=str,
+                            default=None,
+                            help="Specify which board to connect to using FTDI serial. You can get serial with 'aiot-board list'")
+
+    #parser.add_argument('command', type=str,
+    #    choices=['reset', 'download', 'power', 'program-ftdi', 'list'],
+    #    help=)
+    subparsers = parser.add_subparsers(
+        dest = 'command',
+    )
+
+    list_parser = subparsers.add_parser('list',
+                                        help = "List the serial number in EEPROM of all connected FTDI chips."
+    )
+
+    ftdi_parser = subparsers.add_parser('program-ftdi',
+                                        help = "Program the FTDI EEPROM, such as serial, product name, and configure the CBUS(GPIO) settings used by reset, download, and power commands."
+    )
+    ftdi_parser.add_argument('--ftdi-product-name', type=str, default='undefined', help="Currently no effect.")
+    ftdi_parser.add_argument('--ftdi-serial', '--set-serial', type=str, default=None, help="Update the serial number in eeprom.")
+
+    board_parsers = [
+        ftdi_parser,
+        subparsers.add_parser('reset', help = "Reset the board"),
+        subparsers.add_parser('download', help = "Reset and put the board into download mode"),
+        subparsers.add_parser('power', help="Power on the board"),
+    ]
+
+    for b in board_parsers:
+        b.add_argument('-c', '--gpio-chip', type=int, help='GPIOChip device')
+        b.add_argument('-r', '--gpio-reset', type=int, default=1,
+            help='GPIO to use to reset the SoC')
+        b.add_argument('-d', '--gpio-download', type=int, default=2,
+            help='GPIO to use to put the SoC in download mode (KPCOL0 pin)')
+        b.add_argument('-p', '--gpio-power', type=int, default=0,
+            help='GPIO to use to power on the SoC')
+        b.set_defaults(func=do_board_command)
 
     args = app.execute()
 
-    if args.command == 'program-ftdi':
-        ftdi = aiot.FtdiControl()
-        try:
+    if not args.command:
+        logger.error("No command(list/program-ftdi/reset/download) speficied.")
+        parser.print_usage()
+        sys.exit(-1)
+    
+    try:
+        if args.command == 'list':
+            ftdi = aiot.FtdiControl(args.serial)
+            ftdi.print_device_list()
+        elif args.command == 'program-ftdi':
+            ftdi = aiot.FtdiControl(args.serial)
             ftdi.program(args.ftdi_product_name, args.gpio_reset,
-                         args.gpio_download, args.gpio_power)
-        except Exception as e:
-            logger.error(e)
-            sys.exit(-1)
+                         args.gpio_download, args.gpio_power,
+                         new_serial = args.ftdi_serial)
+        else:
+            args.func(args)
         sys.exit(0)
+    except Exception as e:
+        logger.error(e, exc_info = args.verbose)
+        sys.exit(-1)
 
-    board = aiot.BoardControl(args.gpio_reset, args.gpio_download,
-                              args.gpio_power, args.gpio_chip)
-
-    if args.command == 'reset':
-        board.reset()
-    elif args.command == 'download':
-        board.download_mode_boot()
-    elif args.command == 'power':
-        board.power()
+if __name__ == '__main__':
+    main()
```

## aiot/flash.py

```diff
@@ -130,33 +130,51 @@
             type = lambda num: int(num, 0),
             help = 'Size of the U-Boot environment storage. Default to 4096 bytes.')
         group.add_argument('--uboot-env-redund-offset', 
             default = -1,
             type = lambda num: int(num, 0),
             help = 'Enable U-Boot redundant env generation and assign offset of the redundant data. No redundant env by default.')
 
+    def add_firmware_group(self, parser):
+        group = parser.add_argument_group('Firmware')
+        group.add_argument('--serialno', type=str, \
+            help="Customize serial number used in adb and fastboot, e.g. the result of 'adb devices'\n"
+                 "This is not the serial used by 'aiot-board -s' and 'aiot-flash -s',"
+                 "which is FTDI serial connected to UART0.")
+
     def setup_parser(self):
         self.parser.add_argument('targets', type=str, nargs='*',
             help='Name of the partition or group of partition to flash')
         self.parser.add_argument('--dry-run', action="store_true")
 
         # Bootstrap
         add_bootstrap_group(self.parser)
 
+        self.add_firmware_group(self.parser)
         self.add_uboot_group(self.parser)
 
         if platform.system() == 'Linux':
             group = self.parser.add_argument_group('Board Control (using libgpiod)')
             group.add_argument('-c', '--gpio-chip', type=int, help='GPIOChip device')
             group.add_argument('-r', '--gpio-reset', type=int, default=1,
                 help='GPIO to use to reset the SoC')
             group.add_argument('-d', '--gpio-download', type=int, default=2,
                 help='GPIO to use to put the SoC in download mode (KPCOL0 pin)')
             group.add_argument('-p', '--gpio-power', type=int, default=0,
                 help='GPIO to use to power on the SoC')
+        
+        if platform.system() == 'Windows':
+            group = self.parser.add_argument_group('Board Control (using ftd2xx driver)')
+            group.add_argument('-c', '--ftdi-serial', '-s', type=str, default=None, help='Serial number of the board control COM port. This should be the serial reported by "aiot-board list".')
+            group.add_argument('-r', '--gpio-reset', type=int, default=1,
+                help='GPIO to use to reset the SoC')
+            group.add_argument('-d', '--gpio-download', type=int, default=2,
+                help='GPIO to use to put the SoC in download mode (KPCOL0 pin)')
+            group.add_argument('-p', '--gpio-power', type=int, default=0,
+                help='GPIO to use to power on the SoC')
 
         for name, image in images.items():
             image.define_local_parser(self.parser)
 
         for name, image in images.items():
             image_group = self.parser.add_argument_group(name)
             image.setup_parser(image_group)
@@ -179,21 +197,38 @@
 
         print(image)
 
         flasher = aiot.Flash(image, dry_run=args.dry_run)
         if not flasher.check(args.targets):
             return
 
-        if not args.dry_run and platform.system() == 'Linux':
+        if not args.dry_run:
             try:
-                board = aiot.BoardControl(args.gpio_reset, args.gpio_download,
-                                          args.gpio_power, args.gpio_chip)
+                self.logger.info("Try to automatically reset the board into DOWNLOAD mode...")
+                if platform.system() == 'Linux':
+                    board = aiot.BoardControl(args.gpio_reset, args.gpio_download,
+                                            args.gpio_power, args.gpio_chip,
+                                            serial = None)
+                elif platform.system() == 'Windows':
+                    board = aiot.BoardControl(args.gpio_reset, args.gpio_download,
+                                            args.gpio_power, None,
+                                            serial = args.ftdi_serial)
                 board.download_mode_boot()
+            except RuntimeError as r:
+                self.logger.warning(r)
+                self.logger.warning("Unable to find and reset the board. Possible causes are:\n"
+                                    "1. This is not a Genio 350/700 EVK, nor a Pumpkin board.\n"
+                                    "2. The board port UART0 is not connected.\n"
+                                    "3. The UART0 port is being opened by another tool, such as TeraTerm on Windows.\n"
+                                    "You can now manually reset the board into DOWNLOAD mode.\n")
+                self.logger.info("Continue flashing...")
             except Exception as e:
                 self.logger.warning(str(e))
+                self.logger.warning("Board control failed. You could try manually put the board in DOWNLOAD mode.")
+                self.logger.info("Continue flashing...")
 
         if not args.skip_bootstrap and not args.dry_run:
             run_bootrom(args)
 
         flasher.flash(args.targets)
 
 def main():
```

## aiot/version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '1.4a0'
-__version_tuple__ = version_tuple = (1, 4)
+__version__ = version = '1.4a1.dev9'
+__version_tuple__ = version_tuple = (1, 4, 'dev9')
```

## aiot/image/android.py

```diff
@@ -58,17 +58,14 @@
         return p.exists()
 
     @classmethod
     def setup_parser(cls, parser):
         parser.add_argument('--dtbo-index', type=str, \
             help='Enable one or multiple DTBO(s)')
 
-        parser.add_argument('--serialno', type=str, \
-            help='Customize serial number used by adb/fastboot')
-
     @classmethod
     def define_local_parser(cls, parser):
         cls.parser = argparse.ArgumentParser(parents = [parser], add_help=False)
 
     @classmethod
     def setup_local_parser(cls):
         cls.setup_parser(cls.parser)
```

## aiot/image/yocto.py

```diff
@@ -135,14 +135,18 @@
                     self.partitions[partition] = f"{name}-{machine}.wic.img"
                 elif partition == "modules":
                     self.partitions[partition] = f"modules-{machine}.modimg.ext4"
 
     def generate_uboot_env(self):
         env = aiot.UBootEnv(self.args.uboot_env_size,
                             f"{self.path}/u-boot-initial-env")
+
+        if self.args.serialno:
+            env.add("serial#", self.args.serialno)
+
         if len(self.kernel_dtbo_autoload) > 0:
             boot_conf = f"#conf-{self.kernel_dtb.replace('/', '_')}"
             list_dtbo = ""
             for dtbo in self.kernel_dtbo_autoload:
                 boot_conf += f"#conf-{dtbo}"
                 list_dtbo += f"{dtbo} "
             env.update('boot_conf', boot_conf)
```

## Comparing `genio_tools-1.4a0.dist-info/LICENSE` & `genio_tools-1.4a1.dev9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genio_tools-1.4a0.dist-info/METADATA` & `genio_tools-1.4a1.dev9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genio-tools
-Version: 1.4a0
+Version: 1.4a1.dev9
 Summary: Tools for flashing boards using MediaTek Genio SoCs
 Home-page: https://gitlab.com/mediatek/aiot/bsp/genio-tools
 Author: Fabien Parent
 Maintainer: Pablo Sun
 Maintainer-email: pablo.sun@mediatek.com
 License: UNKNOWN
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Requires-Dist: genio-bootrom
 Requires-Dist: gpiod (==1.4.0)
 Requires-Dist: oyaml
 Requires-Dist: packaging
 Requires-Dist: pyftdi
 Requires-Dist: pyusb
 Requires-Dist: pyudev ; platform_system == "Linux"
+Requires-Dist: ftd2xx ; platform_system == "Windows"
 
 # Genio tools
 
 The Genio tools are a set of tools to flash, control or configure MediaTek
 boards, and in particular the Genio evaluation kits.
```

## Comparing `genio_tools-1.4a0.dist-info/RECORD` & `genio_tools-1.4a1.dev9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-aiot/__init__.py,sha256=SiKepCTWSVEH0YwGGNCeYCow7yrHw23_VX8YwfX_zCA,428
+aiot/__init__.py,sha256=UFjWAjLTr4XsKz4rh3EylTU4CK7yjT310VB_HOvslnk,570
 aiot/app.py,sha256=MrZGCFauA1rkV5UEhCts64Mv7UUUMKz2jRu2R6Fy9mI,1088
-aiot/board.py,sha256=M8uNLHA4AIQc5ac4o6rz2bBMxd-a1p1WP9ZajDFkm-w,3640
+aiot/board.py,sha256=xUQIEZsk0ee_CtYrgXtNkztjKwjbva-bBEFV0g66qMU,4953
+aiot/boardcontrol_linux.py,sha256=aP0EvUYsBioMWmQs9zPVeKIXfE0Nf6zDFZd3Zu8Yhhg,1973
+aiot/boardcontrol_win.py,sha256=akXb0cvwsvR8zl45RP3Bv_9uNdZHCzHoe6TQGBuSwHI,2472
 aiot/bootrom.py,sha256=CN6fpFU9mL6RbPRqGxAJTYVc81pZH5wxHCgbsPXyPOA,2460
 aiot/config.py,sha256=7QyWsCFN8H282l0Rbxn1agBNNXZasfRV2vW3DCmHCFY,3402
 aiot/efuse.py,sha256=fVTc6gCe8ByDYjE-lmWDTg8fmV2La69PEqULi1PSidk,4040
 aiot/fastboot.py,sha256=G_e0SB7-hU5oHRbrsDtwhF83p9-X9Afpf2Y91-T-0MI,1306
-aiot/flash.py,sha256=iv0p3B1qL9Zb8euwpVeI960Gp49tvZdgy5D_fxPo0Qg,6682
+aiot/flash.py,sha256=WH_Xjdj-fi7MmDYq54Knf-YGyyx2bbBRjME2LSbktCk,9131
 aiot/ftdi.py,sha256=WqkGyZYztZ93mB_O7vDiPvoMnjwty5bTecUGi4Kg8so,1377
+aiot/ftdi_win.py,sha256=cpyK0VkxOWqU0tPqWilEGFKdF7ZOOELRRS69MeYc0iE,3861
 aiot/rpmb.py,sha256=PGpqRwvVALaTq0bHA6VcQaF5Br_zn20uaWKt-imHO80,800
 aiot/ubootenv.py,sha256=9nYAkA5RfMaJlwPjKGJhkDG48CSk65uZj3EzJtMffpg,2665
-aiot/version.py,sha256=rVDPvsMhoNFGSppQg4eidxKW63gvUKDejUqUD4ODFqQ,157
+aiot/version.py,sha256=fpKqDEuTE5f-utqYttuT5EjqSIgAs-fGM4aSiJJEPAo,170
 aiot/image/__init__.py,sha256=jb2-bE8l44Ml6qQk16XnvoDcjaivODUd-LjUD_Ksp-U,126
-aiot/image/android.py,sha256=dNyvGsBQFJPeaZ_2LXSWrcuAazirs4QqD0j5yMYRHlc,2526
+aiot/image/android.py,sha256=_8_ntf6EwIB3ttSDlLgLDo_48ixlehTMkQIOtilR3lM,2406
 aiot/image/ubuntu.py,sha256=jYyrpa1L4hOv6kOz1SGGvnqgoyRhsHbE8hBRcYkT0S8,6736
-aiot/image/yocto.py,sha256=qP3iqSVfES5B5IWw2dVnkAuNA6XLLLmF240rLc3xHHw,9043
-genio_tools-1.4a0.dist-info/LICENSE,sha256=5_0VvMgYcuw5GLW1PUKNoExF_dlOfU0HjC2qbk0Z-vM,1091
-genio_tools-1.4a0.dist-info/METADATA,sha256=kQOpC82ewHS18mRdKSZuXiD1ipRwXvjtgxDQpgmr3b4,873
-genio_tools-1.4a0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genio_tools-1.4a0.dist-info/entry_points.txt,sha256=Io_q9lqIMOoRXd5vn1p4OAvYWzL7AqP_DbFJDAMsSUY,334
-genio_tools-1.4a0.dist-info/top_level.txt,sha256=SO4EJaYCTPaFdWDC4m9vjRKVX5YBQ1ofUr85dMEXMU4,5
-genio_tools-1.4a0.dist-info/RECORD,,
+aiot/image/yocto.py,sha256=NPg67AjJcid5-XqutMUzT4N8qcDqqiQ9t0TxknA2Nc8,9127
+genio_tools-1.4a1.dev9.dist-info/LICENSE,sha256=5_0VvMgYcuw5GLW1PUKNoExF_dlOfU0HjC2qbk0Z-vM,1091
+genio_tools-1.4a1.dev9.dist-info/METADATA,sha256=M-gORDtxaAd0fh1pKah1dfXN5qGCE8AfJHd2TOEVJYw,931
+genio_tools-1.4a1.dev9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genio_tools-1.4a1.dev9.dist-info/entry_points.txt,sha256=Io_q9lqIMOoRXd5vn1p4OAvYWzL7AqP_DbFJDAMsSUY,334
+genio_tools-1.4a1.dev9.dist-info/top_level.txt,sha256=SO4EJaYCTPaFdWDC4m9vjRKVX5YBQ1ofUr85dMEXMU4,5
+genio_tools-1.4a1.dev9.dist-info/RECORD,,
```

