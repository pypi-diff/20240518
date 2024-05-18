# Comparing `tmp/extended_configparser-1.0.1.tar.gz` & `tmp/extended_configparser-1.1.0.tar.gz`

## Comparing `extended_configparser-1.0.1.tar` & `extended_configparser-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/noxfile.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/interpolator.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/matcher.py
--rw-r--r--   0        0        0    10406 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/parser.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/__init__.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/configuration.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/entries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_config_matcher.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_env_interpolation.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_inquirer.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_parser.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config1.cfg
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config1_result.cfg
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config2_result.cfg
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/env_config.cfg
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/LICENSE
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/README.md
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/noxfile.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/__init__.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/interpolator.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/matcher.py
+-rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/parser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/configuration.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/entries/__init__.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/entries/base.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/entries/confirmation.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/entries/section.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/src/extended_configparser/configuration/entries/selection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/test_config_matcher.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/test_env_interpolation.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/test_inquirer.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/test_parser.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/data/config1.cfg
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/data/config1_result.cfg
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/data/config2_result.cfg
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/tests/data/env_config.cfg
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/README.md
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 extended_configparser-1.1.0/PKG-INFO
```

### Comparing `extended_configparser-1.0.1/.pre-commit-config.yaml` & `extended_configparser-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/.github/workflows/python-publish.yml` & `extended_configparser-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/src/extended_configparser/interpolator.py` & `extended_configparser-1.1.0/src/extended_configparser/interpolator.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 import configparser
 import os
 import re
 
 
 class EnvInterpolation(configparser.ExtendedInterpolation):
+    """
+    Interpolation which expands environment variables in values.
+    Subclass of ExtendedInterpolation, thus it also supports the ${section:option} syntax.
+
+    To interpolate environment variables in values, use the following syntax:
+    value = ${ENV_VAR_NAME}
+    """
+
     ENV_PATTERN = re.compile(r"\$\[([^\}]+)\]")
     _KEYCRE = re.compile(r"\$\{([^}]+)\}")
 
     def __init__(self, allow_uninterpolated_values: bool = False) -> None:
         self.allow_uninterpolated_values = allow_uninterpolated_values
 
     def _interpolate_some(self, parser, option, accum, rest, section, map, depth) -> None:  # type: ignore
```

### Comparing `extended_configparser-1.0.1/src/extended_configparser/matcher.py` & `extended_configparser-1.1.0/src/extended_configparser/matcher.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/src/extended_configparser/parser.py` & `extended_configparser-1.1.0/src/extended_configparser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 
 logger = logging.getLogger(__name__)
 
 from extended_configparser.matcher import ConfigMatcher
 
 
 class ExtendedConfigParser(configparser.ConfigParser):
-    """ConfigParser that can write comments to a file."""
+    """
+    ConfigParser that can read from and write comments to a file.
+
+    Use get_comment(section, option) and set_comment(section, option, comment) to get and set comments
+    or use it directly when setting values with set(section, option, value, comment).
+    """
 
     def __init__(
         self,
         defaults=None,
         dict_type=dict,
         allow_no_value: bool = False,
         *,
@@ -44,16 +49,16 @@
             default_section=default_section,
             interpolation=interpolation,
             converters=converters,
         )
 
         self.top_comment = None
         self.end_comment = None
-        self._option_comments: dict[str, dict[str, str]] = {}
-        self._section_comments: dict[str, str] = {}
+        self._option_comments: dict[str, dict[str, str | None]] = {}
+        self._section_comments: dict[str, str | None] = {}
         self._delimiters = delimiters
         self._comment_prefixes = comment_prefixes
 
     #############################################################################
     ### INTERNAL AND OVERRIDE METHODS
     #############################################################################
 
@@ -113,15 +118,16 @@
         if self.end_comment:
             fp.write(ConfigMatcher.add_prefix(self.end_comment, self._comment_prefixes[0]))
 
     def _write_section(self, fp, section_name: str, section_items: dict[str, str], delimiter: str) -> None:
         """Write a single section to the specified `fp`."""
         if section_name in self._section_comments:
             comment = self._section_comments[section_name]
-            fp.write(ConfigMatcher.add_prefix(comment, self._comment_prefixes[0]) + "\n")
+            if comment is not None:
+                fp.write(ConfigMatcher.add_prefix(comment, self._comment_prefixes[0]) + "\n")
 
         fp.write("[{}]\n".format(section_name))
         for key, value in section_items:
             value = self._interpolation.before_write(self, section_name, key, value)
             if value is not None or not self._allow_no_value:
                 value = delimiter + str(value).replace("\n", "\n\t")
             else:
