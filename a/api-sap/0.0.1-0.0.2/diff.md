# Comparing `tmp/api_sap-0.0.1.tar.gz` & `tmp/api_sap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_sap-0.0.1.tar", last modified: Fri May 19 23:41:24 2023, max compression
+gzip compressed data, was "api_sap-0.0.2.tar", last modified: Sat May 20 14:12:03 2023, max compression
```

## Comparing `api_sap-0.0.1.tar` & `api_sap-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:41:24.415129 api_sap-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-19 23:22:49.000000 api_sap-0.0.1/LICENCE
--rw-rw-rw-   0        0        0    29674 2023-05-19 23:41:24.406781 api_sap-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    29094 2023-05-19 23:35:15.000000 api_sap-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 23:41:24.367897 api_sap-0.0.1/api_sap.egg-info/
--rw-rw-rw-   0        0        0    29674 2023-05-19 23:41:24.000000 api_sap-0.0.1/api_sap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-19 23:41:24.000000 api_sap-0.0.1/api_sap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:41:24.000000 api_sap-0.0.1/api_sap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-19 23:41:24.000000 api_sap-0.0.1/api_sap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-19 23:41:24.000000 api_sap-0.0.1/api_sap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 23:41:24.394327 api_sap-0.0.1/py_sap/
--rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-0.0.1/py_sap/__init__.py
--rw-rw-rw-   0        0        0    29082 2023-05-08 18:17:20.000000 api_sap-0.0.1/py_sap/py_sap.py
--rw-rw-rw-   0        0        0       42 2023-05-19 23:41:24.416146 api_sap-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      494 2023-05-19 23:41:04.000000 api_sap-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.728513 api_sap-0.0.2/
+-rw-rw-rw-   0        0        0     1075 2023-05-20 12:58:20.000000 api_sap-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      428 2023-05-20 14:12:03.717578 api_sap-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-05-20 13:14:53.000000 api_sap-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.677669 api_sap-0.0.2/api_sap.egg-info/
+-rw-rw-rw-   0        0        0      428 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.701793 api_sap-0.0.2/py_sap/
+-rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-0.0.2/py_sap/__init__.py
+-rw-rw-rw-   0        0        0    29082 2023-05-08 18:17:20.000000 api_sap-0.0.2/py_sap/py_sap.py
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:12:03.728513 api_sap-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-20 14:04:45.000000 api_sap-0.0.2/setup.py
```

### Comparing `api_sap-0.0.1/LICENCE` & `api_sap-0.0.2/LICENCE`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-The MIT License (MIT)
-
 Copyright (c) 2023 Wilton Melo.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `api_sap-0.0.1/PKG-INFO` & `api_sap-0.0.2/py_sap/py_sap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-Metadata-Version: 2.1
-Name: api_sap
-Version: 0.0.1
-Summary: Teste de geração de biblioteca
-Home-page: UNKNOWN
-Author: Wilton Melo
-Author-email: pmelo.wilton@gmail.com
-License: MIT License
-Keywords: api sap
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Teste.
-
-"""MÃ³dulo para utilizar o SAP com Python."""
+"""Módulo para utilizar o SAP com Python."""
 from typing import List
 
 import psutil
 import PySimpleGUI as sg
 import win32com.client
 
 
@@ -30,145 +15,145 @@
     __active_connection: win32com.client.CDispatch = None
     __session: win32com.client.CDispatch = None
     __active_session: win32com.client.CDispatch = None
     __active_window: win32com.client.CDispatch = None
     sg.theme('DarkAmber')
 
     def __init__(self):
-        """MÃ©todo construtor para o objeto SAP."""
+        """Método construtor para o objeto SAP."""
         self.__check_process()
 
     def __check_process(self) -> None:
-        """MÃ©todo para checar se o aplicativo SAP estÃ¡ aberto."""
+        """Método para checar se o aplicativo SAP está aberto."""
         if "saplogon.exe" in (
             process.name() for process in psutil.process_iter()
         ):
             for process in psutil.process_iter(attrs=['name', 'connections']):
                 if process.info['name'] == 'saplogon.exe':
                     number_connections: int = len(process.info['connections'])
             if number_connections > 0:
                 self.__initialize_logged_in_process()
             else:
                 sg.popup_ok(
-                    'Workspaces e ambientes do SAP nÃ£o foram selecionados!',
-                    title='AtenÃ§Ã£o!'
+                    'Workspaces e ambientes do SAP não foram selecionados!',
+                    title='Atenção!'
                 )
