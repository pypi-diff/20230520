# Comparing `tmp/pyskroutz-0.1.8.tar.gz` & `tmp/pyskroutz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyskroutz-0.1.8.tar", last modified: Thu Feb 11 21:09:40 2021, max compression
+gzip compressed data, was "pyskroutz-0.2.0.tar", max compression
```

## Comparing `pyskroutz-0.1.8.tar` & `pyskroutz-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)    35149 2021-01-14 22:34:19.000000 pyskroutz-0.1.8/LICENSE
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)       62 2021-01-14 22:56:23.000000 pyskroutz-0.1.8/MANIFEST.in
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     2417 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/PKG-INFO
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1334 2021-02-11 20:38:12.000000 pyskroutz-0.1.8/README.md
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)     1011 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/setup.cfg
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)      473 2021-01-20 22:11:55.000000 pyskroutz-0.1.8/setup.py
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/src/
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/src/pyskroutz/
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)      353 2021-02-11 21:00:24.000000 pyskroutz-0.1.8/src/pyskroutz/__init__.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     2106 2021-02-07 22:18:18.000000 pyskroutz-0.1.8/src/pyskroutz/client.py
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)       80 2021-01-25 10:02:35.000000 pyskroutz-0.1.8/src/pyskroutz/exceptions.py
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/src/pyskroutz/models/
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)      177 2021-01-24 17:37:09.000000 pyskroutz-0.1.8/src/pyskroutz/models/__init__.py
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)     2485 2021-01-29 22:24:46.000000 pyskroutz-0.1.8/src/pyskroutz/models/base.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1656 2021-02-07 21:20:14.000000 pyskroutz-0.1.8/src/pyskroutz/models/books.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1587 2021-02-07 21:20:14.000000 pyskroutz-0.1.8/src/pyskroutz/models/categories.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      440 2021-02-11 20:54:37.000000 pyskroutz-0.1.8/src/pyskroutz/models/flags.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      428 2021-02-07 21:20:14.000000 pyskroutz-0.1.8/src/pyskroutz/models/manufacturers.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1084 2021-02-07 21:19:46.000000 pyskroutz-0.1.8/src/pyskroutz/models/products.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      850 2021-02-07 21:20:14.000000 pyskroutz-0.1.8/src/pyskroutz/models/shops.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1714 2021-02-11 20:33:44.000000 pyskroutz-0.1.8/src/pyskroutz/models/skus.py
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/src/pyskroutz/resources/
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      401 2021-01-29 21:26:00.000000 pyskroutz-0.1.8/src/pyskroutz/resources/__init__.py
--rw-r--r--   0 psimakis  (1001) psimakis  (1001)     1487 2021-02-07 22:08:22.000000 pyskroutz-0.1.8/src/pyskroutz/resources/base.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     4339 2021-02-07 21:59:41.000000 pyskroutz-0.1.8/src/pyskroutz/resources/books.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     4290 2021-02-07 22:14:35.000000 pyskroutz-0.1.8/src/pyskroutz/resources/categories.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      621 2021-02-11 20:41:46.000000 pyskroutz-0.1.8/src/pyskroutz/resources/flags.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1466 2021-02-07 21:04:33.000000 pyskroutz-0.1.8/src/pyskroutz/resources/manufacturers.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1817 2021-02-07 21:04:33.000000 pyskroutz-0.1.8/src/pyskroutz/resources/products.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     4480 2021-02-07 21:10:26.000000 pyskroutz-0.1.8/src/pyskroutz/resources/skus.py
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1460 2021-02-07 21:59:41.000000 pyskroutz-0.1.8/src/pyskroutz/utils.py
-drwxrwxr-x   0 psimakis  (1001) psimakis  (1001)        0 2021-02-11 21:09:40.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     2417 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/PKG-INFO
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)      937 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/SOURCES.txt
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)        1 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/dependency_links.txt
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)        1 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/not-zip-safe
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)     1219 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/requires.txt
--rw-rw-r--   0 psimakis  (1001) psimakis  (1001)       10 2021-02-11 21:09:39.000000 pyskroutz-0.1.8/src/pyskroutz.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-02-09 17:41:48.521303 pyskroutz-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7672 2023-03-04 15:25:31.520281 pyskroutz-0.2.0/README.md
+-rw-r--r--   0        0        0     1430 2023-05-20 20:14:11.754247 pyskroutz-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      682 2023-02-09 17:41:48.525303 pyskroutz-0.2.0/src/pyskroutz/__init__.py
+-rw-r--r--   0        0        0     2188 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/client.py
+-rw-r--r--   0        0        0      367 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/__init__.py
+-rw-r--r--   0        0        0     2551 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/base.py
+-rw-r--r--   0        0        0     1679 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/books.py
+-rw-r--r--   0        0        0     1575 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/categories.py
+-rw-r--r--   0        0        0      878 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/favorites.py
+-rw-r--r--   0        0        0      529 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/filters.py
+-rw-r--r--   0        0        0      483 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/flags.py
+-rw-r--r--   0        0        0      441 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/manufacturers.py
+-rw-r--r--   0        0        0     1203 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/notifications.py
+-rw-r--r--   0        0        0     1159 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/products.py
+-rw-r--r--   0        0        0     1240 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/search.py
+-rw-r--r--   0        0        0     1512 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/shops.py
+-rw-r--r--   0        0        0     2019 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/skus.py
+-rw-r--r--   0        0        0     2029 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/models/users.py
+-rw-r--r--   0        0        0      401 2023-02-09 17:41:48.525303 pyskroutz-0.2.0/src/pyskroutz/resources/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/resources/base.py
+-rw-r--r--   0        0        0     3955 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/resources/books.py
+-rw-r--r--   0        0        0     3680 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/resources/categories.py
+-rw-r--r--   0        0        0     2957 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/resources/favorites.py
+-rw-r--r--   0        0        0      770 2023-05-20 20:11:35.971636 pyskroutz-0.2.0/src/pyskroutz/resources/filters.py
+-rw-r--r--   0        0        0      566 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/flags.py
+-rw-r--r--   0        0        0     1501 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/manufacturers.py
+-rw-r--r--   0        0        0     1336 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/notifications.py
+-rw-r--r--   0        0        0     1535 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/products.py
+-rw-r--r--   0        0        0      830 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/search.py
+-rw-r--r--   0        0        0     1121 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/shops.py
+-rw-r--r--   0        0        0     4461 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/skus.py
+-rw-r--r--   0        0        0     5207 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/resources/users.py
+-rw-r--r--   0        0        0     1452 2023-05-20 20:11:35.975636 pyskroutz-0.2.0/src/pyskroutz/utils.py
+-rw-r--r--   0        0        0     9240 1970-01-01 00:00:00.000000 pyskroutz-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyskroutz-0.1.8/LICENSE` & `pyskroutz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyskroutz-0.1.8/src/pyskroutz/client.py` & `pyskroutz-0.2.0/src/pyskroutz/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from typing import Dict
 
 import requests
 
 
 class SkroutzClient:
-    """Skroutz Client Class. This is the main class that let's you interact with Skroutz API.
+    """Skroutz Client Class. This is the main class that lets you interact with Skroutz API.
 
     Examples:
         In order to interact with Skroutz API you have to initiate a `SkroutzClient` object.
         You have to provide the client id and the client secret.
 
         >>> import pyskroutz
         >>> client = pyskroutz.client("<client-id>", "<client-secret>")
 
         Check out the available endpoints for further details.
-
-    Attributes:
-        BASE_URL: The base url of Skroutz API.
     """
 
     _access_token: str
     _access_token_type: str
 
     def __init__(
         self, client_id: str, client_secret: str, raise_auth_error: bool = True
@@ -50,20 +47,28 @@
         if raise_auth_error:
             req.raise_for_status()
 
         self._access_token = req.json().get("access_token", "test")
         self._access_token_type = req.json().get("token_type", "test")
 
     @property
-    def _headers(self) -> Dict[str, str]:
+    def headers(self) -> Dict[str, str]:
         """Get headers using the access token.
 
         Returns: Headers dictionary.
         """
         return {
             "Accept": "application/vnd.skroutz+json; version=3",
             "Authorization": "%s %s"
             % (
                 getattr(self, "_access_token_type", "").capitalize(),
                 getattr(self, "_access_token", ""),
             ),
         }
+
+    @property
+    def session(self):
+        return self._session
+
+    @session.setter
+    def session(self, value):
+        self._session = value
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/models/base.py` & `pyskroutz-0.2.0/src/pyskroutz/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, HttpUrl, PositiveInt
 
 
 class PaginationItem(BaseModel):
     """Pagination model.
 
@@ -21,15 +21,15 @@
 
 class AvailabilityItem(BaseModel):
     count: int
     id: int
     label: str
 
 
-class DistaceItem(BaseModel):
+class DistanceItem(BaseModel):
     count: int
     id: int
     label: str
 
 
 class AvailabilityFilterItem(BaseModel):
     availabilities: Optional[List[AvailabilityItem]]
@@ -57,15 +57,15 @@
     label: str
     lat: str
     lng: str
     type: str
 
 
 class PaymentMethodTypeItem(BaseModel):
