# Comparing `tmp/imessagedb-1.2.9.tar.gz` & `tmp/imessagedb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.9.tar", max compression
+gzip compressed data, was "imessagedb-1.3.0.tar", max compression
```

## Comparing `imessagedb-1.2.9.tar` & `imessagedb-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 03:16:08.542343 imessagedb-1.2.9/LICENSE
--rw-r--r--   0        0        0     8509 2023-05-18 03:16:08.542343 imessagedb-1.2.9/README.md
--rw-r--r--   0        0        0     1309 2023-05-18 03:16:52.974677 imessagedb-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     9342 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3055 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2518 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23179 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/html.py
--rw-r--r--   0        0        0     4975 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/message.py
--rw-r--r--   0        0        0     4896 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/text.py
--rw-r--r--   0        0        0      538 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/utils.py
--rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 imessagedb-1.2.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-20 01:31:15.923159 imessagedb-1.3.0/LICENSE
+-rw-r--r--   0        0        0     9175 2023-05-20 01:31:15.923159 imessagedb-1.3.0/README.md
+-rw-r--r--   0        0        0     1309 2023-05-20 01:31:46.287568 imessagedb-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12415 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3300 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/default.ini
+-rw-r--r--   0        0        0     1092 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    24226 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/html.py
+-rw-r--r--   0        0        0     4975 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6269 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     6558 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/text.py
+-rw-r--r--   0        0        0      677 2023-05-20 01:31:15.935159 imessagedb-1.3.0/src/imessagedb/utils.py
+-rw-r--r--   0        0        0     9881 1970-01-01 00:00:00.000000 imessagedb-1.3.0/PKG-INFO
```

### Comparing `imessagedb-1.2.9/LICENSE` & `imessagedb-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.9/README.md` & `imessagedb-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 
 If you specify html output, `imessagedb` will copy your attachments so that they are accessible
 to the web browser. In addition, it will convert certain types of attachments so that they 
 can be viewed in the browser. For instance, it will convert HEIC files to PNG so that they 
 browser can display it, and will convert various type of movie files to mp4 and various audio
 files to mp3. If you have many attachments, this can take a long time and take a lot of space. 
 
+### Example Output
+
+This is what the default html version looks like. Note that I am hovering over one of the
+links to show the image.
+
+![](JulioHtml.png)
+
+This is the same conversation rendered in text.
+
+![](JulioText.png)
+
 ### Command Line
 
 ```python
 imessagedb [-h] [--handle [HANDLE ...] | --name NAME] [-c CONFIGFILE]
                [-o OUTPUT_DIRECTORY] [--database DATABASE] [-m ME]
                [-t {text,html}] [-i] [-f | --no_copy] [--no_attachments] [-v]
                [--start_time START_TIME] [--end_time END_TIME]
@@ -58,16 +69,17 @@
   --no_attachments      Don't process attachments at all
   -v, --verbose         Turn on additional output
   --start_time START_TIME
                         The start time of the messages in YYYY-MM-DD HH:MM:SS
                         format
   --end_time END_TIME   The end time of the messages in YYYY-MM-DD HH:MM:SS
                         format
-
-
+  --version             Show the version number and exit
+  --get_handles         Display the list of handles in the database and exit
+  --get_chats           Display the list of chats in the database and exit
 ```
 
 #### Command line options
 
 **-h** prints a help message                                                                        |
 
 **--handle [HANDLE ...]**  A list of handles to search against. 
@@ -114,14 +126,17 @@
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
 **--version**  Shows the version number and exits
 
 
+**--get_handles** Display the list of handles in the database and exit
+
+**--get_chats** Display the list of chats in the database and exit
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
 
 ```python
 [CONTROL]
@@ -226,7 +241,10 @@
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 
 `imessagedb` was created by Xev Gittler. It is licensed under the terms of the MIT license.
 
+## Documentation
+
+Full documentation available at https://imessagedb.readthedocs.io/en/latest/
```

### Comparing `imessagedb-1.2.9/pyproject.toml` & `imessagedb-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.9"
+version = "1.3.0"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.2.9/src/imessagedb/__init__.py` & `imessagedb-1.3.0/src/imessagedb/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import configparser
 import logging
 import argparse
 import sys
 from datetime import datetime
 from imessagedb.db import DB
-
+from imessagedb.utils import *
 
 DEFAULT_CONFIGURATION = '''
 [CONTROL]
 
 # Whether or not to copy the attachments into a different directory. This is needed for two reasons:
 #  1) The web browser does not have access to the directory that the attachments are stored, so it cannot display them
 #  2) Some of the attachments need to be converted in order to be viewed in the browser
@@ -67,35 +67,35 @@
 me = Me
 
 # The color for the name in text output. No color is used if 'use text color' is false.
 #  The color can only be one of the following options:
 #   black, red, green, yellow, blue, magenta, cyan, white, light_grey, dark_grey,
 #   light_red, light_green, light_yellow, light_blue, light_magenta, light_cyan
 
+# The way that the color selection works is that it will use the first color on the color list for the first person
+#  in the conversation, the second for the second, third for the third, etc. If there are more participants than colors,
+#  it will wrap around to the first color.
+
 use text color = True
-me text color = blue
-them text color = magenta
+text color list = red, green, yellow, blue, magenta, cyan
 reply text color = light_grey
 
-# The background color of the text messages for you and for the other person in html output
+# The background and name color of the messages in html output
 # The options for colors can be found here: https://www.w3schools.com/cssref/css_colors.php
 
-me html background color = AliceBlue
-them html background color = Lavender
+# The way that the color selection works is that it will use the first color on the color list for the first person
+#  in the conversation, the second for the second, third for the third, etc. If there are more participants than colors,
+#  it will wrap around to the first color.
+
+html background color list = AliceBlue, Cyan, Gold, Lavender, LightGreen, PeachPuff, Wheat
+html name color list = Blue, DarkCyan, DarkGoldenRod, Purple, DarkGreen, Orange, Sienna
 
 # The background color of the thread in replies
 
 thread background = HoneyDew
-me thread background = AliceBlue
-them thread background = Lavender
-
-# The color of the name in the html output
-
-me html name color = Blue
-them html name color = Purple
 
 
 [CONTACTS]
 
 # A person that you text with can have multiple numbers, and you may not always want to specify the full specific
 #  number as stored in the handle database, so you can do the mapping here, providing the name of a person,
 #  and a comma separated list of numbers
@@ -104,47 +104,52 @@
    s12ddd2@colt.edu
 Abe: +16103499696
 Marissa: +14029490739
 '''
 
 
 def _create_default_configuration(filename: str) -> None:
