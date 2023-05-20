# Comparing `tmp/tootbot-7.0.3.tar.gz` & `tmp/tootbot-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootbot-7.0.3.tar", last modified: Sun Mar  5 05:23:16 2023, max compression
+gzip compressed data, was "tootbot-7.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tootbot-7.0.3.tar` & `tootbot-7.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4489 2023-03-05 05:16:32.980257 tootbot-7.0.3/README.rst
--rw-r--r--   0        0        0     3833 2023-03-05 05:16:32.984257 tootbot-7.0.3/pyproject.toml
--rw-r--r--   0        0        0      698 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/__init__.py
--rw-r--r--   0        0        0     7676 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/app.py
--rw-r--r--   0        0        0    34170 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/collect.py
--rw-r--r--   0        0        0    15815 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/control.py
--rw-r--r--   0        0        0     4774 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/create_config.py
--rw-r--r--   0        0        0     4497 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/debug.py
--rw-r--r--   0        0        0     2472 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/monitoring.py
--rw-r--r--   0        0        0    17147 2023-03-05 05:16:32.984257 tootbot-7.0.3/src/tootbot/publish.py
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4489 2023-05-20 04:42:27.706811 tootbot-7.1.0/README.rst
+-rw-r--r--   0        0        0     3833 2023-05-20 04:42:27.714810 tootbot-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/__init__.py
+-rw-r--r--   0        0        0     7645 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/app.py
+-rw-r--r--   0        0        0    31577 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/collect.py
+-rw-r--r--   0        0        0    18239 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/control.py
+-rw-r--r--   0        0        0     4774 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/create_config.py
+-rw-r--r--   0        0        0     4466 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/debug.py
+-rw-r--r--   0        0        0     2472 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/monitoring.py
+-rw-r--r--   0        0        0    16491 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/publish.py
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.1.0/PKG-INFO
```

### Comparing `tootbot-7.0.3/README.rst` & `tootbot-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `tootbot-7.0.3/pyproject.toml` & `tootbot-7.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tootbot-7.0.3/src/tootbot/__init__.py` & `tootbot-7.1.0/src/tootbot/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Package 'tootbot' level definitions."""
 import sys
 from typing import Final
 
-__version__: Final[str] = "7.0.3"
+__version__: Final[str] = "7.1.0"
 __display_name__: Final[str] = "Tootbot"
 __package_name__: Final[str] = __display_name__.lower()
 
 # Package level Static Variables
 POST_RECORDER_SQLITE_DB: Final[str] = "history.db"
+POST_RECORDER_HISTORY_RETENTION_DAYS: Final[int] = 31
 USER_AGENT: Final[str] = __display_name__
 CLIENT_WEBSITE: Final[str] = "https://pypi.org/project/tootbot/"
 PROGRESS_BAR_FORMAT: Final[
     str
 ] = "{desc}: {percentage:3.0f}%|{bar}| Eta: {remaining} - Elapsed: {elapsed}"
 FATAL_TOOTBOT_ERROR: Final[str] = "Tootbot cannot continue, now shutting down"
 VERSION_DEBUG: Final[
```

### Comparing `tootbot-7.0.3/src/tootbot/app.py` & `tootbot-7.1.0/src/tootbot/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
         progress_bar.update(0.0002)
 
         reddit = RedditHelper(config=config, api_secret=secrets["reddit"])
         progress_bar.update(0.0008)
 
         try:
             media_helper = LinkedMediaHelper(
-                config=config,
                 imgur_secrets=secrets["imgur"],
             )
             progress_bar.update(0.999)
         except ImgurClientError as imgur_error:
             logger.error("Error on creating ImgurClient: %s", imgur_error)
             logger.error(FATAL_TOOTBOT_ERROR)
             await config.bot.post_recorder.close_db()
```

### Comparing `tootbot-7.0.3/src/tootbot/collect.py` & `tootbot-7.1.0/src/tootbot/collect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,67 @@
 """Helper classes and methods to assist with the collection of content to be posted to Mastodon."""
 import asyncio
 import configparser
 import hashlib
 import logging
 import os
 import re
+import tempfile
+from dataclasses import dataclass
 from typing import Any
 from typing import Dict
-from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import TypeVar
 from urllib.parse import urlsplit
 
 import aiofiles
 import aiohttp
+import arrow
 import asyncpraw.exceptions
 import asyncprawcore
 import magic
 import yt_dlp.utils
 from asyncpraw.models import Submission
 from imgurpython import ImgurClient
 from imgurpython.helpers.error import ImgurClientError
+from imgurpython.helpers.error import ImgurClientRateLimitError
 from tqdm import tqdm
 from tqdm.asyncio import tqdm as aiotqdm
 
 from . import PROGRESS_BAR_FORMAT
 from . import USER_AGENT
 from . import __display_name__
 from .control import Configuration
 from .control import Secret
 from .control import SubredditConfig
 
 logger = logging.getLogger(__display_name__)
 
 RH = TypeVar("RH", bound="RedditHelper")
 LMH = TypeVar("LMH", bound="LinkedMediaHelper")
-MA = TypeVar("MA", bound="MediaAttachment")
 
 
-async def get_file(img_url: str, file_path: str, progress_label: str) -> Optional[str]:
-    """Save a file located at img_url to a file located at filepath.
-
-    :param img_url: url of imgur image to download
-    :param file_path: directory and filename where to save the downloaded image to
-    :param progress_label: Message to add to progress bar
-
-    :returns:
-        file_path (string): path to downloaded image or None if no image was downloaded
-    """
-    logger.debug(
-        "collect.py - get_file(img_url=%s, file_path=%s, progress_label=%s)",
-        img_url,
-        file_path,
-        progress_label,
-    )
-    chunk_size = 64 * 1024
-    try:
-        client = aiohttp.ClientSession(raise_for_status=True)
-        meta = await client.head(url=img_url)
-        download_size = int(meta.headers["content-length"])
-
-        file_out = await aiofiles.open(file=file_path, mode="wb")
-        progress_bar = tqdm(
-            unit="B",
-            unit_scale=True,
-            unit_divisor=1024,
-            desc=f"{progress_label:.<60}",
-            ncols=120,
-            total=download_size,
-            leave=True,
-        )
-        response = await client.get(url=img_url)
-        async for data_chunk in response.content.iter_chunked(chunk_size):
-            await file_out.write(data_chunk)
-            progress_bar.update(len(data_chunk))
-
-        await file_out.close()
-        await client.close()
-        await asyncio.sleep(0)  # allow client session to close before continuing
-        logger.debug("collect.py - get_file(...) -> file_path=%s", file_path)
-        return file_path
-
-    except aiohttp.ClientError as save_image_error:
-        logger.error(
-            "collect.py - get_file(...) -> None - download failed with: %s",
-            save_image_error,
-        )
-        return None
+@dataclass()
+class Attachment:
+    """Represents a media attachment. temp_file is a temporary file object containing media attachment content."""
+
+    temp_file: Any
+    mime_type: Optional[str]
+    checksum: Optional[str]
+
+    def __init__(self) -> None:
+        """Create temporary file object to store the content of the media attachment."""
+        self.temp_file = tempfile.TemporaryFile()
+        self.checksum = None
+        self.mime_type = None
+
+    def __del__(self) -> None:
+        """Close temporary file object when deleting attachment instance. This will also clean up the temporary file."""
+        self.temp_file.close()
 
 
 async def get_secrets(config_dir: str) -> Dict[str, Secret]:
     """Collect all api secrets either from already store secrets files or from user input.
 
     :param config_dir: directory to check read config.ini file from
     """