-    type: str
+    type: Any
 
 
 class PersonalizationItem(BaseModel):
     location: LocationItem
     payment_method: PaymentMethodTypeItem
 
 
@@ -100,35 +100,35 @@
 
     Attributes:
         id:
         name:
     """
 
     id: PositiveInt
-    name: str
+    name: Optional[str]
 
 
 class BuyableItemBase(BaseModel):
     """Item Buy base model.
 
     Attributes:
         price_min:
         price_max:
         shop_count:
         reviewscore:
         reviews_count:
         reviewable:
     """
 
-    price_max: float
-    price_min: float
+    price_max: Optional[float]
+    price_min: Optional[float]
     reviewable: Optional[bool]
-    reviews_count: int
-    reviewscore: float
-    shop_count: int
+    reviews_count: Optional[int]
+    reviewscore: Optional[float]
+    shop_count: Optional[int]
 
 
 class ImageItemBase(BaseModel):
     """Item image base model.
 
     Attributes:
         main:
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/models/books.py` & `pyskroutz-0.2.0/src/pyskroutz/models/books.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Response models for book resources
 """
 
-from typing import List, Optional, Any
-from pydantic import BaseModel, PositiveInt, HttpUrl, EmailStr, AnyUrl
+from typing import Any, List, Optional
+
+from pydantic import BaseModel, EmailStr, HttpUrl, PositiveInt
 
 from pyskroutz.models.base import (
-    ItemBase,
     BuyableItemBase,
-    WebUriBaseItem,
     ImageItemBase,
+    ItemBase,
     MetaItemBase,
+    WebUriBaseItem,
 )
 
 
 class BookItem(ItemBase, BuyableItemBase, WebUriBaseItem):
     """Book response model.
 
     Attributes:
@@ -61,16 +62,16 @@
 
 
 class BookAuthorRetrieve(BaseModel):
     author: BookAuthorItem
 
 
 class BooksList(BaseModel):
-    books: List[BookItem]
-    meta: MetaItemBase
+    books: Optional[List[BookItem]]
+    meta: Optional[MetaItemBase]
 
 
 class PublisherItem(ItemBase):
     id: PositiveInt
     name: str
     address: str
     email: EmailStr
@@ -86,12 +87,12 @@
 class BookCategory(BaseModel):
     id: PositiveInt
     name: str
     match_count: Optional[int]
 
 
 class BookCategoryRetrieve(BaseModel):
-    category: BookCategory
+    category: Optional[BookCategory]
 
 
 class BookCategoriesList(BaseModel):
     categories: List[BookCategory]
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/models/categories.py` & `pyskroutz-0.2.0/src/pyskroutz/models/categories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """Response models for category resources
 """
-from pydantic import BaseModel
 from typing import List, Optional
 
-from ..models.base import (
-    MetaItemBase,
-    ItemBase,
-    WebUriBaseItem,
-    HttpUrl,
-)
+from pydantic import BaseModel
+
+from pyskroutz.models.base import HttpUrl, ItemBase, MetaItemBase, WebUriBaseItem
 
 
 class GroupItem(BaseModel):
     """
 
     Attributes:
         id:
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/models/products.py` & `pyskroutz-0.2.0/src/pyskroutz/models/products.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """Response models for product resources
 """
+from typing import Any, List, Optional
+
 from pydantic import BaseModel, HttpUrl
-from typing import List, Any, Optional
-from .base import WebUriBaseItem, ItemBase, MetaItemBase, PersonalizationItem
-from .shops import ShopItem
+
+from pyskroutz.models.base import (
+    ItemBase,
+    MetaItemBase,
+    PersonalizationItem,
+    WebUriBaseItem,
+)
+from pyskroutz.models.shops import ShopItem
 
 
 class BlpItem(BaseModel):
     shipping_cost: float
     payment_method_cost: Optional[float]
     final_price: Optional[float]
 
@@ -23,16 +30,16 @@
     sizes: List
     blp: Optional[BlpItem]
     price: float
     immediate_pickup: bool
 
 
 class ProductRetrieve(BaseModel):
-    product: ProductItem
-    meta: MetaItemBase
+    product: Optional[ProductItem]
+    meta: Optional[MetaItemBase]
 
 
 class ProductsList(BaseModel):
     products: List[ProductItem]
 
 
 class CardItem(BaseModel):
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/models/skus.py` & `pyskroutz-0.2.0/src/pyskroutz/models/users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,106 @@
-"""Response models for SKUs resources
+"""Response models for User resources
 """
 import datetime
+from enum import Enum
+from typing import Dict, List, Optional
 