@@ -130,48 +136,56 @@
             comment = self._option_comments.get(section_name, {}).get(key, "")
             if comment:
                 fp.write("{}\n".format(ConfigMatcher.add_prefix(comment, self._comment_prefixes[0])))
             fp.write("{}{}\n".format(key, value))
         fp.write("\n")
 
     def _parse_comments(self, text: str | Iterable[str]) -> None:
+        """Internal function to parse comments from the content string of a file."""
 
         matcher = ConfigMatcher(self._delimiters, self._comment_prefixes)
         matches = list(matcher.get_matches(text))
         # print("Matches:", len(matches))
         for m in matches:
             # print("Match:", m.comment, m.section, m.option)
             if m.section is None and m.option is None:
                 if self.top_comment is None:
                     self.top_comment = m.comment
                 else:
                     self.end_comment = m.comment
             else:
                 self.set_comment(m.section, m.option, m.comment)
 
+    def __str__(self) -> str:
+        from io import StringIO
+
+        s = StringIO()
+        self.write(s)
+        return s.getvalue()
+
     #############################################################################
     ### PUBLIC METHODS
     #############################################################################
 
-    def get_comment(self, section: str, option: str | None = None) -> str:
+    def get_comment(self, section: str, option: str | None = None) -> str | None:
         """Return the comment for a section or option.
 
         Parameters
         ----------
         section : str
             Section name
         option : str, optional
             Option name. If None, the comment for the section is returned.
         Returns
         -------
-        str
+        str | None
             The comment for the section or option.
         """
         if option is None:
-            return self._section_comments.get(section, "")
+            return self._section_comments.get(section, None)
 
         option = option.lower()
         return self._option_comments.get(section, {}).get(option, "")
 
     def set_comment(self, section: str | None, option: str | None = None, comment: str | None = None) -> None:
         """Set a comment for a section or option.
 
@@ -196,18 +210,23 @@
 
         option = option.lower()
         if section not in self._option_comments:
             self._option_comments[section] = {}
 
         self._option_comments[section][option] = comment
 
-    def set(self, section: str, option: str, value: str | None, comment: str | None = None):
+    def set(
+        self, section: str, option: str, value: str | None, comment: str | None = None, add_section_if_missing=True
+    ):
         """Set an option in a section.
         Optionally set a comment for the option.
         """
+        if not self.has_section(section) and add_section_if_missing:
+            self.add_section(section)
+
         super().set(section, option, value)
         if comment:
             self.set_comment(section, option, comment)
 
     def add_section(self, section: str, comment: str | None = None):
         """Add a section to the configuration.
         Optionally set a comment for the section.
@@ -217,19 +236,32 @@
             self.set_comment(section, comment=comment)
 
     #############################################################################
     ### ADDITIONAL GETTER METHODS
     #############################################################################
 
     @staticmethod
-    def split_to_list(list_str: str, delimiter: str = ",") -> list[str]:
+    def split_to_list(list_str: str, delimiter: str = ",", remove_brackets=["[]"]) -> list[str]:
         if list_str is None or list_str == "":
             return []
+
+        for bracket in remove_brackets:
+            list_str = list_str.lstrip(bracket).rstrip(bracket)
+
         return [i.strip() for i in list_str.split(delimiter)]
 