@@ -386,299 +356,379 @@
             else:
                 caption += submission.shortlink
         caption += promo_string
         return caption
 
 
 class LinkedMediaHelper:
-    """ImgurHelper provides methods to collect data / content from Imgur and
-    Gfycat.
-    """
+    """Helper class providing methods to get media attachments."""
 
     def __init__(
         self: LMH,
-        config: Configuration,
         imgur_secrets: Secret,
     ) -> None:
         """Initialise LinkedMediaHelper instance.
 
-        :param config: Configuration settings
         :param imgur_secrets: secrets to use with imgur api
 
         """
-        self.save_dir = config.media.folder
+        self.imgur_client = None
+        try:
+            self.imgur_client = ImgurClient(
+                client_id=imgur_secrets.client_id,
+                client_secret=imgur_secrets.client_secret,
+            )
 
-        self.imgur_client = ImgurClient(
-            client_id=imgur_secrets.client_id,
-            client_secret=imgur_secrets.client_secret,
-        )
+            logger.debug(
+                "Imgur rate limiting information: %s", self.imgur_client.credits
+            )
+            reset_epoch = self.imgur_client.credits.get("UserReset")
+            if reset_epoch:
+                reset_at = arrow.get(reset_epoch).format("YYYY-MM-DD HH:mm:ss")
+                reset_in = arrow.get(reset_epoch).humanize()
+                logger.debug("Imgur rate limit resetting %s at %s", reset_in, reset_at)
+        except ImgurClientRateLimitError as rate_limited:
+            logger.error("Hit ratelimit at imgur: %s", rate_limited)
+
+    async def get_attachments(  # noqa: C901
+        self: LMH,
+        reddit_post: Submission,
+    ) -> List[Attachment]:
+        """Determine which method to call depending on which site the media_url is pointing to.
+
+        :returns:
+        list of Attachment objects
+        """
+        attachments: List[Attachment] = []
+        single_attachment = None
+        multiple_attachments = None
+
+        # Download and save the linked media
+        if any(s in reddit_post.url for s in ("i.redd.it", "i.reddituploads.com")):
+            single_attachment = await LinkedMediaHelper.get_reddit_image(
+                reddit_post.url
+            )
+
+        elif "v.redd.it" in reddit_post.url and not reddit_post.media:
+            logger.error(
+                "Reddit API returned no media for this URL: %s",
+                reddit_post.url,
+            )
+        elif "v.redd.it" in reddit_post.url:
+            single_attachment = await self.get_reddit_video(reddit_post)
+
+        elif "imgur.com" in reddit_post.url:
+            multiple_attachments = await self.get_imgur_image(reddit_post.url)
+
+        # Todo: Gfycat might be defunct and might soon need to be removed
+        elif "gfycat.com" in reddit_post.url:
+            single_attachment = await LinkedMediaHelper.get_gfycat_image(
+                reddit_post.url
+            )
+
+        elif "giphy.com" in reddit_post.url:
+            single_attachment = await LinkedMediaHelper.get_giphy_image(reddit_post.url)
+
+        elif "reddit.com/gallery/" in reddit_post.url:  # Need to check for gallery post
+            if hasattr(reddit_post, "is_gallery"):
+                logger.debug("%s is a gallery post", reddit_post.id)
+                multiple_attachments = await LinkedMediaHelper.get_reddit_gallery(
+                    reddit_post
+                )
+
+        else:
+            single_attachment = await LinkedMediaHelper.get_generic_image(
+                reddit_post.url
+            )
+
+        if single_attachment:
+            attachments.append(single_attachment)
+        if multiple_attachments:
+            attachments.extend(multiple_attachments)
+
+        return attachments
+
+    @staticmethod
+    async def get_single_attachment(
+        att_url: str,
+        progress_label: str,
+    ) -> Optional[Attachment]:
+        """Download single attachment and store in an Attachment instance.
+        Calculates a checksum for the content of this media.
+        Determine mime/type.
+
+        :param att_url: URL from which the media attachment should be collected
+        :param progress_label: Label to use for progress bar
+
+        :returns:
+        Attachment instance or None
+        """
+        chunk_size = 64 * 1024
+
+        attachment = Attachment()
+        try:
+            client = aiohttp.ClientSession(raise_for_status=True)
+            meta = await client.head(url=att_url)
+            download_size = int(meta.headers["content-length"])
+            attachment.mime_type = str(meta.headers.get("content-type", None))
+            sha256 = hashlib.sha256()
+
+            progress_bar = tqdm(
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+                desc=f"{progress_label:.<60}",
+                ncols=120,
+                total=download_size,
+                leave=True,
+            )
+            response = await client.get(url=att_url)
+            async for data_chunk in response.content.iter_chunked(chunk_size):
+                attachment.temp_file.write(data_chunk)
+                sha256.update(data_chunk)
+                progress_bar.update(len(data_chunk))
+
+            await client.close()
+            attachment.checksum = sha256.hexdigest()
+            logger.debug(
+                "collect.py - get_attachment(...) -> Attachment=%s", attachment
+            )
+            return attachment
+
+        except aiohttp.ClientError as save_image_error:
+            logger.error(
+                "collect.py - get_attachment(...) -> None - download failed with: %s",
+                save_image_error,
+            )
+            return None
 
     async def get_imgur_image(
-        self: LMH, img_url: str, max_images: int = 4
-    ) -> List[str]:
+        self: LMH,
+        img_url: str,
+        max_images: int = 4,
+    ) -> List[Attachment]:
         """Download images from imgur.
 
         :param img_url: url of imgur image to download
         :param max_images: maximum number of images to download and process, Defaults to 4
 
         :returns:
-        path to downloaded image or None if no image was downloaded
+        list of attachments, will be empty list if no attachments
         """