-from .base import *
-from typing import Optional
+from pydantic import AnyHttpUrl, BaseModel, EmailStr
 
 
-class SkuItem(ItemBase, BuyableItemBase, WebUriBaseItem):
-    ean: str
-    pn: str
-    display_name: str
-    category_id: int
-    first_product_shop_info: Optional[str]
-    click_url: Optional[HttpUrl]
-    plain_spec_summary: str
-    manufacturer_id: int
-    future: bool
-    virtual: bool
-    images: ImageItemBase
-    favorited: Optional[bool]
-    comparable: Optional[bool]
-    name_source: Optional[str]
+class SexEnum(Enum):
+    male = "male"
+    female = "female"
 
 
-class SkuList(BaseModel):
-    skus: List[SkuItem]
-    meta: MetaItemBase
-    available_filters: Optional[AvailabilityFilterItem]
+class StatsItem(BaseModel):
+    sku_review_count: int
+    shop_review_count: int
+    sku_comment_count: int
+    received_votes: int
 
 
-class SkuRetrieve(BaseModel):
-    sku: SkuItem
+class EmailNotificationItem(BaseModel):
+    field: str
+    label: str
+    description: str
+    enabled: bool
 
 
-class SentimentItem(BaseModel):
-    positive: Optional[List[str]]
-    mediocre: Optional[List[str]]
-
-
-class ReviewItem(BaseModel):
+class UserItem(BaseModel):
     id: int
-    user_id: int
-    review: str
-    rating: int
+    username: str
+    avatar: AnyHttpUrl
+    sex: SexEnum
     created_at: datetime.datetime
-    demoted: bool
-    votes_count: int
-    helpful_votes_count: int
-    voted: bool
-    flagged: bool
-    helpful: bool
-    sentiments: Optional[SentimentItem]
+    email: EmailStr
+    birthyear: Optional[int]
+    mobile: Optional[str]
+    type: str
+    stats: StatsItem
+    email_notifications: List[EmailNotificationItem]
 
 
-class ReviewList(BaseModel):
-    reviews: List[ReviewItem]
-    meta: MetaItemBase
+class UserRetrieve(BaseModel):
+    user: Optional[UserItem]
 
 
-class VoteItem(BaseModel):
+class AvatarList(BaseModel):
+    avatars: List[AnyHttpUrl]
+
+
+class AddressItem(BaseModel):
     id: int
-    sku_review_id: int
-    user_id: int
-    helpful: bool
-    created_at: datetime.datetime
-    sku_review: Optional[ReviewItem]
+    label: Optional[str]
+    first_name: Optional[str]
+    last_name: Optional[str]
+    street_name: Optional[str]
+    street_number: int
+    city: str
+    zip: Optional[str]
+    region: str
+    phone: Optional[str]
+    mobile: Optional[str]
+    lng: Optional[str]
+    lat: Optional[str]
 
 
-class VoteRetrieve(BaseModel):
-    sku_review_vote: VoteItem
+class AddressList(BaseModel):
+    addresses: List[AddressItem]
 
 
-class AnswerItem(BaseModel):
-    id: int
-    text: str
+class AddressRetrieve(BaseModel):
+    address: AddressItem
 
 
-class QuestionItem(BaseModel):
-    text: str
-    type: str
-    answers: List[AnswerItem]
+class AddressFormItem(BaseModel):
+    required: List[str]
+    optional: List[str]
+    regions: Dict[str, int]
+
+
+class AddressFormRetrieve(BaseModel):
+    address_form: AddressFormItem
+
+
+class LineItem(BaseModel):
+    name: str
+    quantity: int
+    price: float
+    image: Optional[AnyHttpUrl]
+    sku_id: Optional[int]
+    product_id: Optional[int]
+    category_id: Optional[int]
 
 
-class ReviewFormItem(BaseModel):
-    requires_body: bool
-    questions: List[QuestionItem]
+class OrderItem(BaseModel):
+    date: datetime.datetime
+    product_cost: Optional[float]
+    shipping_cost: float
+    total_cost: float
+    line_items: List[LineItem]
+    shop_id: int
+    order_code: str
 
 
-class ReviewFormRetrieve(BaseModel):
-    review_form: ReviewFormItem
+class SavedOrdersList(BaseModel):
+    saved_orders: Optional[List[OrderItem]]
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/resources/base.py` & `pyskroutz-0.2.0/src/pyskroutz/resources/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import Any, Type, Dict, Optional, Type
+from typing import Type
 
 import requests
 from pydantic import BaseModel
 
-from pyskroutz.exceptions import SkroutzApiError
-from pyskroutz.utils import rsetattr
 from pyskroutz.client import SkroutzClient
 
 
 class ApiResource:
     _session: requests.Session