+    @staticmethod
+    def list_to_str(list: list[str] | str, delimiter: str = ",", brackets: str = "[]") -> str:
+        if isinstance(list, str):
+            return list
+        s = delimiter.join(list)
+        if brackets and len(brackets) == 2:
+            s = brackets[0] + s + brackets[1]
+        return s
+
     def get_list(self, section: str, option: str, delimiter: str = ",", fallback: Any = None) -> list[str]:
         """Get a list from a configuration option.
 
         Parameters
         ----------
         section : str
             Section name
@@ -247,15 +279,15 @@
         """
         v = self.get(section, option, fallback=None)
         if v is None:
             return fallback
         return self.split_to_list(v, delimiter)
 
     def get_abs_path(
-        self, option: str, section: str, root_dir: str | None = None, create_dir: bool = False, fallbac: Any = None
+        self, option: str, section: str, root_dir: str | None = None, create_dir: bool = False, fallback: Any = None
     ) -> str | None:
         """Get an absolute path from a configuration option.
 
         Parameters
         ----------
         option : str
             Option name
```

### Comparing `extended_configparser-1.0.1/src/extended_configparser/configuration/configuration.py` & `extended_configparser-1.1.0/src/extended_configparser/configuration/configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
+import io
 import logging
 import os
 from configparser import Interpolation
+from configparser import SectionProxy
 
 from extended_configparser.configuration.entries import ConfigEntry
 from extended_configparser.configuration.entries import ConfigEntryCollection
 from extended_configparser.interpolator import EnvInterpolation
 from extended_configparser.parser import ExtendedConfigParser
 
 logger = logging.getLogger(__name__)
@@ -17,19 +19,49 @@
     Super class for custom Configuration classes representing a configuration file in ini format.
 
     In your subclass, define your entries as attributes of type ConfigEntry or ConfigEntryCollection.
     Those defined entries will be read from and written to the configuration file.
     With `inqure()` the user will be asked to provide the values for the defined entries.
     """
 
-    def __init__(self, path: str, interpolation: Interpolation = EnvInterpolation()) -> None:
+    def __init__(
+        self,
+        path: str,
+        interpolation: Interpolation = EnvInterpolation(),
+        base_paths: list[str] | None = None,
+        auto_save: bool = False,
+    ) -> None:
+        """Create a new Configuration object.
+
+        Parameters
+        ----------
+        path : str
+            File path to the configuration file.
+        interpolation : Interpolation, optional
+            Interpolation to use for the configuration file, by default EnvInterpolation()
+        base_paths : list[str] | None, optional
+            If the values of the configuration using interpolation reference other configuration files, those file paths can be specified here.
+        auto_save : bool, optional
+            If True, the configuration will be saved automatically after setting a value.
+        """
+
         self.config_path = path
+        """File path to the configuration file."""
+
+        self.auto_save = auto_save
+        """If True, the configuration will be saved automatically after setting a value."""
+
+        self.base_paths = base_paths or []
+        """Paths to other configuration files that are automatically read."""
 
         self._entries: list[ConfigEntry] = []
+        """Cache for the entries of the configuration."""
+
         self._config_parser = ExtendedConfigParser(interpolation=interpolation)
+        """ConfigParser object used to read and write the configuration file."""
 
     @staticmethod
     def get_config_entries_in_object(cfg: Configuration, ignore: list[str] = ["entries"]) -> list[ConfigEntry]:
         """
         Get all ConfigEntries in the given object.
         Members in the ignore list will be skipped.
         """
@@ -43,84 +75,91 @@
             elif isinstance(getattr(cfg, attr), ConfigEntryCollection):
                 entries.extend(Configuration.get_config_entries_in_object(getattr(cfg, attr)))
 
         return entries
 
     @property
     def entries(self) -> list[ConfigEntry]:
+        """
+        Get all ConfigEntries in the configuration object.
+        Based on the defined ConfigEntrie or ConfigEntryCollection members of the object.
+        """
+
         if len(self._entries) == 0:
             # Iter over each attribute of the object and check if it is a ConfigEntry or a subclass of it
             self._entries = Configuration.get_config_entries_in_object(self)
 
         return self._entries
 
-    def load(self, use_default_for_missing_options: bool = True, inquire_if_missing: bool = False) -> None:
+    def load(self, inquire_if_missing: bool = False, quiet: bool = False) -> None:
         """Load the configuration file and set the values of the entries.
 
 
         Parameters
         ----------
-        use_default_for_missing_options : bool, optional
-            If True, a missing option in the read configfile will be set to its default. Otherwise, raise a ValueError. By default True
+        inquire_if_missing : bool, optional
+            If True, the user will be asked to provide the values for the configuration entries.
+        quiet : bool, optional
+            If True, no warning will be printed if the configuration file is missing.
 
         Raises
         ------
         ValueError
             If a required option is missing and use_default_for_missing_options is False
         """
+
+        for base_path in self.base_paths:
+            if not os.path.exists(base_path):
+                logger.warning(f"Base configuration file {base_path} not found.")
+                continue
+
+            self._config_parser.read(base_path)
+
         if not os.path.exists(self.config_path):
-            logger.warning(f"Configuration file {self.config_path} not found. Creating new configuration file.")
+            if not quiet:
+                logger.warning(f"Configuration file {self.config_path} not found.")
             if inquire_if_missing:
                 self.inquire()
