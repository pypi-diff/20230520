# Comparing `tmp/easy_post_twitter-1.0.5.tar.gz` & `tmp/easy_post_twitter-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_post_twitter-1.0.5.tar", max compression
+gzip compressed data, was "easy_post_twitter-1.0.6.tar", max compression
```

## Comparing `easy_post_twitter-1.0.5.tar` & `easy_post_twitter-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.5/easy_post_twitter/__init__.py
--rw-r--r--   0        0        0     9345 2023-05-09 13:46:49.905237 easy_post_twitter-1.0.5/easy_post_twitter/twitter.py
--rw-r--r--   0        0        0      415 2023-05-09 21:43:16.746278 easy_post_twitter-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.6/easy_post_twitter/__init__.py
+-rw-r--r--   0        0        0    10361 2023-05-19 14:28:46.273859 easy_post_twitter-1.0.6/easy_post_twitter/twitter.py
+-rw-r--r--   0        0        0      415 2023-05-17 21:00:36.173097 easy_post_twitter-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.6/PKG-INFO
```

### Comparing `easy_post_twitter-1.0.5/easy_post_twitter/twitter.py` & `easy_post_twitter-1.0.6/easy_post_twitter/twitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dotenv import load_dotenv
-from datetime import datetime
+from datetime import date, datetime
 from time import sleep
 from loguru import logger as log
 import os
 from pathlib import Path
 import tweepy
 from tweepy.auth import OAuth1, OAuthHandler
 
@@ -198,12 +198,36 @@
         client = self.__get_client()
         try:
             response = client.create_tweet(text=text)
             log.info(f'Tweet created successfully. ID: {response.data["id"]}')
         except Exception as e:
             log.error(f'Error creating tweet. Error: {e}')
 
+    def tweetNthread(self, text, isThread, id):
+        ''' This method do not use twitter's api search to determine if
+        a tweet is the day's opening one or a response to an early one. A state 
+        local file keeps the state that informs the last day when the 
+        state was last updated and the ID of the last tweet.
+        '''
+        client = self.__get_client()
+        if isThread:
+            try:
+                print('Thread. Last tweet id:',id)
+                response = client.create_tweet(text=text, in_reply_to_tweet_id=id)
+                return response
+            except Exception as e:
+                log.error(f'Error creating thread. Error: {e}')
+        else:
+            try:
+                response = client.create_tweet(text=text)
+                log.info(f'Tweet created successfully. ID: {response.data["id"]}')
+                return response
+            except Exception as e:
+                log.error(f'Error creating tweet. Error: {e}')
+            
+        
+
 if __name__ == '__main__':
     img = '/home/drakon/Documents/DEV/projetos/easy_post_twitter/imgs/market1.png'
     tw = Twitter(with_images=True)
     status = 'B3 interbank deposit futures: today and a month ago #FuturodoCDI #mercadofinanceiro'
     tw.tweet_to_publish_with_image(text=status, imgs=img, sequential=False)
```

