# Comparing `tmp/gpt4-openai-api-0.2.1.tar.gz` & `tmp/gpt4-openai-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.2.1.tar", last modified: Thu May 11 21:05:05 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.3.0.tar", last modified: Sat May 20 10:57:13 2023, max compression
```

## Comparing `gpt4-openai-api-0.2.1.tar` & `gpt4-openai-api-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.873761 gpt4-openai-api-0.2.1/
--rw-rw-rw-   0        0        0     5123 2023-05-11 21:05:05.871755 gpt4-openai-api-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.835759 gpt4-openai-api-0.2.1/gpt4_openai/
--rw-rw-rw-   0        0        0     2559 2023-05-11 20:46:34.000000 gpt4-openai-api-0.2.1/gpt4_openai/__init__.py
--rw-rw-rw-   0        0        0    24235 2023-05-11 20:46:44.000000 gpt4-openai-api-0.2.1/gpt4_openai/driver.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.865759 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0     5123 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 21:05:05.873761 gpt4-openai-api-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-05-11 21:05:02.000000 gpt4-openai-api-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.869755 gpt4-openai-api-0.2.1/test/
--rw-rw-rw-   0        0        0      434 2023-05-11 20:47:25.000000 gpt4-openai-api-0.2.1/test/test.py
--rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.2.1/test/test_langchain.py
+drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.876604 gpt4-openai-api-0.3.0/
+-rw-rw-rw-   0        0        0     5826 2023-05-20 10:57:13.875604 gpt4-openai-api-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.825606 gpt4-openai-api-0.3.0/gpt4_openai/
+-rw-rw-rw-   0        0        0     2607 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/gpt4_openai/__init__.py
+-rw-rw-rw-   0        0        0    24200 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/gpt4_openai/driver.py
+drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.865604 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0     5826 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 10:57:13.000000 gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 10:57:13.877604 gpt4-openai-api-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 10:57:13.872604 gpt4-openai-api-0.3.0/test/
+-rw-rw-rw-   0        0        0      460 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/test/test-browsing.py
+-rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.3.0/test/test.py
+-rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.3.0/test/test_langchain.py
```

### Comparing `gpt4-openai-api-0.2.1/PKG-INFO` & `gpt4-openai-api-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: # GPT4 OpenAI unofficial API
         
         ## Unofficial GPT-4 API access via chat.openai.com using Selenium
         
         Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. It uses [selenium webdriver](https://www.selenium.dev/) to emulate user interaction on [chat.openai.com](chat.openai.com). If the account has `ChatGPT Plus`, the driver **will use GPT-4**, otherwise it will use the default GPT-3.5.
         
+        It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
+        
         **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
         
         The core logic was taken from the [IntelligenzaArtificiale/Free-Auto-GPT](https://github.com/IntelligenzaArtificiale/Free-Auto-GPT).
         
         ## Demo
         
         ![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
         
         ## Demo script
         
         ```python
         from gpt4_openai import GPT4OpenAI
         
         # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False)
+        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4')
         # GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
         response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
         print(response)
         ```
         
         As seen on the demo gif (above), GPT-4 answers correctly.
         
+        ## Browsing support
+        
+        ```python
+        from gpt4_openai import GPT4OpenAI
+        
+        # Token is the __Secure-next-auth.session-token from chat.openai.com
+        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4-browsing')
+        # ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
+        response = llm('What is the age difference between Dua Lipa and her boyfriend?')
+        print(response)
+        ```
+        
         ## Langchain support
         
         `GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
         
         ```python
         from gpt4_openai import GPT4OpenAI
         from langchain import LLMChain
```

### Comparing `gpt4-openai-api-0.2.1/gpt4_openai/__init__.py` & `gpt4-openai-api-0.3.0/gpt4_openai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     history_data: Optional[List] = []
     token : Optional[str]
     chatbot : Optional[ChatGptDriver] = None
     call : int = 0
     conversation : Optional[str] = ""
     headless : bool = True
     __file__ = __file__
+    model: str = "gpt-4"
 
     #### WARNING : for each api call this library will create a new chat on chat.openai.com
     @property
     def _llm_type(self) -> str:
         return "custom"
 
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
@@ -26,27 +27,27 @@
             #raise ValueError("stop kwargs are not permitted.")
         #token is a must check
         if self.chatbot is None:
             if self.token is None:
                 raise ValueError("Need a token , check https://chat.openai.com/api/auth/session for get your token")
             else:
                 if self.conversation == "":
-                    self.chatbot = ChatGptDriver(self.token, headless=self.headless)
+                    self.chatbot = ChatGptDriver(self.token, headless=self.headless, model=self.model)
                 elif self.conversation != "" :
-                    self.chatbot = ChatGptDriver(self.token, headless=self.headless, conversation_id=self.conversation)
+                    self.chatbot = ChatGptDriver(self.token, headless=self.headless, model=self.model, conversation_id=self.conversation)
                 else:
                     raise ValueError("Something went wrong")
 
         response = ""
         # OpenAI: 50 requests / hour for each account
         if self.call >= 45:
             raise ValueError("You have reached the maximum number of requests per hour ! Help me to Improve. Abusing this tool is at your own risk")
         else:
             sleep(2)
-            data = self.chatbot.send_message(prompt, model='gpt4')
+            data = self.chatbot.send_message(prompt)
             #print(data)
             response = data["message"]
             self.conversation = data["conversation_id"]
             FullResponse = data
             self.call += 1
 
         #add to history
```

### Comparing `gpt4-openai-api-0.2.1/gpt4_openai/driver.py` & `gpt4-openai-api-0.3.0/gpt4_openai/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,16 @@
 chatgpt_clear_convo = (By.LINK_TEXT, 'Clear conversations')
 chatgpt_confirm_clear_convo = (By.LINK_TEXT, 'Confirm clear conversations')
 chatgpt_chats_list_first_node = (
     By.XPATH,
     "//li[@class='relative z-[15]']//a",
 )
 
-model_selector = (By.XPATH, "//button[starts-with(@id, 'headlessui-listbox-button')]")
-gpt4_selector = (By.XPATH, "//ul[@role='listbox']/li[contains(.//text(), 'GPT-4')][1]")
-
-chatgpt_chat_url = 'https://chat.openai.com'
+stop_generating = (By.XPATH, "//button[contains(., 'Stop generating')]")
+regenerate_response = (By.XPATH, "//button[contains(., 'Regenerate response')]")
 
 
 class ChatGptDriver:
     '''
     An unofficial Python wrapper for OpenAI's ChatGPT API
     '''
 
@@ -57,14 +55,15 @@
         conversation_id: str = '',
         auth_type: str = None,
         email: str = None,
         password: str = None,
         login_cookies_path: str = '',
         captcha_solver: str = 'pypasser',
         solver_apikey: str = '',
+        model: str = 'gpt4',
         proxy: str = None,
         chrome_args: list = [],
         moderation: bool = True,
         verbose: bool = False,
         headless: bool = True,
     ):
         '''
@@ -94,14 +93,17 @@
         self.__captcha_solver = captcha_solver
         self.__solver_apikey = solver_apikey
         self.__proxy = proxy
         self.__chrome_args = chrome_args
         self.__moderation = moderation
         self.__headless = headless
 
+        self._model = model
+        self._chatgpt_chat_url = 'https://chat.openai.com'
+
         if not self.__session_token and (
             not self.__email or not self.__password or not self.__auth_type
         ):
             raise ValueError(
                 'Please provide either a session token or login credentials'
             )
         if self.__auth_type not in [None, 'google', 'microsoft', 'openai']:
@@ -129,14 +131,17 @@
 
                 subprocess.run(['ffdl', 'install'])
             os.environ['PATH'] += os.pathsep + ffdl.ffmpeg_dir
 
         self.__init_browser()
         weakref.finalize(self, self.__del__)
 
+    def _get_url(self):
+        return f"{self._chatgpt_chat_url}/?model={self._model}"
+
     def __del__(self):
         '''
         Close the browser and display
         '''
         self.__is_active = False
         if hasattr(self, 'driver'):
             self.logger.debug('Closing browser...')
@@ -232,15 +237,16 @@
                 {'urls': ['https://chat.openai.com/backend-api/moderations']},
             )
 
         self.logger.debug('Ensuring Cloudflare cookies...')
         self.__ensure_cf()
 
         self.logger.debug('Opening chat page...')
-        self.driver.get(f'{chatgpt_chat_url}/{self.__conversation_id}')
+        self.driver.get(self._get_url())
+        # self.driver.execute_script("window.localStorage.setItem('oai/apps/hasSeenOnboarding/chat', '2023-05-15')")
         self.__check_blocking_elements()
 
         self.__is_active = True
         Thread(target=self.__keep_alive, daemon=True).start()
 
     def __ensure_cf(self, retry: int = 3) -> None:
         '''
@@ -375,26 +381,26 @@
             self.__sleep(60)
 
     def __check_blocking_elements(self) -> None:
         '''
         Check for blocking elements and dismiss them
         '''
         self.logger.debug('Looking for blocking elements...')
-        
+
         try:
             # FInd a button to dismiss the dialog with class="btn relative btn-primary" inside the div[@role="dialog"]
             btn_to_dismiss = WebDriverWait(self.driver, 5).until(
                 EC.presence_of_element_located((By.XPATH, '//div[@role="dialog"]//button[@class="btn relative btn-primary"]'))
             )
             if btn_to_dismiss:
                 self.logger.debug('Dismissing dialog...')
                 self.driver.execute_script('arguments[0].click()', btn_to_dismiss)
         except:
             pass
-        
+
         try:
             # for 3 times
             i = 0
             while i<=2:
                 self.__sleep(0.4)
                 if i !=2:
                     #get the button with class="btn relative btn-neutral ml-auto"
@@ -427,15 +433,15 @@
             content = response.text
             if content != prev_content:
                 yield content[len(prev_content) :]
                 prev_content = content
             if not result_streaming:
                 break
 
-    def send_message(self, message: str, stream: bool = False, model: str = "default") -> dict:
+    def send_message(self, message: str, stream: bool = False) -> dict:
         '''
         Send a message to ChatGPT\n
         :param message: Message to send
         :return: Dictionary with keys `message` and `conversation_id`
         '''
         self.logger.debug('Ensuring Cloudflare cookies...')
         self.__ensure_cf()
@@ -445,31 +451,14 @@
         try:
             textbox = WebDriverWait(self.driver, 10).until(
                 EC.element_to_be_clickable(chatgpt_textbox)
             )
         except SeleniumExceptions.ElementClickInterceptedException():
             pass
 
-        # If we have paid access, we should select GPT4 model
-        try:
-            if model == "gpt4":
-                self.logger.debug('Trying to select model...')
-                WebDriverWait(self.driver, 3).until(
-                    EC.presence_of_element_located(model_selector)
-                ).click()
-                self.logger.debug('Paid access detected, selecting GPT4 model...')
-                self.__sleep(1.0)
-                WebDriverWait(self.driver, 3).until(
-                    EC.presence_of_element_located(gpt4_selector)
-                ).click()
-                self.logger.debug('GPT4 model selected')
-        except SeleniumExceptions.TimeoutException:
-            print(">>> WARNING <<<\n>> You don't have paid access to GPT4, using default model...")
-            self.logger.debug('Paid access not detected, using default model...')
-
         self.logger.debug('Sending message...')
         try:
             textbox = WebDriverWait(self.driver, 3).until(
                 EC.element_to_be_clickable(chatgpt_textbox)
             )
             textbox.click()
         except SeleniumExceptions.ElementClickInterceptedException():
@@ -491,33 +480,47 @@
         textbox.send_keys(Keys.ENTER)
 
         if stream:
             for i in self.__stream_message():
                 print(i, end='')
                 self.__sleep(0.1)
             return print()
+        
+        # Check whether GPT is generating the result
+        # WebDriverWait(self.driver, 1).until_not(
+        #     EC.presence_of_element_located(stop_generating)
+        # )
 
         self.logger.debug('Waiting for completion...')
-        WebDriverWait(self.driver, 120).until_not(
-            EC.presence_of_element_located(chatgpt_streaming)
+        WebDriverWait(self.driver, 20).until(
+            # When the "Stop generating" button is gone, it means the generation is done
+            EC.presence_of_element_located(stop_generating)
         )
 
+        try:
+            WebDriverWait(self.driver, 100).until(
+                # When the "Regenerate response" button is available, it means the generation is done
+                EC.presence_of_element_located(regenerate_response)
+            )
+        except SeleniumExceptions.NoSuchElementException:
+            self.logger.debug('Regenerate response button not found!')
+
         self.logger.debug('Getting response...')
         responses = self.driver.find_elements(*chatgpt_big_response)
         if responses:
             response = responses[-1]
             if 'text-red' in response.get_attribute('class'):
                 self.logger.debug('Response is an error')
                 raise ValueError(response.text)
         response = self.driver.find_elements(*chatgpt_small_response)[-1]
 
         content = markdownify(response.get_attribute('innerHTML')).replace(
             'Copy code`', '`'
         )
-                
+
         pattern = re.compile(
             r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
         )
         matches = pattern.search(self.driver.current_url)
         if not matches:
             self.driver.refresh()
             self.__sleep(2)
@@ -544,29 +547,29 @@
         """
         time.sleep(random.uniform(sec, sec * multiplier))
 
     def reset_conversation(self) -> None:
         '''
         Reset the conversation
         '''
-        if not self.driver.current_url.startswith(chatgpt_chat_url):
+        if not self.driver.current_url.startswith(self._chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping reset')
 
         self.logger.debug('Resetting conversation...')
         try:
             self.driver.find_element(*chatgpt_new_chat).click()
         except SeleniumExceptions.NoSuchElementException:
             self.logger.debug('New chat button not found')
             self.driver.save_screenshot('reset_conversation_failed.png')
 
     def clear_conversations(self) -> None:
         '''
         Clear all conversations
         '''
-        if not self.driver.current_url.startswith(chatgpt_chat_url):
+        if not self.driver.current_url.startswith(self._chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping clear')
 
         self.logger.debug('Clearing conversations...')
         try:
             self.driver.find_element(*chatgpt_clear_convo).click()
         except SeleniumExceptions.NoSuchElementException:
             self.logger.debug('Clear conversations button not found')
@@ -583,13 +586,13 @@
         except SeleniumExceptions.TimeoutException:
             self.logger.debug('Clear conversations failed')
 
     def refresh_chat_page(self) -> None:
         '''
         Refresh the chat page
         '''
-        if not self.driver.current_url.startswith(chatgpt_chat_url):
+        if not self.driver.current_url.startswith(self._chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping refresh')
 
-        self.driver.get(chatgpt_chat_url)
-        self.__check_capacity(chatgpt_chat_url)
+        self.driver.get(self._get_url())
+        self.__check_capacity(self._get_url())
         self.__check_blocking_elements()
```

### Comparing `gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/PKG-INFO` & `gpt4-openai-api-0.3.0/gpt4_openai_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: # GPT4 OpenAI unofficial API
         
         ## Unofficial GPT-4 API access via chat.openai.com using Selenium
         
         Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. It uses [selenium webdriver](https://www.selenium.dev/) to emulate user interaction on [chat.openai.com](chat.openai.com). If the account has `ChatGPT Plus`, the driver **will use GPT-4**, otherwise it will use the default GPT-3.5.
         
+        It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
+        
         **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
         
         The core logic was taken from the [IntelligenzaArtificiale/Free-Auto-GPT](https://github.com/IntelligenzaArtificiale/Free-Auto-GPT).
         
         ## Demo
         
         ![Demo GIF](https://user-images.githubusercontent.com/18037362/236707120-e93d40bc-b73b-4f72-bc7d-d0449a082946.gif)
         
         ## Demo script
         
         ```python
         from gpt4_openai import GPT4OpenAI
         
         # Token is the __Secure-next-auth.session-token from chat.openai.com
-        llm = GPT4OpenAI(token=my_session_token, headless=False)
+        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4')
         # GPT3.5 will answer 8, while GPT4 should be smart enough to answer 10
         response = llm('If there are 10 books in a room and I read 2, how many books are still in the room?')
         print(response)
         ```
         
         As seen on the demo gif (above), GPT-4 answers correctly.
         
+        ## Browsing support
+        
+        ```python
+        from gpt4_openai import GPT4OpenAI
+        
+        # Token is the __Secure-next-auth.session-token from chat.openai.com
+        llm = GPT4OpenAI(token=my_session_token, headless=False, model='gpt-4-browsing')
+        # ChatGPT will first browse the web for the name/age of her boyfriend, then return the answer
+        response = llm('What is the age difference between Dua Lipa and her boyfriend?')
+        print(response)
+        ```
+        
         ## Langchain support
         
         `GPT4OpenAI` actually extends `LLM` class from `langchain.llms.base`. So you can easily use this library inside langchain ecosystem. Example:
         
         ```python
         from gpt4_openai import GPT4OpenAI
         from langchain import LLMChain
```

### Comparing `gpt4-openai-api-0.2.1/setup.py` & `gpt4-openai-api-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = Path(__file__).parent.resolve()
 readme_file = root / 'readme.md'
 long_description = readme_file.read_text(encoding='utf-8')
 
 setup(
     name="gpt4-openai-api",
-    version="0.2.1",
+    version="0.3.0",
     description="Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Erol444",
     author_email="erol123444@gmail.com",
     url="https://github.com/Erol444/gpt4-openai-api",
     packages=["gpt4_openai"],
```

### Comparing `gpt4-openai-api-0.2.1/test/test_langchain.py` & `gpt4-openai-api-0.3.0/test/test_langchain.py`

 * *Files identical despite different names*