-            self.write()
-            return
+        else:
+            self._config_parser.read(self.config_path)
 
-        self._config_parser.read(self.config_path)
+        auto_save = self.auto_save
+        self.auto_save = False
 
         for entry in self.entries:
-            if entry.required and not self._config_parser.has_option(entry.section, entry.option):
-                if use_default_for_missing_options:
-                    entry.value = entry.default
-                    continue
-
-                raise ValueError(
-                    f"Required option {entry.option} not found in section {entry.section} for configuration {self.config_path}"
-                )
-            entry.value = self._config_parser.get(entry.section, entry.option, fallback=entry.default, raw=True)
+            entry.configparser = self._config_parser
+            entry.configuration = self
+            entry.value = entry.raw_value
+
+        self.auto_save = auto_save
 
     def write(self) -> None:
         """Write the configuration to the file path."""
-        for entry in self.entries:
-            self._set_entry(entry)
-
         # Check if the directory exists
         if not os.path.exists(os.path.dirname(self.config_path)):
             os.makedirs(os.path.dirname(self.config_path))
 
-        with open(self.config_path, "w") as f:
-            self._config_parser.write(f)
-
-    def _set_entry(self, entry: ConfigEntry) -> None:
-        """Set the value of the entry in the configuration parser.
-
-        Parameters
-        ----------
-        entry : ConfigEntry
-            The entry to set.
-        """
-        if not self._config_parser.has_section(section=entry.section):
-            self._config_parser.add_section(section=entry.section)
+        # We cannot just write the config file, as there could be base configs, whose content should not appear in this config.
+        parser = ExtendedConfigParser()
+        if os.path.exists(self.config_path):
+            parser.read(self.config_path)
+        for entry in self.entries:
+            parser.set(entry.section, entry.option, entry.raw_value, entry.get_comment())
 
-        self._config_parser.set(entry.section, entry.option, entry.value, entry.get_comment())
+        with io.open(self.config_path, "w") as f:
+            # self._config_parser.write(f)
+            parser.write(f)
 
-    def inquire(self) -> None:
+    def inquire(self, use_existing_values: bool = True) -> None:
         """Inquire the user for the values of the entries."""
 
         logger.debug(f"Configuring @ {self.config_path}")
-        self.load()
+        self.load(quiet=True)
         for entry in self.entries:
-            entry.inquire()
-            self._set_entry(entry)
+            entry.inquire(use_existing_values)
+            # self._set_entry(entry)
+
+        logger.debug(f"Configuration of {self.config_path} completed.")
 
-        self.write()
-        self.load()
-        logger.debug("Configuration of {self.config_path} completed.")
+    def __getitem__(self, key: str) -> SectionProxy:
+        """Returns the section with the given key."""
+        return self._config_parser[key]
```

### Comparing `extended_configparser-1.0.1/src/extended_configparser/configuration/entries.py` & `extended_configparser-1.1.0/src/extended_configparser/configuration/entries/confirmation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,95 @@
 from __future__ import annotations
 
 import logging
+from typing import Any
 
-logger = logging.getLogger(__name__)
-
-
-class ConfigEntryCollection:
-    """
-    Super class for grouping ConfigEntries together.
-
-    If you want to structure your configuration entries in a configuration class by grouping entries together in another data class,
-    inherit from this class and define your entries as attributes of type ConfigEntry or ConfigEntryCollection.
-    """
-
-    pass
-
-
-class ConfigSection:
-    """
-    Helper class to group ConfigEntries together under a section.
-    Create entries by calling `section.ConfigSection("section_name")`.
-    """
-
-    def __init__(self, name: str) -> None:
-        self.name = name
+from extended_configparser.configuration.entries.base import ConfigEntry
+from extended_configparser.configuration.entries.base import InquireCondition
 
-    def ConfigOption(
-        self,
-        option: str,
-        default: str,
-        message: str,
-        required: bool = True,
-        **inquirer_kwargs,
-    ) -> ConfigEntry:
-        """Create a ConfigEntry for that section with the given parameters."""
-        return ConfigEntry(
-            section=self.name,
-            option=option,
-            default=default,
-            message=message,
-            required=required,
-            **inquirer_kwargs,
-        )
+logger = logging.getLogger(__name__)
 
 
-class ConfigEntry:
+class ConfigConfirmationEntry(ConfigEntry[bool]):
     """
-    Represents a single configuration entry.
+    Represents a single confirmation configuration entry (yes/no).
     """
 
     def __init__(
         self,
         section: str,
         option: str,
-        default: str,
+        default: bool,
         message: str,
-        required: bool = True,
-        inquire: bool = True,
-        use_existing_as_default=True,
+        inquire: InquireCondition = True,
         **inquirer_kwargs,
     ) -> None:
