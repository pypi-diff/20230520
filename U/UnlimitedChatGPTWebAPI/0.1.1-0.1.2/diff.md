# Comparing `tmp/UnlimitedChatGPTWebAPI-0.1.1.tar.gz` & `tmp/UnlimitedChatGPTWebAPI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedChatGPTWebAPI-0.1.1.tar", last modified: Wed May 17 09:15:17 2023, max compression
+gzip compressed data, was "UnlimitedChatGPTWebAPI-0.1.2.tar", last modified: Sat May 20 15:58:34 2023, max compression
```

## Comparing `UnlimitedChatGPTWebAPI-0.1.1.tar` & `UnlimitedChatGPTWebAPI-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/js/preload.js
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-17 09:15:17.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 09:15:17.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:15:17.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 09:15:17.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 09:15:17.000000 UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-17 09:14:57.000000 UnlimitedChatGPTWebAPI-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:15:17.730358 UnlimitedChatGPTWebAPI-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/js/preload.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-20 15:58:34.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-20 15:58:34.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:58:34.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-20 15:58:34.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 15:58:34.000000 UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-20 15:58:14.000000 UnlimitedChatGPTWebAPI-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:58:34.977115 UnlimitedChatGPTWebAPI-0.1.2/setup.cfg
```

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/LICENSE` & `UnlimitedChatGPTWebAPI-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/PKG-INFO` & `UnlimitedChatGPTWebAPI-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedChatGPTWebAPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unlimited ChatGPT WebAPI
 Author-email: AkashiCoin <l1040186796@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AkashiCoin/UnlimitedChatGPTWebAPI
 Project-URL: Repository, https://github.com/AkashiCoin/UnlimitedChatGPTWebAPI
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/README.md` & `UnlimitedChatGPTWebAPI-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/data.py` & `UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,28 +165,29 @@
         self.save()
 
     @property
     def cf_clearance(self) -> str:
         """Return a random cf_clearance"""
         if not self.cf_clearances:
             return ""
-        cf_clearance = random.choice(list(self.cf_clearances.keys()))
-        if cf_clearance := self.get_cf_clearance(cf_clearance=cf_clearance):
+        cf_id = random.choice(list(self.cf_clearances.keys()))
+        if cf_clearance := self.get_cf_clearance(cf_id=cf_id):
             return cf_clearance
         return self.cf_clearance
 
-    def get_cf_clearance(self, cf_clearance):
-        if cf_clearance not in self.cf_clearances:
+    def get_cf_clearance(self, cf_id):
+        """Get a cf_clearance"""
+        if cf_id not in self.cf_clearances:
             return None
 
-        cf_clearance_info = self.cf_clearances[cf_clearance]
+        cf_clearance_info = self.cf_clearances[cf_id]
         expires = cf_clearance_info.get("expires")
 
         if expires is not None and expires < time.time():
-            del self.cf_clearances[cf_clearance]
+            del self.cf_clearances[cf_id]
             return None
 
         return cf_clearance_info.get("cf_clearance")
 
     def save_cf_clearance(self, cf_clearance: str) -> None:
         """Save a cf_clearance"""
         if cf_clearance:
@@ -195,18 +196,21 @@
             self.cf_clearances[cf_id] = {
                 "cf_clearance": cf_clearance,
                 "expires": expires,
             }
             self.save()
 
     def delete_cf_clearance(self, cf_clearance: str) -> bool:
-        if cf_clearance in self.cf_clearances:
-            del self.cf_clearances[cf_clearance]
-            self.save()
-            return True
+        """Delete a cf_clearance"""
+        if cf_clearance:
+            [cf_id, expires, _, _, _, _] = cf_clearance.split("-")
+            if cf_id in self.cf_clearances:
+                del self.cf_clearances[cf_id]
+                self.save()
+                return True
         return False
 
     @root_validator(pre=True)
     def init(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if cls.__file_path.is_file():
             return json.loads(cls.__file_path.read_text("utf-8"))
         return values
```

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/js/preload.js` & `UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/js/preload.js`

 * *Files identical despite different names*

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI/session.py` & `UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Response,
     async_playwright,
     JSHandle,
     BrowserContext,
     Browser,
     PlaywrightContextManager,
 )
-from playwright._impl._api_types import Error
+from playwright._impl._api_types import Error as PlaywrightError
 
 from .data import CookieManager, StreamResponse
 
 
 SESSION_TOKEN_KEY = "__Secure-next-auth.session-token"
 CF_CLEARANCE_KEY = "cf_clearance"
 
@@ -72,14 +72,15 @@
         playwright = await self.playwright.start()
         self.browser = await playwright.chromium.launch(
             headless=True,
             proxy={"server": self.proxies}
             if self.proxies
             else None,  # your proxy
         )
+        # ua = None
         ua = f"Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:72.0) Gecko/20100101 Firefox/{self.browser.version}"
         # ua = f"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{self.browser.version} Safari/537.36"
         self.content = await self.browser.new_context(user_agent=ua)
 
     async def set_cookie(self, key: str, value: str, expires: float = -1):
         """Set Cookie"""
         await self.content.add_cookies(
@@ -124,16 +125,18 @@
         self.page = page
         await page.add_init_script(path=Path(__file__).parent / "js" / "preload.js")
         await self.get_cf_cookies()
         await page.expose_function("set_cookie", self.set_cookie)
         await page.expose_function("get_cookie", self.get_cookie)
         return page
 
-    async def get_cf_cookies(self, retry: int = 20) -> None:
+    async def get_cf_cookies(self, retry: int = 20, wait: bool = False) -> None:
         await self.set_status(False)
+        if wait:
+            await self.wait_for_task()
         logger.debug("Start get Cloudflare cookies")
         await self.content.add_cookies(
             [
                 {
                     "name": CF_CLEARANCE_KEY,
                     "value": self.cookie_manager.cf_clearance,  # Get cf_clearance from cookie_manager
                     "domain": ".chat.openai.com",
@@ -176,14 +179,15 @@
         await self.set_status(True)
         self.cf_clearance = await self.get_cookie(CF_CLEARANCE_KEY)
         self.cookie_manager.save_cf_clearance(self.cf_clearance)
         logger.debug("Get Cloudflare cookies success")
 
     async def wait_for_task(self, timeout: int = 60):
         """Wait for task, called when restart"""
+        logger.debug("Wait for task...")
         await self.set_status(False)
         await self.page.evaluate(
             "([timeout]) => waitForNoFetch(timeout)", [timeout * 1000]
         )
 
     @asynccontextmanager
     async def fetch(
@@ -242,15 +246,15 @@
                 timeout=timeout,
             ) as response:
                 if response.status == 403:
                     self.cookie_manager.delete_cf_clearance(self.cf_clearance)
                     logger.warning(
                         "Cloudflare cookies had expired, trying to get new Cloudflare cookies..."
                     )
-                    asyncio.ensure_future(self.get_cf_cookies())
+                    asyncio.ensure_future(self.get_cf_cookies(wait=True))
                 elif response.status == 429 and "/api/auth/session" in url:
                     logger.warning(
                         "Too many session requests, trying to get new Cloudflare cookies..."
                     )
                     response.status = 403
                     if await self.get_status():
                         asyncio.ensure_future(self.init_page(restart=True))
@@ -258,20 +262,19 @@
                     return
                 if session_token:
                     if token := await self.get_cookie(SESSION_TOKEN_KEY):
                         response.headers[
                             "set-cookie"
                         ] = f"{SESSION_TOKEN_KEY}={token}; path=/; max-age=31536000; secure; httponly"
                 yield response
-        except Error as e:
+        except PlaywrightError as e:
             logger.error(f"Playwright Error: {e.message}")
             yield StreamResponse(status=403)
-        except Exception as e:
-            logger.opt(exception=e).error("Call API failed")
-            yield response
+        # except Exception as e:
+        #     logger.opt(exception=e).error("Call API failed")
 
 
 class SessionManager:
     def __init__(
         self,
         proxies: str = None,
         cookie_manager: CookieManager = CookieManager(),
@@ -286,15 +289,15 @@
             asyncio.ensure_future(session.init_page())
 
     async def get_sessions(self):
         """Get available sessions"""
         return [
             session
             for session in self.sessions
-            if await session.get_status() and not session.running
+            if (await session.get_status() and not session.running)
         ]
 
     async def get_session(self):
         """Get a random available session"""
         sessions = await self.get_sessions()
         if sessions:
             return random.choice(sessions)
@@ -327,18 +330,18 @@
             )
         ):
             session_token = None
         async with session._call_api(
             method, url, headers, data=data, session_token=session_token
         ) as resp:
             if resp.status == 403:
-                if first:
-                    # Retry once
-                    async with self.call_api(
-                        method, url, headers, data, session_token, False
-                    ) as resp:
-                        yield resp
-                else:
+                if not first:
                     resp.status = 499
                     yield resp
             else:
                 yield resp
+        if resp.status == 403 and first:
+            # Retry once
+            async with self.call_api(
+                method, url, headers, data, session_token, False
+            ) as resp:
+                yield resp
```

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/UnlimitedChatGPTWebAPI.egg-info/PKG-INFO` & `UnlimitedChatGPTWebAPI-0.1.2/UnlimitedChatGPTWebAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedChatGPTWebAPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unlimited ChatGPT WebAPI
 Author-email: AkashiCoin <l1040186796@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AkashiCoin/UnlimitedChatGPTWebAPI
 Project-URL: Repository, https://github.com/AkashiCoin/UnlimitedChatGPTWebAPI
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `UnlimitedChatGPTWebAPI-0.1.1/pyproject.toml` & `UnlimitedChatGPTWebAPI-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "UnlimitedChatGPTWebAPI"
-version = "0.1.1"
+version = "0.1.2"
 description = "Unlimited ChatGPT WebAPI"
 authors = [
     {name = "AkashiCoin", email = "l1040186796@gmail.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["playwright>=1.28.0", "pydantic>=1.9.0", "loguru>=0.6.0"]
 requires-python = ">=3.8"
```