-    _client: SkroutzClient
+    client: SkroutzClient
 
     BASE_URL: str = "https://api.skroutz.gr"
 
     def __init__(self, client: SkroutzClient) -> None:
-        self._client = client
+        self.client = client
 
     def _set_prepared_request(
         self,
         url: str = None,
         method: str = "GET",
         data=None,
         headers: dict = None,
@@ -37,25 +35,26 @@
             params:
             json:
 
         Returns:
 
         """
         self._model = model
-        self._prepared_request = self._client._session.prepare_request(
+        self._prepared_request = self.client.session.prepare_request(
             requests.Request(
                 method=method,
                 url=url,
                 data=data,
-                headers=self._client._headers,
+                headers=self.client.headers,
                 params=params,
                 json=json,
             )
         )
 
     def execute(
         self,
     ):
         if not hasattr(self, "_prepared_request"):
             raise ValueError("You have to select the retrieve method first")
-        resp = self._client._session.send(self._prepared_request).json()
-        return self._model(**resp)
+        resp = self.client.session.send(self._prepared_request).json()
+        if self._model is not None:
+            return self._model(**resp)
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/resources/books.py` & `pyskroutz-0.2.0/src/pyskroutz/resources/books.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,173 +1,141 @@
-from .base import ApiResource
-from ..models.books import (
-    BookCategoriesList,
-    BookCategoryRetrieve,
-    PublisherRetrieve,
-    BooksRetrieve,
-    BooksList,
-    BookDetailsRetrieve,
-    BookAuthorRetrieve,
-)
 from typing import Optional
-from ..utils import fluent
+
+from pyskroutz.models import books
+from pyskroutz.resources import PaginationParams
+from pyskroutz.resources.base import ApiResource
+from pyskroutz.utils import fluent
 
 
 class Books(ApiResource):
     """This Class holds the group of Books related endpoints.
     More details in [category](https://developer.skroutz.gr/api/v3/category/) section.
     """
 
     ENDPOINT_PATH: str = "books"
 
     @fluent
-    def get(self, id: int) -> None:
+    def get(self, _id: int) -> None:
         """Retrieve a single Book
 
         Args:
-            id: Book identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get(242327).execute()
+            _id: Book identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}",
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}",
             method="GET",
-            model=BooksRetrieve,
+            model=books.BooksRetrieve,
         )
 
     @fluent
-    def get_details(self, id: int) -> None:
+    def get_details(self, _id: int) -> None:
         """Retrieve Book details
 
         Args:
-            id: Book identifier.
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_details(242327).execute()
+            _id: Book identifier.
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/details",
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/details",
             method="GET",
-            model=BookDetailsRetrieve,
+            model=books.BookDetailsRetrieve,
         )
 
     @fluent
-    def get_author(self, id: int) -> None:
+    def get_author(self, _id: int) -> None:
         """Retrieve Book Author
 
         Args:
-            id: author identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_author(385).execute()
+            _id: author identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/author/{id}",
-            model=BookAuthorRetrieve,
+            url=f"{self.BASE_URL}/author/{_id}",
+            model=books.BookAuthorRetrieve,
         )
 
     @fluent
-    def get_author_books(self, id: int) -> None:
+    def get_author_books(self, _id: int, **pag_params: PaginationParams) -> None:
         """Retrieve Author Books
 
         Args:
-            id: author identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_author_books(385).execute()
+            _id: author identifier
+            pag_params: pagination parameters
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/author/{id}/books", model=BooksList
+            url=f"{self.BASE_URL}/author/{_id}/books",
+            model=books.BooksList,
+            params=pag_params,
         )
 
     @fluent
-    def get_similar_by_author(self, id: int) -> None:
+    def get_similar_by_author(self, _id: int, **pag_params: PaginationParams) -> None:
         """Retrieve similar Books by Author
 
         Args:
-            id: author identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_similar_by_author(242327).execute()
+            _id: author identifier
+            pag_params: pagination parameters
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/similar_by_author",
-            model=BooksList,
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/similar_by_author",
+            model=books.BooksList,
+            params=pag_params,
         )
 
     @fluent
-    def get_publisher(self, id: int) -> None:
+    def get_publisher(self, _id: int) -> None:
         """Retrieve Book Publisher
 
         Args:
-            id: publisher identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_publisher(78).execute()
+            _id: publisher identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/publisher/{id}", model=PublisherRetrieve
+            url=f"{self.BASE_URL}/publisher/{_id}", model=books.PublisherRetrieve
         )
 
     @fluent
-    def get_publisher_books(self, id: int) -> None:
+    def get_publisher_books(self, _id: int, **pag_params: PaginationParams) -> None:
         """Retrieve Publisher Books
 
         Args:
-            id: publisher identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_publisher_books(78).execute()
+            _id: publisher identifier
+            pag_params: pagination parameters
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/publisher/{id}/books", model=BooksList
+            url=f"{self.BASE_URL}/publisher/{_id}/books",
+            model=books.BooksList,
+            params=pag_params,
         )
 
     @fluent
     def get_book_categories(self) -> None:
-        """Retrieve Book Categories
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_book_categories().execute()
-        """
+        """Retrieve Book Categories"""
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/book_categories", model=BookCategoriesList
+            url=f"{self.BASE_URL}/book_categories", model=books.BookCategoriesList
         )
 
-    def get_category(self, id: int) -> None:
+    @fluent
+    def get_category(self, _id: int) -> None:
         """Retrieve Book Category
 
         Args:
-            id: book identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_category(1857).execute()
+            _id: book identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/book_categories/{id}", model=BookCategoryRetrieve
+            url=f"{self.BASE_URL}/book_categories/{_id}",
+            model=books.BookCategoryRetrieve,
         )
 
+    @fluent
     def get_category_books(
-        self, id: int, order_by: Optional[str] = None, order_dir: Optional[str] = None
+        self, _id: int, order_by: Optional[str] = None, order_dir: Optional[str] = None
     ) -> None:
         """Retrieve Book Category's Books
 
         Args:
-            id: category identifier
-
-        Examples:
-
-            >>> pyskroutz.books(client).get_category_books(1857).execute()
+            _id: category identifier
+            order_by: order by
+            order_dir: order dir
         """
+        if order_by or order_dir:
+            raise NotImplemented
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/book_categories/{id}/books", model=BooksList
+            url=f"{self.BASE_URL}/book_categories/{_id}/books", model=books.BooksList
         )
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/resources/categories.py` & `pyskroutz-0.2.0/src/pyskroutz/resources/skus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,148 @@
-from pyskroutz.resources.base import ApiResource
-from ..models.categories import (
-    CategoryList,
-    CategoryRetrieve,
-    SpecificationList,
+from typing import List, Optional
+
+from pyskroutz.models.skus import (
+    ReviewFormRetrieve,
+    ReviewList,
+    SkuList,
+    SkuRetrieve,
+    VoteRetrieve,
 )
-from ..resources import PaginationParams
-from ..utils import fluent
-from typing import Optional
+from pyskroutz.resources import PaginationParams
+from pyskroutz.resources.base import ApiResource
+from pyskroutz.resources.categories import Categories
+from pyskroutz.utils import fluent
 
 
-class Categories(ApiResource):
-    """This Class holds the group of Categories related endpoints. More details in [category](https://developer.skroutz.gr/api/v3/category/) section."""
+class Skus(ApiResource):
+    """This Class holds the group of SKU related endpoints. A SKU (Stock Keeping Unit) is an aggregation of products.
+    More details in [sku](https://developer.skroutz.gr/api/v3/sku/) section.
+    """
 
-    ENDPOINT_PATH: str = "categories"
+    ENDPOINT_PATH: str = "skus"
 
     @fluent
-    def get(self, id: Optional[int] = None, **pag_params: PaginationParams) -> None:
-        """Retrieve a single category or list them all.
+    def list(
+        self,
+        _id: int,
+        q: Optional[str] = None,
+        manufacturer_ids: Optional[List[int]] = None,
+        filter_ids: Optional[List[int]] = None,
+        **pag_params: PaginationParams,
+    ) -> None:
+        """List SKUs of specific category
 
         Args:
-            id: category identifier
-            pag_params: pagination parameters
-
-        Examples:
-
-            >>> pyskroutz.categories(client).get(88).execute()
+            _id: Category identifier.
+            q: The keyword to search by.
+            manufacturer_ids: The ids of the manufacturers of the SKUs.
+            filter_ids: The ids of the filters to be applied on the SKUs.
+            **pag_params: pagination parameters
         """
+        params: dict = dict(**pag_params)
+
+        params.update(
+            {
+                n: v
+                for n, v in zip(
+                    ("q", "manufacturer_ids[]", "filter_ids"),
+                    (q, manufacturer_ids, filter_ids),
+                )
+                if v is not None
+            }
+        )
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}"
-            if id is not None
-            else f"{self.BASE_URL}/{self.ENDPOINT_PATH}",
-            model=CategoryRetrieve if id is not None else CategoryList,
-            params=pag_params,
+            url=f"{self.BASE_URL}/{Categories.ENDPOINT_PATH}/{_id}/skus",
+            model=SkuList,
+            params=params,
         )
 
     @fluent
-    def get_parent(self, id: int) -> None:
-        """Retrieve the parent of a category.
+    def get(self, _id: int) -> None:
+        """Retrieve a single SKU.
 
         Args:
-            id: category identifier.
-
-        Examples:
-
-            >>> pyskroutz.categories(client).get_parent(88).execute()
+            _id: SKU identifier.
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/parent",
-            model=CategoryRetrieve,
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}", model=SkuRetrieve
         )
 
     @fluent
-    def get_root(self) -> None:
-        """Retrieve the root category.
+    def get_similar(self, _id: int, **pag_params: PaginationParams) -> None:
+        """Retrieve similar SKUs.
 
-        Examples:
-
-            >>> pyskroutz.categories(client).get_root().execute()
+        Args:
+            _id: SKU identifier.
+            pag_params: pagination parameters.
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/root", model=CategoryRetrieve
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/similar",
+            model=SkuList,
+            params=pag_params,
         )
 
     @fluent
-    def list_children(self, id: int, **pag_params: PaginationParams) -> None:
-        """List the children categories of a category.
+    def get_reviews(
+        self,
+        _id: int,
+        include_meta: Optional[str] = None,
+        **pag_params: PaginationParams,
+    ) -> None:
+        """Retrieve a SKU's reviews
 
         Args:
-            id: category identifier.
-            **pag_params: pagination params.
-
-        Examples:
-
-            >>> pyskroutz.categories(client).list_children(252).execute()
+            _id: sku identifier
+            include_meta: You may choose to include extra meta information using the following parameters: (sku_rating_breakdown, sku_reviews_aggregation)
+            **pag_params: pagination params
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/children",
-            model=CategoryList,
-            params=pag_params,
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/reviews",
+            params=dict(**pag_params)
+            if include_meta is None
+            else dict(include_meta=include_meta, **pag_params),
+            model=ReviewList,
         )
 
     @fluent
-    def get_specifications(
-        self, id: int, include_group: bool = None, **pag_params: PaginationParams
-    ) -> None:
-        """List a category's specifications.
+    def vote_review(self, _id: int, review_id: int, helpful: bool) -> None:
+        """Vote a SKU's review
 
         Args:
-            id: category identifier.
-            include_group: Include group.
-            **pag_params: pagination params.
-
-        Examples:
-
-            >>> pyskroutz.categories(client).get_specifications(40, include_group=True).execute()
+            _id: SKU Identifier.
+            review_id: Review identifier.
+            helpful: Helpful or not.
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/specifications",
-            model=SpecificationList,
-            params=pag_params
-            if include_group is None
-            else dict(include="group", **pag_params),  # type: ignore
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/reviews/{review_id}/votes",
+            method="POST",
+            json={"vote": {"helpful": helpful}},
+            model=VoteRetrieve,
         )
 
     @fluent
-    def get_manufacturers(
-        self, id: int, order_dir: str = None, **pag_params: PaginationParams
-    ) -> None:
-        """List a category's manufacturers.
+    def flag_review(self, _id: int, review_id: int, reason: str) -> None:
+        """Flag a SKU's review
 
         Args:
-            id: category identifier.
-            order_dir: Order ascending or descending (`asc`, `desc` default)
-            **pag_params: pagination params.
-
-        Examples:
-
-            >>> pyskroutz.categories(client).get_manufacturers(2).execute()
+            _id: SKU Identifier.
+            review_id: Review identifier.
+            reason: bad_language, wrong_section or spam
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/manufacturers",
-            model=SpecificationList,
-            params=dict(**pag_params)
-            if order_dir is None
-            else dict(order_dir=order_dir, **dict(pag_params)),  # type: ignore
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/reviews/{review_id}/flags",
+            method="POST",
+            model=VoteRetrieve,
+            json={"vote": {"reason": reason}},
         )
 
     @fluent
-    def get_favorites(self, id: int) -> None:
-        """List a category's favorites.
+    def get_review_form(self, _id: int) -> None:
+        """Retrieve a SKU review form
 
         Args:
-            id: category identifier.
-
-        Examples:
-
-            >>> pyskroutz.categories(client).get_favorites(40).execute()
+            _id: SKU Identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/favorites",
-            model=SpecificationList,
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/reviews/new",
+            model=ReviewFormRetrieve,
         )
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/resources/flags.py` & `pyskroutz-0.2.0/src/pyskroutz/resources/flags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-from .base import ApiResource
-from ..models.flags import FlagList
-from ..utils import fluent
+from pyskroutz.models.flags import FlagList
+from pyskroutz.resources.base import ApiResource
+from pyskroutz.utils import fluent
 
 
 class Flags(ApiResource):
     """This Class holds the group of Flags related endpoints.
     More details in [flags](https://developer.skroutz.gr/api/v3/flag/) section.
     """
 
     ENDPOINT_PATH: str = "flags"
 
     @fluent
     def get(self) -> None:
-        """List all flags
-
-        Examples:
-
-            >>> pyskroutz.flags(client).get().execute()
-        """
+        """List all flags"""
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}",
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}",
             method="GET",
             model=FlagList,
         )
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/resources/manufacturers.py` & `pyskroutz-0.2.0/src/pyskroutz/resources/manufacturers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Optional
 
-from .base import ApiResource
-from ..models.categories import CategoryList
-from ..models.manufacturers import ManufacturerRetrieve, ManufacturersList
-from ..utils import fluent
+from pyskroutz.models.categories import CategoryList
+from pyskroutz.models.manufacturers import ManufacturerRetrieve, ManufacturersList
+from pyskroutz.resources import PaginationParams
+from pyskroutz.resources.base import ApiResource
+from pyskroutz.utils import fluent
 
 
 class Manufacturers(ApiResource):
-    """This Class holds the group of Manufacturers related endpoints. More details in [category](https://developer.skroutz.gr/api/v3/category/) section."""
+    """
+    This Class holds the group of Manufacturers related endpoints.
+    More details in [category](https://developer.skroutz.gr/api/v3/category/) section.
+    """
 
     ENDPOINT_PATH: str = "manufacturers"
 
     @fluent
-    def get(self, id: Optional[int] = None) -> None:
+    def get(self, _id: Optional[int] = None) -> None:
         """Retrieve a single manufacturer or list them all.
 
         Args:
-            id: manufacturer identifier
-
-        Examples:
-
-            >>> pyskroutz.manufacturers(client).get(12907).execute()
+            _id: manufacturer identifier
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}"
-            if id is not None
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}"
+            if _id is not None
             else f"{self.BASE_URL}/{self.ENDPOINT_PATH}",
             method="GET",
-            model=ManufacturerRetrieve if id is not None else ManufacturersList,
+            model=ManufacturerRetrieve if _id is not None else ManufacturersList,
         )
 
     @fluent
-    def get_manufacturer_categories(self, id: int) -> None:
+    def get_manufacturer_categories(
+        self, _id: int, **pag_params: PaginationParams
+    ) -> None:
         """
 
         Args:
-            id: Manufacturer identifier
-
-        Examples:
-
-            >>> pyskroutz.manufacturers(client).get_manufacturer_categories(12907).execute()
+            _id: Manufacturer identifier
+            pag_params: Pagination parameters
         """
         self._set_prepared_request(
-            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{id}/categories",
+            url=f"{self.BASE_URL}/{self.ENDPOINT_PATH}/{_id}/categories",
             method="GET",
             model=CategoryList,
+            params=pag_params,
         )
```

### Comparing `pyskroutz-0.1.8/src/pyskroutz/utils.py` & `pyskroutz-0.2.0/src/pyskroutz/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 from typing import Any
 
 
-def rsetattr(obj: object, attr: str, val):
+def rsetattr(obj: object, attr: str, val) -> Any:
     """Set attribute recursively.
 
     Examples:
 
         >>> from argparse import Namespace
         >>> from pyskroutz.utils import rsetattr
         >>> ns_obj = Namespace()
@@ -15,42 +15,38 @@
         >>> ns_obj.a.b
         1
 
     Args:
         obj: Object.
         attr: Attribute name (period separated for nested attributes).
         val: Attribute value.
-
-    Returns:
-
     """
     pre, _, post = attr.rpartition(".")
     return setattr(rgetattr(obj, pre) if pre else obj, post, val)
 
 
 def rgetattr(obj, attr: str, *args) -> Any:
     """Get recursive attribute.
 
     Examples:
 
         >>> from argparse import Namespace
-        >>>from pyskroutz.utils import rgetattr
+        >>> from pyskroutz.utils import rgetattr
         >>> ns_obj = Namespace()
         >>> ns_obj.a = Namespace()
         >>> ns_obj.a.b = 1
         >>> rgetattr(ns_obj, 'a.b')
         1
 
     Args:
         obj: Object.
         attr: Attribute name (period separated for nested attributes).
         *args:
 
     Returns: Attribute value
-
     """
 
     def _getattr(obj, attr) -> Any:
         return getattr(obj, attr, *args)
 
     return functools.reduce(_getattr, [obj] + attr.split("."))
```

