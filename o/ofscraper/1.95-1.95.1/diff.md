# Comparing `tmp/ofscraper-1.95.tar.gz` & `tmp/ofscraper-1.95.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.95.tar", max compression
+gzip compressed data, was "ofscraper-1.95.1.tar", max compression
```

## Comparing `ofscraper-1.95.tar` & `ofscraper-1.95.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-05-19 18:02:23.727934 ofscraper-1.95/LICENSE
--rw-r--r--   0        0        0     5177 2023-05-19 18:02:23.727934 ofscraper-1.95/README.md
--rw-r--r--   0        0        0      607 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/__init__.py
--rw-r--r--   0        0        0      998 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      838 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/init.py
--rw-r--r--   0        0        0     2243 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/me.py
--rw-r--r--   0        0        0     4359 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9170 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     6457 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     4999 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     3611 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    22508 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3655 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8994 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10859 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/config.py
--rw-r--r--   0        0        0      993 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    17597 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     4540 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5369 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3008 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     1505 2023-05-19 18:02:58.707954 ofscraper-1.95/pyproject.toml
--rw-r--r--   0        0        0     6556 1970-01-01 00:00:00.000000 ofscraper-1.95/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-20 19:39:41.219814 ofscraper-1.95.1/LICENSE
+-rw-r--r--   0        0        0     5177 2023-05-20 19:39:41.219814 ofscraper-1.95.1/README.md
+-rw-r--r--   0        0        0      607 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2243 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0     4359 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9170 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     6457 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     4999 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     3611 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    21369 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3938 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8994 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10859 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      993 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    17597 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     1926 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     4540 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5377 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3008 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     1545 2023-05-20 19:40:15.672136 ofscraper-1.95.1/pyproject.toml
+-rw-r--r--   0        0        0     6618 1970-01-01 00:00:00.000000 ofscraper-1.95.1/PKG-INFO
```

### Comparing `ofscraper-1.95/LICENSE` & `ofscraper-1.95.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/README.md` & `ofscraper-1.95.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/__init__.py` & `ofscraper-1.95.1/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/__version__.py` & `ofscraper-1.95.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/highlights.py` & `ofscraper-1.95.1/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/init.py` & `ofscraper-1.95.1/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/me.py` & `ofscraper-1.95.1/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/messages.py` & `ofscraper-1.95.1/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/paid.py` & `ofscraper-1.95.1/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/posts.py` & `ofscraper-1.95.1/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/profile.py` & `ofscraper-1.95.1/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/subscriptions.py` & `ofscraper-1.95.1/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/api/timeline.py` & `ofscraper-1.95.1/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/constants.py` & `ofscraper-1.95.1/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/db/operations.py` & `ofscraper-1.95.1/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/db/queries.py` & `ofscraper-1.95.1/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/interaction/like.py` & `ofscraper-1.95.1/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/prompts/prompt_functions.py` & `ofscraper-1.95.1/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/prompts/prompts.py` & `ofscraper-1.95.1/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/scraper.py` & `ofscraper-1.95.1/ofscraper/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 import ofscraper.utils.profiles as profiles
 import ofscraper.api.init as init
 import ofscraper.utils.download as download
 import ofscraper.interaction.like as like
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.constants as constants
+import ofscraper.utils.filters as filters
 
 
 
 console=Console()
 log=logger.init_logger(logging.getLogger(__package__))
 args=args_.getargs()
 log.debug(args)
@@ -154,15 +155,15 @@
     output=[]
     for ele in enumerate(urls):
         count=ele[0]
         data=ele[1]
         output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
     avatars=list(filter(lambda x:x.filename=='avatar',output))
     if len(avatars)>0:
-        log.info(f"Avatar : {avatars[0].url}")
+        log.warning(f"Avatar : {avatars[0].url}")
     return output
 
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
@@ -194,44 +195,19 @@
             if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
             if 'Stories'  in args.posts:
                 stories_dicts=highlights_tuple[1]   
             if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
                 stories_dicts=highlights_tuple[1]               
-    return posts_filter(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
+    return filters.filterMedia(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
             archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts]))
 
 )
 