+        attachments: List[Attachment] = []
+        if not self.imgur_client:
+            return attachments
+
         # Working demo of regex: https://regex101.com/r/G29uGl/2
         regex = r"(?:.*)imgur\.com(?:\/gallery\/|\/a\/|\/)(.*?)(?:\/.*|\.|$)"
         regex_match = re.search(regex, img_url, flags=0)
 
         if not regex_match:
             logger.error("Could not identify Imgur image/gallery ID at: %s", img_url)
             return []
 
         # Get the Imgur image/gallery ID
         imgur_id = regex_match.group(1)
 
         image_urls = self._get_image_urls(img_url, imgur_id)
 
         # Download and process individual images (up to max_images)
-        imgur_paths: List[str] = []
         for url in image_urls:
-            # If the URL is a GIFV or MP4 link, change it to the GIF version
-            file_extension = os.path.splitext(url)[-1].lower()
             image_url = url
-            if file_extension == ".gifv":
-                file_extension = ".gif"
-                image_url = url.replace(".gifv", ".gif")
-            elif file_extension == ".mp4":
-                file_extension = ".gif"
-                image_url = url.replace(".mp4", ".gif")
-
-            # Download the image
-            file_path = (
-                self.save_dir
-                + "/"
-                + imgur_id
-                + "_"
-                + str(len(imgur_paths))
-                + file_extension
-            )
-            logger.debug(
-                "Downloading Imgur image at URL %s to %s", image_url, file_path
-            )
-            saved_paths = await get_file(
-                img_url=image_url,
-                file_path=file_path,
+            logger.debug("Downloading Imgur image at URL %s", image_url)
+
+            attachment = await LinkedMediaHelper.get_single_attachment(
+                att_url=image_url,
                 progress_label="Downloading Imgur image",
             )
 
-            # Imgur will sometimes return a single-frame thumbnail
-            # instead of a GIF, so we need to check for this
-            if saved_paths and (
-                file_extension != ".gif" or self._check_imgur_gif(saved_paths)
-            ):
-                imgur_paths.append(saved_paths)
+            if attachment:
+                attachments.append(attachment)
 
-            if len(imgur_paths) == max_images:
+            if len(attachments) == max_images:
                 break
 
-        return imgur_paths
+        return attachments
 
     def _get_image_urls(self: LMH, img_url: str, imgur_id: str) -> List[str]:
         """Build a list of urls of all Imgur images identified by imgur_id.
 
         :param img_url: URL to IMGUR post
         :param imgur_id: ID for IMGUR post
 
         :returns:
         imgur_urls: List of urls to images of Imgur post identified byr imgur_id
         """
-        image_urls = []
+        image_urls: List[str] = []
+        if self.imgur_client is None:
+            return image_urls
+
         try:
             if any(s in img_url for s in ("/a/", "/gallery/")):  # Gallery links
                 logger.debug("Imgur link points to gallery: %s", img_url)
                 images = self.imgur_client.get_album_images(imgur_id)
                 for image in images:
                     image_urls.append(image.link)
             else:  # Single image
                 imgur_img = self.imgur_client.get_image(imgur_id)
                 image_urls = [imgur_img.link]  # pylint: disable=no-member
 
+            logger.debug(
+                "Imgur rate limiting information: %s", self.imgur_client.credits
+            )
+            reset_epoch = self.imgur_client.credits.get("UserReset")
+            if reset_epoch:
+                reset_at = arrow.get(reset_epoch).format("YYYY-MM-DD HH:mm:ss")
+                reset_in = arrow.get(reset_epoch).humanize()
+                logger.debug("Imgur rate limit resetting %s at %s", reset_in, reset_at)
+
         except ImgurClientError as imgur_error:
             logger.error("Could not get information from imgur: %s", imgur_error)
+        except ImgurClientRateLimitError as rate_limited:
+            logger.error("Hit ratelimit at imgur: %s", rate_limited)
+            logger.debug("Imgur Rate Limits: %s", self.imgur_client.credits)
         return image_urls
 
-    def _check_imgur_gif(self: LMH, file_path: str) -> bool:
-        """Check if a file downloaded from imgur is indeed a gif. If file is not a gif, remove the file.
-
-        :param file_path: file name and path to downloaded image
-
-        :returns:
-        True if downloaded image is indeed a GIF, otherwise returns False
-        """
-        mime = magic.from_file(filename=file_path, mime=True)
-        if mime != "image/gif":
-            logger.warning("Imgur: not a GIF, not posting")
-            try:
-                os.remove(file_path)
-            except OSError as remove_error:
-                logger.error("Error while deleting media file: %s", remove_error)
-            return False
-
-        return True
-
-    def get_gfycat_image(self: LMH, img_url: str) -> Optional[str]:
+    # Todo: Gfycat might be defunct and might soon need to be removed
+    @staticmethod
+    async def get_gfycat_image(img_url: str) -> Optional[Attachment]:
         """Download full resolution images from gfycat.
 
         :param img_url: url of gfycat image to download
 
         :returns:
-        file_path (string): path to downloaded image or None if no image was downloaded
+        Attachment or None
         """
         logger.debug("LinkedMediaHelper.get_gfycat_image(img_url=%s)", img_url)
 
-        saved_paths = LinkedMediaHelper._get_video_with_yt_dlp(
-            video_url=img_url,
-            save_as=self.save_dir + "/" + os.path.basename(urlsplit(img_url).path),
-        )
-        return saved_paths
+        attachment = await LinkedMediaHelper._get_video_with_yt_dlp(video_url=img_url)
+        return attachment
 
-    async def get_reddit_image(self: LMH, img_url: str) -> Optional[str]:
+    @staticmethod
+    async def get_reddit_image(img_url: str) -> Optional[Attachment]:
         """Download full resolution images from i.reddit or reddituploads.com.
 
-        :param img_url (string): url of imgur image to download
+        :param img_url: url of imgur image to download
 
         :returns:
-        file_path (string): path to downloaded image or None if no image was downloaded
+        Attachment or None
         """
-        file_name = os.path.basename(urlsplit(img_url).path)
+        os.path.basename(urlsplit(img_url).path)
         file_extension = os.path.splitext(img_url)[1].lower()
         # Fix for issue with i.reddituploads.com links not having a
         # file extension in the URL
         if not file_extension:
-            file_extension += ".jpg"
-            file_name += ".jpg"
             img_url += ".jpg"
-        # Download the file
-        file_path = self.save_dir + "/" + file_name
+
         logger.debug(
-            "Downloading file at URL %s to %s, file type identified as %s",
+            "LinkedMediaHelper.get_reddit_image(img_url=%s)",
             img_url,
-            file_path,
-            file_extension,
         )
 
-        saved_path = await get_file(
-            img_url=img_url,
-            file_path=file_path,
-            progress_label="Downloading reddit image",
+        attachment = await LinkedMediaHelper.get_single_attachment(
+            att_url=img_url, progress_label="Downloading reddit image"
         )
 
-        return saved_path
+        return attachment
 
+    @staticmethod
     async def get_reddit_gallery(
-        self: LMH,
         reddit_post: Submission,
         max_images: int = 4,
-    ) -> List[Optional[str]]:
+    ) -> List[Attachment]:
         """Download up to max_images images from a reddit gallery post and returns a List of file_paths
         downloaded images.
 
         :param reddit_post:  reddit post / submission object
         :param max_images: [optional] maximum number of images to download. Default is 4
 
         :returns:
-        file_paths (List[str]) a list of the paths to downloaded files. If no images have been downloaded, and empty
-        list will be returned.
+        attachments (List[Attachment]) a list of media attachments to be posted. Empty list if no attachments.
         """
-        file_paths: List[Optional[str]] = []
-        if reddit_post.gallery_data.get("items"):
-            gallery_items: List[Dict[str, Any]] = reddit_post.gallery_data["items"]
+        attachments: List[Attachment] = []
+        if gallery_items := reddit_post.gallery_data.get("items"):
             tasks: List[Any] = []
             for item in gallery_items:
                 media_id = item["media_id"]
                 meta = reddit_post.media_metadata[media_id]
                 logger.debug("Media Metadata: %s", meta)
                 if "e" in meta and meta["e"] == "Image":
                     source = meta["s"]
-                    save_path = (
-                        self.save_dir + "/" + media_id + "." + meta["m"].split("/")[1]
-                    )
-                    logger.debug(
-                        "Gallery file_path, source: %s - %s", save_path, source["u"]
-                    )
                     tasks.append(
-                        get_file(source["u"], save_path, f"image {len(tasks)+1}")
+                        LinkedMediaHelper.get_single_attachment(
+                            att_url=source["u"],
+                            progress_label=f"image {len(tasks) + 1}",
+                        ),
                     )
 
                     if len(tasks) == max_images:
                         break
 
             print("Downloading images from reddit gallery")
-            file_paths = await asyncio.gather(*tasks)
+            attachments = await asyncio.gather(*tasks)
 
-        return file_paths
+        return attachments
 
-    def get_reddit_video(self: LMH, reddit_post: Submission) -> Optional[str]:
+    @staticmethod
+    async def get_reddit_video(reddit_post: Submission) -> Optional[Attachment]:
         """Download full resolution video from i.reddit or reddituploads.
 
         :param reddit_post: reddit post / submission object
 
         :returns:
-        file_path (string): path to downloaded video or None if no image was downloaded
+        attachment or None
         """
         logger.debug(
             "LinkedMediaHelper.get_reddit_video(reddit_post = %s)",
             reddit_post.id,
         )
         logger.debug(
             "LinkedMediaHelper.get_reddit_video - reddit_post.media: \n%s)",
             reddit_post.media,
         )
 
         # Download video with yt-dlp
         yt_dlp_url = reddit_post.media["reddit_video"]["hls_url"]
         print(f"Downloading Reddit video from {yt_dlp_url}")
 
-        filepath = LinkedMediaHelper._get_video_with_yt_dlp(
-            video_url=yt_dlp_url,
-            save_as=self.save_dir + "/" + reddit_post.id,
+        attachment = await LinkedMediaHelper._get_video_with_yt_dlp(
+            video_url=yt_dlp_url
         )
-        return filepath
+        return attachment
 
     @staticmethod
-    def _get_video_with_yt_dlp(video_url: str, save_as: str) -> Optional[str]:
+    async def _get_video_with_yt_dlp(video_url: str) -> Optional[Attachment]:
         """Download video files with embedded yt-dlp.
 
         :param video_url: URL for video to download
-        :param save_as: path and file name excluding file extension for yt-dlp to
-                download video file to
 
         :returns:
             (string) containing file name inclusive file extension and path where yt-dlp
                 has saved the downloaded video.
                 This can be None if yt-dlp has been unsuccessful.
         """
         logger.debug(
-            "LinkedMediaHelper._get_video_with_yt_dlp(video_url=%s, save_as=%s)",
+            "LinkedMediaHelper._get_video_with_yt_dlp(video_url=%s)",
             video_url,
-            save_as,
         )
         yt_dlp_options = {
-            "outtmpl": save_as + ".%(ext)s",
             "quiet": "true",
             "ignoreerrors": "true",
             "progress": "true",
             "format": "bestvideo+bestaudio",
         }
 
         with yt_dlp.YoutubeDL(yt_dlp_options) as ytdl:
             meta = ytdl.extract_info(video_url, download=True)
             meta_san = ytdl.sanitize_info(meta)
 
         # If there was an error with yt-dlp download meta will be None
         if not meta:
             logger.debug(
-                "LinkedMediaHelper.get_reddit_video - yt-dlp unsuccessful -> None"
+                "LinkedMediaHelper._get_video_with_yt_dlp - yt-dlp unsuccessful -> None"
             )
             return None
 
         yt_dlp_filepath: str = meta.get("filepath")
         if yt_dlp_filepath:
             logger.debug(
                 "LinkedMediaHelper.get_reddit_video - yt-dlp DIRECT filepath: '%s'",
@@ -690,57 +740,85 @@
                 "LinkedMediaHelper.get_reddit_video - yt-dlp 3 DEEP filepath: '%s'",
                 yt_dlp_filepath,
             )
         logger.debug(
             "LinkedMediaHelper.get_reddit_video (...) -> '%s'", yt_dlp_filepath
         )
 
-        return yt_dlp_filepath
+        # Spool downloaded file into a temporary file in an Attachment class instance
+        attachment = await LinkedMediaHelper._attachment_from_file(
+            filepath=yt_dlp_filepath
+        )
+
+        return attachment
 
-    async def get_giphy_image(self: LMH, img_url: str) -> Optional[str]:
+    @staticmethod
+    async def _attachment_from_file(filepath: str) -> Attachment:
+        """Convert standard file to an Attachment instance.
+
+        :param filepath: path to file to convert
+
+        :returns:
+        instance of Attachment
+        """
+        chunk_size = 64 * 1024
+
+        attachment = Attachment()
+        sha256 = hashlib.sha256()
+        async with aiofiles.open(file=filepath, mode="rb") as input_file:
+            while True:
+                data_chunk = await input_file.read(chunk_size)
+                if not data_chunk:
+                    break
+                attachment.temp_file.write(data_chunk)
+                sha256.update(data_chunk)
+        attachment.checksum = sha256.hexdigest()
+        attachment.mime_type = magic.from_file(filename=filepath, mime=True)
+        os.remove(filepath)
+
+        return attachment
+
+    @staticmethod
+    async def get_giphy_image(img_url: str) -> Optional[Attachment]:
         """Download full or low resolution image from giphy.
 
         :param img_url: url of giphy image to download
 
         :returns:
-        file_path (string): path to downloaded image or None if no image was downloaded
+        Attachment or None
         """
-        # Working demo of regex: https://regex101.com/r/o8m1kA/2
-        regex = (
-            r"https?://((?:.*)giphy\.com/media/|giphy.com"
-            r"/gifs/|i.giphy.com/)(.*-)?(\w+)(/|\n)"
-        )
-        match = re.search(regex, img_url, flags=0)
+        # Working demo of regex: https://regex101.com/r/Cw6YJc/1
+        regex = r"https?://((?:.*)giphy\.com/media/|giphy.com/gifs/|i.giphy.com/)(.*-)?(\w+)"
+        match = re.match(pattern=regex, string=img_url, flags=0)
         if not match:
             logger.error("Could not identify Giphy ID in this URL: %s", img_url)
             return None
 
         # Get the Giphy ID
         giphy_id = match.group(3)
         # Download the MP4 version of the GIF
         giphy_url = "https://media.giphy.com/media/" + giphy_id + "/giphy.mp4"
-        file_path = self.save_dir + "/" + giphy_id + "giphy.mp4"
 
-        saved_paths = await get_file(
-            img_url=giphy_url,
-            file_path=file_path,
+        attachment = await LinkedMediaHelper.get_single_attachment(
+            att_url=giphy_url,
             progress_label="Downloading Giphy image/video",
         )
 
-        logger.debug("Downloaded Giphy at URL %s to %s", giphy_url, saved_paths)
+        logger.debug("Downloaded Giphy from URL %s", giphy_url)
 
-        return saved_paths
+        return attachment
 
-    async def get_generic_image(self: LMH, img_url: str) -> Optional[str]:
+    @staticmethod
+    async def get_generic_image(img_url: str) -> Optional[Attachment]:
         """Download image or video from a generic url to a media file.
 
         :param img_url: url to image or video file
 
         :returns:
-        file_path (string): path to downloaded video or None if no image was downloaded
+        attachment: media attachment
         """
         logger.debug("LinkedMediaHelper.get_generic_image(img_url=%s)", img_url)
 
         # First check if URL starts with http:// or https://
         regex = r"^https?://"
         match = re.search(regex, img_url, flags=0)
         if not match:
@@ -770,138 +848,15 @@
             return None
 
         if content_type not in image_formats:
             logger.debug("URL does not point to a valid image file: %s", img_url)
             return None
 
         # URL appears to be an image, so download it
-        file_name = os.path.basename(urlsplit(img_url).path)
-        file_path = self.save_dir + "/" + file_name
-        logger.debug("Downloading file at URL %s to %s", img_url, file_path)
-
-        saved_path = await get_file(
-            img_url=img_url,
-            file_path=file_path,
+        logger.debug("Downloading file at URL %s", img_url)
+
+        attachment = await LinkedMediaHelper.get_single_attachment(
+            att_url=img_url,
             progress_label="Downloading generic image",
         )
 
-        return saved_path
-
-
-class MediaAttachment:
-    """MediaAttachment contains code to retrieve the appropriate images or
-    videos to include in a reddit post to be shared on Mastodon.
-    """
-
-    def __init__(
-        self: MA, reddit_post: Submission, image_helper: LinkedMediaHelper
-    ) -> None:
-        """Initialise MediaAttachment instance.
-
-        :param reddit_post: reddit post / submission
-        :param image_helper: MediaHelper to deal with images or videos linked in reddit post
-        """
-        self.media_paths: Dict[str, str] = {}
-        self.reddit_post = reddit_post
-        self.media_url = self.reddit_post.url
-        self.image_helper = image_helper
-
-    async def get_media_files(self: MA) -> None:
-        """Download media files linked to given reddit_post."""
-        logger.debug("URL for post(%s): %s ", self.reddit_post, self.media_url)
-
-        media_paths = await self.get_media()
-        for media_path in media_paths:
-            logger.debug("Media path for checksum calculation: %s", media_path)
-            if media_path:
-                sha256 = hashlib.sha256()
-                async with aiofiles.open(file=media_path, mode="rb") as media_file:
-                    # Read and update hash string value in blocks of 64K
-                    while True:
-                        data = await media_file.read(2**16)
-                        if not data:
-                            break
-                        sha256.update(data)
-
-                self.media_paths[sha256.hexdigest()] = media_path
-
-    def destroy(self: MA) -> None:
-        """Remove any files downloaded and clear out the object attributes."""
-        try:
-            for media_path in self.media_paths.values():
-                if media_path is not None:
-                    os.remove(media_path)
-                    logger.debug("Deleted media file at %s", media_path)
-        except OSError as delete_error:
-            logger.error("Error while deleting media file: %s", delete_error)
-
-        self.media_paths = {}
-        self.media_url = None
-
-    def destroy_one_attachment(self: MA, checksum: str) -> None:
-        """Remove file with checksum downloaded.
-
-        :param checksum: key to media_paths dictionary for file to be removed.
-        """
-        try:
-            media_path = self.media_paths[checksum]
-            if media_path is not None:
-                os.remove(media_path)
-                logger.debug("Deleted media file at %s", media_path)
-            self.media_paths.pop(checksum)
-        except OSError as delete_error:
-            logger.error("Error while deleting media file: %s", delete_error)
-
-    async def get_media(self: MA) -> List[Optional[str]]:
-        """Determine which method to call depending on which site the media_url is pointing to.
-
-        :returns:
-        list of file-paths of downloaded images. Can be None
-        """
-        if not os.path.exists(self.image_helper.save_dir):
-            os.makedirs(self.image_helper.save_dir)
-            logger.debug(
-                "Media folder not found, created new folder: %s",
-                self.image_helper.save_dir,
-            )
-
-        file_paths = []
-        saved_media_path: Optional[str]
-        saved_media_paths: Iterable[Optional[str]]
-
-        # Download and save the linked image
-        if any(s in self.media_url for s in ("i.redd.it", "i.reddituploads.com")):
-            saved_media_path = await self.image_helper.get_reddit_image(self.media_url)
-            file_paths.append(saved_media_path)
-        elif "v.redd.it" in self.media_url and not self.reddit_post.media:
-            logger.error(
-                "Reddit API returned no media for this URL: %s", self.media_url
-            )
-        elif "v.redd.it" in self.media_url:
-            saved_media_path = self.image_helper.get_reddit_video(self.reddit_post)
-            file_paths.append(saved_media_path)
-
-        elif "imgur.com" in self.media_url:
-            saved_media_paths = await self.image_helper.get_imgur_image(self.media_url)
-            file_paths.extend(saved_media_paths)
-
-        elif "gfycat.com" in self.media_url:
-            saved_media_path = self.image_helper.get_gfycat_image(self.media_url)
-            file_paths.append(saved_media_path)
-
-        elif "giphy.com" in self.media_url:
-            saved_media_path = await self.image_helper.get_giphy_image(self.media_url)
-            file_paths.append(saved_media_path)
-
-        elif "reddit.com/gallery/" in self.media_url:  # Need to check for gallery post
-            if hasattr(self.reddit_post, "is_gallery"):
-                logger.debug("%s is a gallery post", self.reddit_post.id)
-                save_media_paths = await self.image_helper.get_reddit_gallery(
-                    self.reddit_post
-                )
-                file_paths.extend(save_media_paths)
-
-        else:
-            saved_media_path = await self.image_helper.get_generic_image(self.media_url)
-            file_paths.append(saved_media_path)
-
-        return file_paths
+        return attachment
```

### Comparing `tootbot-7.0.3/src/tootbot/control.py` & `tootbot-7.1.0/src/tootbot/control.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import sys
 from dataclasses import dataclass
 from logging import DEBUG
 from logging import Formatter
 from logging import StreamHandler
 from logging import getLogger
 from logging.handlers import TimedRotatingFileHandler
+from sqlite3 import OperationalError
 from typing import Any
 from typing import Final
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import aiosqlite
+import arrow
 from minimal_activitypub import __display_name__ as minimal_activitypub_logger
 
+from . import POST_RECORDER_HISTORY_RETENTION_DAYS
 from . import POST_RECORDER_SQLITE_DB
 from . import __display_name__
 
 PR = TypeVar("PR", bound="PostRecorder")
 ConfigClass = TypeVar("ConfigClass", bound="Configuration")
 
 logger = getLogger(__display_name__)
@@ -44,37 +47,88 @@
         self.history_db: Optional[aiosqlite.Connection] = None
 
     async def db_init(self: PR) -> None:
         """Initialise DB connection and tables if necessary."""
         self.history_db = await aiosqlite.connect(database=self.history_db_file)
         # Make sure DB tables exist
         await self.history_db.execute(
-            "CREATE TABLE IF NOT EXISTS post (id TEXT PRIMARY KEY) WITHOUT ROWID"
+            "CREATE TABLE IF NOT EXISTS history (created_at FLOAT NOT NULL PRIMARY KEY, "
+            "id TEXT, url TEXT, checksum TEXT)"
         )
         await self.history_db.execute(
-            "CREATE TABLE IF NOT EXISTS share "
-            "(url TEXT PRIMARY KEY) "
+            "CREATE TABLE IF NOT EXISTS settings "
+            "(key TEXT PRIMARY KEY, value) "
             "WITHOUT ROWID"
         )
+
+        # Create indexes
         await self.history_db.execute(
-            "CREATE TABLE IF NOT EXISTS hash "
-            "(checksum TEXT PRIMARY KEY) "
-            "WITHOUT ROWID"
+            "CREATE UNIQUE INDEX IF NOT EXISTS created_at_index ON history (created_at)"
         )
         await self.history_db.execute(
-            "CREATE TABLE IF NOT EXISTS settings "
-            "(key TEXT PRIMARY KEY, value) "
-            "WITHOUT ROWID"
+            "CREATE INDEX IF NOT EXISTS id_index ON history (id)"
+        )
+        await self.history_db.execute(
+            "CREATE INDEX IF NOT EXISTS url_index ON history (url)"
         )
         await self.history_db.execute(
+            "CREATE INDEX IF NOT EXISTS checksum_index ON history (checksum)"
+        )
+
+        # Create default entries
+        await self.history_db.execute(
             "INSERT OR IGNORE INTO settings (key, value) VALUES (:key, :value)",
             {"key": PostRecorder.LAST_POST_TS, "value": 0},
         )
+
         await self.history_db.commit()
 
+        # Migrate data from old tables to new table
+        try:
+            async with self.history_db.execute("SELECT id FROM post") as cursor:
+                async for row in cursor:
+                    now_ts = arrow.now(tz="UTC").timestamp()
+                    await self.history_db.execute(
+                        "INSERT INTO history (created_at, id) VALUES (:ts, :id)",
+                        {"ts": now_ts, "id": row[0]},
+                    )
+            await self.history_db.execute("DROP TABLE post")
+            await self.history_db.commit()
+        except OperationalError:
+            # Skipping this error as it probably means that the old table post doesn't exist anymore
+            pass
+
+        try:
+            async with self.history_db.execute("SELECT url FROM share") as cursor:
+                async for row in cursor:
+                    now_ts = arrow.now(tz="UTC").timestamp()
+                    await self.history_db.execute(
+                        "INSERT INTO history (created_at, url) VALUES (:ts, :url)",
+                        {"ts": now_ts, "url": row[0]},
+                    )
+            await self.history_db.execute("DROP TABLE share")
+            await self.history_db.commit()
+        except OperationalError:
+            # Skipping this error as it probably means that the old table 'share' doesn't exist anymore
+            pass
+
+        try:
+            async with self.history_db.execute("SELECT checksum FROM hash") as cursor:
+                async for row in cursor:
+                    now_ts = arrow.now(tz="UTC").timestamp()
+                    await self.history_db.execute(
+                        "INSERT INTO history (created_at, checksum) VALUES (:ts, :checksum)",
+                        {"ts": now_ts, "checksum": row[0]},
+                    )
+            await self.history_db.execute("DROP TABLE hash")
+            await self.history_db.commit()
+        except OperationalError:
+            # Skipping this error as it probably means that the old table 'hash' doesn't exist anymore
+            pass
+
     async def duplicate_check(self: PR, identifier: str) -> bool:
         """Check identifier can be found in log file of content posted to
         Mastodon.
 
         :param identifier:
                 Any identifier we want to make sure has not already been posted.
                 This can be id of reddit post, url of media attachment file to be
@@ -88,31 +142,16 @@
         logger.debug("PostRecorder.duplicate_check(identifier=%s)", identifier)
 
         if self.history_db is None:
             raise AssertionError("Have you called db_init() first?")
 
         # check for reddit_id
         cursor = await self.history_db.execute(
-            "SELECT * FROM post where id=:id", {"id": identifier}
-        )
-        if await cursor.fetchone():
-            logger.debug("PostRecorder.duplicate_check(...) -> True")
-            return True
-
-        # check for Shared URL
-        cursor = await self.history_db.execute(
-            "SELECT * FROM share where url=:url", {"url": identifier}
-        )
-        if await cursor.fetchone():
-            logger.debug("PostRecorder.duplicate_check(...) -> True")
-            return True
-
-        # check for attachment hash
-        cursor = await self.history_db.execute(
-            "SELECT * FROM hash where checksum=:checksum", {"checksum": identifier}
+            "SELECT * FROM history WHERE id=:id OR url=:url OR checksum=:checksum",
+            {"id": identifier, "url": identifier, "checksum": identifier},
         )
         if await cursor.fetchone():
             logger.debug("PostRecorder.duplicate_check(...) -> True")
             return True
 
         logger.debug("PostRecorder.duplicate_check(...) -> False")
         return False
@@ -136,23 +175,22 @@
         logger.debug(
             "PostRecorder.log_post(reddit_id=%s ,shared_url= %s, checksum= %s)",
             reddit_id,
             shared_url,
             check_sum,
         )
 
+        now_ts = arrow.now(tz="UTC").timestamp()
         if self.history_db is None:
             raise AssertionError("Have you called db_init() first?")
 
-        if reddit_id:
-            await self.history_db.execute("INSERT INTO post VALUES (?)", (reddit_id,))
-        if shared_url:
-            await self.history_db.execute("INSERT INTO share VALUES (?)", (shared_url,))
-        if check_sum:
-            await self.history_db.execute("INSERT INTO hash VALUES (?)", (check_sum,))
+        await self.history_db.execute(
+            "INSERT INTO history (created_at, id, url, checksum) VALUES (:ts, :id, :url, :checksum)",
+            {"ts": now_ts, "id": reddit_id, "url": shared_url, "checksum": check_sum},
+        )
         await self.history_db.commit()
 
     async def get_setting(
         self: PR,
         key: str,
     ) -> Any:
         """Retrieve a setting from database.
@@ -202,15 +240,31 @@
         )
 
         await self.history_db.commit()
 
     async def close_db(self: PR) -> None:
         """Close db connection."""
         logger.debug("PostRecorder.close_db()")
+
+        delete_earlier_than_ts = (
+            arrow.now(tz="UTC")
+            .shift(days=-POST_RECORDER_HISTORY_RETENTION_DAYS)
+            .timestamp()
+        )
+        logger.debug(
+            "PostRecorder.close_db() - removing history prior to TS=%s",
+            delete_earlier_than_ts,
+        )
+
         if self.history_db:
+            await self.history_db.execute(
+                "DELETE FROM history WHERE created_at < :ts",
+                {"ts": delete_earlier_than_ts},
+            )
+            await self.history_db.commit()
             await self.history_db.close()
 
 
 @dataclass
 class Secret:
     """Dataclass for API login secrets."""
```

### Comparing `tootbot-7.0.3/src/tootbot/create_config.py` & `tootbot-7.1.0/src/tootbot/create_config.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.0.3/src/tootbot/debug.py` & `tootbot-7.1.0/src/tootbot/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,14 @@
             secrets=secrets["mastodon"],
         )
 
         reddit = RedditHelper(config=config, api_secret=secrets["reddit"])
 
         try:
             media_helper = LinkedMediaHelper(
-                config=config,
                 imgur_secrets=secrets["imgur"],
             )
         except ImgurClientError as imgur_error:
             logger.error("Error on creating ImgurClient: %s", imgur_error)
             logger.error(FATAL_TOOTBOT_ERROR)
             await config.bot.post_recorder.close_db()
             sys.exit(1)
```

### Comparing `tootbot-7.0.3/src/tootbot/monitoring.py` & `tootbot-7.1.0/src/tootbot/monitoring.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.0.3/src/tootbot/publish.py` & `tootbot-7.1.0/src/tootbot/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import aiofiles
 import aiohttp
-import magic
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ActivityPubError
 from tqdm.asyncio import tqdm
 
 from . import CLIENT_WEBSITE
 from . import USER_AGENT
 from . import __display_name__
+from .collect import Attachment
 from .collect import LinkedMediaHelper
-from .collect import MediaAttachment
 from .collect import RedditHelper
 from .control import BotConfig
 from .control import Configuration
 from .control import MastodonConfig
 from .control import PromoConfig
 from .control import Secret
 
@@ -172,15 +171,15 @@
                 file=secrets_file,
                 mode="r",
             ) as file:
                 mastodon_secrets.client_secret = await file.readline()
 
         return mastodon_secrets
 
-    async def make_post(  # noqa: C901
+    async def make_post(  # noqa: C901 PLR0912
         self: MP,
         posts: Dict[Any, Any],
         reddit_helper: RedditHelper,
         media_helper: LinkedMediaHelper,
         duplicate_checks: bool = True,
     ) -> None:
         """Post status on mastodon from a selection of reddit submissions.
@@ -210,53 +209,50 @@
 
             for post in source_posts:
                 # Find out if we have any attachments to include with toot.
                 logger.debug(
                     "MastodonPublisher.make_post - Getting attachments for post %s",
                     source_posts[post].id,
                 )
-                attachments = MediaAttachment(source_posts[post], media_helper)
-                await attachments.get_media_files()
+                attachments = await media_helper.get_attachments(
+                    reddit_post=source_posts[post]
+                )
                 if duplicate_checks:
-                    await self._remove_posted_earlier(attachments)
+                    attachments = await self._remove_posted_earlier(attachments)
 
                 # Make sure the post contains media,
                 # if MEDIA_POSTS_ONLY in config is set to True
-                logger.debug(
-                    "MastodonPublisher.make_post - attachments.media_paths: %s",
-                    attachments.media_paths,
-                )
-                if self.media_only and len(attachments.media_paths) == 0:
+                if self.media_only and len(attachments) == 0:
                     logger.warning(
                         "MastodonPublisher.make_post - "
                         "Skipping %s, non-media posts disabled or media file not found",
                         source_posts[post].id,
                     )
                     # Log the post anyway
                     if duplicate_checks:
                         await self.bot.post_recorder.log_post(
                             reddit_id=source_posts[post].id,
                         )
                         continue
 
-                try:
-                    # Generate promo message if needed
-                    promo_message = None
-                    if self.num_non_promo_posts >= self.promo.every > 0:
-                        promo_message = self.promo.message
-                        self.num_non_promo_posts = -1
-
-                    # Generate post caption
-                    caption = reddit_helper.get_caption(
-                        source_posts[post],
-                        MastodonPublisher.MAX_LEN_TOOT,
-                        add_hash_tags=additional_hashtags,
-                        promo_message=promo_message,
-                    )
+                # Generate promo message if needed
+                promo_message = None
+                if self.num_non_promo_posts >= self.promo.every > 0:
+                    promo_message = self.promo.message
+                    self.num_non_promo_posts = -1
+
+                # Generate post caption
+                caption = reddit_helper.get_caption(
+                    source_posts[post],
+                    MastodonPublisher.MAX_LEN_TOOT,
+                    add_hash_tags=additional_hashtags,
+                    promo_message=promo_message,
+                )
 
+                try:
                     # Upload media files if available
                     media_ids = await self._post_attachments(
                         attachments=attachments,
                         duplicate_checks=duplicate_checks,
                     )
                     if self.media_only and len(media_ids) == 0:
                         # Skip posts where no media has been able to be uploaded
@@ -300,147 +296,142 @@
                     # same error
                     await self.bot.post_recorder.log_post(
                         reddit_id=source_posts[post].id
                     )
                     self.mastodon_config.number_of_errors += 1
 
                 # Clean up media file
-                attachments.destroy()
+                for attachment in attachments:
+                    del attachment
+                del attachments
 
                 # Return control to main loop
                 break_to_mainloop = True
                 break
 
     async def _post_attachments(
         self: MP,
-        attachments: MediaAttachment,
+        attachments: List[Attachment],
         duplicate_checks: bool,
     ) -> List[str]:
         """_post_attachments post any media in attachments.media_paths list.
 
-        :param attachments: object with a list of paths to media to be posted on Mastodon
+        :param attachments: List of Attachment objects to be posted on Mastodon
         :param duplicate_checks: specifying if duplicate checks should be performed (True) or not (False)
 
         Returns
         -------
             media_ids: List of dicts returned by mastodon.media_post
         """
         media_ids: List[str] = []
-        if len(attachments.media_paths) == 0:
+        if len(attachments) == 0:
             return media_ids
 
         print("Uploading attachments")
         tasks: List[Any] = []
-        for checksum, media_path in attachments.media_paths.items():
-            mime_type = magic.from_file(media_path, mime=True)
-            logger.debug(
-                "MastodonPublisher._post_attachements - Media %s (%s) with checksum: %s",
-                media_path,
-                mime_type,
-                checksum,
-            )
-            attachment = FileManager(file_name=media_path)
+
+        for single_att in attachments:
+            attachment = FileManager(temp_file=single_att.temp_file)
             tasks.append(
                 self.instance.post_media(
                     file=attachment.file_reader(),
-                    mime_type=mime_type,
+                    mime_type=single_att.mime_type,
                 )
             )
 
             # Log the media upload
             if duplicate_checks:
-                await self.bot.post_recorder.log_post(check_sum=checksum)
+                await self.bot.post_recorder.log_post(check_sum=single_att.checksum)
         try:
             medias = await asyncio.gather(*tasks)
             for media in medias:
                 logger.debug("MastodonPublisher._post_attachments - result: %s", media)
                 media_ids.append(media.get("id"))
         except (ActivityPubError, TypeError) as error:
             logger.debug(
                 "MastodonPublisher._post_attachements - Error when uploading media: %s",
                 error,
             )
 
         logger.debug("MastodonPublisher._post_attachments - media_ids: %s", media_ids)
         return media_ids
 
-    async def _remove_posted_earlier(self: MP, attachments: MediaAttachment) -> None:
+    async def _remove_posted_earlier(
+        self: MP, attachments: List[Attachment]
+    ) -> List[Attachment]:
         """_remove_posted_earlier checks che checksum of all proposed
         attachments and removes any from the list that have already been posted
         earlier.
 
         :param attachments: object with list of paths to media files proposed to be
             posted on Mastodon
         :type attachments: MediaAttachment
         """
         # Build a list of checksums for files that have already been posted earlier
         logger.debug(
             "MastodonPublisher._remove_posted_earlier(attachments=%s)", attachments
         )
         logger.debug(
             "MastodonPublisher._remove_posted_earlier(...) - number of attachements %s",
-            len(attachments.media_paths),
+            len(attachments),
         )
-        checksums = []
-        for checksum in attachments.media_paths:
-            logger.debug(
-                "Media attachment (path, checksum): %s, %s",
-                attachments.media_paths[checksum],
-                checksum,
-            )
-            if attachments.media_paths[checksum] is None:
-                checksums.append(checksum)
-            # Check for duplicate of attachment sha256
-            elif await self.bot.post_recorder.duplicate_check(checksum):
+        non_duplicates = []
+        for attachment in attachments:
+            if attachment.checksum and await self.bot.post_recorder.duplicate_check(
+                attachment.checksum
+            ):
                 logger.debug(
                     "MastodonPublisher._remove_posted_earlier(...) - "
                     "Media with checksum %s has already been posted",
-                    checksum,
+                    attachment.checksum,
                 )
-                checksums.append(checksum)
-        # Remove all empty or previously posted images
-        for checksum in checksums:
-            attachments.destroy_one_attachment(checksum)
+                del attachment
+            else:
+                non_duplicates.append(attachment)
 
         logger.debug(
             "MastodonPublisher._remove_posted_earlier(...) - number of attachements after check %s",
-            len(attachments.media_paths),
+            len(non_duplicates),
         )
 
+        return non_duplicates
+
 
 class FileManager:
     """Class to wrap around file reads with a tqdm progress bar."""
 
     def __init__(
         self: FileManagerClass,
-        file_name: str,
+        temp_file: Any,
         chunk_size: int = 64 * 1024,
     ) -> None:
         """Initialise new FileManager instance.
 
-        :param file_name: Name of file
+        :param temp_file: file handle of TemporaryFile
         :param chunk_size: Size of chunks of data. Defaults to 64kb
         """
-        self.name = file_name
+        self.temp_file = temp_file
         self.chunk_size = chunk_size
-        self.size = os.path.getsize(self.name)
+        self.size = os.path.getsize(temp_file.name)
+        description = f"Attachment id {temp_file.name}"
         self.pbar = tqdm(
-            total=os.path.getsize(filename=self.name),
-            desc=f"{self.name:.<60}",
+            total=os.path.getsize(filename=temp_file.name),
+            desc=f"{description:.<60}",
             unit="B",
             unit_scale=True,
             unit_divisor=1024,
             ncols=120,
             leave=True,
         )
 
     async def file_reader(self: FileManagerClass) -> AsyncIterator[bytes]:
         """file_reader returns file contents in chunks of bytes and updates an
         associated progress bar.
         """
-        async with aiofiles.open(self.name, "rb") as file:
-            chunk = await file.read(self.chunk_size)
-            while chunk:
-                self.pbar.update(len(chunk))
-                yield chunk
-                chunk = await file.read(self.chunk_size)
-            self.pbar.close()
+        # async with aiofiles.open(self.name, "rb") as file:
+        self.temp_file.seek(0)
+        chunk = self.temp_file.read(self.chunk_size)
+        while chunk:
+            self.pbar.update(len(chunk))
+            yield chunk
+            chunk = self.temp_file.read(self.chunk_size)
+        self.pbar.close()
```

### Comparing `tootbot-7.0.3/PKG-INFO` & `tootbot-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootbot
-Version: 7.0.3
+Version: 7.1.0
 Summary: A Python bot that looks up posts from specified subreddits and automatically posts them on Mastodon
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
```

