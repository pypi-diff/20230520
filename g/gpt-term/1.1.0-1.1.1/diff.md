# Comparing `tmp/gpt-term-1.1.0.tar.gz` & `tmp/gpt-term-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.1.0.tar", last modified: Thu May 18 13:34:43 2023, max compression
+gzip compressed data, was "gpt-term-1.1.1.tar", last modified: Sat May 20 13:58:39 2023, max compression
```

## Comparing `gpt-term-1.1.0.tar` & `gpt-term-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.660858 gpt-term-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 13:34:31.000000 gpt-term-1.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-18 13:34:31.000000 gpt-term-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 13:34:31.000000 gpt-term-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-18 13:34:43.656858 gpt-term-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/README.assets/
--rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.assets/image-20230303233352970.png
--rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.assets/small.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.zh-CN.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-18 13:34:31.000000 gpt-term-1.1.0/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term/locale/
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.de.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.en.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.jp.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.zh_CN.yml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47638 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-18 13:34:31.000000 gpt-term-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-18 13:34:31.000000 gpt-term-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:34:43.660858 gpt-term-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.679308 gpt-term-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.683308 gpt-term-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-20 13:58:28.000000 gpt-term-1.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-20 13:58:28.000000 gpt-term-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 13:58:28.000000 gpt-term-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-20 13:58:39.687308 gpt-term-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.683308 gpt-term-1.1.1/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-20 13:58:28.000000 gpt-term-1.1.1/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.de.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.en.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.jp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.zh_CN.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48431 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-20 13:58:28.000000 gpt-term-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 13:58:28.000000 gpt-term-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:58:39.687308 gpt-term-1.1.1/setup.cfg
```

### Comparing `gpt-term-1.1.0/.github/workflows/pypi-publish.yml` & `gpt-term-1.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.0/LICENSE` & `gpt-term-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.0/PKG-INFO` & `gpt-term-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,16 +51,26 @@
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
+### Related Projects
+
+[GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
+
+[gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
+
 ## Changelog
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
 ### 2023-05-18
 
 - Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 
 <details>
   <summary>More Change log</summary>
 
@@ -122,14 +132,16 @@
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
    ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
 2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
+   **Attention: Try not to use the Python that comes with the system (including Windows 11 app store version and MacOS pre-installed Python), otherwise the gpt-term command will not be found after installation ([#38](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/38))**
+
 ## Installation
 
 
 1. Install `GPT-Term` using `pip`
 
    ```shell
    pip3 install gpt-term
@@ -157,14 +169,20 @@
 
 Run with the following command:
 
 ```shell
 gpt-term
 ```
 
+Or:
+
+```shell
+python3 -m gpt_term
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
@@ -173,28 +191,31 @@
 - `Ctrl+K`: Delete all characters to the right of the cursor
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
-| Arguments     | Description                     | Example                                       |
-| ------------- | ------------------------------- | --------------------------------------------- |
-| -h, --help    | show this help message and exit | `gpt-term --help`                             |
-| --load FILE   | Load chat history from file     | `gpt-term --load chat_history_code_check.json` |
-| --key API_KEY | choose the API key to load      | `gpt-term --key OPENAI_API_KEY1`              |
-| --model MODEL | choose the AI model to use      | `gpt-term --model gpt-3.5-turbo`              |
-| -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
-| -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
-| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
-| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
-| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
-| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
-| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
-| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
+| Arguments | Description | Examples |
+| ------------- | --------------------------------- | - ----------------------------------------------- |
+| -h, --help | show this help message and exit | `gpt-term --help` |
+| --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
+| --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
+| --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
+| --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
+| -m, --multi | Enable multiline mode | `gpt-term --multi` |
+| -r, --raw | Enable raw mode | `gpt-term --raw` |
+| -l, --lang LANG | Set the current running language: en, zh_CN, jp, de | `gpt-term --lang en` |
+| --set-host HOST | Set API Host address (this is usually used to configure proxy) | `gpt-term --set-host https://closeai.deno.dev` |
+| --set-apikey KEY | Set OpenAI API key | `gpt-term --set-apikey sk-xxx` |
+| --set-timeout SEC | Set the maximum wait time for API requests | `gpt-term --set-timeout 10` |
+| --set-gentitle BOOL | Set whether to auto-generate title for chat | `gpt-term --set-gentitle True` |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL | Set log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG` |
+| --set-lang LANG | Set language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
```

### Comparing `gpt-term-1.1.0/README.assets/image-20230303233352970.png` & `gpt-term-1.1.1/README.assets/image-20230303233352970.png`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.0/README.assets/small.gif` & `gpt-term-1.1.1/README.assets/small.gif`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.0/README.md` & `gpt-term-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,26 @@
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
+### Related Projects
+
+[GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
+
+[gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
+
 ## Changelog
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
 ### 2023-05-18
 
 - Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 
 <details>
   <summary>More Change log</summary>
 
@@ -86,14 +96,16 @@
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
    ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
 2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
+   **Attention: Try not to use the Python that comes with the system (including Windows 11 app store version and MacOS pre-installed Python), otherwise the gpt-term command will not be found after installation ([#38](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/38))**
+
 ## Installation
 
 
 1. Install `GPT-Term` using `pip`
 
    ```shell
    pip3 install gpt-term
@@ -121,14 +133,20 @@
 
 Run with the following command:
 
 ```shell
 gpt-term
 ```
 
+Or:
+
+```shell
+python3 -m gpt_term
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
@@ -137,28 +155,31 @@
 - `Ctrl+K`: Delete all characters to the right of the cursor
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
-| Arguments     | Description                     | Example                                       |
-| ------------- | ------------------------------- | --------------------------------------------- |
-| -h, --help    | show this help message and exit | `gpt-term --help`                             |
-| --load FILE   | Load chat history from file     | `gpt-term --load chat_history_code_check.json` |
-| --key API_KEY | choose the API key to load      | `gpt-term --key OPENAI_API_KEY1`              |
-| --model MODEL | choose the AI model to use      | `gpt-term --model gpt-3.5-turbo`              |
-| -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
-| -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
-| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
-| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
-| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
-| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
-| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
-| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
+| Arguments | Description | Examples |
+| ------------- | --------------------------------- | - ----------------------------------------------- |
+| -h, --help | show this help message and exit | `gpt-term --help` |
+| --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
+| --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
+| --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
+| --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
+| -m, --multi | Enable multiline mode | `gpt-term --multi` |
+| -r, --raw | Enable raw mode | `gpt-term --raw` |
+| -l, --lang LANG | Set the current running language: en, zh_CN, jp, de | `gpt-term --lang en` |
+| --set-host HOST | Set API Host address (this is usually used to configure proxy) | `gpt-term --set-host https://closeai.deno.dev` |
+| --set-apikey KEY | Set OpenAI API key | `gpt-term --set-apikey sk-xxx` |
+| --set-timeout SEC | Set the maximum wait time for API requests | `gpt-term --set-timeout 10` |
+| --set-gentitle BOOL | Set whether to auto-generate title for chat | `gpt-term --set-gentitle True` |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL | Set log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG` |
+| --set-lang LANG | Set language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
```

### Comparing `gpt-term-1.1.0/README.zh-CN.md` & `gpt-term-1.1.1/README.zh-CN.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,26 @@
 
 > 注意，终端需能正常访问外网（配置代理的环境变量）才能运行代码，如系统已开启代理但没有配置终端代理，API 请求就会从国内 IP 发起，可能导致账号停用 ([#2](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/2))
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 默认使用 [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) 模型，也就是 ChatGPT(免费版) 所使用的模型。
 
+### 相关项目
+
+[C/C++实现的GPTerm](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
+
+[可以调用 POE API 的 gpt-term](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
+
 ## 更新记录
 
+### 2023-05-20
+
+- 新增 host 配置项支持，在使用自建 API 反向代理服务器的时候很有用([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49))，你现在可以使用 `gpt-term --set-host HOST` 来配置 host，默认为 https://api.openai.com。
+
 ### 2023-05-18
 
 - 新增多语言支持：英语、中文、日语、德语，默认跟随系统语言，现在可以使用 `/lang` 来切换语言
 
 <details>
   <summary>更多 Change log</summary>
 
@@ -89,14 +99,16 @@
 
    OpenAI 的 API 密钥可在主页右上角点击 "View API keys" 打开的页面中生成，直达链接：https://platform.openai.com/account/api-keys
 
    ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
 2. [Python](https://www.python.org/downloads/) 3.7 或更高版本
 
+   **注意：尽量不要使用系统自带的 Python（包括Windows11 的应用商店版 Python 和 MacOS 的预装 Python），否则会出现安装好后gpt-term 命令找不到的情况 ([#38](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/38))**
+
 ## 安装
 
 1. 使用 `pip` 安装 `GPT-Term`
 
    ```shell
    pip3 install gpt-term
    ```
@@ -124,14 +136,20 @@
 
 使用以下命令运行：
 
 ```shell
 gpt-term
 ```
 
+或者：
+
+```shell
+python3 -m gpt_term
+```
+
 在默认的单行模式下输入提问时，使用 `Esc` + `Enter` 换行，`Enter` 提交
 
 以下是一些常见的快捷键（同时也是shell的快捷键）：
 
 - `Ctrl+_`: 撤消
 - `Ctrl+L`: 清屏，相当于shell中的`clear`命令
 - `Ctrl+C`: 停止当前回答或取消当前输入
@@ -146,18 +164,21 @@
 
 | 选项          | 功能                              | 示例                                          |
 | ------------- | --------------------------------- | --------------------------------------------- |
 | -h, --help    | 显示此帮助信息并退出              | `gpt-term --help`                             |
 | --load FILE   | 从文件中加载聊天记录              | `gpt-term --load chat_history_code_check.json` |
 | --key API_KEY | 选择 config.ini 文件中要使用的 API 密钥 | `gpt-term --key OPENAI_API_KEY1`              |
 | --model MODEL | 选择要使用的 AI 模型              | `gpt-term --model gpt-3.5-turbo`              |
+| --host HOST | 设置在本次运行中使用的 API Host 地址（这通常被用来配置代理） | `gpt-term --host https://closeai.deno.dev`              |
 | -m, --multi   | 启用多行模式                      | `gpt-term --multi`                            |
 | -r, --raw     | 启用原始模式                      | `gpt-term --raw`                              |
+| -l, --lang LANG | 设置本次运行语言：en, zh_CN, jp, de | `gpt-term --lang en` |
+| --set-host HOST        | 设置API Host地址（这通常被用来配置代理）              | `gpt-term --set-host https://closeai.deno.dev` |
 | --set-apikey KEY        | 设置 OpenAI 的 API 密钥                          | `gpt-term --set-apikey sk-xxx` |
-| --set-timeout SEC       | 设置 API 请求的最大等待时间                         | `gpt-term --set-timeout 10` |
+| --set-timeout SEC       | 设置 API 请求的最大等待时间                        | `gpt-term --set-timeout 10` |
 | --set-gentitle BOOL     | 设置是否为聊天自动生成标题                          | `gpt-term --set-gentitle True` |
 | --set-saveperfix PERFIX | 设置聊天历史文件的保存前缀                          | `gpt-term --set-saveperfix chat_history_` |
 | --set-loglevel LEVEL    | 设置日志级别：DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG` |
 | --set-lang LANG    | 设置语言：en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > 多行模式与 raw 模式可以同时使用
```

### Comparing `gpt-term-1.1.0/gpt_term/config.ini` & `gpt-term-1.1.1/gpt_term/config.ini`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,11 @@
 # At the same time, the prefix can also be specified as a directory + / to allow the program to save the chat history in a folder (note that the corresponding folder needs to be created in advance), for example: CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # Log level, default is INFO, available value: DEBUG, INFO, WARNING, ERROR, CRITICAL
 LOG_LEVEL=INFO
 
 # Set the language of the program, the default is empty, it will follow the system language
-LANGUAGE=
+LANGUAGE=
+
+# Set the host of the api, the default is https://api.openai.com
+openai_host=
```

### Comparing `gpt-term-1.1.0/gpt_term/locale/gpt_term.de.yml` & `gpt-term-1.1.1/gpt_term/locale/gpt_term.de.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,16 @@
   usage_getting: "[cyan]Kredit Gebrauch Infos anfordern..."
   usage_granted: "[bold green]Insgesamt gewährt:[/]\t$%{credit_total_granted}"
   usage_used_month: "[bold cyan]Nutzung dieses Monats:[/]\t$%{credit_used_this_month}"
   usage_total: "[bold blue]Insgesamt Nutzung:[/]\t$%{credit_total_used}"
   usage_title: "Kredit Statistik"
   usage_plan: "[bright_blue]Plan: %{credit_plan}"
   #
+  host_set: "[dim]API Host wurde auf '%{new_host}' gesetzt."
+  #
   model_set: "[dim]Leere Eingabe, erhält das Modell '%{old_model}' unverändert."
   model_changed: "[dim]Das Modell wurde von '%{old_model}' auf '%{new_model}' geändert."
   #
   multi_line_enable: "[dim]Multi-Linie-Mode [green]aktiviert[/], pressen [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] einzureichen."
   multi_line_disabled: "[dim]Multi-Linie-Mode [bright_red]deaktiviert[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT denkt nach..."
@@ -97,29 +99,30 @@
   load_file_not: "[bright_red]Datei nicht gefunden: %{file_path}"
   load_json_error: "[bright_red]Ungültiges JSON-Format in der Datei: %{file_path}"
   #
   new_lang_prompt: "Sprache: "
   lang_switch: "[dim]Wechselt zu [bright_magenta]Deutsch[/]."
   lang_config_unsupport: "[red]Nicht unterstützte Sprache in der Konfiguration `%{config_lang}`. Die Sprache des Benutzers wird verwendet."
   lang_unsupport: "[red]Nicht unterstützte Sprache `%{new_lang}`."
-
   #
   upgrade_title: "Neue Version verfügbar: [red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "Verwenden `pip install --upgrade gpt-term` zum Upgrade."
   upgrade_see_git: "Sehen unsere [GitHub Site](https://github.com/xiaoxx970/chatgpt-in-terminal) um zu sehen, was geändert wurde!"
   #
   help_description: "Verwenden ChatGPT im Terminal"
   help_help: "Zeigt diese Hilfemeldung an und beendet sich"
   help_v: "Zeigt die Version des Programms an und beenden"
   help_load: "Chatverlauf aus Datei laden"
   help_key: "Wählen Sie den Namen des API-Schlüssels aus, der aus der Konfigurationsdatei geladen werden soll."
   help_model: "Wählen das zu verwendende AI-Modell"
+  help_host: "Stellen den API Host ein, der in diesem Lauf verwendet werden (wird normalerweise zur Konfiguration des Proxys verwendet)"
   help_m: "Aktivieren den Multi-Linie-Mode"
   help_r: "Aktivieren den Rhomode"
   help_lang: "Sprache wählen"
+  help_set_host: "API Host einstellen (wird normalerweise zur Konfiguration des Proxys verwendet)"
   help_set_key: "API-Schlüssel für OpenAI einstellen"
   help_set_timeout: "Maximale Wartezeit für API-Anfragen einstellen"
   help_set_gentitle: "Festlegen, ob automatisch ein Titel für den Chat generiert werden soll"
   help_set_lang: "Sprache einstellen"
   help_set_saveperfix: "Speicherperfix für die Chatverlaufsdatei einstellen"
   help_set_loglevel: "Log-Stufe einstellen:"
   #
```

### Comparing `gpt-term-1.1.0/gpt_term/locale/gpt_term.en.yml` & `gpt-term-1.1.1/gpt_term/locale/gpt_term.en.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
   usage_getting: "[cyan]Getting credit usage..."
   usage_granted: "[bold green]Total Granted:[/]\t\t$%{credit_total_granted}"
   usage_used_month: "[bold cyan]Used This Month:[/]\t$%{credit_used_this_month}"
   usage_total: "[bold blue]Used Total:[/]\t\t$%{credit_total_used}"
   usage_title: "Credit Summary"
   usage_plan: "[bright_blue]Plan: %{credit_plan}"
   #
+  host_set: "[dim]API Host set to '%{new_host}'."
+  #
   model_set: "[dim]Empty input, the model remains '%{old_model}'."
   model_changed: "[dim]Model has been set from '%{old_model}' to '%{new_model}'."
   #
   multi_line_enabled: "[dim]Multi-line mode [green]enabled[/], press [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] to submit."
   multi_line_disabled: "[dim]Multi-line mode [bright_red]disabled[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT is thinking..."
@@ -108,17 +110,19 @@
   #
   help_description: "Use ChatGPT in terminal"
   help_help: "show this help message and exit"
   help_v: "show program's version number and exit"
   help_load: "Load chat history from file"
   help_key: "Choose the name of API key in config file to load"
   help_model: "Choose the AI model to use"
+  help_host: "Set the API Host to use in this run (usually used to configure proxy)"
   help_m: "Enable multi-line mode"
   help_r: "Enable raw mode"
   help_lang: "Choose language"
+  help_set_host: "Set the API Host to use (usually used to configure proxy)"
   help_set_key: "Set API key for OpenAI"
   help_set_timeout: "Set maximum waiting time for API requests"
   help_set_gentitle: "Set whether to automatically generate a title for chat"
   help_set_lang: "Set language"
   help_set_saveperfix: "Set chat history file's save perfix"
   help_set_loglevel: "Set log level:"
   #
```

### Comparing `gpt-term-1.1.0/gpt_term/locale/gpt_term.jp.yml` & `gpt-term-1.1.1/gpt_term/locale/gpt_term.jp.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
   usage_getting: "[cyan]クレジット使用状況の取得中..."
   usage_granted: "[bold green]合計付与額：[/]\t\t$%{credit_total_granted}"
   usage_used_month: "[bold cyan]今月の使用額：[/]\t$%{credit_used_this_month}"
   usage_total: "[bold blue]合計使用額：[/]\t\t$%{credit_total_used}"
   usage_title: "クレジットの概要"
   usage_plan: "[bright_blue]プラン： %{credit_plan}"
   #
+  host_set: "[dim]APIホストが '%{new_host}' に設定されました。"
+  #
   model_set: "[dim]空の入力です。モデルは'%{old_model}'のままです。"
   model_changed: "[dim]モデルが'%{old_model}'から'%{new_model}'に変更されました。"
   #
   multi_line_enabled: "[dim][green]マルチラインモードが有効になりました[/]、[[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]]を押して送信してください。"
   multi_line_disabled: "[dim][bright_red]マルチラインモードが無効になりました[/]。"
   #
   ChatGPT_thinking: "[bold cyan]ChatGPTが考え中です...[/]"
@@ -92,35 +94,35 @@
   version_name: "バージョン"
   #
   tokens_reached: "トークン制限に達しました。現在のチャットの最初のメッセージを忘れてもよろしいですか？"
   tokens_approaching : "[dim]トークン制限に近づいています：残り%{token_left}トークン"
   #
   load_file_not: "[bright_red]ファイルが見つかりません：%{file_path}"
   load_json_error: "[bright_red]ファイル内の無効なJSON形式です：%{file_path}"
-  
   #
   new_lang_prompt: "言語："
   lang_switch: "[dim]すでに[bright_magenta]日本語[/]に切り替わっています。"
   lang_config_unsupport: "[red]設定でサポートされていない言語 `%{config_lang}` です。ユーザーのローカル言語が使用されます。"
   lang_unsupport: "[red]サポートされていない言語 `%{new_lang}` です。"
-
   #
   upgrade_title: "新しいバージョンが利用可能です：[red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "`pip install --upgrade gpt-term`\nを使用してアップグレードしてください。"
   upgrade_see_git: "変更内容を確認するには、[GitHubサイト](https://github.com/xiaoxx970/chatgpt-in-terminal)を訪問してください！"
   #
   help_description: "ターミナルでChatGPTを使用する"
   help_help: "このヘルプメッセージを表示して終了する"
   help_v: "プログラムのバージョン番号を表示して終了する"
   help_load: "チャット履歴をファイルから読み込む"
   help_key: "設定ファイルから読み込む API キーの名前を選択してください。"
   help_model: "使用するAIモデルを選択する"
+  help_host: "この実行で使用するAPIホストを設定する（通常、プロキシを設定するために使用します。）"
   help_m: "マルチラインモードを有効にする"
   help_r: "ロー モードを有効にする"
   help_lang: "言語を選択する"
+  help_set_host: "使用するAPIホストを設定する（通常、プロキシを設定するために使用します。）"
   help_set_key: "OpenAIのAPIキーを設定する"
   help_set_timeout: "APIリクエストの最大待ち時間を設定する"
   help_set_gentitle: "チャットのタイトルを自動生成するかどうかを設定する"
   help_set_lang: "言語を設定する"
   help_set_saveperfix: "チャット履歴ファイルの保存プレフィックスを設定する"
   help_set_loglevel: "ログレベルを設定する:"
   #
```

### Comparing `gpt-term-1.1.0/gpt_term/locale/gpt_term.zh_CN.yml` & `gpt-term-1.1.1/gpt_term/locale/gpt_term.zh_CN.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 zh_CN:
   welcome: "[dim]你好, 欢迎和 GPT 聊天. 输入`[bright_magenta]/help[/]` 显示可用命令."
   exit: "退出中..."
-  spent_token: "[bright_magenta]已花费的 Token总数:[bold]%{total_tokens_spent}" 
+  spent_token: "[bright_magenta]已花费的 token 总数:[bold]%{total_tokens_spent}" 
   save_api_key: "将 API Key 保存到配置文件中?" 
   input_api_key: "未找到 OpenAI API Key, 请输入:"
   config_key_to_shell_key: "配置项 `[bright_magenta]%{key_word}[/]` 已设置为 [green]%{val}[/]"
   log_level_error: "[dim]无效的日志级别: %{e}，请检查 config.ini文件. 日志级别将设置为 INFO."
   system_prompt: "系统提示词: "
   new_temperature: "新随机值: "
   #
@@ -37,14 +37,16 @@
   usage_getting: "[cyan]正在获取额度使用情况..."
   usage_granted: "[bold green]总授权额度: [/]\t\t$%{credit_total_granted}"
   usage_used_month: "[bold cyan]本月已用: [/]\t\t$%{credit_used_this_month}"
   usage_total: "[bold blue]累计使用: [/]\t\t$%{credit_total_used}"
   usage_title: "额度摘要"
   usage_plan: "[bright_blue]计划: %{credit_plan}"
   #
+  host_set: "[dim]API主机地址已被设为 '%{new_host}'"
+  #
   model_set: "[dim]输入为空，模型保持为 '%{old_model}'."
   model_changed: "[dim]模型已从 '%{old_model}' 修改为 '%{new_model}'."
   #
   multi_line_enabled: "[dim]多行模式[green]已启用[/]，按 [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] 提交." 
   multi_line_disabled: "[dim]多行模式[bright_red]已禁用[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT 正在思考..."
@@ -108,17 +110,19 @@
   #
   help_description: "在终端中使用 ChatGPT"
   help_help: "显示此帮助信息并退出"
   help_v: "显示程序的版本号并退出"
   help_load: "从文件中加载聊天历史记录"
   help_key: "选择要从配置文件加载的API密钥名称"
   help_model: "选择要使用的AI模型"
+  help_host: "设置在本次运行中使用的API Host地址（这通常被用来配置代理）"
   help_m: "启用多行模式"
   help_r: "启用原始模式"
   help_lang: "选择语言"
+  help_set_host: "设置API Host地址（这通常被用来配置代理）"
   help_set_key: "设置OpenAI的API密钥"
   help_set_timeout: "设置API请求的最大等待时间"
   help_set_gentitle: "设置是否自动生成聊天标题"
   help_set_lang: "设置语言"
   help_set_saveperfix: "设置聊天历史记录文件的保存前缀"
   help_set_loglevel: "设置日志级别: "
   #
```

### Comparing `gpt-term-1.1.0/gpt_term/main.py` & `gpt-term-1.1.1/gpt_term/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         else:
             console.print(_("gpt_term.multi_line_disabled"))
 
 
 class ChatGPT:
     def __init__(self, api_key: str, timeout: float):
         self.api_key = api_key
-        self.endpoint = "https://api.openai.com/v1/chat/completions"
+        self.host = "https://api.openai.com"
+        self.endpoint = self.host + "/v1/chat/completions"
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {api_key}"
         }
         self.messages = [
             {"role": "system", "content": f"You are a helpful assistant.\nKnowledge cutoff: 2021-09\nCurrent date: {datetime.now().strftime('%Y-%m-%d')}"}]
         self.model = 'gpt-3.5-turbo'
@@ -401,15 +402,15 @@
             return None
         except requests.exceptions.RequestException as e:
             console.print(_("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             return None
 
     def fetch_credit_total_granted(self):
-        url_subscription = "https://api.openai.com/dashboard/billing/subscription"
+        url_subscription = self.host + "/dashboard/billing/subscription"
         response_subscription = self.send_get(url_subscription)
         if not response_subscription:
             self.credit_total_granted = None
         response_subscription_json = response_subscription.json()
         self.credit_total_granted = response_subscription_json["hard_limit_usd"]
         self.credit_plan = response_subscription_json["plan"]["title"]
 
@@ -421,15 +422,15 @@
             url_usage, params=usage_get_params_monthly)
         if not response_monthly_usage:
             self.credit_used_this_month = None
         self.credit_used_this_month = response_monthly_usage.json()[
             "total_usage"] / 100
 
     def get_credit_usage(self):
-        url_usage = "https://api.openai.com/dashboard/billing/usage"
+        url_usage = self.host + "/dashboard/billing/usage"
         try:
             # get response from /dashborad/billing/subscription for total granted credit
             fetch_credit_total_granted_thread = threading.Thread(
                 target=self.fetch_credit_total_granted)
             fetch_credit_total_granted_thread.start()
 
             # get usage this month
@@ -471,14 +472,18 @@
         except Exception as e:
             console.print(
                 _("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             self.save_chat_history_urgent()
             raise EOFError
         return True
+    
+    def set_host(self, host: str):
+        self.host = host
+        self.endpoint = self.host + "/v1/chat/completions"
 
     def modify_system_prompt(self, new_content: str):
         if self.messages[0]['role'] == 'system':
             old_content = self.messages[0]['content']
             self.messages[0]['content'] = new_content
             console.print(
                 _("gpt_term.system_prompt_moodified",old_content=old_content,new_content=new_content))
@@ -992,21 +997,25 @@
     with open(f'{data_dir}/config.ini', 'w') as configfile:
         config_ini.write(configfile)
 
 
 def set_config_by_args(args: argparse.Namespace, config_ini: ConfigParser):
     global _
     config_need_to_set = {}
+    if args.set_host:       config_need_to_set.update({"OPENAI_HOST"         : args.set_host})
     if args.set_apikey:     config_need_to_set.update({"OPENAI_API_KEY"      : args.set_apikey})
     if args.set_timeout:    config_need_to_set.update({"OPENAI_API_TIMEOUT"  : args.set_timeout})
     if args.set_saveperfix: config_need_to_set.update({"CHAT_SAVE_PERFIX"    : args.set_saveperfix})
     if args.set_loglevel:   config_need_to_set.update({"LOG_LEVEL"           : args.set_loglevel})
     if args.set_gentitle:   config_need_to_set.update({"AUTO_GENERATE_TITLE" : args.set_gentitle})
     # 新的语言设置:
-    if args.set_lang:       config_need_to_set.update({"LANGUAGE"            : args.set_lang})
+    if args.set_lang:       
+        config_need_to_set.update({"LANGUAGE": args.set_lang})
+        _=set_lang(args.set_lang)
+    # here: when set lang is called, set language before printing 'set-successful' messages
 
     if len(config_need_to_set) == 0:
         return
     # nothing to set
     for key, val in config_need_to_set.items():
         config_ini['DEFAULT'][key] = str(val)
         console.print(_("gpt_term.config_key_to_shell_key",key_word=str(key),val=str(val)))
@@ -1029,30 +1038,32 @@
     config = config_ini['DEFAULT']
 
     # 读取语言配置
     config_lang = config.get("language")
     if config_lang:
         if config_lang in supported_langs:
             _=set_lang(config_lang)
-            console.print(_("gpt_term.lang_switch"))
         else:
             console.print(_("gpt_term.lang_config_unsupport", config_lang=config_lang))
+        # if lang set in config is not support, print infos and use default local_lang
 
     parser = argparse.ArgumentParser(description=_("gpt_term.help_description"),add_help=False)
     parser.add_argument('-h', '--help',action='help', help=_("gpt_term.help_help"))
     parser.add_argument('-v','--version', action='version', version=f'%(prog)s v{local_version}',help=_("gpt_term.help_v"))
     parser.add_argument('--load', metavar='FILE', type=str, help=_("gpt_term.help_load"))
     parser.add_argument('--key', type=str, help=_("gpt_term.help_key"))
     parser.add_argument('--model', type=str, help=_("gpt_term.help_model"))
+    parser.add_argument('--host', metavar='HOST', type=str, help=_("gpt_term.help_host"))
     parser.add_argument('-m', '--multi', action='store_true', help=_("gpt_term.help_m"))
     parser.add_argument('-r', '--raw', action='store_true', help=_("gpt_term.help_r"))
     ## 新添加的选项：--lang
     parser.add_argument('-l','--lang', type=str, choices=['en', 'zh_CN', 'jp', 'de'], help=_("gpt_term.help_lang"))
     # normal function args
 
+    parser.add_argument('--set-host', metavar='HOST', type=str, help=_("gpt_term.help_set_host"))
     parser.add_argument('--set-apikey', metavar='KEY', type=str, help=_("gpt_term.help_set_key"))
     parser.add_argument('--set-timeout', metavar='SEC', type=int, help=_("gpt_term.help_set_timeout"))
     parser.add_argument('--set-gentitle', metavar='BOOL', type=str, help=_("gpt_term.help_set_gentitle"))
     ## 新添加的选项：--set-lang
     parser.add_argument('--set-lang', type=str, choices=['en', 'zh_CN', 'jp', 'de'], help=_("gpt_term.help_set_lang"))
     parser.add_argument('--set-saveperfix', metavar='PERFIX', type=str, help=_("gpt_term.help_set_saveperfix"))
     parser.add_argument('--set-loglevel', metavar='LEVEL', type=str, help=_("gpt_term.help_set_loglevel")+'DEBUG, INFO, WARNING, ERROR, CRITICAL')
@@ -1103,24 +1114,31 @@
 
     api_timeout = config.getfloat("OPENAI_API_TIMEOUT", 30)
     log.debug(f"API Timeout set to {api_timeout}")
 
     chat_save_perfix = config.get("CHAT_SAVE_PERFIX", "./chat_history_")
 
     chat_gpt = ChatGPT(api_key, api_timeout)
+    
+    if config.get("OPENAI_HOST"):
+        chat_gpt.set_host(config.get("OPENAI_HOST"))
 
     if not config.getboolean("AUTO_GENERATE_TITLE", True):
         chat_gpt.auto_gen_title_background_enable = False
         log.debug("Auto title generation [bright_red]disabled[/]")
 
     gen_title_daemon_thread = threading.Thread(
         target=chat_gpt.auto_gen_title_background, daemon=True)
     gen_title_daemon_thread.start()
     log.debug("Title generation daemon thread started")
 
+    if args.host:
+        chat_gpt.set_host(args.host)
+        console.print(_("gpt_term.host_set", new_host=args.host))
+
     if args.model:
         chat_gpt.set_model(args.model)
 
     if args.multi:
         ChatMode.toggle_multi_line_mode()
 
     if args.raw:
```

### Comparing `gpt-term-1.1.0/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.1.1/gpt_term.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,16 +51,26 @@
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
+### Related Projects
+
+[GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
+
+[gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
+
 ## Changelog
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
 ### 2023-05-18
 
 - Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 
 <details>
   <summary>More Change log</summary>
 
@@ -122,14 +132,16 @@
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
    ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
 2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
+   **Attention: Try not to use the Python that comes with the system (including Windows 11 app store version and MacOS pre-installed Python), otherwise the gpt-term command will not be found after installation ([#38](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/38))**
+
 ## Installation
 
 
 1. Install `GPT-Term` using `pip`
 
    ```shell
    pip3 install gpt-term
@@ -157,14 +169,20 @@
 
 Run with the following command:
 
 ```shell
 gpt-term
 ```
 
+Or:
+
+```shell
+python3 -m gpt_term
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
@@ -173,28 +191,31 @@
 - `Ctrl+K`: Delete all characters to the right of the cursor
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
-| Arguments     | Description                     | Example                                       |
-| ------------- | ------------------------------- | --------------------------------------------- |
-| -h, --help    | show this help message and exit | `gpt-term --help`                             |
-| --load FILE   | Load chat history from file     | `gpt-term --load chat_history_code_check.json` |
-| --key API_KEY | choose the API key to load      | `gpt-term --key OPENAI_API_KEY1`              |
-| --model MODEL | choose the AI model to use      | `gpt-term --model gpt-3.5-turbo`              |
-| -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
-| -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
-| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
-| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
-| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
-| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
-| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
-| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
+| Arguments | Description | Examples |
+| ------------- | --------------------------------- | - ----------------------------------------------- |
+| -h, --help | show this help message and exit | `gpt-term --help` |
+| --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
+| --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
+| --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
+| --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
+| -m, --multi | Enable multiline mode | `gpt-term --multi` |
+| -r, --raw | Enable raw mode | `gpt-term --raw` |
+| -l, --lang LANG | Set the current running language: en, zh_CN, jp, de | `gpt-term --lang en` |
+| --set-host HOST | Set API Host address (this is usually used to configure proxy) | `gpt-term --set-host https://closeai.deno.dev` |
+| --set-apikey KEY | Set OpenAI API key | `gpt-term --set-apikey sk-xxx` |
+| --set-timeout SEC | Set the maximum wait time for API requests | `gpt-term --set-timeout 10` |
+| --set-gentitle BOOL | Set whether to auto-generate title for chat | `gpt-term --set-gentitle True` |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL | Set log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG` |
+| --set-lang LANG | Set language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
```

### Comparing `gpt-term-1.1.0/gpt_term.egg-info/SOURCES.txt` & `gpt-term-1.1.1/gpt_term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.0/pyproject.toml` & `gpt-term-1.1.1/pyproject.toml`

 * *Files identical despite different names*

