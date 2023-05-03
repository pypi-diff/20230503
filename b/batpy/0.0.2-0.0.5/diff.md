# Comparing `tmp/batpy-0.0.2.tar.gz` & `tmp/batpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.0.2.tar", max compression
+gzip compressed data, was "batpy-0.0.5.tar", max compression
```

## Comparing `batpy-0.0.2.tar` & `batpy-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rwxr-xr-x   0        0        0     1074 2023-04-28 10:44:09.848817 batpy-0.0.2/LICENSE
--rw-r--r--   0        0        0     2932 2023-05-02 16:29:54.199754 batpy-0.0.2/README.md
--rw-r--r--   0        0        0      942 2023-05-02 16:35:26.635219 batpy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4843 2023-05-02 16:29:54.202083 batpy-0.0.2/src/batpy/BatPaC_battery.py
--rw-r--r--   0        0        0    26286 2023-05-02 16:29:54.202372 batpy-0.0.2/src/batpy/BatPaC_tool.py
--rw-r--r--   0        0        0      107 2023-04-28 10:44:09.864319 batpy-0.0.2/src/batpy/__init__.py
--rw-r--r--   0        0        0     2013 2023-05-02 16:29:54.202662 batpy-0.0.2/src/batpy/is_version_compatible.py
--rw-r--r--   0        0        0     3721 1970-01-01 00:00:00.000000 batpy-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-03 15:32:02.682992 batpy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3840 2023-05-03 15:32:02.682992 batpy-0.0.5/README.md
+-rw-r--r--   0        0        0     1825 2023-05-03 15:32:37.207071 batpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0    27747 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0     2158 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30586 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    83193 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48369 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2177 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/is_version_compatible.py
+-rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 batpy-0.0.5/PKG-INFO
```

### Comparing `batpy-0.0.2/LICENSE` & `batpy-0.0.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `batpy-0.0.2/src/batpy/BatPaC_tool.py` & `batpy-0.0.5/src/batpy/batpac_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # -*- coding: UTF-8 -*-
-import xlwings as xw
+"""Module, which includes the class BatpacTool
+"""
+import logging
+import warnings
+from pathlib import Path
+
+import semantic_version
 import toml
+import xlwings as xw
 from prettytable import PrettyTable
-from pathlib import Path
 from tqdm import tqdm
-import logging
-import semantic_version
-from batpy.BatPaC_battery import BatPaC_battery
+
+from batpy.batpac_battery import BatpacBattery
 from batpy.is_version_compatible import is_version_compatible
-import warnings
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
-    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t%(lineno)s\t- %(message)s",
+    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t\
+        %(lineno)s\t- %(message)s",
     filename="batpy.log",
     filemode="w",
     level=logging.INFO,
 )
 
 
-class BatPaC_tool:
+class BatpacTool:
     """BatPaC class which interacts with the BatPaC Excel tool
 
-    This BatPaC class is used to interact directly with the BatPaC Excel tool and can store individual batteries (class BatPaC_battery)
-    and additional parameters of the BatPaC Excel tool in the dictionary properties.
+    This BatPaC class is used to interact directly with the BatPaC Excel tool
+    and can store individual batteries (class BatPaC_battery) and additional
+    parameters of the BatPaC Excel tool in the dictionary properties.
     """
 
     def __init__(
         self,
         batpac_workbook_path: Path,
         cell_definition_user_input_toml_path: Path,
         cell_definition_calculation_and_validation_results: Path = None,
@@ -40,175 +46,213 @@
         Initialize the BatPaC object.
 
         Parameters
         ----------
         batpac_workbook_path : Path
             Path to the BatPaC Excel tool (*.xlsm).
         cell_definition_user_input_toml_path : Path
-            Path to the TOML file, which contains the configuration for the standard user input cells (defined by Argonne National Laboratory)
+            Path to the TOML file, which contains the configuration for the
+            standard user input cells (defined by Argonne National Laboratory)
             in the BatPaC Excel tool.
         cell_definition_calculation_and_validation_results : Path, optional
-            Path to the TOML file, which contains the configuration for the calculation and validation results
+            Path to the TOML file, which contains the configuration for the
+            calculation and validation results
             in the BatPaC Excel tool, by default None.
         cell_definition_additional_user_input_toml_path : Path, optional
-            Path to the TOML file, which contains additional cells for user input, that are not included in the standard user inputs
-            in the BatPaC Excel tool, by default None.
+            Path to the TOML file, which contains additional cells for user
+            input, that are not included in the standard user inputs in the
+            BatPaC Excel tool, by default None.
         cell_definition_additional_user_results_toml_path : Path, optional
-            Path to the TOML file, which contains additional cells for  user input, that are not included in the standard user inputs
-            in the BatPaC Excel tool, by default None.
+            Path to the TOML file, which contains additional cells for  user
+            input, that are not included in the standard user inputs in the
+            BatPaC Excel tool, by default None.
         excel_visible : bool, optional
-            True, if Excel should be visible during operation, by default False.
+            True, if Excel should be visible during operation, by default
+            False.
         """
         logging.info(
-            f"[ ] Create BatPaC from {batpac_workbook_path} and load cell references from {cell_definition_user_input_toml_path}"
+            "[ ] Create BatPaC from %s and load cell references from %s",
+            batpac_workbook_path,
+            cell_definition_user_input_toml_path,
         )
         self.version = semantic_version.Version("0.1.0")
         self.workbook_path = batpac_workbook_path
         self.toml_path = cell_definition_user_input_toml_path
         self.toml_calculation_validation_results_path = (
             cell_definition_calculation_and_validation_results
         )
         config = toml.load(self.toml_path)
         config_metadata = config.pop("batpy")
         self.batpac_version = config_metadata["BatPaC version"]
         if is_version_compatible(
-            self.version, semantic_version.Version(config_metadata["BatPaC SemVer"])
+            self.version,
+            semantic_version.Version(config_metadata["BatPaC SemVer"]),
         ):
             self.batpac_semver = semantic_version.Version(
                 config_metadata["BatPaC SemVer"]
             )
 
         self.excel_cells = config
-        self.batteries = list()
+        self.batteries = []
         self.wb = xw.Book(batpac_workbook_path)
         self.app = self.wb.app
         self.app.visible = excel_visible
         self.max_batteries = 7
         self.properties = {}
         logging.info(
-            f"[+] Created BatPaC version {self.batpac_version} (SemVer: {self.batpac_semver}) from {self.workbook_path} and load cell references from {self.toml_path}"
+            "[+] Created BatPaC version %s (SemVer: %s) from %s and load \
+                    cell references from %s",
+            self.batpac_version,
+            self.batpac_semver,
+            self.workbook_path,
+            self.toml_path,
         )
 
     def __del__(self) -> None:
         """Destructor of BatPac object
 
-        Set the Excel calculation method to "automatic" and the "screen_updating" to True after object destruction.
+        Set the Excel calculation method to "automatic" and the
+        "screen_updating" to True after object destruction.
         """
         try:
             self.wb.app.calculation = "automatic"
             self.wb.app.screen_updating = True
-        except:
-            pass
+        except BaseException as error:
+            logging.error("An exception occurred: %s", error)
 
     def is_version_compatible(
-        self, version_to_check: semantic_version.Version, include_minor: bool = False
+        self,
+        version_to_check: semantic_version.Version,
+        include_minor: bool = False,
     ) -> bool:
         """Check for version compatibility
 
-        Check if two versions (major.minor.patch) are compatible. Thereby a version is compatible if major is equal.
-        If minor should also be included a version is compatible if major is equal and minor is greater or equal.
+        Check if two versions (major.minor.patch) are compatible. Thereby a
+        version is compatible if major is equal. If minor should also be
+        included a version is compatible if major is equal and minor is greater
+        or equal.
 
         Parameters
         ----------
         version_to_check : semantic_version.Version
             Version to be checked against self.version.
         include_minor : bool, optional
-            Check if minor version of version_to_check is greater or equal to self.version's minor, by default False.
+            Check if minor version of version_to_check is greater or equal to
+            self.version's minor, by default False.
 
         Returns
         -------
         bool
             True, if version is compatible.
 
         Raises
         ------
         ValueError
             If version is not compatible a ValueError will occur.
         """
-        return is_version_compatible(self.version, version_to_check, include_minor)
+        return is_version_compatible(
+            self.version, version_to_check, include_minor
+        )
 
     def load_batpac_file(self, path_to_batpac_file: Path) -> None:
         """Load BatPaC configuration
 
-        Load the properties for the BatPaC object from a TOML battery configuration file.
+        Load the properties for the BatPaC object from a TOML battery
+        configuration file.
 
         Parameters
         ----------
         path_to_batpac_file : Path
             Path to the TOML BatPaC configuration file.
         """
-        logging.info(f"[ ] Load BatPaC file from {path_to_batpac_file}")
+        logging.info("[ ] Load BatPaC file from %s", path_to_batpac_file)
         self.properties = toml.load(path_to_batpac_file)
-        logging.info(f"[+] Loaded BatPaC file from {path_to_batpac_file}")
-        logging.debug(f"[ ] BatPaC properties {self.properties}")
+        logging.info("[+] Loaded BatPaC file from %s", path_to_batpac_file)
+        logging.debug("[ ] BatPaC properties %s", self.properties)
 
-    def add_battery(self, batteries: list[BatPaC_battery]) -> None:
+    def add_battery(self, batteries: list[BatpacBattery]) -> None:
         """Add battery object to BatPaC object
 
         Add multiple battery objects to the BatPaC object.
 
         Parameters
         ----------
         batteries : list[BatPaC_battery]
             List of BatPaC_battery objects to include in the BatPaC object.
         """
         for battery in batteries:
             if len(self.batteries) + 1 <= self.max_batteries:
                 self.batteries.append(battery)
             else:
                 print(
-                    f"Battery {battery.name} ({battery}) exceeds the limit of batteries for a single workbook"
+                    f"Battery {battery.name} ({battery}) exceeds the limit of \
+                        batteries for a single workbook"
                 )
                 logging.warning(
-                    f"[!] Battery {battery.name} ({battery}) exceeds the limit of batteries for a single workbook"
+                    "[!] Battery %s (%s) exceeds the limit of batteries for a \
+                        single workbook",
+                    battery.name,
+                    battery,
                 )
 
     def set_new_property(self, sheet: str, name: str, value: any) -> None:
         """Set a new property of the battery
 
-        Set an existing property of the BatPaC tool or create a new one in the format {"sheet" : {"name" : value} }.
+        Set an existing property of the BatPaC tool or create a new one in the
+        format {"sheet" : {"name" : value} }.
 
         Parameters
         ----------
         sheet : str
             Name of the BatPaC Excel sheet.
         name : str
             Name of the BatPaC Excel cell description.
         value : any
             Value of the BatPaC Excel cell.
         """
         try:
             self.properties[sheet][name] = value
-        except:
+        except KeyError:
             self.properties.update({sheet: {name: value}})
 
     def load_batteries_file(
-        self, path_to_batteries_file: Path, batteries: list[BatPaC_battery]
+        self, path_to_batteries_file: Path, batteries: list[BatpacBattery]
     ) -> None:
         """Load batteries configuration
 
-        Load the configuration for the batteries from TOML configuration file and add these batteries to the BatPaC object.
-        Beware: This will clear all previous assigned batteries of the BatPaC object!
+        Load the configuration for the batteries from TOML configuration file
+        and add these batteries to the BatPaC object.
+        Beware: This will clear all previous assigned batteries of the BatPaC
+        object!
 
         Parameters
         ----------
         path_to_batteries_file : Path
             Path to the TOML batteries configuration file.
         batteries : list[BatPaC_battery]
-            List of BatPaC_battery objects to load battery properties from file and add to BatPaC object.
+            List of BatPaC_battery objects to load battery properties from file
+            and add to BatPaC object.
         """
-        logging.info(f"[ ] Load batteries from file {path_to_batteries_file}")
+        logging.info("[ ] Load batteries from file %s", path_to_batteries_file)
         self.batteries.clear()
         self.add_battery(batteries)
         for battery in self.batteries:
             battery.load_battery_file(path_to_batteries_file, battery.name)
-            logging.debug(f"[ ] Battery {battery.name} properties {battery.properties}")
-        logging.info(f"[+] Batteries from file {path_to_batteries_file} loaded")
+            logging.debug(
+                "[ ] Battery %s properties %s",
+                battery.name,
+                battery.properties,
+            )
+        logging.info(
+            "[+] Batteries from file %s loaded", path_to_batteries_file
+        )
 
-    def write_value_direct(self, worksheet: str, range: str, value: any) -> None:
+    def write_value_direct(
+        self, worksheet: str, range: str, value: any
+    ) -> None:
         """Write value in BatPaC Excel tool
 
         Write a value directly in the BatPaC Excel tool.
 
         Parameters
         ----------
         worksheet : str
@@ -236,54 +280,59 @@
         -------
         any
             Value of the BatPaC Excel tool cell.
 
         Raises
         ------
         KeyError
-            Raises KeyError if the specified worksheet or range could not be found.
+            Raises KeyError if the specified worksheet or range could not be
+            found.
         """
         try:
             value = self.wb.sheets[worksheet][range].value
             return value
-        except:
-            logging.warning(f"[!] Key {worksheet} , {range} not found")
+        except BaseException as error:
+            logging.error("An exception occurred: %s", error)
+            logging.warning("[!] Key %s , %s not found", worksheet, range)
             raise KeyError
 
     def wb_helper_range(
         self,
         worksheet: str,
         name: str,
-        battery: BatPaC_battery = None,
+        battery: BatpacBattery = None,
         additional_cell_config: Path | dict = None,
     ) -> str:
         """Helper function for workbook range
 
         Function to find the cell range of a specified cell description.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery, optional
-            BatPaC_battery object, if the returned cell is battery specific, by default None.
+            BatPaC_battery object, if the returned cell is battery specific, by
+            default None.
         additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell configuration to consider, by default None.
+            Path to TOML file or dictionary, which contains additional cell
+            configuration to consider, by default None.
 
         Returns
         -------
         str
             Excel cell range.
 
         Raises
         ------
         KeyError
-            Raises KeyError, if worksheet name or cell description could not be found.
+            Raises KeyError, if worksheet name or cell description could not be
+            found.
         """
         try:
             if additional_cell_config is not None:
                 if type(additional_cell_config) is Path:
                     additional_cell_config = toml.load(additional_cell_config)
                 range_dict = additional_cell_config
             else:
@@ -292,16 +341,17 @@
             if battery is None:
                 range = range_dict[worksheet][name]
             else:
                 range = range_dict[worksheet][
                     "Battery " + str(self.batteries.index(battery) + 1)
                 ][name]
             return range
-        except:
-            logging.warning(f"[!] Key {worksheet} , {name} not found")
+        except BaseException as error:
+            logging.error("An exception occurred: %s", error)
+            logging.warning("[!] Key %s , %s not found", worksheet, name)
             raise KeyError
 
     def write_value(self, worksheet: str, name: str, value: any) -> None:
         """Write value in BatPaC Excel tool
 
         Write value in BatPaC Excel tool without input the exact cell range.
 
@@ -310,34 +360,44 @@
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         value : any
             Value to write in the BatPaC Excel tool.
         """
-        self.write_value_direct(worksheet, self.wb_helper_range(worksheet, name), value)
+        self.write_value_direct(
+            worksheet, self.wb_helper_range(worksheet, name), value
+        )
         logging.debug(
-            f"[ ] Write in {worksheet} {self.wb_helper_range(worksheet, name)} ({name}) = {value}"
+            "[ ] Write in %s %s (%s) = %s",
+            worksheet,
+            self.wb_helper_range(worksheet, name),
+            name,
+            value,
         )
 
     def read_value(
-        self, worksheet: str, name: str, additional_cell_config: Path | dict = None
+        self,
+        worksheet: str,
+        name: str,
+        additional_cell_config: Path | dict = None,
     ) -> any:
         """Read value from BatPaC Excel tool
 
         Read value from BatPaC Excel tool without input the exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell configuration to consider, by default None.
+            Path to TOML file or dictionary, which contains additional cell
+            configuration to consider, by default None.
 
         Returns
         -------
         any
             Value of the BatPaC Excel tool cell.
         """
         return self.read_value_direct(
@@ -350,65 +410,77 @@
             ),
         )
 
     def read_value_battery(
         self,
         worksheet: str,
         name: str,
-        battery: BatPaC_battery,
+        battery: BatpacBattery,
         additional_cell_config: Path | dict = None,
     ) -> any:
         """Read battery specific value from BatPaC Excel tool
 
-        Read battery specific value from BatPaC Excel tool without input the exact cell range.
+        Read battery specific value from BatPaC Excel tool without input the
+        exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery
-            BatPaC_battery object, if the returned cell is battery specific, by default None.
+            BatPaC_battery object, if the returned cell is battery specific, by
+            default None.
         additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell configuration to consider, by default None.
+            Path to TOML file or dictionary, which contains additional cell
+            configuration to consider, by default None.
 
         Returns
         -------
         any
             Value of the BatPaC Excel tool cell.
         """
         return self.read_value_direct(
             worksheet,
-            self.wb_helper_range(worksheet, name, battery, additional_cell_config),
+            self.wb_helper_range(
+                worksheet, name, battery, additional_cell_config
+            ),
         )
 
     def write_value_battery(
-        self, worksheet: str, name: str, battery: BatPaC_battery, value: any
+        self, worksheet: str, name: str, battery: BatpacBattery, value: any
     ) -> None:
         """Write specific battery value in BatPaC Excel tool
 
-        Write a speicif battery value in the BatPaC Excel tool without input the exact cell range.
+        Write a speicif battery value in the BatPaC Excel tool without input
+        the exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery
-            BatPaC_battery object, if the returned cell is battery specific, by default None.
+            BatPaC_battery object, if the returned cell is battery specific,
+            by default None.
         value : any
             Value to write in the BatPaC Excel tool.
         """
         self.write_value_direct(
             worksheet, self.wb_helper_range(worksheet, name, battery), value
         )
         logging.debug(
-            f"[ ] Write for {battery.name} in {worksheet} {self.wb_helper_range(worksheet, name, battery)} ({name}) = {value}"
+            "[ ] Write for %s in %s %s (%s) = %s",
+            battery.name,
+            worksheet,
+            self.wb_helper_range(worksheet, name, battery),
+            name,
+            value,
         )
 
     def stop_automatic_calculation(self) -> None:
         """Stop automatic Excel calculation
         Stop the automatic Excel and BatPaC calculation.
         """
         self.write_value("Dashboard", "Restart (0/1)", 0)
@@ -420,62 +492,64 @@
         Start the automatic Excel and BatPaC calculation.
         """
         reset_macro = self.wb.macro("Module1.Reset")
         reset_macro()
         self.wb.app.calculation = "automatic"
         self.wb.app.screen_updating = True
 
-    def read_from_user_input(user_read_file: Path) -> dict:
+    def read_from_user_input(self, user_read_file: Path) -> dict:
         """Read user specified input from BatPaC Excel tool
 
-        Read additional cell values from BatPaC Excel tool specified by user input.
+        Read additional cell values from BatPaC Excel tool specified by user
+        input.
 
         Parameters
         ----------
         user_read_file : Path
-            Path to the TOML file containing additional cell ranges from which values are to be read.
+            Path to the TOML file containing additional cell ranges from which
+            values are to be read.
 
         Returns
         -------
         dict
             Dictionary in the format {"sheet" : {"name" : value} }
 
         Raises
         ------
         ValueError
             Raises ValueError, if the user input is not valid.
         """
         warnings.warn("This function is not implemented.")
         if user_read_file.is_file():
             return True
-        else:
-            logging.warning(f"[!] {user_read_file} is not a valid file")
-            raise ValueError(f"{user_read_file} is not a valid file")
+        logging.warning("[!] %s is not a valid file", user_read_file)
+        raise ValueError(f"{user_read_file} is not a valid file")
 
     def read_calculation_and_validation_results(
         self, toml_file_calculation_validation_results: Path = None
     ) -> dict | bool:
         """Read calculation and validation results
 
         Read the calculation and validation results from the BatPaC Excel tool.
 
         Parameters
         ----------
         toml_file_calculation_validation_results : Path, optional
-            Path to the TOML file containing the specified cell ranges of the calculation and validation results, by default None.
+            Path to the TOML file containing the specified cell ranges of the
+            calculation and validation results, by default None.
 
         Returns
         -------
         dict | bool
             Returns a dictionary if a TOML file is specified, otherwise False.
         """
         if toml_file_calculation_validation_results is None:
             if self.toml_calculation_validation_results_path is None:
                 logging.warning(
-                    f"[!] No toml file for calculation and validation found"
+                    "[!] No toml file for calculation and validation found"
                 )
                 return False
         else:
             self.toml_calculation_validation_results_path = (
                 toml_file_calculation_validation_results
             )
 
@@ -505,28 +579,34 @@
                     "Configuration Warnings (see table  to right)",
                     battery,
                     additional_cell_config,
                 )
             )
             plant_size.append(
                 self.read_value_battery(
-                    "Dashboard", "Plant Size, GWh", battery, additional_cell_config
+                    "Dashboard",
+                    "Plant Size, GWh",
+                    battery,
+                    additional_cell_config,
                 )
             )
             power_to_energy.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Power-to-energy ratio",
                     battery,
                     additional_cell_config,
                 )
             )
             adequacy_cooling.append(
                 self.read_value_battery(
-                    "Dashboard", "Adequacy of cooling", battery, additional_cell_config
+                    "Dashboard",
+                    "Adequacy of cooling",
+                    battery,
+                    additional_cell_config,
                 )
             )
             cathode_thickness.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Cathode thickness limited by",
                     battery,
@@ -559,15 +639,16 @@
         }
 
         return dict_table
 
     def calculate(self) -> None:
         """Calculate the batteries in the BatPaC Excel tool
 
-        Read all BatPaC_tool properties and its included [BatPaC_battery] properties, write these properties in the BatPaC Excel tool,
+        Read all BatPaC_tool properties and its included [BatPaC_battery]
+        properties, write these properties in the BatPaC Excel tool,
         and calculate the batteries in the BatPaC Excel tool.
         """
         logging.info("[ ] Start calculation")
         self.stop_automatic_calculation()
         for sheet in tqdm(
             self.properties, "Processing BatPaC configuration in each sheet"
         ):
@@ -576,18 +657,22 @@
                     self.write_value(sheet, key, value)
 
         sheets = set()
         for battery in self.batteries:
             sheets.update(battery.properties.keys())
 
         logging.debug(
-            f"[ ] Sheets type is {type(sheets)} and sheets available: {sheets}"
+            "[ ] Sheets type is %s and sheets available: %s",
+            type(sheets),
+            sheets,
         )
 
-        for sheet in tqdm(sheets, "Processing battery configuration in each sheet"):
+        for sheet in tqdm(
+            sheets, "Processing battery configuration in each sheet"
+        ):
             sheet_buffer = {}
             for i, battery in enumerate(self.batteries):
                 if sheet in battery.properties:
                     for key, value in battery.properties[sheet].items():
                         if key not in sheet_buffer:
                             sheet_buffer[key] = [None] * self.max_batteries
                         sheet_buffer[key][i] = value
@@ -596,97 +681,108 @@
 
         self.start_automatic_calculation()
         logging.info("[+] Finished calculation")
 
     def save(self, path: Path = None) -> None:
         """Save BatPaC Excel tool
 
-        Save the BatPaC Excel tool or save the BatPaC Excel tool in another path.
+        Save the BatPaC Excel tool or save the BatPaC Excel tool in another
+        path.
 
         Parameters
         ----------
         path : Path, optional
-            If the path is specified, the BatPaC Excel tool will be saved under the path, by default None will overwrite the current BatPaC Excel tool.
+            If the path is specified, the BatPaC Excel tool will be saved under
+            the path, by default None will overwrite the current BatPaC Excel
+            tool.
         """
         logging.info("[ ] Save workbook")
         if path is None:
             path = self.workbook_path
         self.wb.save(path)
         self.wb = xw.Book(path)
         self.app = self.wb.app
-        logging.info(f"[+] Saved workbook in {path}")
+        logging.info("[+] Saved workbook in %s", path)
 
     def close(self) -> bool:
         """Close BatPaC Excel tool
 
-        Close the BatPaC Excel tool if other workbooks are open, otherwise the Excel instance will be closed.
+        Close the BatPaC Excel tool if other workbooks are open, otherwise the
+        Excel instance will be closed.
 
         Returns
         -------
         bool
             True, if BatPaC Excel tool is closed.
         """
         if len(self.wb.app.books) == 1:
             self.wb.app.quit()
             logging.info("[+] Workbook and Excel closed")
             return True
-        else:
-            self.wb.close()
-            logging.info("[+] Workbook closed")
-            return True
+        self.wb.close()
+        logging.info("[+] Workbook closed")
+        return True
 
-    def save_config(self, batpac_path: Path = None, battery_path: Path = None) -> None:
+    def save_config(
+        self, batpac_path: Path = None, battery_path: Path = None
+    ) -> None:
         """Save BatPaC_tool configuration
 
-        Read all BatPaC_tool properties and its included [BatPaC_battery] properties from the BatPaC Excel tool, save these properties in the BatPaC_tool and
-        [BatPaC_battery] objects, and write them as TOML file.
+        Read all BatPaC_tool properties and its included [BatPaC_battery]
+        properties from the BatPaC Excel tool, save these properties in the
+        BatPaC_tool and [BatPaC_battery] objects, and write them as TOML file.
 
         Parameters
         ----------
         batpac_path : Path, optional
-            If specified, storage path to the TOML file for BatPaC_tool properties, by default None.
+            If specified, storage path to the TOML file for BatPaC_tool
+            properties, by default None.
         battery_path : Path, optional
-            If specified, storage path to the TOML file for [BatPaC_battery] properties, by default None.
+            If specified, storage path to the TOML file for [BatPaC_battery]
+            properties, by default None.
         """
         for sheet in self.excel_cells:
             for key, value in self.excel_cells[sheet].items():
-                if type(value) is dict:
+                if isinstance(value, dict):
                     battery_number = int(key.replace("Battery ", "")) - 1
                     for battery_key, battery_value_range in value.items():
                         self.batteries[battery_number].set_new_property(
                             sheet,
                             battery_key,
                             self.read_value_direct(sheet, battery_value_range),
                         )
                 else:
-                    self.set_new_property(sheet, key, self.read_value(sheet, key))
+                    self.set_new_property(
+                        sheet, key, self.read_value(sheet, key)
+                    )
 
         if batpac_path is not None:
             with open(batpac_path, "w") as toml_file:
                 for sheet in tqdm(
                     self.properties, "Saving BatPaC config from each sheet"
                 ):
                     toml_file.write(f'["{sheet}"]\n')
                     for key, value in self.properties[sheet].items():
                         if value is None or key == "Restart (0/1)":
                             toml_file.write("# ")
-                        if type(value) is str:
+                        if isinstance(value, str):
                             toml_file.write(f"'{key}' = '{value}'\n")
                         else:
                             toml_file.write(f"'{key}' = {value}\n")
                     toml_file.write("\n")
 
         if battery_path is not None:
             with open(battery_path, "w") as toml_file:
                 for battery in tqdm(
-                    self.batteries, "Saving battery configuration for each battery"
+                    self.batteries,
+                    "Saving battery configuration for each battery",
                 ):
                     for sheet in battery.properties:
                         toml_file.write(f'["{battery.name}"."{sheet}"]\n')
                         for key, value in battery.properties[sheet].items():
                             if value is None:
                                 toml_file.write("# ")
-                            if type(value) is str:
+                            if isinstance(value, str):
                                 toml_file.write(f"'{key}' = '{value}'\n")
                             else:
                                 toml_file.write(f"'{key}' = {value}\n")
                     toml_file.write("\n")
```