-        """Create a new ConfigEntry.
+        """Create a new ConfigConfirmationEntry.
 
         Parameters
         ----------
         section : str
             Section name.
         option : str
             Option name.
-        default : str
+        default : bool
             Default value.
         message : str
             Message to be asked to the user for configurating this entry.
-        required : bool, optional
-            If the entry is required, by default True
-        inquire : bool, optional
-            If the entry should be inquired to the user, by default True
-        use_existing_as_default : bool, optional
-            If True, the existing value of a config is taken as default value when asking the user, otherwise take the given default value, by default True
+        inquire : InquireCondition, optional
+            Whether to inquire the user for the value of this entry.
         """
-        self.section = self.escape_whitespace(section)
-        self.option = self.escape_whitespace(option)
-        self.default = default
-        self.message = message
-        self.required = required
-        self.value: str | None = default
-        self.use_existing_as_default = use_existing_as_default
-        self.inquirer_kwargs = inquirer_kwargs
-        self.do_inquire = inquire
-
-        if "qmark" not in self.inquirer_kwargs:
-            self.inquirer_kwargs["qmark"] = "?"
-
-        if "amark" not in self.inquirer_kwargs:
-            self.inquirer_kwargs["amark"] = ">"
-
-    def __str__(self) -> str:
-        return f"{self.section}:{self.option} = {self.value}"
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    @staticmethod
-    def escape_whitespace(value: str) -> str:
-        return value.replace(" ", "_")
+        super().__init__(
+            section=section,
+            option=option,
+            default=self.get_bool_str(default),
+            message=message,
+            inquire=inquire,
+            value_getter=self.to_bool,
+            value_setter=self.get_bool_str,
+            **inquirer_kwargs,
+        )
 
-    def inquire(self) -> None:
+    def inquire(self, use_existing_as_default: bool = True) -> None:
         """Inquire the user for the value of this entry."""
 
-        if not self.do_inquire:
+        if not self.do_inquire():
             return
 
         from InquirerPy import inquirer
 
-        msg = self.message.strip()
-        msg = msg.strip(".:") + ":"
-        self.value = inquirer.text(
+        msg = self.get_msg(self.message)
+        self.value = inquirer.confirm(
             message=msg,
-            default=(self.value if self.use_existing_as_default else self.default),
+            default=(self.to_bool(self.value) if use_existing_as_default else self.default),
             **self.inquirer_kwargs,
         ).execute()
 
-    def get_comment(self) -> str:
-        s = self.message
-        if "instruction" in self.inquirer_kwargs:
-            s += f"\nInstruction: {self.inquirer_kwargs['instruction']}"
-        if "long_instruction" in self.inquirer_kwargs:
-            s += f"\nLong Instruction: {self.inquirer_kwargs['long_instruction']}"
+    @staticmethod
+    def to_bool(value: Any):
+        """Transform values to boolean."""
+
+        if value is None:
+            return False
+
+        if isinstance(value, bool):
+            return value
 
-        return s
+        if isinstance(value, int):
+            if value > 0:
+                return True
+
+        if isinstance(value, str):
+            v = value.lower()
+            if v == "true" or v == "yes" or v == "1":
+                return True
+
+            return False
+
+        try:
+            return bool(value)
+        except:
+            return False
+
+    @staticmethod
+    def get_bool_str(value: bool) -> str:
+        return "Yes" if value else "No"
```

### Comparing `extended_configparser-1.0.1/tests/test_config_matcher.py` & `extended_configparser-1.1.0/tests/test_config_matcher.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/tests/test_env_interpolation.py` & `extended_configparser-1.1.0/tests/test_env_interpolation.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/tests/test_inquirer.py` & `extended_configparser-1.1.0/tests/test_inquirer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,55 @@
 
 import io
 import pathlib
 
 import pytest
 
 from extended_configparser.configuration.configuration import Configuration
-from extended_configparser.configuration.entries import ConfigEntry
-from extended_configparser.configuration.entries import ConfigEntryCollection
-from extended_configparser.configuration.entries import ConfigSection
+from extended_configparser.configuration.entries.base import ConfigEntry
+from extended_configparser.configuration.entries.base import ConfigEntryCollection
+from extended_configparser.configuration.entries.confirmation import (
+    ConfigConfirmationEntry,
+)
+from extended_configparser.configuration.entries.section import ConfigSection
+from extended_configparser.configuration.entries.selection import ConfigSelectionEntry
 
 
 class MainConfigPaths(ConfigEntryCollection):
     def __init__(self):
         section = ConfigSection("Dirs")
-        self.data_root_dir = section.ConfigOption(
+        self.data_root_dir = section.Option(
             "data_root_dir",
             r"${HOME}/test/",
             "Root directory for all data",
             long_instruction="This is a longer description of what you have to do.",
         )
 
         subdir_section = ConfigSection("Subdirs")
-        self.sub_dir = subdir_section.ConfigOption("sub_dir", r"${Dirs:data_root_dir}/subdir/", "Main subdirectory.")
+        self.sub_dir = subdir_section.Option("sub_dir", r"${Dirs:data_root_dir}/subdir/", "Main subdirectory.")
 
 
 class MainConfig(Configuration):
     def __init__(self, path: str):
         super().__init__(path)
         self.paths = MainConfigPaths()
         self.test = ConfigEntry("Test", "Foo", "Bla", "Test entry")
 
+        self.confirmation = ConfigConfirmationEntry("Test", "Confirmation", False, "Test confirmation entry")
+
+        self.selection = ConfigSelectionEntry(
+            "Test",
+            "Selection",
+            ["b"],
+            "Test selection entry",
+            choices=["a", "b", "c"],
+            multiselect=True,
+            delimiter=",\n",
+        )
+
 
 # TODO: Automate the input for testing. Currently it is manual.
 def inquire(shared_datadir):
 
     config = MainConfig(shared_datadir / "test_config.cfg")
 
     # mocker.patch("builtins.input", side_effect=["/tmp/test", "/tmp/test/subdir", "TestValue"])
@@ -53,13 +69,25 @@
 [Subdirs]
 # Main subdirectory.
 sub_dir = ${Dirs:data_root_dir}/subdir/
 
 [Test]
 # Test entry
 foo = Bla
+# Test confirmation entry
+confirmation = Yes
+# Test selection entry
+selection = a,
+        b,
+        c
 """
     assert content.strip() == s.strip()
 
 
 if __name__ == "__main__":