-                raise ValueError('AplicaÃ§Ã£o encerrada!')
+                raise ValueError('Aplicação encerrada!')
         else:
             sg.popup_ok(
-                'O Sap Logon nÃ£o estÃ¡ ativo!',
-                title='AtenÃ§Ã£o!'
+                'O Sap Logon não está ativo!',
+                title='Atenção!'
             )
-            raise ValueError('AplicaÃ§Ã£o encerrada!')
+            raise ValueError('Aplicação encerrada!')
 
     def __initialize_logged_in_process(self) -> None:
-        """MÃ©todo para inicializar com o SAP logado."""
+        """Método para inicializar com o SAP logado."""
         self.__get_object_sap_gui()
         self.__get_scripting_engine_sap_gui()
         self.__connection_sap_gui()
         self.__active_connection_sap_gui()
         self.__session_sap_gui()
         self.__active_session_sap_gui()
         self.__window_sap_gui()
         self.maximize()
         if self.check_logon_screen():
             sg.popup_ok(
-                'O SAP nÃ£o estÃ¡ logado!',
-                title='AtenÃ§Ã£o!'
+                'O SAP não está logado!',
+                title='Atenção!'
             )
             self.disconnect()
-            raise ValueError('AplicaÃ§Ã£o encerrada!')
+            raise ValueError('Aplicação encerrada!')
         if not self.check_session_manager():
             definition = sg.popup_yes_no(
-                "O sistema estÃ¡ em uso, deseja continuar?",
-                title="AtenÃ§Ã£o!"
+                "O sistema está em uso, deseja continuar?",
+                title="Atenção!"
             )
             if definition == "Yes":
                 self.end_transaction()
             else:
                 self.disconnect()
-                raise ValueError('AplicaÃ§Ã£o encerrada!')
+                raise ValueError('Aplicação encerrada!')
 
     def __get_object_sap_gui(self) -> None:
-        """MÃ©todo para criar o objeto SAPGUI."""
+        """Método para criar o objeto SAPGUI."""
         self.__sap_gui = win32com.client.GetObject('SAPGUI')
 
     @property
     def sapgui(self) -> win32com.client.CDispatch:
-        """MÃ©todod para retornar o objeto SAPGUI."""
+        """Métodod para retornar o objeto SAPGUI."""
         return self.__sap_gui
 
     def __get_scripting_engine_sap_gui(self) -> None:
-        """MÃ©todo para criar o objeto SAPGUI habilitado para script."""
+        """Método para criar o objeto SAPGUI habilitado para script."""
         self.__scripting_engine = self.__sap_gui.GetScriptingEngine
 
     @property
     def scripting(self):
-        """MÃ©todo para retornar o objeto SAPGUI habilitado para script."""
+        """Método para retornar o objeto SAPGUI habilitado para script."""
         return self.__scripting_engine
 
     def __connection_sap_gui(self) -> None:
-        """MÃ©todo para criar a conexao com o objeto SAPGUI."""
+        """Método para criar a conexao com o objeto SAPGUI."""
         self.__connection = self.__scripting_engine.Connections
 
     @property
     def connections(self):
-        """MÃ©todo para retornar a conexao com o SAPGUI."""
+        """Método para retornar a conexao com o SAPGUI."""
         return self.__connection
 
     def __active_connection_sap_gui(self) -> None:
-        """MÃ©todo para ativar a conexÃ£o do objeto SAPGUI."""
+        """Método para ativar a conexão do objeto SAPGUI."""
         self.__active_connection = self.__connection[
             self.__connection.Count - 1
         ]
 
     @property
     def connection(self):
-        """MÃ©todo para retornar o objeto SAPGUI com a conexÃ£o ativa."""
+        """Método para retornar o objeto SAPGUI com a conexão ativa."""
         return self.__active_connection
 
     def __session_sap_gui(self) -> None:
-        """MÃ©todo para criar a sessÃ£o do objeto SAPGUI."""
+        """Método para criar a sessão do objeto SAPGUI."""
         self.__session = self.__active_connection.Sessions
 
     @property
     def sessions(self):
-        """MÃ©todo para retornar a sessÃ£o do objeto SAPGUI."""
+        """Método para retornar a sessão do objeto SAPGUI."""
         return self.__session
 
     def __active_session_sap_gui(self) -> None:
-        """MÃ©todo para ativar a sessÃ£o do objeto SAPGUI."""
+        """Método para ativar a sessão do objeto SAPGUI."""
         self.__active_session = self.__session[self.__session.Count - 1]
 
     @property
     def session(self):
-        """MÃ©todo para retornar o objeto SAPGUI com a sessÃ£o ativa."""
+        """Método para retornar o objeto SAPGUI com a sessão ativa."""
         return self.__active_session
 
     def __window_sap_gui(
         self,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para ativar a janela do objeto SAPGUI.
+        """Método para ativar a janela do objeto SAPGUI.
 
         Args:
             item_window (str, optional): Item da janela utilizada.
                 Defaults to "0".
         """
         self.__active_window = self.__active_session.findById(
             f"wnd[{item_window}]"
         )
 
     @property
     def window(self):
-        """MÃ©todo para retornar o objeto SAPGUI com a janela ativa."""
+        """Método para retornar o objeto SAPGUI com a janela ativa."""
         return self.__active_window
 
     def get_session_info(self) -> dict:
-        """MÃ©todo para retornar informaÃ§Ãµes da session."""
+        """Método para retornar informações da session."""
         IsLowSpeedConnection = self.__active_session.Info.IsLowSpeedConnection
         return {
             'is active': self.__active_session.IsActive,
             'is busy': self.__active_session.Busy,
             'connection index': self.__active_session.Parent.Id,
             'session index': self.__active_session.Id,
             'Application Server': self.__active_session.Info.ApplicationServer,
@@ -193,18 +178,18 @@
     def find_object(
         self,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> win32com.client:
-        """MÃ©todo para localizar um objeto.
+        """Método para localizar um objeto.
 
         Args:
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
 
@@ -220,18 +205,18 @@
     def get_text(
         self,
         name_get_text_object: str,
         type_get_text_object: str = "",
         item_get_text_object: int = 0,
         item_window: str = "0"
     ) -> str:
-        """MÃ©todo para retornar o texto de um objeto.
+        """Método para retornar o texto de um objeto.
 
         Args:
-            name_get_text_object (str): Informar o nome da Ã¡rea da tela.
+            name_get_text_object (str): Informar o nome da área da tela.
             type_get_text_object (str, optional)): Informar o tipo do objeto.
                 Defaults to "".
             item_get_text_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
 
@@ -249,19 +234,19 @@
         self,
         text_set_text_object: str,
         name_set_text_object: str,
         type_set_text_object: str = "",
         item_set_text_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para inserir um texto em um objeto.
+        """Método para inserir um texto em um objeto.
 
         Args:
             text_set_text_object (str): Informar o texto que deseja inserir.
-            name_set_text_object (str): Informar o nome da Ã¡rea da tela.
+            name_set_text_object (str): Informar o nome da área da tela.
             type_set_text_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_set_text_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
 
@@ -272,76 +257,76 @@
             name_set_text_object,
             type_set_text_object,
             item_set_text_object,
             item_window
         ).Text = text_set_text_object
 
     def send_v_key(self, key_SendVKey: int) -> None:
-        """MÃ©todo para pressionar uma tÃ©cla de atalho.
+        """Método para pressionar uma técla de atalho.
 
         Args:
-            key_SendVKey (int): Inserir cÃ³digo da tecla de atalho.
+            key_SendVKey (int): Inserir código da tecla de atalho.
         """
         self.__active_window.SendVKey(key_SendVKey)
 
     def start_transaction(self, transaction: str) -> None:
-        """MÃ©todo para inicair uma transaÃ§Ã£o.
+        """Método para inicair uma transação.
 
         Args:
-            transaction (str): Informar cÃ³digo da transaÃ§Ã£o.
+            transaction (str): Informar código da transação.
         """
         self.__active_session.StartTransaction(transaction)
 
     def end_transaction(self) -> None:
-        """MÃ©todo para encerrar uma transaÃ§Ã£o."""
+        """Método para encerrar uma transação."""
         self.__active_session.EndTransaction()
 
     def check_logon_screen(self) -> bool:
-        """MÃ©todo para verificar se a tela Ã© de logon.
+        """Método para verificar se a tela é de logon.
 
         Returns:
             bool: Retornar verdadeiro ou falso.
         """
         if (
             self.get_session_info()["Transaction"] == "S000" and
             self.get_session_info()["Client"] == "000" and
             self.get_session_info()["User ID"] == ""
         ):
             return True
         return False
 
     def check_session_manager(self) -> bool:
-        """MÃ©todo para vewrificar se estÃ¡ na tela inicial.
+        """Método para vewrificar se está na tela inicial.
 
         Returns:
             bool: Retorna verdadeiro ou falso.
         """
         if (
             self.get_session_info()["Transaction"] == "SESSION_MANAGER" or
             self.get_session_info()["Transaction"] == "SMEN"
         ):
             return True
         return False
 
     def disconnect(self) -> None:
-        """MÃ©todo para desconectar do SAP logon."""
+        """Método para desconectar do SAP logon."""
         self.__active_window = None
         self.__active_session = None
         self.__session = None
         self.__active_connection = None
         self.__connection = None
         self.__scripting_engine = None
         self.__sap_gui = None
 
     def maximize(self) -> None:
-        """MÃ©todo para maximizar a tela principal."""
+        """Método para maximizar a tela principal."""
         self.__active_window.Maximize()
 
     def print_screen(self, path_and_name_imagem: str) -> None:
-        """MÃ©todo para printar a tela em uso.
+        """Método para printar a tela em uso.
 
         Args:
             path_and_name_imagem (str): Inserir caminho e nome do arquivo.
         """
         with open(f"{path_and_name_imagem}.bmp", "wb") as file:
             file.write(
                 self.__active_window.HardCopyToMemory(0)
@@ -350,15 +335,15 @@
     def press(
         self,
         name_press_object: str,
         type_press_object: str = "",
         item_press_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para pressionar um objeto.
+        """Método para pressionar um objeto.
 
         Args:
             name_press_object (str): Inserir nome do objeto.
             type_press_object (str, optional): Inserir tipo do objeto.
                 Defaults to "".
             item_press_object (int, optional): Inserir item do objeto.
                 Defaults to 0.
@@ -375,15 +360,15 @@
     def select(
         self,
         name_press_object: str,
         type_press_object: str = "",
         item_press_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para selecionar um objeto.
+        """Método para selecionar um objeto.
 
         Args:
             name_press_object (str): Inserir nome do objeto.
             type_press_object (str, optional): Inserir tipo do objeto.
                 Defaults to "".
             item_press_object (int, optional): Inserir item do objeto.
                 Defaults to 0.
@@ -397,101 +382,101 @@
             item_window
         ).Select()
 
     def find_object_id(
         self,
         id_find: str
     ) -> win32com.client:
-        """MÃ©todo para localizar um objeto pelo seu Id.
+        """Método para localizar um objeto pelo seu Id.
 
         Args:
             id_find (str): Informar o Id do objeto.
         """
         return self.__active_session.FindById(id_find)
 
     def tree_expand_node(
         self,
         id_find: str,
         node_key: str
     ) -> None:
-        """MÃ©todo para expandir o nÃ³ de uma Ã¡rvore.
+        """Método para expandir o nó de uma árvore.
 
         Args:
             id_find (str): Informar o Id do objeto.
-            node_key (str): Informar a chave do nÃ³.
+            node_key (str): Informar a chave do nó.
         """
         self.find_object_id(id_find).ExpandNode(node_key)
 
     def tree_select_node(
         self,
         id_find: str,
         node_key: str
     ) -> None:
-        """MÃ©todo para selecionar o nÃ³ de uma Ã¡rvore.
+        """Método para selecionar o nó de uma árvore.
 
         Args:
             id_find (str): Informar o Id do objeto.
-            node_key (str): Informar a chave do nÃ³.
+            node_key (str): Informar a chave do nó.
         """
         self.find_object_id(id_find).SelectNode(node_key)
 
     def tree_doble_click_node(
         self,
         id_find: str,
         node_key: str
     ) -> None:
-        """MÃ©todo para efetuar o duplo clique em um nÃ³ de uma Ã¡rvore.
+        """Método para efetuar o duplo clique em um nó de uma árvore.
 
         Args:
             id_find (str): Informar o Id do objeto.
-            node_key (str): Informar a chave do nÃ³.
+            node_key (str): Informar a chave do nó.
         """
         self.find_object_id(id_find).DoubleClickNode(node_key)
 
     def tree_unselect_node(
         self,
         id_find: str,
         node_key: str
     ) -> None:
-        """MÃ©todo para deselecionar o nÃ³ de uma Ã¡rvore.
+        """Método para deselecionar o nó de uma árvore.
 
         Args:
             id_find (str): Informar o Id do objeto.
-            node_key (str): Informar a chave do nÃ³.
+            node_key (str): Informar a chave do nó.
         """
         self.find_object_id(id_find).UnselectNode(node_key)
 
     def insert_dynamic_selection(
         self,
         id_find: str,
         node_key_expand: str,
         node_key_select: str
     ) -> None:
-        """MÃ©todo para inserir um item de seleÃ§Ã£o dinamica.
+        """Método para inserir um item de seleção dinamica.
 
         Args:
             id_find (str): Informar o Id do objeto.
-            node_key (str): Informar a chave do nÃ³.
+            node_key (str): Informar a chave do nó.
         """
         self.tree_expand_node(id_find, node_key_expand)
         self.tree_select_node(id_find, node_key_select)
         self.tree_doble_click_node(id_find, node_key_select)
         self.tree_unselect_node(id_find, node_key_select)
 
     def show_context_menu(
         self,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para mostar o menu de contexto de um objeto.
+        """Método para mostar o menu de contexto de um objeto.
 
         Args:
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
         """
@@ -502,29 +487,29 @@
             item_window
         ).ShowContextMenu()
 
     def select_context_menu(
         self,
         select_context: str
     ) -> None:
-        """MÃ©todo para selecionar o contexto.
+        """Método para selecionar o contexto.
 
         Args:
             select_context (str): Inserir nome do contexto.
         """
         self.find_object("usr").SelectContextMenuItem(select_context)
 
     def apply_context(
         self,
         select_context: str,
         list_apply_context: list,
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para aplicar um contexto do menu.
+        """Método para aplicar um contexto do menu.
 
         Args:
             select_context (str): Inserir nome do contexto.
             list_apply_context: Lista com nomes e tipos dos objetos.
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
@@ -544,19 +529,19 @@
         list_itens: list,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0",
         column_itens: int = 1
     ) -> None:
-        """MÃ©todo para inserir um texto em uma cÃ©lula.
+        """Método para inserir um texto em uma célula.
 
         Args:
             list_itens (list): Informar a lista de itens a serem inseridos.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
             column_itens (int, optional): Qual coluna deseja utilizar.
@@ -580,26 +565,26 @@
         row_cell: int,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0",
         column_cell: int = 0,
     ) -> None:
-        """MÃ©todo para pressionar uma cÃ©lula.
+        """Método para pressionar uma célula.
 
         Args:
-            row_cell (int): Informar a linha da cÃ©lula.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            row_cell (int): Informar a linha da célula.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
-            column_cell (int, optional): Informar a coluna da cÃ©lula.
+            column_cell (int, optional): Informar a coluna da célula.
                 Defaults to 0.
         """
         self.find_object(
             name_find_object,
             type_find_object,
             item_find_object,
             item_window
@@ -610,20 +595,20 @@
         row_shell: int,
         column_shell: str,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para efetuar um duplo click em uma shell.
+        """Método para efetuar um duplo click em uma shell.
 
         Args:
-            row_cell (int): Informar a linha da cÃ©lula.
+            row_cell (int): Informar a linha da célula.
             column_shell (str): Informar o nome da coluna.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
         """
@@ -640,19 +625,19 @@
         self,
         type_selection: bool,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para selecionar ou descelecionar uma checkbox.
+        """Método para selecionar ou descelecionar uma checkbox.
 
         Args:
-            type_selection (bool): Informar tipo da seleÃ§Ã£o.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            type_selection (bool): Informar tipo da seleção.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
         """
@@ -668,20 +653,20 @@
         name_layout: str,
         column_shell: str,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para selecionar um layout.
+        """Método para selecionar um layout.
 
         Args:
             name_layout (str): Informar a nome do layout.
             column_shell (str): Informar o nome da coluna.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
         """
@@ -713,19 +698,19 @@
         self,
         item_radio_button: int,
         name_find_object: str,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> None:
-        """MÃ©todo para selecionar um radio button.
+        """Método para selecionar um radio button.
 
         Args:
-            item_radio_button (int): Informar o item do rÃ¡dio button.
-            name_find_object (str): Informar o nome da Ã¡rea da tela.
+            item_radio_button (int): Informar o item do rádio button.
+            name_find_object (str): Informar o nome da área da tela.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to 0.
         """
@@ -733,18 +718,18 @@
             name_find_object,
             type_find_object,
             item_find_object,
             item_window
         ).GroupMembers.Item(item_radio_button).Select()
 
     def message(self) -> None:
-        """MÃ©todo para verificar se a mensagem Ã© de erro.
+        """Método para verificar se a mensagem é de erro.
 
         Raises:
-            Exception: Retorna a informaÃ§Ã£o sobre o erro.
+            Exception: Retorna a informação sobre o erro.
         """
         message = self.find_object(
             "sbar",
             "GuiStatusbar"
         )
         if message.MessageType in [
             "E",
@@ -755,15 +740,15 @@
             )
 
     def __return_items(
         self,
         objetc: win32com.client.CDispatch,
         index: int
     ) -> List[str]:
-        """MÃ©todo para retornar o modelo do layout de retorno.
+        """Método para retornar o modelo do layout de retorno.
 
         Args:
             objetc (win32com.client.CDispatch): Informar o objeto a ser
                 tratado.
             index (int): Informar o tipo de retorno desejado.
 
         Returns:
@@ -790,38 +775,38 @@
         return_type: int = 0,
         search_field: str = 'all',
         search_text: str = None,
         type_find_object: str = "",
         item_find_object: int = 0,
         item_window: str = "0"
     ) -> List[str]:
-        """MÃ©todo para retornar uma lista com as informaÃ§Ãµes desejadas.
+        """Método para retornar uma lista com as informações desejadas.
 
         Args:
             name_find_object (str): Informar nome do objeto que se deseja
                 visualizar.
             return_type (int, optional): Tipo de retorno que se deseja
                 retornar. Defaults to 0.
-            search_field (str, optional): Escolher o tipo de visualizaÃ§Ã£o
-                desejada, sÃ£o elas:
-                all - onde nÃ£o de faz filtro,
-                text - onde o filtro se baseia no texto da cÃ©lula e
+            search_field (str, optional): Escolher o tipo de visualização
+                desejada, são elas:
+                all - onde não de faz filtro,
+                text - onde o filtro se baseia no texto da célula e
                 type onde o filtro se baseio no tipo do objeto.
                 Defaults to 'all'.
             search_text (str, optional): Texto a ser localizado.
                 Defaults to None.
             type_find_object (str, optional): Informar o tipo do objeto.
                 Defaults to "".
             item_find_object (int, optional): Qual objeto deseja retornar.
                 Defaults to 0.
             item_window (str, optional): Qual janela deseja utilizar.
                 Defaults to "0".
 
         Returns:
-            List[str]: Retorna uma lista com as informaÃ§Ãµes desejadas.
+            List[str]: Retorna uma lista com as informações desejadas.
         """
         list_items: List[str] = []
         for item in self.find_object(
             name_find_object=name_find_object,
             type_find_object=type_find_object,
             item_find_object=item_find_object,
             item_window=item_window
@@ -837,9 +822,7 @@
                     )
             elif search_field == 'type':
                 if item.Type == search_text:
                     list_items.append(
                         self.__return_items(item, return_type)
                     )
         return list_items
-
-
```