-def posts_filter(media):
-    filtersettings=config.get_filter(config.read_config())
-    output=[]
-    ids=set()
-    log.info("Removing duplicate media")
-    log.debug(f"[bold]Combined Media Count with dupes[/bold]  {len(media)}")
-    for item in media:
-        if not item.id or item.id not in ids:
-            output.append(item)
-            ids.add(item.id)
-    log.debug(f"[bold]Combined Media Count without dupes[/bold] {len(output)}")
-    output=list(sorted(output,key=lambda x:x.date,reverse=True))
-    if isinstance(filtersettings,str):
-        filtersettings=filtersettings.split(",")
-    if isinstance(filtersettings,list):
-        filtersettings=list(map(lambda x:x.lower().replace(" ",""),filtersettings))
-        filtersettings=list(filter(lambda x:x!="",filtersettings))
-        if len(filtersettings)==0:
-            return media
-        log.info(f"filtering Media to {','.join(filtersettings)}")
-        output= list(filter(lambda x:x.mediatype.lower() in filtersettings,output))
-    else:
-        log.info("The settings you picked for the filter are not valid\nNot Filtering")
-        log.debug(f"[bold]Combined Media Count Filtered:[/bold] {len(output)}")
-    return output
 
         
 
 
 
 def get_usernames(parsed_subscriptions: list) -> list:
     usernames = [sub[0] for sub in parsed_subscriptions]
```

### Comparing `ofscraper-1.95/ofscraper/utils/args.py` & `ofscraper-1.95.1/ofscraper/utils/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import logging
 import sys
-import pkg_resources
+import arrow
 from ofscraper.__version__ import __version__ 
 
 args=None
 log=logging.getLogger(__package__)
 def getargs(input=None):
     global args
     if args and input==None:
@@ -44,14 +44,21 @@
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
     post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
     post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
+    post.add_argument(
+        '-be', '--before', help = 'Download post at or before the given date general synax is Month/Day/Year',type=arrow.get)
+ 
+    post.add_argument(
+        '-af', '--after', help = 'Download post at or after the given date Month/Day/Year',type=arrow.get)
+    
+    
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-t', '--account-type', help = 'Filter Free or paid accounts',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
     filters.add_argument(
```

### Comparing `ofscraper-1.95/ofscraper/utils/auth.py` & `ofscraper-1.95.1/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/config.py` & `ofscraper-1.95.1/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/dates.py` & `ofscraper-1.95.1/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/download.py` & `ofscraper-1.95.1/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/encoding.py` & `ofscraper-1.95.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/exit.py` & `ofscraper-1.95.1/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/logger.py` & `ofscraper-1.95.1/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/paths.py` & `ofscraper-1.95.1/ofscraper/utils/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 def createDir(path):
     try:
         path.mkdir(exist_ok=True,parents=True)
     except:
         log.info("Error creating directory, check the directory and make sure correct permissions have been issued.")
         sys.exit()
 def databasePathHelper(model_id,username):
-    return pathlib.Path(config_.get_metadata(config_.read_config()).format(configpath=homeDir / constants.configPath,profile=profiles.get_current_profile(),model_username=username,username=username,model_id=model_id,sitename="Onlyfans",site_name="Onlyfans",first_letter=username[0],save_location=pathlib.Path((config_.get_save_location(config_.read_config())))),"user_data.db")
+    formatStr=config_.get_metadata(config_.read_config())
+    return pathlib.Path(formatStr.format(configpath=homeDir / constants.configPath,profile=profiles.get_current_profile(),model_username=username,username=username,model_id=model_id,sitename="Onlyfans",site_name="Onlyfans",first_letter=username[0],save_location=config_.get_save_location(config_.read_config())),"user_data.db")
 
 def getmediadir(ele,username,model_id):
     root= pathlib.Path((config_.get_save_location(config_.read_config())))
     downloadDir=config_.get_dirformat(config_.read_config())\
     .format(sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele.responsetype.capitalize(),mediatype=ele.mediatype.capitalize(),value=ele.value.capitalize(),date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())))
     return root /downloadDir
```

### Comparing `ofscraper-1.95/ofscraper/utils/profiles.py` & `ofscraper-1.95.1/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/ofscraper/utils/separate.py` & `ofscraper-1.95.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95/pyproject.toml` & `ofscraper-1.95.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.95"
+version = "1.95.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
@@ -23,14 +23,15 @@
 win32-setctime = "^1.1.0"
 pathvalidate = "^2.5.2"
 xxhash = "^3.2.0"
 mpegdash = "^0.3.1"
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
+poetry-dynamic-versioning = "^0.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
```

### Comparing `ofscraper-1.95/PKG-INFO` & `ofscraper-1.95.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.95
+Version: 1.95.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,15 @@
 Requires-Dist: dunamai (>=1.17.0,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
+Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
```