-    inquire(pathlib.Path(__file__).parent / "tmp")
+    path = pathlib.Path(__file__).parent / "tmp"
+    # If path exists, delete all files in the dir
+    if path.exists():
+        for f in path.iterdir():
+            f.unlink()
+
+    inquire(path)
```

### Comparing `extended_configparser-1.0.1/tests/test_parser.py` & `extended_configparser-1.1.0/tests/test_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,31 @@
     result_lines = [line.strip() for line in result_lines if len(line.strip()) > 0]
 
     assert len(output_lines) == len(result_lines)
     for output_line, result_line in zip(output_lines, result_lines):
         assert output_line.strip() == result_line.strip()
 
 
+def test_str(shared_datadir, tmp_path):
+    contents = (shared_datadir / "config1.cfg").read_text()
+    result = (shared_datadir / "config1_result.cfg").read_text()
+
+    parser = ExtendedConfigParser()
+    parser.read_string(contents)
+
+    output_path = tmp_path / "output.cfg"
+    with open(output_path, "w") as f:
+        parser.write(f)
+
+    output_contents = output_path.read_text()
+    output_str = str(parser)
+
+    assert output_contents.strip() == output_str.strip()
+
+
 def test_change_comment(shared_datadir, tmp_path):
     contents = (shared_datadir / "config1.cfg").read_text()
     result = (shared_datadir / "config2_result.cfg").read_text()
 
     parser = ExtendedConfigParser()
     parser.read_string(contents)
