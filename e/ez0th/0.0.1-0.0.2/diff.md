# Comparing `tmp/ez0th-0.0.1.tar.gz` & `tmp/ez0th-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez0th-0.0.1.tar", last modified: Fri May 19 03:56:16 2023, max compression
+gzip compressed data, was "ez0th-0.0.2.tar", last modified: Sat May 20 05:54:49 2023, max compression
```

## Comparing `ez0th-0.0.1.tar` & `ez0th-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 03:56:16.124876 ez0th-0.0.1/
--rw-rw-rw-   0        0        0     9534 2023-05-19 03:56:16.124876 ez0th-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7824 2023-05-14 14:26:44.000000 ez0th-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 03:56:16.119706 ez0th-0.0.1/ez0th/
--rw-rw-rw-   0        0        0     6886 2023-05-19 03:55:34.000000 ez0th-0.0.1/ez0th/__init__.py
--rw-rw-rw-   0        0        0     1419 2023-05-19 03:56:05.000000 ez0th-0.0.1/ez0th/test.py
-drwxrwxrwx   0        0        0        0 2023-05-19 03:56:16.123657 ez0th-0.0.1/ez0th.egg-info/
--rw-rw-rw-   0        0        0     9534 2023-05-19 03:56:15.000000 ez0th-0.0.1/ez0th.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-19 03:56:15.000000 ez0th-0.0.1/ez0th.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 03:56:15.000000 ez0th-0.0.1/ez0th.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-19 03:56:15.000000 ez0th-0.0.1/ez0th.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 03:56:15.000000 ez0th-0.0.1/ez0th.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 03:56:16.124876 ez0th-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-05-19 03:56:13.000000 ez0th-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 05:54:49.735970 ez0th-0.0.2/
+-rw-rw-rw-   0        0        0     9534 2023-05-20 05:54:49.735465 ez0th-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7824 2023-05-14 14:26:44.000000 ez0th-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 05:54:49.722461 ez0th-0.0.2/ez0th/
+-rw-rw-rw-   0        0        0     6877 2023-05-20 05:20:24.000000 ez0th-0.0.2/ez0th/__init__.py
+-rw-rw-rw-   0        0        0     1419 2023-05-19 03:56:05.000000 ez0th-0.0.2/ez0th/test.py
+drwxrwxrwx   0        0        0        0 2023-05-20 05:54:49.734081 ez0th-0.0.2/ez0th.egg-info/
+-rw-rw-rw-   0        0        0     9534 2023-05-20 05:54:49.000000 ez0th-0.0.2/ez0th.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-20 05:54:49.000000 ez0th-0.0.2/ez0th.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 05:54:49.000000 ez0th-0.0.2/ez0th.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-20 05:54:49.000000 ez0th-0.0.2/ez0th.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 05:54:49.000000 ez0th-0.0.2/ez0th.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 05:54:49.735970 ez0th-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-05-20 05:54:43.000000 ez0th-0.0.2/setup.py
```

### Comparing `ez0th-0.0.1/PKG-INFO` & `ez0th-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
```

### Comparing `ez0th-0.0.1/README.md` & `ez0th-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ez0th-0.0.1/ez0th/__init__.py` & `ez0th-0.0.2/ez0th/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 		"read": read_func,
 		"update": create_update_func,
 		"delete": delete_func,
 		"contains": contains_func,
 	}
 
 # アカウント存在確認 [ez0th]
-def is_exists(
+def exists(
 	u_id,	# ログインid (登録されたいずれのidも可)
 	db = "auto",	# データベース
 ):
 	if db == "auto": db = json_stock("./__ez0th_user_db__/")
 	# 引数インジェクションチェック (セキュリティー対策; ptnを満たす文字列かどうかをチェック)
 	check_injection(u_id)
 	return db["contains"]("id_"+u_id)
@@ -81,15 +81,15 @@
 ):
 	if db == "auto": db = json_stock("./__ez0th_user_db__/")
 	# 引数インジェクションチェック (セキュリティー対策; ptnを満たす文字列かどうかをチェック)
 	for id_type in id_dic: check_injection(id_dic[id_type])
 	check_injection(password)
 	# アカウント存在確認
 	for id_type in id_dic:
-		if is_exists(id_dic[id_type], db) is True: return False
+		if exists(id_dic[id_type], db) is True: return False
 	# パスワードのハッシュ化 (パスワードを安全に保管するため)
 	pw_salt, pw_hash = gen_pw_hash(password)
 	# 内部ユーザーidの生成 (システム内で利用するため; "inner_id_"で開始するID)
 	inner_id = gen_inner_id(db)
 	# DBへの登録
 	new_value = {"inner_id": inner_id, "id_dic": id_dic, "pw_salt": pw_salt, "pw_hash": pw_hash, "info": info}
 	db["create"](inner_id, new_value)
@@ -129,15 +129,15 @@
 	db = "auto"	# データベース
 ):
 	if db == "auto": db = json_stock("./__ez0th_user_db__/")
 	# 引数インジェクションチェック (セキュリティー対策; ptnを満たす文字列かどうかをチェック)
 	check_injection(u_id)
 	check_injection(password)
 	# アカウント存在確認 [ez0th]
-	if is_exists(u_id, db) is False: return False, None	# success_flag, sess_token
+	if exists(u_id, db) is False: return False, None	# success_flag, sess_token
 	# パスワード正当性確認
 	inner_id = db["read"]("id_" + u_id)
 	account_data = db["read"](inner_id)
 	_, temp_hash = gen_pw_hash(password, account_data["pw_salt"])	# パスワードのハッシュ化 (パスワードを安全に保管するため)
 	if temp_hash != account_data["pw_hash"]: return False, None	# success_flag, sess_token
 	# セッショントークンの発行
 	sess_token = gen_sess_token(inner_id, timeout, db)
```

### Comparing `ez0th-0.0.1/ez0th/test.py` & `ez0th-0.0.2/ez0th/test.py`

 * *Files identical despite different names*

### Comparing `ez0th-0.0.1/ez0th.egg-info/PKG-INFO` & `ez0th-0.0.2/ez0th.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
```

### Comparing `ez0th-0.0.1/setup.py` & `ez0th-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 657a 3074 682f 2229  develop_ez0th/")
 000000c0: 2061 7320 703a 0d0a 0973 6574 7570 280d   as p:...setup(.
 000000d0: 0a09 096e 616d 6520 3d20 2265 7a30 7468  ...name = "ez0th
 000000e0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-000000f0: 2230 2e30 2e31 222c 0d0a 0909 6465 7363  "0.0.1",....desc
+000000f0: 2230 2e30 2e32 222c 0d0a 0909 6465 7363  "0.0.2",....desc
 00000100: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 00000110: 6e20 4c69 6272 6172 7920 666f 7220 4561  n Library for Ea
 00000120: 7379 2041 7574 6865 6e74 6963 6174 696f  sy Authenticatio
 00000130: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
 00000140: 696f 6e22 2c0d 0a09 0961 7574 686f 7220  ion",....author 
 00000150: 3d20 2262 6962 5f69 6e66 222c 0d0a 0909  = "bib_inf",....
 00000160: 6175 7468 6f72 5f65 6d61 696c 203d 2022  author_email = "
```