-    """Generates a default configuration if one is not passed in
-
-    """
+    """Generates a default configuration if one is not passed in"""
 
     f = open(filename, "w")
     f.write(DEFAULT_CONFIGURATION)
     f.close()
     return
 
 
-def get_contacts(configuration: configparser.ConfigParser) -> dict:
+def _get_contacts(configuration: configparser.ConfigParser) -> dict:
     result = {}
     contact_list = configuration.items('CONTACTS')
     for contact in contact_list:
         key = contact[0]
         value = contact[1]
 
         # Get rid of spaces and newlines
         stripped = value.replace('\n', '').replace(' ', '')
         number_list = stripped.split(',')
         result[key] = number_list
     return result
 
 
 def run() -> None:
+    """ Run the imessagedb command line"""
+
+    out = sys.stdout
+
     logging.basicConfig(level=logging.INFO, format='%(asctime)s <%(name)s> %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
     logger = logging.getLogger('main')
     logger.debug("Processing parameters")
 
     argument_parser = argparse.ArgumentParser()
-    person_mutex_group = argument_parser.add_mutually_exclusive_group()
-    person_mutex_group.add_argument('--handle', help="A list of handles to search against", nargs='*')
-    person_mutex_group.add_argument("--name", help="Person to get conversations about")
+    argument_parser.add_argument("--name", help="Person to get conversations about")
+
+    type_mutex_group = argument_parser.add_mutually_exclusive_group()
+    type_mutex_group.add_argument('--handle', help="A list of handles to search against", nargs='*')
+    type_mutex_group.add_argument('--chat', help="A chat to print")
+
     argument_parser.add_argument("-c", "--configfile", help="Location of the configuration file",
                                  default=f'{os.environ["HOME"]}/.config/iMessageDB.ini')
     argument_parser.add_argument("-o", "--output_directory",
                                  help="The output directory where the output and attachments go")
     argument_parser.add_argument("--database", help="The database file to open",
                                  default=f"{os.environ['HOME']}/Library/Messages/chat.db")
     argument_parser.add_argument("-m", "--me", help="The name to use to refer to you", default="Me")
@@ -154,14 +159,18 @@
     copy_mutex_group.add_argument("-f", "--force", help="Force a copy of the attachments", action="store_true")
     copy_mutex_group.add_argument("--no_copy", help="Don't copy the attachments", action="store_true")
     argument_parser.add_argument("--no_attachments", help="Don't process attachments at all", action="store_true")
     argument_parser.add_argument("-v", "--verbose", help="Turn on additional output", action="store_true")
     argument_parser.add_argument('--start_time', help="The start time of the messages in YYYY-MM-DD HH:MM:SS format")
     argument_parser.add_argument('--end_time', help="The end time of the messages in YYYY-MM-DD HH:MM:SS format")
     argument_parser.add_argument('--version', help="Prints the version number", action="store_true")
+    argument_parser.add_argument('--get_handles', '--get-handles',
+                                 help="Display the list of handles in the database and exit", action="store_true")
+    argument_parser.add_argument('--get_chats', '--get-chats',
+                                 help="Display the list of chats in the database and exit", action="store_true")
 
     args = argument_parser.parse_args()
 
     if args.version:
         print(f"imessagedb {__version__}", file=sys.stderr)
         exit(0)
 
@@ -172,35 +181,14 @@
     config.read(args.configfile)
 
     CONTROL = 'CONTROL'
     DISPLAY = 'DISPLAY'
 
     config.set(CONTROL, 'verbose', str(args.verbose))
 
-    if not args.name and not args.handle:
-        argument_parser.print_help(sys.stderr)
-        print("\n ** You must supply either a name or one or more handles")
-        exit(1)
-
-    person = None
-    numbers = None
-
-    if args.handle:
-        numbers = args.handle
-        person = ', '.join(numbers)
-    if args.name:
-        person = args.name
-        contacts = get_contacts(config)
-        if person.lower() not in contacts.keys():
-            logger.error(f"{person} not known. Please edit your contacts list.")
-            argument_parser.print_help()
-            exit(1)
-
-    config.set(CONTROL, 'Person', person)
-
     if args.output_directory:
         config.set(CONTROL, 'copy directory', args.output_directory)
     if args.no_copy:
         config.set(CONTROL, 'copy', 'False')
     if args.output_type:
         config.set(CONTROL, 'output type', args.output_type)
     if args.force:
@@ -229,34 +217,104 @@
             exit(1)
         config.set(CONTROL, 'end time', str(end_date))
     if start_date and end_date and start_date >= end_date:
         argument_parser.print_help(sys.stderr)
         print(f"\n **Start date ({start_date}) must be before end date ({end_date})", file=sys.stderr)
         exit(1)
 
-    out = sys.stdout
+    generic_database_request = False
+    if args.get_handles or args.get_chats:
+        config[CONTROL]['skip attachments'] = 'True'
+        generic_database_request = True
 
-    copy_directory = config[CONTROL].get('copy directory', fallback="/tmp")
-    attachment_directory = f"{copy_directory}/{person}_attachments"
-    config[CONTROL]['attachment directory'] = attachment_directory
-
-    filename = f'{person}.html'
-    out = open(f"{copy_directory}/{filename}", 'w')
-    try:
-        os.mkdir(attachment_directory)
-    except FileExistsError:
-        pass
+    person = None
+    numbers = None
+
+    if not generic_database_request:
+        if args.chat:
+            person = f"chat_{args.chat}"
+        else:
+            if args.handle:
+                numbers = args.handle
+                if args.name:
+                    person = args.name
+                else:
+                    person = ', '.join(numbers)
+            elif args.name:
+                person = args.name
+                contacts = _get_contacts(config)
+                if person.lower() not in contacts.keys():
+                    logger.error(f"{person} not known. Please edit your contacts list.")
+                    argument_parser.print_help()
+                    exit(1)
+                # Get rid of new lines and split it into a list
+                numbers = config['CONTACTS'][person].replace('\n', '').split(',')
+            else:
+                argument_parser.print_help(sys.stderr)
+                print("\n ** You must supply either a name or one or more handles")
+                exit(1)
+
+            config.set(CONTROL, 'Person', person)
+
+        copy_directory = config[CONTROL].get('copy directory', fallback="/tmp")
+        attachment_directory = f"{copy_directory}/{safe_filename(person)}_attachments"
+        config[CONTROL]['attachment directory'] = attachment_directory
+
+        filename = f'{safe_filename(person)}.html'
+        out = open(f"{copy_directory}/{filename}", 'w')
+        try:
+            os.mkdir(attachment_directory)
+        except FileExistsError:
+            pass
+
+    # Connect to the database
 
     database = DB(args.database, config=config)
-    message_list = database.Messages(person, contacts[person.lower()])
+
+    if args.get_handles:
+        print(f"Available handles in the database:\n{database.handles.get_handles()}")
+        sys.exit(0)
+
+    if args.get_chats:
+        print(f"Available chats in the database:\n{database.chats.get_chats()}")
+        sys.exit(0)
+
+    if args.chat:
+        chat_id = args.chat
+        title = args.chat
+        if args.chat in database.chats.chat_names:
+            chats = database.chats.chat_names[args.chat]
+            if len(chats) != 1:
+                error_string = f"You have {len(chats)} chats named {args.chat}, " \
+                               f"but this program can only handle the case where there is one. " \
+                               f"Rename your group and try again."
+                logger.error(error_string)
+                exit(1)
+            chat_id = chats[0].rowid
+            title = args.chat
+        elif args.chat in database.chats.chat_list:
+            chat_id = args.chat
+            if database.chats.chat_list[chat_id].chat_name:
+                title = database.chats.chat_list[chat_id].chat_name
+            else:
+                title = chat_id
+        else:
+            logger.error(f"{args.chat} not recognized as a chat. Run 'imessagedb --get_chats' to get the list of chats")
+            argument_parser.print_help()
+            exit(1)
+
+        message_list = database.Messages('chat', title, chat_id=chat_id)
+    else:
+
+        message_list = database.Messages('person', person, numbers=numbers)
 
     output_type = config[CONTROL].get('output type', fallback='html')
     if output_type == 'text':
-        database.TextOutput(args.me, person, message_list, output_file=out).print()
+        database.TextOutput(args.me, message_list, output_file=out).print()
     else:
-        database.HTMLOutput(args.me, person, message_list, output_file=out)
+        database.HTMLOutput(args.me, message_list, output_file=out)
 
     database.disconnect()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `imessagedb-1.2.9/src/imessagedb/attachment.py` & `imessagedb-1.3.0/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.9/src/imessagedb/attachments.py` & `imessagedb-1.3.0/src/imessagedb/attachments.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,18 @@
             self._copy_directory = self._database.control.get('attachment directory', fallback="/tmp/attachments")
         else:
             self._copy_directory = copy_directory
 
         self._attachment_list = {}
         self._message_join = {}
 
-        # Get the list of all the attachments
+        # Get the list of all the attachments, unless we are skipping them
+
+        if self._database.control.getboolean('skip attachments', fallback=False):
+            return
 
         self._database.connection.execute('select count(rowid)from attachment')
         (row_count_total) = self._database.connection.fetchone()
         row_count_total = row_count_total[0]
 
         self._database.connection.execute('select rowid, filename, mime_type from attachment')
```

### Comparing `imessagedb-1.2.9/src/imessagedb/chat.py` & `imessagedb-1.3.0/src/imessagedb/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,15 +51,20 @@
 
     @property
     def participants(self) -> str:
         """ Returns the participants in the chat """
         strings = []
         for handle_id in self._participants:
             if handle_id in self._database.handles.handles:
-                strings.append(f'{self._database.handles.handles[handle_id].number} ({handle_id})')
+                number = self._database.handles.handles[handle_id].number
+                name = self._database.handles.name_for_number(number)
+                if name is None:
+                    strings.append(f'{number} ({handle_id})')
+                else:
+                    strings.append(f'{name} ({number}):({handle_id})')
             else:
                 strings.append(f'{handle_id}')
         return ', '.join(strings)
 
     def add_participant(self, participant: str):
         """ Add a participant to the chat """
         if participant not in self._participants:
```

### Comparing `imessagedb-1.2.9/src/imessagedb/chats.py` & `imessagedb-1.3.0/src/imessagedb/chats.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 from imessagedb.chat import Chat
 
 
 class Chats:
-    """ All handles in the database """
+    """ All Chats in the database """
 
     def __init__(self, database) -> None:
         """
             Parameters
             ----------
             database : imessagedb.DB
                 An instance of a connected database"""
 
         self._database = database
-        self._chat_list = {}
-        self._chat_identifiers = {}
+        self._chat_list = {}  # Chat list by rowid
+        self._chat_identifiers = {}  # Chat list by identifier
+        self._chat_names = {}  # Chat list by name
 
-        self._get_chats()
+        self._get_chats_from_database()
         return
 
     def __repr__(self) -> str:
         string_array = []
         for i in sorted(self.chat_list):
             string_array.append(str(self.chat_list[i]))
         return '\n'.join(string_array)
 
     def __len__(self) -> int:
         return len(self._chat_list)
 
-    def _get_chats(self) -> None:
+    def _get_chats_from_database(self) -> None:
         self._database.connection.execute('select rowid, chat_identifier, display_name from chat')
         rows = self._database.connection.fetchall()
         for row in rows:
             rowid = row[0]
             chat_identifier = row[1]
             display_name = row[2]
             new_chat = Chat(self._database, rowid, chat_identifier, display_name)
             self.chat_list[new_chat.rowid] = new_chat
+
+            # Add the chat to the chat_identifiers
             if new_chat.chat_identifier in self.chat_identifiers:
-                self.chat_identifiers[new_chat.chat_identifier].append(new_chat)
+                self._chat_identifiers[new_chat.chat_identifier].append(new_chat)
             else:
-                self.chat_identifiers[new_chat.chat_identifier] = [new_chat]
+                self._chat_identifiers[new_chat.chat_identifier] = [new_chat]
+
+            # Add the chat to the chat_names
+            if new_chat.chat_name != "":
+                if new_chat.chat_name in self._chat_names:
+                    self._chat_names[new_chat.chat_name].append(new_chat)
+                else:
+                    self._chat_names[new_chat.chat_name] = [new_chat]
 
         # Add the last chat date to all the chats
         for i in self.chat_list.values():
             select_string = "select " \
                     "datetime(max(message_date)/1000000000 + strftime('%s', '2001-01-01'),'unixepoch','localtime') " \
                     f"from chat_message_join cmj where chat_id = {i.rowid}"
 
@@ -58,16 +68,47 @@
             chat_id = row[0]
             handle_id = row[1]
 
             self.chat_list[row[0]].add_participant(row[1])
 
         return
 
+    def get_chats(self) -> str:
+        """ Return a string with the list of chats in the database"""
+        return_array = []
+        for chat_id in sorted(self._chat_list):
+            chat = self._chat_list[chat_id]
+            chat_name = ""
+            if chat.chat_name and chat.chat_name != '':
+                chat_name = f"{chat.rowid} ({chat.chat_name}):"
+            else:
+                chat_name = f"{chat.rowid}:"
+            chat_string = f"{chat_name} Participants: {chat.participants}, Last Message Sent: {chat.last_message_date}"
+            return_array.append(chat_string)
+        return '\n'.join(return_array)
+
     @property
     def chat_list(self) -> dict:
         """ Return the list of chats by rowid in a dict"""
         return self._chat_list
 
     @property
+    def chat_names(self) -> dict:
+        """ Return the list of chats by rowid in a dict"""
+        return self._chat_names
+
+    @property
     def chat_identifiers(self) -> dict:
         """ Return the list of chats by chat identifier in a dict"""
         return self._chat_identifiers
+
+    def __getitem__(self, item) -> Chat:
+        if item in self._chat_names:
+            return self._chat_names[item]
+
+        if item in self._chat_list:
+            return self._chat_list[item]
+
+        if item in self._chat_identifiers:
+            return self._chat_identifiers[item]
+
+        raise KeyError
```

### Comparing `imessagedb-1.2.9/src/imessagedb/db.py` & `imessagedb-1.3.0/src/imessagedb/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import sqlite3
-import os
 import configparser
+import os
+import sqlite3
 
 import imessagedb
 from imessagedb.attachments import Attachments
-from imessagedb.messages import Messages
-from imessagedb.message import Message
 from imessagedb.chats import Chats
 from imessagedb.handles import Handles
 from imessagedb.html import HTMLOutput
+from imessagedb.messages import Messages
 from imessagedb.text import TextOutput
 
 
 class DB:
     """
     A class to connect to an iMessage database
 
@@ -44,28 +43,28 @@
 
         # Preload some of the data
         self._handles = Handles(self)
         self._chats = Chats(self)
         self._attachment_list = Attachments(self)
         return
 
-    def Messages(self, person: str, numbers: list) -> Messages:
+    def Messages(self, query_type: str, title: str, numbers: list = None, chat_id: str = None) -> Messages:
         """A wrapper to create a Messages class
         """
-        return Messages(self, person, numbers)
+        return Messages(self, query_type, title, numbers=numbers, chat_id=chat_id)
 
-    def HTMLOutput(self, me: str, person: str, message_list: Messages, inline=False, output_file=None) -> HTMLOutput:
+    def HTMLOutput(self, me: str, message_list: Messages, inline=False, output_file=None) -> HTMLOutput:
         """A wrapper to create an HTMLOutput class
         """
-        return HTMLOutput(self, me, person, message_list, inline, output_file)
+        return HTMLOutput(self, me, message_list, inline, output_file)
 
-    def TextOutput(self, me: str, person: str, message_list: Messages, output_file=None) -> TextOutput:
+    def TextOutput(self, me: str, message_list: Messages, output_file=None) -> TextOutput:
         """A wrapper to create a TextOutput class
         """
-        return TextOutput(self, me, person, message_list, output_file)
+        return TextOutput(self, me, message_list, output_file)
 
     def disconnect(self) -> None:
         """Disconnects from the database
 
         """
         self._chat_connection.close()
         return
```

### Comparing `imessagedb-1.2.9/src/imessagedb/default.ini` & `imessagedb-1.3.0/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.9/src/imessagedb/handle.py` & `imessagedb-1.3.0/src/imessagedb/handle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 
 class Handle:
     """ Class for holding information about a Handle """
 
-    def __init__(self, database, rowid: str, number: str, service: str) -> None:
+    def __init__(self, database, rowid: str, name: str, number: str, service: str) -> None:
         """
             Parameters
             ----------
             database : imessagedb.DB
                 An instance of a connected database
 
             rowid, number, service : str
-                The parameters are the fields in the database"""
+                The parameters are the fields in the database
+
+            name : str
+                A name to associate with it, from the contacts list"""
 
         self._database = database
         self._rowid = rowid
         self._number = number
         self._service = service
-        self._name = "Unknown"
+        self._name = name.title()
 
     def __repr__(self) -> str:
-        return f'{self._rowid}: ID => {self._number}, Service => {self._service}, Name => {self._name}'
+        return f'{self._rowid}: Name => {self._name}, ID => {self._number}, Service => {self._service} '
 
     @property
     def rowid(self) -> str:
         return self._rowid
 
     @property
     def number(self) -> str:
```

### Comparing `imessagedb-1.2.9/src/imessagedb/html.py` & `imessagedb-1.3.0/src/imessagedb/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,16 @@
 from datetime import datetime
 import re
+import string
 import imessagedb
 from imessagedb.message import Message
 from imessagedb.messages import Messages
 from alive_progress import alive_bar
 
 
-def _generate_thread_row(message: Message) -> str:
-    if message.is_from_me:
-        style = 'me'
-    else:
-        style = 'them'
-
-    text = message.text
-    row_string = f'{" ":16s}<tr>\n' \
-                 f'{" ":18s}<td class="reply_text_thread">\n' \
-                 f'{" ":20s}<a href="#{message.rowid}">\n' \
-                 f'{" ":22s}<button class="reply_text_{style}"> {text}</button>\n' \
-                 f'{" ":20s}</a>\n' \
-                 f'{" ":18s}</td>\n' \
-                 f'{" ":16s}</tr>\n'
-    return row_string
-
-
-def _generate_thread_table(message_list: list, style: str) -> str:
-    table_string = f'{" ":14s}<table class="thread_table_{style}">\n'
-    for message in message_list:
-        table_string = f'{table_string}{_generate_thread_row(message)}'
-    table_string = f'{table_string}' \
-                   f'{" ":14s}</table>\n' \
-                   f'{" ":14s}<p>\n'
-    return table_string
-
-
 url_pattern = re.compile(r"((https?):((//)|(\\\\))+[\w\d:#@%/;$()~_?\+-=\\\.&]*)", re.MULTILINE | re.UNICODE)
 mailto_pattern = re.compile(r"([\w\-\.]+@(\w[\w\-]+\.)+[\w\-]+)", re.MULTILINE | re.UNICODE)
 
 
 def _replace_url_to_link(value: str) -> str:
     """ From https://gist.github.com/guillaumepiot/4539986 """
 
@@ -70,81 +44,75 @@
                 If inline attachments are true, then the images will be part of the HTML. If
                 it is false, then there will be a popup when you hover over the attachment text that will show
                 the attachment on demand. This will make the load much faster and the output far less cluttered.
 
     me = Me :
                 The name to put for your part of the conversation. It defaults to 'Me'.
 
-    me html background color = AliceBlue
-    them html background color = Lavender :
-                The background color of the text messages for you and for the other person.
-                The options for colors can be found here: https://www.w3schools.com/cssref/css_colors.php
-
-
-    thread background = HoneyDew
-    me thread background = AliceBlue
-    them thread background = Lavender :
-                The background color of the thread in replies
-
-    me html name color = Blue
-    them html name color = Purple :
-                The color of the name
+    html background color list = AliceBlue, Cyan, Gold, Lavender, LightGreen, PeachPuff, Wheat
+    html name color list = Blue, DarkCyan, DarkGoldenRod, Purple, DarkGreen, Orange, Sienna :
+        The background and name color of the messages in html output
+        The options for colors can be found here: https://www.w3schools.com/cssref/css_colors.php
+
+        The way that the color selection works is that it will use the first color on the color list for the
+        first person in the conversation, the second for the second, third for the third, etc. If there are more
+        participants than colors, it will wrap around to the first color.
 
+    thread background = HoneyDew :
+        The background color of the thread in replies
     """
 
-    def __init__(self, database, me: str, person: str, message_list: Messages,
-                 inline=False, output_file=None) -> None:
+    def __init__(self, database, me: str, messages: Messages, inline=False, output_file=None) -> None:
         """
             Parameters
             ----------
             database : imessagedb.DB
                 An instance of a connected database
 
             me : str
                 Your display name
 
-            person : str
-                The name of the person in the conversation
-
-            message_list: imessagedb.DB.Messages
+            messages: imessagedb.DB.Messages
                  The messages
 
             inline : bool
                 Display attachments inline or not
 
             output_filename : str
                 The name of the output file"""
 
         self._database = database
         self._me = me
-        self._person = person
-        self._message_list = message_list
+        self._messages = messages
         self._attachment_list = self._database.attachment_list
         self._inline = inline
         self._output_file = output_file
 
+        self._name_map = {}
+        self._color_list = self._get_next_color()
         self._day = 'UNK'
         self._html_array = []
         self._print_and_save(self._generate_head(), self._html_array)
         self._print_and_save("<body>\n", self._html_array)
 
         start_time = self._database.control.get('start time', fallback=None)
         end_time = self._database.control.get('end time', fallback=None)
         date_string = ""
         if start_time:
             date_string = f"from {start_time} "
         if end_time:
             date_string = f"{date_string} until {end_time}"
 
-        self._print_and_save(f"Exchanged {len(self._message_list):,} messages with {self._person} {date_string}<p>\n",
+        self._print_and_save(f"Exchanged {len(self._messages):,} messages with " +
+                             f"{self._messages.title} {date_string}<p>\n",
                              self._html_array)
         self._print_and_save(f'{" ":2s}<div class="picboxframe"  id="picbox"> <img src="" /> </div>\n',
                              self._html_array)
 
-        self._html_array.append(self._generate_table(self._message_list))
+        self._html_array.append(self._generate_table(self._messages))
         self._print_and_save('</body>\n</html>\n',
                              self._html_array)
 
     def __repr__(self) -> str:
         return ''.join(self._html_array)
 
     def save(self) -> None:
@@ -159,14 +127,42 @@
 
     def _print_and_save(self, message: str, array: list) -> None:
         """ Save to the output file while it is processing """
         array.append(message)
         if self._output_file:
             print(message, end="", file=self._output_file)
 
+    def _generate_thread_row(self, message: Message) -> str:
+        who_data = self._get_name(message.handle_id)
+        who = who_data['name']
+        style = who_data['style']
+
+        text = message.text
+        row_string = f'{" ":16s}<tr>\n' \
+                     f'{" ":18s}<td class="reply_name" style="color: {who_data["name_color"]};"> ' \
+                     f'{who_data["name"]}: </td>\n' \
+                     f'{" ":18s}<td class="reply_text_thread">\n' \
+                     f'{" ":20s}<a href="#{message.rowid}">\n' \
+                     f'{" ":22s}<button class="reply_text_{style}" style="background: ' \
+                     f'{who_data["background_color"]};"> ' \
+                     f'{text}</button>\n' \
+                     f'{" ":20s}</a>\n' \
+                     f'{" ":18s}</td>\n' \
+                     f'{" ":16s}</tr>\n'
+        return row_string
+
+    def _generate_thread_table(self, message_list: list, style: str) -> str:
+        table_string = f'{" ":14s}<table class="thread_table_{style}">\n'
+        for message in message_list:
+            table_string = f'{table_string}{self._generate_thread_row(message)}'
+        table_string = f'{table_string}' \
+                       f'{" ":14s}</table>\n' \
+                       f'{" ":14s}<p>\n'
+        return table_string
+
     def _generate_table(self, message_list: Messages) -> str:
         table_array = []
         self._print_and_save(f'{" ":2s}<table class="main_table">\n', table_array)
 
         previous_day = ''
 
         message_count = 0
@@ -189,41 +185,74 @@
                     bar()
                 else:
                     bar(skipped=True)
 
         self._print_and_save(f'{" ":2s}</table>\n', table_array)
         return ''.join(table_array)
 
+    def _get_next_color(self):
+        """ A generator function to return the next color"""
+
+        counter = -1
+        default_background_color_list = 'AliceBlue, Cyan, Gold, Lavender, LightGreen, PeachPuff, Wheat'
+        default_name_color_list = 'Blue, DarkCyan, DarkGoldenRod, Purple, DarkGreen, Orange, Sienna'
+        background_color_list = self._database.config.get('DISPLAY', 'html background color list',
+                                                          fallback=default_background_color_list)
+        name_color_list = self._database.config.get('DISPLAY', 'html name color list',
+                                                    fallback=default_name_color_list)
+
+        background_colors = background_color_list.translate({ord(c): None for c in string.whitespace}).split(',')
+        name_colors = name_color_list.translate({ord(c): None for c in string.whitespace}).split(',')
+
+        while True:
+            counter += 1
+            yield [background_colors[counter % len(background_color_list)],
+                   name_colors[counter % len(name_color_list)]]
+
+    def _get_name(self, handle_id: str) -> dict:
+        if handle_id not in self._name_map:
+            (background_color, name_color) = next(self._color_list)
+            handle_list = self._database.handles.handles
+            if handle_id == 0:  # 0 is me
+                self._name_map[handle_id] = {'name': self._me, 'background_color': background_color,
+                                             'name_color': name_color, 'style': 'me'}
+            elif handle_id in handle_list:
+                handle = handle_list[handle_id]
+                self._name_map[handle_id] = {'name': handle.name, 'background_color': background_color,
+                                             'name_color': name_color, 'style': 'them'}
+            else:
+                self._name_map[handle_id] = {'name': handle_id, 'background_color': background_color,
+                                             'name_color': name_color, 'style': 'them'}
+
+        return self._name_map[handle_id]
+
     def _generate_row(self, message: Message) -> str:
         # Specify if the message is from me, or the other person
-        if message.is_from_me:
-            who = self._me
-            style = 'me'
-        else:
-            who = self._person
-            style = 'them'
+        who_data = self._get_name(message.handle_id)
+        who = who_data['name']
+        style = who_data['style']
 
         # Check to see if we want the media box floating or fixed
         floating_option = self._database.config['DISPLAY'].get('popup location', fallback='floating')
         floating = floating_option == 'floating'
 
         # If this message is part of a thread, then show the messages in the thread before it
         thread_table = ""
         if message.thread_originator_guid:
-            if message.thread_originator_guid in self._message_list.guids:
-                original_message = self._message_list.guids[message.thread_originator_guid]
+            if message.thread_originator_guid in self._messages.guids:
+                original_message = self._messages.guids[message.thread_originator_guid]
                 thread_list = original_message.thread
                 thread_list[original_message.rowid] = original_message
                 print_thread = []
                 # sort the threads by the date sent
                 for i in sorted(thread_list.values(), key=lambda x: x.date):
-                    if i == message: # stop at the current message
+                    if i == message:  # stop at the current message
                         break
                     print_thread.append(i)
-                thread_table = _generate_thread_table(print_thread, style)
+                thread_table = self._generate_thread_table(print_thread, style)
 
         # Generate the attachment string
         attachments_string = ""
         if message.attachments:
             for attachment_key in message.attachments:
                 if attachment_key not in self._attachment_list.attachment_list:
                     attachments_string = f'{attachments_string} <span class="missing"> Attachment missing </span> '
@@ -299,15 +328,14 @@
 
         text = _replace_url_to_link(f'{message.text} {attachments_string}')
 
         # Check for edits on the text. If there are edits, then set up the html to allow for that. The row
         #   doesn't exist if there is no edits
 
         edited_string = ""
-        edit_table = ""
         text_cell_edit_row = ""
 
         if len(message.edits) > 0:
             edit_table = f'{" ":14s}<div class="edits_{style}">\n'
             for i in range(0, len(message.edits)):
                 edit_table = f'{edit_table}{" ":16s}"{message.edits[i]["text"]} <p>\n'
             edit_table = f'{edit_table}{" ":14s}</div>\n'
@@ -333,21 +361,21 @@
                         f'{" ":12s}</td>\n'
             info_button = f'{" ":12s}<td class="button-wrapper"> <button class="text_{style}" ' \
                           f'onclick="ToggleDisplay(\'{message.rowid}info\')"> ℹ️ </button> </td>\n'
 
         # Put together the row cells
 
         date_cell = f'{" ":6s}<td class="date"> {self._day} {message.date} </td>\n'
-        name_cell = f'{" ":6s}<td class="name_{style}"> {who}: </td>\n'
+        name_cell = f'{" ":6s}<td class="name_{style}" style="color: {who_data["name_color"]};"> {who}: </td>\n'
 
         text_cell = f'{" ":6s}<td>\n ' \
                     f'{" ":8s}<table>\n' \
                     f'{text_cell_edit_row}' \
                     f'{" ":10s}<tr>\n' \
-                    f'{" ":12s}<td class="text_{style}">\n' \
+                    f'{" ":12s}<td class="text_{style}" style="background: {who_data["background_color"]};">\n' \
                     f'{thread_table}' \
                     f'{" ":14s}{text} {edited_string}\n' \
                     f'{" ":12s}</td>\n' \
                     f'{info_text}' \
                     f'{info_button}' \
                     f'{" ":10s}</tr>\n' \
                     f'{" ":8s}</table>\n' \
@@ -364,28 +392,16 @@
     def _generate_head(self) -> str:
         popup = self._database.config['DISPLAY'].get('popup location', fallback='upper right')
         if popup == 'upper right':
             popup_location = 'right'
         else:
             popup_location = 'left'
 
-        me_html_background_color = self._database.config['DISPLAY'].get('me html background_color',
-                                                                        fallback='AliceBlue')
-        them_html_background_color = self._database.config['DISPLAY'].get('them html background color',
-                                                                          fallback='Lavender')
         thread_background_color = self._database.config['DISPLAY'].get('thread background',
                                                                        fallback='HoneyDew')
-        me_thread_background_color = self._database.config['DISPLAY'].get('me thread background',
-                                                                          fallback='AliceBlue')
-        them_thread_background_color = self._database.config['DISPLAY'].get('them thread background',
-                                                                            fallback='Lavender')
-        me_html_name_color = self._database.config['DISPLAY'].get('me html name color',
-                                                                  fallback='Blue')
-        them_html_name_color = self._database.config['DISPLAY'].get('them html name color',
-                                                                    fallback='Purple')
 
         css = '''    <style>
 table {''' + f'''
     width: 100%;
     table-layout: auto;
 ''' + ''' }
 
@@ -424,48 +440,44 @@
     vertical-align: text-middle;
     font-size: 80%;
 ''' + ''' }
 
 td.name_me {''' + f'''
     text-align: right;
     font-weight: bold;
-    color: {me_html_name_color};
     width: 50px;
     padding-right: 5px;
     vertical-align: text-middle;
     font-size: 80%;
     
 ''' + ''' }
 
 td.name_them {''' + f'''
     text-align: right;
     font-weight: bold;
-    color: {them_html_name_color};
     width: 50px;
     padding-right: 5px;
     vertical-align: text-middle;
     font-size: 80%;
 ''' + ''' }
 
 td.text_me {''' + f'''
     text-align: right;
     word-wrap: break-word;
     border-radius: 30px;
     padding: 15px;
     border-spacing: 40px;
-    background: {me_html_background_color};  
 ''' + ''' }
 
 td.text_them {''' + f'''
     text-align: left;
     word-wrap: break-word;
     border-radius: 30px;
     padding: 15px;
     border-spacing: 40px;
-    background: {them_html_background_color};
 ''' + ''' }
 
 .edits_me {''' + f'''
     display: none;
     font-size: 70%;
     font-style: italics;
     text-align: right;
@@ -514,60 +526,53 @@
     border-spacing: 0px;
     text-align: center;
     width:0.1%;
     background-color: transparent; 
 ''' + ''' }
 
 button.text_me {''' + f'''
-    background: {me_html_background_color};
     border-radius: 30px;
     font-size: 50%;
     padding-left: 0px;
     padding-right: 0px;
     border-spacing: 0px;
     border-bottom: 0px;
     margin-right: 0px;
     margin-left: 0px;
     text-align: center;
     border: 0px;
 ''' + ''' }
 
 button.text_them {''' + f'''
-    background: {them_html_background_color};
     border-radius: 30px;
     font-size: 50%;
     padding-left: 0px;
     padding-right: 0px;
     border-spacing: 0px;
     border-bottom: 0px;
     margin-right: 0px;
     margin-left: 0px;
     text-align: center;
     border: 0px;
 ''' + ''' }
 
-reply_text_thread {''' + f'''
-    border: 2px solid;
-    background: {thread_background_color};
-    border-radius: 6px;
-    border-radius: 50px;
-    font-size: 60%
-''' + ''' }
+.reply_name {
+    font-size: 50%; 
+    text-align: right;
+}
 
 .reply_text_me {''' + f'''
     border: 2px solid;
-    background: {me_thread_background_color};
     border-radius: 6px;
     border-radius: 50px;
     font-size: 60%
 ''' + ''' }
 
 .reply_text_them {''' + f'''
     border: 2px solid;
-    background: {them_thread_background_color};
     border-radius: 6px;
     border-radius: 50px;
     font-size: 60%
 ''' + ''' }
 
 td.blank {''' + f'''
     border: none;
@@ -648,9 +653,9 @@
   </script>'''
 
         head_string = '''<!DOCTYPE html>
 <html lang="en-US">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     ''' \
-                      f'    <title> {self._person} </title>\n{css}\n{script}\n</head>\n'
+                      f'    <title> {self._messages.title} </title>\n{css}\n{script}\n</head>\n'
         return head_string
```

### Comparing `imessagedb-1.2.9/src/imessagedb/message.py` & `imessagedb-1.3.0/src/imessagedb/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         text = text.split(b'\x86')[0]
     return text.decode('utf-8', errors='replace')
 
 
 class Message:
     """ Class for holding information about a message """
 
-    def __init__(self, database, rowid: int, guid: str, date: str, is_from_me: bool, handle_id: int,
+    def __init__(self, database, rowid: int, guid: str, date: str, is_from_me: bool, handle_id: str,
                  attributed_body: bytes, message_summary_info: bytes, text: str, reply_to_guid: str,
-                 thread_originator_guid: str, thread_originator_part: str, chat_id: int, message_attachments: list):
+                 thread_originator_guid: str, thread_originator_part: str, chat_id: str, message_attachments: list):
         """
                 Parameters
                 ----------
                 database : imessagedb.DB
                     An instance of a connected database
 
                 rowid, guid, date, is_from_me, handle_id, attributed_body, message_summary_info, text,
```

### Comparing `imessagedb-1.2.9/src/imessagedb/messages.py` & `imessagedb-1.3.0/src/imessagedb/messages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,107 @@
 from imessagedb.utils import *
 from alive_progress import alive_bar
 from imessagedb.message import Message
 
 
 class Messages:
     """ All messages in a conversation or conversations with a particular person """
-    def __init__(self, database, person: str, numbers: list) -> None:
+
+    def __init__(self, database, query_type: str, title: str, numbers: list = None, chat_id: str = None) -> None:
         """
                 Parameters
                 ----------
                 database : imessagedb.DB
                     An instance of a connected database
 
-                person : str
-                    The name of the person in the conversation
+                query_type : str
+                    The type of messages, either 'person' or 'chat'
+
+                title : str
+                    The name of the conversation
 
-                numbers: list
+                numbers : list
                     A list of numbers associated with the person, as represented in the handle data table
 
+                chat_id : str
+                    The id of the chat
                 """
+
         self._database = database
-        self._person = person
+        self._query_type = query_type
         self._numbers = numbers
+        self._chat_id = chat_id
+        self._title = title
         self._guids = {}
         self._message_list = {}
 
-        numbers_string = "','".join(self._numbers)
         time_rules = []
         time_where_clause = ""
         start_time = self._database.control.get('start time', fallback=None)
         end_time = self._database.control.get('end time', fallback=None)
         if start_time:
             database_start_date = convert_to_database_date(start_time)
             time_rules.append(f"message.date >= {database_start_date}")
         if end_time:
             database_end_date = convert_to_database_date(end_time)
             time_rules.append(f"message.date <= {database_end_date}")
         if len(time_rules) > 0:
             time_where_clause = f" and {' AND '.join(time_rules)}"
 
-        where_clause = "rowid in (" \
-                       " select message_id from chat_message_join where chat_id in (" \
-                       "  select chat_id from chat_handle_join where handle_id in (" \
-                       f"   select rowid from handle where id in ('{numbers_string}')" \
-                       "  )" \
-                       " )" \
-                       f") {time_where_clause}"
-        select_string = "select message.rowid, guid, " \
-                        "datetime(message.date/1000000000 + strftime('%s', '2001-01-01'),'unixepoch','localtime'), " \
-                        "message.is_from_me, message.handle_id, " \
-                        " message.attributedBody, message.message_summary_info, message.text, " \
-                        "reply_to_guid, thread_originator_guid, thread_originator_part, cmj.chat_id  " \
-                        "from message, chat_message_join cmj " \
-                        f"where message.rowid = cmj.message_id and {where_clause} " \
-                        "order by message.date asc"
+        if self._query_type == "person":
+            numbers_string = "','".join(self._numbers)
+            where_clause = "rowid in (" \
+                           " select message_id from chat_message_join where chat_id in (" \
+                           "  select chat_id from chat_handle_join where handle_id in (" \
+                           f"   select rowid from handle where id in ('{numbers_string}')" \
+                           "  )" \
+                           " )" \
+                           f") {time_where_clause}"
+            select_string = "select message.rowid, guid, " \
+                            "datetime(message.date/1000000000 + strftime('%s', '2001-01-01'),'unixepoch','localtime'), " \
+                            "message.is_from_me, message.handle_id, " \
+                            " message.attributedBody, message.message_summary_info, message.text, " \
+                            "reply_to_guid, thread_originator_guid, thread_originator_part, cmj.chat_id  " \
+                            "from message, chat_message_join cmj " \
+                            f"where message.rowid = cmj.message_id and {where_clause} " \
+                            "order by message.date asc"
+
+        elif self._query_type == "chat":
+            where_clause = f"rowid in (select message_id from chat_message_join where chat_id = {self._chat_id}) " \
+                           f" {time_where_clause}"
+            select_string = "select message.rowid, guid, " \
+                            "datetime(message.date/1000000000 + strftime('%s', '2001-01-01'),'unixepoch','localtime'), " \
+                            "message.is_from_me, message.handle_id, " \
+                            " message.attributedBody, message.message_summary_info, message.text, " \
+                            "reply_to_guid, thread_originator_guid, thread_originator_part, cmj.chat_id  " \
+                            "from message, chat_message_join cmj " \
+                            f"where message.rowid = cmj.message_id and {where_clause} " \
+                            "order by message.date asc"
+
+        else:
+            raise KeyError
+
         row_count_string = f"select count (*) from message where {where_clause}"
 
         self._database.connection.execute(row_count_string)
         (row_count_total) = self._database.connection.fetchone()
         row_count_total = row_count_total[0]
 
         self._database.connection.execute(select_string)
 
         i = self._database.connection.fetchone()
+        skip_attachment = self._database.control.getboolean('skip attachments', fallback=False)
 
         with alive_bar(row_count_total, title="Getting Messages", stats="({rate}, eta: {eta})") as bar:
             message_count = 0
             while i:
                 (rowid, guid, date, is_from_me, handle_id, attributed_body, message_summary_info, text,
                  reply_to_guid, thread_originator_guid, thread_originator_part, chat_id) = i
                 message_count = message_count + 1
 
-                skip_attachment = self._database.control.getboolean('skip attachments', fallback=False)
                 attachment_list = None
                 if not skip_attachment:
                     if rowid in self._database.attachment_list.message_join:
                         attachment_list = self._database.attachment_list.message_join[rowid]
 
                 skipped = True
 
@@ -99,12 +125,16 @@
         """ Returns a list of messages sorted by the date of the message"""
         return self._sorted_message_list
 
     @property
     def guids(self) -> dict:
         return self._guids
 
+    @property
+    def title(self) -> str:
+        return self._title
+
     def __iter__(self):
         return self._sorted_message_list.__iter__()
 
     def __len__(self) -> int:
         return len(self._sorted_message_list)
```

### Comparing `imessagedb-1.2.9/PKG-INFO` & `imessagedb-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.9
+Version: 1.3.0
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,25 @@
 
 If you specify html output, `imessagedb` will copy your attachments so that they are accessible
 to the web browser. In addition, it will convert certain types of attachments so that they 
 can be viewed in the browser. For instance, it will convert HEIC files to PNG so that they 
 browser can display it, and will convert various type of movie files to mp4 and various audio
 files to mp3. If you have many attachments, this can take a long time and take a lot of space. 
 
+### Example Output
+
+This is what the default html version looks like. Note that I am hovering over one of the
+links to show the image.
+
+![](JulioHtml.png)
+
+This is the same conversation rendered in text.
+
+![](JulioText.png)
+
 ### Command Line
 
 ```python
 imessagedb [-h] [--handle [HANDLE ...] | --name NAME] [-c CONFIGFILE]
                [-o OUTPUT_DIRECTORY] [--database DATABASE] [-m ME]
                [-t {text,html}] [-i] [-f | --no_copy] [--no_attachments] [-v]
                [--start_time START_TIME] [--end_time END_TIME]
@@ -78,16 +89,17 @@
   --no_attachments      Don't process attachments at all
   -v, --verbose         Turn on additional output
   --start_time START_TIME
                         The start time of the messages in YYYY-MM-DD HH:MM:SS
                         format
   --end_time END_TIME   The end time of the messages in YYYY-MM-DD HH:MM:SS
                         format
-
-
+  --version             Show the version number and exit
+  --get_handles         Display the list of handles in the database and exit
+  --get_chats           Display the list of chats in the database and exit
 ```
 
 #### Command line options
 
 **-h** prints a help message                                                                        |
 
 **--handle [HANDLE ...]**  A list of handles to search against. 
@@ -134,14 +146,17 @@
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
 **--version**  Shows the version number and exits
 
 
+**--get_handles** Display the list of handles in the database and exit
+
+**--get_chats** Display the list of chats in the database and exit
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
 
 ```python
 [CONTROL]
@@ -246,8 +261,11 @@
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 
 `imessagedb` was created by Xev Gittler. It is licensed under the terms of the MIT license.
 
+## Documentation
+
+Full documentation available at https://imessagedb.readthedocs.io/en/latest/
```