```

### Comparing `extended_configparser-1.0.1/.gitignore` & `extended_configparser-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/LICENSE` & `extended_configparser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.1/README.md` & `extended_configparser-1.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.3
+Name: extended-configparser
+Version: 1.1.0
+Summary: Extended config parser.
+Project-URL: Homepage, https://github.com/vschroeter/extended-configparser
+Project-URL: Issues, https://github.com/vschroeter/extended-configparser/issues
+Author-email: Valentin Schröter <vasc9380@th-wildau.de>
+License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Provides-Extra: cli
+Requires-Dist: inquirerpy; extra == 'cli'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: inquirerpy; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: nox; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-datadir; extra == 'dev'
+Requires-Dist: pytest-mock; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: nox; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-datadir; extra == 'test'
+Requires-Dist: pytest-mock; extra == 'test'
+Description-Content-Type: text/markdown
+
 # Extended Configparser
 
 Extended features for the normal [Python Configparser](https://docs.python.org/3/library/configparser.html):
 - Write comments to and read comments from the configuration file
 - Access and alter the comments of a section or an option in your code
 - Environment variable interpolation inside the configuration file
 
@@ -156,15 +186,15 @@
 This is useful for the first setup of a configuration file.
 
 > [!NOTE]
 > To use the `config.inquire()` method, .you have to install the package in the cli configuration `pip install extended-configparser[cli]`.
 
 ```python
 config = MyConfig("myconfig.cfg")
-# Load the configuration if existing. If it does not exist, a new configuration file with default values is created.
+# Load the configuration if existing.
 config.load()
 # Inquire the user for the configuration values
 # Each ConfigEntry will be asked for its value
 config.inquire()
 # Write the config back
 config.write()
 ```
@@ -176,47 +206,80 @@
 Interpolation of environment variables and other section values is supported by default.
 
 ```python
 
 # Collection of values used in your configuration
 class MainConfigPaths(ConfigEntryCollection):
     def __init__(self):
+        # Shortcut to create options on the same section
         section = ConfigSection("Dirs")
-        self.data_root_dir = section.ConfigOption(
+        self.data_root_dir = section.Option(
             "data_root_dir",
             r"${HOME}/data/",
             "Root directory for all data",
+            is_dir=True, # Access to this value automatically creates the directory
             long_instruction="The subdirectories defined in [Subdirs] will be created in this directory, except you define them as absolute paths.",
         )
-        self.app_data_dir = section.ConfigOption(
+        self.app_data_dir = section.Option(
             "app_data_dir",
             r"/opt/app/data/",
             "Directory for application data from the app.",
+            is_dir=True, # Access to this value automatically creates the directory
         )
 
-        subdir_section = ConfigSection("Subdirs")
-        self.cache_dir = subdir_section.ConfigOption(
+        self.cache_dir = ConfigEntry(
+            "Subdirs
             "cache_dir",
             r"${Dirs:data_root_dir}/cache/",
             "Main directory for cache files, e.g. for the discovering process.",
+            is_dir=True, # Access to this value automatically creates the directory
         )
 
 
 class MyConfig(Configuration):
     def __init__(self, path: str):
         super().__init__(path)
+
+        # Automatically inqiure the user a n/Y question
+        self.enabled = ConfirmationOption("enabled", True, "Enable something")
+
+        # Normal ConfigEntry
         self.value1 = ConfigEntry(
             section="Section1",
             option="value1",
             default="default",
             message="Description of value1"
+            inquire=self.is_enabled, # Only ask for this value if enabled is True
         )
 
+        # Value transformed ConfigEntry
+        self.some_number = ConfigEntry(
+            "some_number",
+            4,
+            "A number:",
+            inquire=self.is_enabled,
+            value_getter=int, # Automatically transforms the string value into an integer
+            # Automatically transforms the integer value into a string on write
+            value_setter=lambda x: str(x), # The same like 'value_setter=str', which is the default
+            long_instruction="This number is a number :D",
+        )
+
+        # Include the ConfigEntryCollection
         self.paths = MainConfigPaths()
 
+        # Selection of multiple predefined values
+        self.selection = ConfigSelectionEntry(
+            section="Test",
+            option="a_selection",
+            default=["b"],
+            message="Test selection entry",
+            choices=["a", "b", "c"],
+            multiselect=True,
+            delimiter=",\n", # Defines how the value is written back and read
+        )
 
 config = MyConfig("myconfig.cfg")
 config.load()
 config.inquire()
 config.write()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `extended_configparser-1.0.1/pyproject.toml` & `extended_configparser-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "extended-configparser"
-version = "1.0.1"
+version = "1.1.0"
 authors = [{ name = "Valentin Schröter", email = "vasc9380@th-wildau.de" }]
 description = "Extended config parser."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = []
 
 classifiers = ["Programming Language :: Python :: 3"]
```

### Comparing `extended_configparser-1.0.1/PKG-INFO` & `extended_configparser-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.3
-Name: extended-configparser
-Version: 1.0.1
-Summary: Extended config parser.
-Project-URL: Homepage, https://github.com/vschroeter/extended-configparser
-Project-URL: Issues, https://github.com/vschroeter/extended-configparser/issues
-Author-email: Valentin Schröter <vasc9380@th-wildau.de>
-License-File: LICENSE
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Provides-Extra: cli
-Requires-Dist: inquirerpy; extra == 'cli'
-Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: flake8; extra == 'dev'
-Requires-Dist: inquirerpy; extra == 'dev'
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: nox; extra == 'dev'
-Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev'
-Requires-Dist: pytest-datadir; extra == 'dev'
-Requires-Dist: pytest-mock; extra == 'dev'
-Provides-Extra: test
-Requires-Dist: nox; extra == 'test'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-datadir; extra == 'test'
-Requires-Dist: pytest-mock; extra == 'test'
-Description-Content-Type: text/markdown
-
 # Extended Configparser
 
 Extended features for the normal [Python Configparser](https://docs.python.org/3/library/configparser.html):
 - Write comments to and read comments from the configuration file
 - Access and alter the comments of a section or an option in your code
 - Environment variable interpolation inside the configuration file
 
@@ -186,15 +156,15 @@
 This is useful for the first setup of a configuration file.
 
 > [!NOTE]
 > To use the `config.inquire()` method, .you have to install the package in the cli configuration `pip install extended-configparser[cli]`.
 
 ```python
 config = MyConfig("myconfig.cfg")
-# Load the configuration if existing. If it does not exist, a new configuration file with default values is created.
+# Load the configuration if existing.
 config.load()
 # Inquire the user for the configuration values
 # Each ConfigEntry will be asked for its value
 config.inquire()
 # Write the config back
 config.write()
 ```
@@ -206,47 +176,80 @@
 Interpolation of environment variables and other section values is supported by default.
 
 ```python
 
 # Collection of values used in your configuration
 class MainConfigPaths(ConfigEntryCollection):
     def __init__(self):
+        # Shortcut to create options on the same section
         section = ConfigSection("Dirs")
-        self.data_root_dir = section.ConfigOption(
+        self.data_root_dir = section.Option(
             "data_root_dir",
             r"${HOME}/data/",
             "Root directory for all data",
+            is_dir=True, # Access to this value automatically creates the directory
             long_instruction="The subdirectories defined in [Subdirs] will be created in this directory, except you define them as absolute paths.",
         )
-        self.app_data_dir = section.ConfigOption(
+        self.app_data_dir = section.Option(
             "app_data_dir",
             r"/opt/app/data/",
             "Directory for application data from the app.",
+            is_dir=True, # Access to this value automatically creates the directory
         )
 
-        subdir_section = ConfigSection("Subdirs")
-        self.cache_dir = subdir_section.ConfigOption(
+        self.cache_dir = ConfigEntry(
+            "Subdirs
             "cache_dir",
             r"${Dirs:data_root_dir}/cache/",
             "Main directory for cache files, e.g. for the discovering process.",
+            is_dir=True, # Access to this value automatically creates the directory
         )
 
 
 class MyConfig(Configuration):
     def __init__(self, path: str):
         super().__init__(path)
+
+        # Automatically inqiure the user a n/Y question
+        self.enabled = ConfirmationOption("enabled", True, "Enable something")
+
+        # Normal ConfigEntry
         self.value1 = ConfigEntry(
             section="Section1",
             option="value1",
             default="default",
             message="Description of value1"
+            inquire=self.is_enabled, # Only ask for this value if enabled is True
         )
 
+        # Value transformed ConfigEntry
+        self.some_number = ConfigEntry(
+            "some_number",
+            4,
+            "A number:",
+            inquire=self.is_enabled,
+            value_getter=int, # Automatically transforms the string value into an integer
+            # Automatically transforms the integer value into a string on write
+            value_setter=lambda x: str(x), # The same like 'value_setter=str', which is the default
+            long_instruction="This number is a number :D",
+        )
+
+        # Include the ConfigEntryCollection
         self.paths = MainConfigPaths()
 
+        # Selection of multiple predefined values
+        self.selection = ConfigSelectionEntry(
+            section="Test",
+            option="a_selection",
+            default=["b"],
+            message="Test selection entry",
+            choices=["a", "b", "c"],
+            multiselect=True,
+            delimiter=",\n", # Defines how the value is written back and read
+        )
 
 config = MyConfig("myconfig.cfg")
 config.load()
 config.inquire()
 config.write()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