### Comparing `batpy-0.0.2/src/batpy/is_version_compatible.py` & `batpy-0.0.5/src/batpy/is_version_compatible.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # -*- coding: UTF-8 -*-
+"""Module, which includes the function is_version_compatible
+"""
 import logging
+
 import semantic_version
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
-    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t%(lineno)s\t- %(message)s",
+    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t\
+        %(lineno)s\t- %(message)s",
     filename="batpy.log",
     filemode="w",
     level=logging.INFO,
 )
 
 
 def is_version_compatible(
     self_version: semantic_version.Version,
     version_to_check: semantic_version.Version,
     include_minor: bool = False,
 ) -> bool:
     """Check for version compatibility
 
-    Check if two versions (major.minor.patch) are compatible. Thereby a version is compatible if major is equal.
-    If minor should also be included a version is compatible if major is equal and minor is greater or equal.
+    Check if two versions (major.minor.patch) are compatible. Thereby a version
+    is compatible if major is equal. If minor should also be included a version
+    is compatible if major is equal and minor is greater or equal.
 
     Parameters
     ----------
     self_version : semantic_version.Version
         Version
     version_to_check : semantic_version.Version
         Version to be checked against self_version.
     include_minor : bool, optional
-        Check if minor version of version_to_check is greater or equal to self_version's minor, by default False.
+        Check if minor version of version_to_check is greater or equal to
+        self_version's minor, by default False.
 
     Returns
     -------
     bool
         True, if version is compatible.
 
     Raises
@@ -47,17 +53,26 @@
 
     min_version = semantic_version.Version(
         major=self_version.major, minor=min_minor, patch=0
     )
 
     if min_version <= version_to_check < min_version.next_major():
         logging.info(
-            f"[+] Version {version_to_check} is compatible: {min_version} <= {version_to_check} < {min_version.next_major()}"
+            "[+] Version %s is compatible: %s <= %s < %s",
+            version_to_check,
+            min_version,
+            version_to_check,
+            min_version.next_major(),
         )
         return True
-    else:
-        logging.warning(
-            f"[!] Version {version_to_check} should be {min_version} <= {version_to_check} < {min_version.next_major()}"
-        )
-        raise ValueError(
-            f"[!] Version {version_to_check} should be {min_version} <= {version_to_check} < {min_version.next_major()}"
-        )
+
+    logging.warning(
+        "[!] Version %s should be %s <= %s < %s",
+        version_to_check,
+        min_version,
+        version_to_check,
+        min_version.next_major(),
+    )
+    raise ValueError(
+        f"[!] Version {version_to_check} should be {min_version} <=\
+            {version_to_check} < {min_version.next_major()}"
+    )
```

### Comparing `batpy-0.0.2/PKG-INFO` & `batpy-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1
-Name: batpy
-Version: 0.0.2
-Summary: A python package to read, write, and calculate batteries in the BatPaC tool.
-License: MIT
-Author: Raphael Ginster
-Author-email: r.ginster@tu-braunschweig.de
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pathlib (>=1.0.1,<2.0.0)
-Requires-Dist: prettytable (>=3.7.0,<4.0.0)
-Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: xlwings (>=0.30.4,<0.31.0)
-Description-Content-Type: text/markdown
+[![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
+[![PyPI version](https://badge.fury.io/py/batpy.svg)](https://badge.fury.io/py/batpy)
+
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 ## Installation
 
+`batpy` is available from [PyPI](https://pypi.org/project/batpy/), and currently requires Python 3.9 or newer. It can be installed with:
 ```bash
 $ pip install batpy
 ```
 
+## Documentation
+
+Documentation for `batpy` is available at [GitHub Pages](https://rginster.github.io/batpy/), including an example and documentation on all the modules and functions.
+
 ## Usage
 
 `batpy` is able to read, write, and calculate batteries in the [BatPaC tool](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 
 
 ```python
-from batpy.BatPaC_battery import BatPaC_battery
-from batpy.BatPaC_tool import BatPaC_tool
+from batpy.batpac_battery import BatpacBattery
+from batpy.batpac_tool import BatpacTool
+
+# Constants
+BATPY_BATPAC_EXCEL = "./BatPaC 5.0 2022-07-22.xlsm"
+
+BATPY_BATPAC_BATTERY_CONFIG = "./batpy_batteries_config.toml"
+BATPY_BATPAC_USER_INPUT_CONFIG = "./batpy_batpac_user_input_cells.toml"
+BATPY_BATPAC_TOOL_CONFIG = "./batpy_batpac_config.toml"
+
+BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG = (
+    "./batpy_batpac_calculation_and_validation_results.toml"
+)
+
 
 # Create batteries
-bat1 = BatPaC_battery("Battery 1")
-bat2 = BatPaC_battery("Battery 2")
-bat3 = BatPaC_battery("Battery 3")
-bat4 = BatPaC_battery("Battery 4")
-bat5 = BatPaC_battery("Battery 5")
-bat6 = BatPaC_battery("Battery 6")
-bat7 = BatPaC_battery("Battery 7")
+bat1 = BatpacBattery("Battery 1")
+bat2 = BatpacBattery("Battery 2")
+bat3 = BatpacBattery("Battery 3")
+bat4 = BatpacBattery("Battery 4")
+bat5 = BatpacBattery("Battery 5")
+bat6 = BatpacBattery("Battery 6")
+bat7 = BatpacBattery("Battery 7")
 
 # Change battery properties
 # a) Write individual properties for created batteries
-bat1.set_new_property("Dashboard", "Number of modules in parallel", 100)
+bat1.set_new_property("Dashboard", "Number of modules in parallel", 10)
 
 # b) Load individiual battery configuration from file
 bat2.load_battery_file(
     "./battery_config.toml", "Battery"
 )
 
 # Create BatPaC instance
-battery_calculation = BatPaC_tool(
-    "./BatPaC 5.0 2022-07-22.xlsm",
-    "./BatPaC_user_input_cells.toml",
-    "./BatPaC_calculation_and_validation_results.toml",
+battery_calculation = BatpacTool(
+    BATPY_BATPAC_EXCEL,
+    BATPY_BATPAC_USER_INPUT_CONFIG,
+    BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG,
     excel_visible=True
 )
 
 # Add batteries to BatPaC instance
 # a) Add individual batteries, which were created before
 battery_calculation.add_battery(
     [
@@ -77,28 +77,28 @@
         bat6,
         bat7,
     ]
 )
 
 # b) Create new batteries from configuration file (will overwrite all batteries)
 battery_calculation.load_batteries_file(
-    "./batteries_config.toml",
+    BATPY_BATPAC_BATTERY_CONFIG,
     [
         bat1,
         bat2,
         bat3,
         bat4,
         bat5,
         bat6,
         bat7,
     ],
 )
 
 # Load configuration file for BatPaC instance
-battery_calculation.load_batpac_file("./BatPaC_config.toml")
+battery_calculation.load_batpac_file(BATPY_BATPAC_TOOL_CONFIG)
 
 # Write configuration in Excel file and calculate batteries
 battery_calculation.calculate()
 battery_calculation.read_calculation_and_validation_results()
 
 # Save configuration from Excel:
 battery_calculation.save_config(
@@ -120,8 +120,7 @@
 ## License
 
 `batpy` was created by [Raphael Ginster](https://www.tu-braunschweig.de/en/aip/pl/team/ginster). It is licensed under the terms of the MIT license.
 
 ## Credits
 
 `batpy` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
-
```

