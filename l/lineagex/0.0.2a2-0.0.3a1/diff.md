# Comparing `tmp/lineagex-0.0.2a2.tar.gz` & `tmp/lineagex-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.2a2.tar", max compression
+gzip compressed data, was "lineagex-0.0.3a1.tar", max compression
```

## Comparing `lineagex-0.0.2a2.tar` & `lineagex-0.0.3a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.2a2/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.2a2/lineagex/app.js
--rw-r--r--   0        0        0    34528 2023-05-12 01:56:56.456690 lineagex-0.0.2a2/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    17230 2023-05-11 22:25:23.093987 lineagex-0.0.2a2/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     1456 2023-05-14 05:10:00.058421 lineagex-0.0.2a2/lineagex/lineagex.py
--rw-r--r--   0        0        0     2355 2023-05-12 02:16:08.034372 lineagex-0.0.2a2/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0     9896 2023-05-12 22:15:49.236456 lineagex-0.0.2a2/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     6556 2023-05-12 02:16:38.442999 lineagex-0.0.2a2/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.2a2/lineagex/stack.py
--rw-r--r--   0        0        0     6760 2023-05-14 05:18:23.887438 lineagex-0.0.2a2/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.2a2/lineagex/vendor.js
--rw-r--r--   0        0        0      449 2023-05-14 05:46:08.238849 lineagex-0.0.2a2/pyproject.toml
--rw-r--r--   0        0        0     3957 2023-05-14 05:36:49.891755 lineagex-0.0.2a2/README.md
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 lineagex-0.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.3a1/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.3a1/lineagex/app.js
+-rw-r--r--   0        0        0    35057 2023-05-19 22:22:34.333282 lineagex-0.0.3a1/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    19121 2023-05-18 23:32:07.683255 lineagex-0.0.3a1/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1632 2023-05-18 22:35:28.479396 lineagex-0.0.3a1/lineagex/lineagex.py
+-rw-r--r--   0        0        0     2375 2023-05-18 23:33:22.199597 lineagex-0.0.3a1/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    10065 2023-05-19 21:57:37.156213 lineagex-0.0.3a1/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-18 22:43:15.279746 lineagex-0.0.3a1/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.3a1/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.3a1/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.3a1/lineagex/vendor.js
+-rw-r--r--   0        0        0      443 2023-05-19 22:22:49.253570 lineagex-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.3a1/README.md
+-rw-r--r--   0        0        0     4858 1970-01-01 00:00:00.000000 lineagex-0.0.3a1/PKG-INFO
```

### Comparing `lineagex-0.0.2a2/lineagex/app.js` & `lineagex-0.0.3a1/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a2/lineagex/ColumnLineage.py` & `lineagex-0.0.3a1/lineagex/ColumnLineage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import re
 from sqlglot import parse_one, exp
 from sqlglot.expressions import CTE
 from sqlglot import expressions
 from psycopg2.extensions import connection
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Any
 
 from .utils import find_column
 
 
 class ColumnLineage:
     def __init__(
         self,
         plan: Optional[dict] = None,
         sql: Optional[str] = "",
-        table_name: Optional[str] = "",
-        conn: connection = None,
+        columns: Optional[List] = None,
+        conn: Any = None,
         part_tables: Optional[str] = None,
         search_schema: Optional[str] = "",
     ) -> None:
         self.split_regex = re.compile(r"[^a-zA-Z0-9._]")
         self.all_used_col = []
         self.possible_columns = []
         self.table_alias = {}
@@ -36,15 +36,15 @@
         self.cte_column = self._find_cte_col()
         self.final_output = ""
         self.final_node_type = ""
         self.subquery_final_output = ""
         self.column_dict = {}
         self.table_list = []
         self._traverse_plan(plan=plan)
-        self._resolve_column_dict(cols=self._find_final_column())
+        self._resolve_column_dict(cols=columns)
         self.table_list = sorted(set(self.table_list))
         # print(self.final_output)
         # print(self.subplan_dict)
         # print(self.table_alias)
         # print(self.cte_dict)
         # print(self.all_used_col)
         # print(self.possible_columns)
@@ -327,25 +327,36 @@
         When there's an index_cond in the plan, handle it and extract the necessary columns
         :param plan: the plan with the index_cond
         """
         temp = plan.get("Index Cond")
         if temp is not None:
             idx_name = plan.get("Index Name")
             if idx_name is not None:
-                cur = self.conn.cursor()
-                cur.execute("""SET search_path TO {};""".format(self.search_schema))
-                cur.execute(
-                    "SELECT schemaname, tablename, indexname, indexdef FROM pg_indexes WHERE indexname = '{}'".format(
-                        idx_name
+                if isinstance(self.conn, connection):
+                    # Postgres
+                    cur = self.conn.cursor()
+                    cur.execute("""SET search_path TO {};""".format(self.search_schema))
+                    cur.execute(
+                        "SELECT schemaname, tablename, indexname, indexdef FROM pg_indexes WHERE indexname = '{}'".format(
+                            idx_name
+                        )
                     )
-                )
-                result = cur.fetchall()[0]
-                cur.close()
-                # the indexdef is at index 3
-                indexdef = result[3]
+                    result = cur.fetchall()[0]
+                    cur.close()
+                    # the indexdef is at index 3
+                    indexdef = result[3]
+                else:
+                    # FalDbt
+                    idx_fal = self.faldbt.execute_sql(
+                        "SELECT schemaname, tablename, indexname, indexdef FROM pg_indexes WHERE indexname = '{}'".format(
+                            idx_name
+                        )
+                    )
+                    result = idx_fal.iloc[0]
+                    indexdef = result["indexdef"]
                 btree_idx = indexdef.find("USING btree")
                 if btree_idx != -1:
                     close_bracket = indexdef.find(")", btree_idx)
                     if close_bracket != -1:
                         idx_cols = indexdef[btree_idx + 13 : close_bracket].split(",")
                         alias = self.table_alias_reversed[result[0] + "." + result[1]]
                         for i in idx_cols:
```

### Comparing `lineagex-0.0.2a2/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.3a1/lineagex/ColumnLineageNoConn.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,37 +32,47 @@
 
     def _run_lineage(self, sql_ast: expressions = None, subquery_flag: bool = False) -> None:
         """
         Run the lineage after all the cte and subquery are resolved
         :param sql_ast: the ast for the sql
         :param subquery_flag: check if it is a subquery
         """
-        #print(sql_ast)
         if not subquery_flag:
+            self.all_used_col = []
+            if isinstance(sql_ast, exp.Union) or isinstance(sql_ast, exp.Except) or isinstance(sql_ast, exp.Intersect):
+                self._handle_union(sql_ast=sql_ast)
             main_tables = self._resolve_table(part_ast=sql_ast)
             self.table_list = self._find_all_tables(temp_table_list=main_tables)
             self.table_list.extend(self.all_subquery_table)
-            self.all_used_col = []
             self._shared_col_conds(part_ast=sql_ast, used_tables=main_tables)
             self.all_used_col.extend(self.sub_cols)
-            if isinstance(sql_ast, exp.Union) or isinstance(sql_ast, exp.Except) or isinstance(sql_ast, exp.Intersect):
-                for col in sql_ast.find_all(exp.Column):
-                    self.all_used_col.extend(self._find_alias_col(col_sql=col.sql(), temp_table=main_tables))
             self.all_used_col = set(self.all_used_col)
             if sql_ast.find(exp.Select):
                 for projection in sql_ast.find(exp.Select).expressions:
                     col_name = projection.alias_or_name
                     self.column_dict = self._resolve_proj(projection=projection, col_name=col_name, target_dict=self.column_dict, source_table=main_tables)
+            self.table_list = list(set(self.table_list))
         else:
             temp_sub_cols = []
             for col in sql_ast.find_all(exp.Column):
                 temp_sub_cols.extend(self._find_alias_col(col_sql=col.sql(), temp_table=self.sub_tables))
             self.sub_cols.extend(temp_sub_cols)
             #print(temp_sub_cols)
 
+    def _handle_union(self, sql_ast: expressions = None) -> None:
+        if isinstance(sql_ast, exp.Union) or isinstance(sql_ast, exp.Except) or isinstance(sql_ast, exp.Intersect):
+            self._handle_union(sql_ast=sql_ast.left)
+            self._handle_union(sql_ast=sql_ast.right)
+        else:
+            main_tables = self._resolve_table(part_ast=sql_ast)
+            self._shared_col_conds(part_ast=sql_ast, used_tables=main_tables)
+            for col in sql_ast.find_all(exp.Column):
+                self.all_used_col.extend(self._find_alias_col(col_sql=col.sql(), temp_table=main_tables))
+            return
+
     def _sub_shared_col_conds(self, sql_ast: expressions = None) -> None:
         """
         After the cte are resolved, run the subquery ast that is with the shared conditions(WHERE, GROUP BY, etc)
         :param sql_ast: the ast without the cte
         """
         # add in more conditions, including FROM/JOIN
         for cond in shared_conditions_with_table:
@@ -101,16 +111,26 @@
             all_cte_sub_table, all_cte_sub_cols = self._sub_shared_col_conds_cte(sql_ast=cte)
             self.all_used_col = []
             temp_cte_dict = {}
             temp_cte_table = self._resolve_table(part_ast=cte)
             cte_name = cte.find(exp.TableAlias).alias_or_name
             self.cte_table_dict[cte_name] = list(set(self._find_all_tables(temp_table_list=temp_cte_table) + all_cte_sub_table))
             # Resolving shared conditions
-            self._shared_col_conds(part_ast=cte, used_tables=temp_cte_table)
-            self.all_used_col.extend(all_cte_sub_cols)
+            if cte.find(exp.Union):
+                if cte.find(exp.Union).depth == cte.depth + 1:
+                    self._handle_union(sql_ast=cte.find(exp.Union))
+            elif cte.find(exp.Except):
+                if cte.find(exp.Except).depth == cte.depth + 1:
+                    self._handle_union(sql_ast=cte.find(exp.Union))
+            elif cte.find(exp.Intersect):
+                if cte.find(exp.Intersect).depth == cte.depth + 1:
+                    self._handle_union(sql_ast=cte.find(exp.Union))
+            else:
+                self._shared_col_conds(part_ast=cte, used_tables=temp_cte_table)
+                self.all_used_col.extend(all_cte_sub_cols)
             self.all_used_col = set(self.all_used_col)
             # Resolving the projection
             for projection in cte.find(exp.Select).expressions:
                 col_name = projection.alias_or_name
                 temp_cte_dict = self._resolve_proj(projection=projection, col_name=col_name, target_dict=temp_cte_dict, source_table=temp_cte_table)
             self.cte_dict[cte_name] = temp_cte_dict
 
@@ -119,36 +139,32 @@
         Resolve the projection given the projection expression
         :param projection: the given projection
         :param col_name: the column name
         :param target_dict: the dict it is outputting to
         :param source_table: all the source tables that this column might originate from
         """
         # Resolve count(*) with no alias, potentially other aggregations, MIN, MAX, SUM
-        if isinstance(projection, exp.Count) or isinstance(projection.unalias(), exp.Count)\
-                or isinstance(projection, exp.Avg) or isinstance(projection.unalias(), exp.Avg)\
-                or isinstance(projection, exp.Max) or isinstance(projection.unalias(), exp.Max)\
-                or isinstance(projection, exp.Min) or isinstance(projection.unalias(), exp.Min)\
-                or isinstance(projection, exp.Sum) or isinstance(projection.unalias(), exp.Sum):
+        if projection.find(exp.Star):
             if isinstance(projection, exp.Count):
                 col_name = "count"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
             elif isinstance(projection, exp.Avg):
                 col_name = "avg"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
             elif isinstance(projection, exp.Max):
                 col_name = "max"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
             elif isinstance(projection, exp.Min):
                 col_name = "min"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
             elif isinstance(projection, exp.Sum):
                 col_name = "sum"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
             else:
-                self._resolve_agg_star(col_name=col_name, projection=projection.unalias(), used_tables=source_table)
+                self._resolve_agg_star(col_name=col_name, projection=projection.unalias(), used_tables=source_table, target_dict=target_dict)
         else:
             proj_columns = []
             # Resolve only *
             if not isinstance(projection, exp.Column) and projection.find(exp.Star):
                 for t_name in source_table:
                     if t_name in self.input_table_dict.keys():
                         star_cols = self.input_table_dict[t_name]
@@ -188,14 +204,17 @@
                     else:
                         target_dict[p.sql()] = [p.sql()] + (list(self.all_used_col))
                 else:
                     # one projection can have many columns, append first
                     proj_columns.extend(self._find_alias_col(col_sql=p.sql(), temp_table=source_table))
             if proj_columns:
                 target_dict[col_name] = sorted(list(set(proj_columns).union(self.all_used_col)))
+            # If the column only uses literals, like MAX(1)
+            if not projection.find(exp.Column):
+                target_dict[col_name] = sorted(list(self.all_used_col))
         return target_dict
 
     def _resolve_table(self, part_ast: expressions = None) -> List:
         """
         Find the tables in the given ast
         :param part_ast: the ast to find the table
         """
@@ -288,39 +307,49 @@
                 t = temp[0]
             if t in self.cte_dict.keys():
                 return self.cte_dict[t][temp[1]]
             else:
                 return [t + "." + temp[1]]
         return [col_sql]
 
-    def _resolve_agg_star(self, col_name: Optional[str] = "", projection: expressions = None, used_tables: Optional[List] = None):
+    def _resolve_agg_star(self, col_name: Optional[str] = "", projection: expressions = None, used_tables: Optional[List] = None, target_dict: Optional[dict] = None):
         """
         Trying to resolve the * and append appropriate columns if the table is able to resolved
         :param col_name: the name of the column
         :param projection: the expression of the sql
         :param used_tables: the tables that are used
         """
         if projection.find(exp.Star):
             # * with a table name
             if projection.find(exp.Identifier):
                 t_name = projection.find(exp.Identifier).text("this")
                 # Resolve alias
                 if t_name in self.table_alias_dict.keys():
                     t_name = self.table_alias_dict[t_name]
-                if t_name in self.input_table_dict.keys():
-                    star_cols = []
-                    for s in self.input_table_dict[t_name]:
-                        star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
-                elif t_name in self.cte_dict.keys():
-                    star_cols = []
-                    for s in list(self.cte_dict[t_name].keys()):
-                        star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
+                if col_name == "*":
+                    if t_name in self.input_table_dict.keys():
+                        for s in self.input_table_dict[t_name]:
+                            self.all_used_col.add(s)
+                            target_dict[s] = sorted(list(set(self._find_alias_col(col_sql=t_name + "." + s, temp_table=used_tables)).union(self.all_used_col)))
+                    elif t_name in self.cte_dict.keys():
+                        for s in list(self.cte_dict[t_name].keys()):
+                            target_dict[s] = sorted(list(set(self._find_alias_col(col_sql=t_name + "." + s, temp_table=used_tables)).union(self.all_used_col)))
+                    else:
+                        target_dict[t_name + ".*"] = sorted(self.all_used_col)
                 else:
-                    star_cols = [t_name + ".*"]
-                self.column_dict[col_name] = sorted(list(set(star_cols).union(self.all_used_col)))
+                    if t_name in self.input_table_dict.keys():
+                        star_cols = []
+                        for s in self.input_table_dict[t_name]:
+                            star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
+                    elif t_name in self.cte_dict.keys():
+                        star_cols = []
+                        for s in list(self.cte_dict[t_name].keys()):
+                            star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
+                    else:
+                        star_cols = [t_name + ".*"]
+                    target_dict[col_name] = sorted(list(set(star_cols).union(self.all_used_col)))
             # only star, like count(*)
             else:
-                self.column_dict[col_name] = sorted(list(self.all_used_col))
-
+                target_dict[col_name] = sorted(list(self.all_used_col) + [t + ".*" for t in used_tables])
 
 if __name__ == "__main__":
     pass
```

### Comparing `lineagex-0.0.2a2/lineagex/lineagex.py` & `lineagex-0.0.3a1/lineagex/lineagex.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from .LineageXNoConn import LineageXNoConn
 
 
 class lineagex:
     def __init__(
             self,
             sql: Optional[Union[List, str]] = None,
-            search_schema: Optional[str] = "public",
+            target_schema: Optional[str] = "public",
             conn_string: Optional[str] = None,
+            search_path_schema: Optional[str] = "public",
     ) -> None:
         if sql is None:
             raise ValueError("the SQL input cannot be empty, please input a list of sql or path to sql")
         elif not isinstance(sql, list) and not isinstance(sql, str):
             raise ValueError("wrong SQL input format, please input a list of sql or path to sql")
         if conn_string:
-            lx = LineageXWithConn(sql, search_schema, conn_string)
+            lx = LineageXWithConn(path=sql, target_schema=target_schema, conn_string=conn_string, search_path_schema=search_path_schema)
             self._save_js_file()
             self.output_dict = lx.output_dict
         else:
-            lx = LineageXNoConn(sql, search_schema)
+            lx = LineageXNoConn(path=sql, search_path_schema=target_schema+","+search_path_schema)
             self._save_js_file()
             self.output_dict = lx.output_dict
 
     def _save_js_file(self):
         data = pkgutil.get_data(__name__, "app.js")
         js_file = open("app.js", "w", encoding="utf-8")
         js_file.write(data.decode("utf-8") )
```

### Comparing `lineagex-0.0.2a2/lineagex/LineageXNoConn.py` & `lineagex-0.0.3a1/lineagex/LineageXNoConn.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from .utils import produce_json
 from .SqlToDict import SqlToDict
 from .ColumnLineageNoConn import ColumnLineageNoConn
 
 
 class LineageXNoConn:
-    def __init__(self, path: Optional[str] = "", search_schema: Optional[str] = "public") -> None:
+    def __init__(self, path: Optional[str] = "", search_path_schema: Optional[str] = "public") -> None:
         self.output_dict = {}
-        search_schema = [x.strip() for x in search_schema.split(",")]
-        self.sql_files_dict = SqlToDict(path, search_schema).sql_files_dict
+        search_path_schema = [x.strip() for x in search_path_schema.split(",")]
+        self.sql_files_dict = SqlToDict(path, search_path_schema).sql_files_dict
         self.input_table_dict = {}
         self._run_lineage_no_conn()
 
     def _run_lineage_no_conn(self):
         """
         The driver function to extract the table lineage information
         :return: output an interactive html for the table lineage information
```

### Comparing `lineagex-0.0.2a2/lineagex/LineageXWithConn.py` & `lineagex-0.0.3a1/lineagex/LineageXWithConn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import re
 import psycopg2
 from psycopg2 import OperationalError
 from psycopg2.extensions import connection
 from typing import Tuple, List, Optional, Union
 
-from .utils import produce_json
+from .utils import produce_json, find_column
 from .SqlToDict import SqlToDict
 from .stack import *
 from .ColumnLineage import ColumnLineage
 
 
 class LineageXWithConn:
     def __init__(
         self,
         path: Optional[Union[List, str]] = None,
-        search_schema: Optional[str] = "public",
+        target_schema: Optional[str] = "public",
         conn_string: Optional[str] = "",
+        search_path_schema: Optional[str] = "public",
     ) -> None:
         self.part_tables = None
         self.df = None
-        self.schema = search_schema.split(",")[0]
-        self.search_schema = search_schema
+        self.schema = target_schema
+        self.search_schema = target_schema + "," + search_path_schema
         self.new_view_list = []
         self.s = Stack()
         self.path = path
         self.sql_files_dict = {}
         self.creation_list = []
         self.finished_list = []
         self.output_dict = {}
@@ -118,33 +119,33 @@
                 elif isinstance(log_plan, dict):
                     log_plan = log_plan["Plan"]
                     break
             if name in self.creation_list:
                 self._create_view(name=name, sql=sql)
                 self.new_view_list.append(self.schema + "." + name)
                 self.creation_list.pop(self.creation_list.index(name))
-                table_name = self.schema + "." + name
             else:
                 cur = self.conn.cursor()
                 cur.execute("""SET search_path TO {};""".format(self.search_schema))
                 cur.execute(
-                    """SELECT CONCAT (schemaname,'.', tablename) from pg_tables WHERE schemaname = ANY('{{{0}}}') and tablename = '{1}'""".format(
-                        self.search_schema, name
+                    """SELECT CONCAT (schemaname,'.', tablename) from pg_tables WHERE schemaname = '{0}' and tablename = '{1}'""".format(
+                        self.schema, name
                     )
                 )
-                table_name = cur.fetchone()
+                table_result = cur.fetchone()
                 cur.close()
-                if table_name:
-                    table_name = table_name[0]
-                else:
-                    table_name = self.schema + "." + name
+                if not table_result:
+                    self._create_view(name=name, sql=sql)
+                    self.new_view_list.append(self.schema + "." + name)
+            table_name = self.schema + "." + name
+            cols = find_column(table_name=table_name, engine=self.conn, search_schema=self.search_schema)
             col_lineage = ColumnLineage(
                 plan=log_plan,
                 sql=sql,
-                table_name=table_name,
+                columns=cols,
                 conn=self.conn,
                 part_tables=self.part_tables,
                 search_schema=self.search_schema,
             )
             self.output_dict[table_name] = {
                 "tables": col_lineage.table_list,
                 "columns": col_lineage.column_dict,
```

### Comparing `lineagex-0.0.2a2/lineagex/SqlToDict.py` & `lineagex-0.0.3a1/lineagex/SqlToDict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 import os
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from .utils import get_files, find_select, remove_comments
 
 rem_regex = re.compile(r"[^a-zA-Z0-9_.]")
 
 
 class SqlToDict:
-    def __init__(self, path: Optional[str] = "", schema_list: Optional[List] = None) -> None:
+    def __init__(self, path: Optional[Union[List, str]] = "", schema_list: Optional[List] = None) -> None:
         self.path = path
         self.schema_list = schema_list
         self.sql_files = []
         self.sql_files_dict = {}
         self.deletion_dict = {}
         self.insertion_dict = {}
         self.curr_name = ""
@@ -29,14 +29,21 @@
                 self._preprocess_sql(org_sql=val, file=str(idx))
         else:
             self.sql_files = get_files(path=self.path)
             for f in self.sql_files:
                 org_sql = open(f, mode="r", encoding="utf-8-sig").read()
                 org_sql = remove_comments(str1=org_sql)
                 org_sql_split = list(filter(None, org_sql.split(";")))
+                # pop DROP IF EXISTS
+                if len(org_sql_split) == 2:
+                    temp_str = org_sql_split[0].upper()
+                    if temp_str.find("SELECT ") == -1 and (temp_str.startswith("DROP TABLE IF EXISTS") or temp_str.startswith("DROP VIEW IF EXISTS")):
+                        org_sql_split.pop(0)
+                if f.endswith(".sql") or f.endswith(".SQL"):
+                    f = os.path.basename(f)[:-4]
                 if len(org_sql_split) <= 1:
                     self._preprocess_sql(org_sql=org_sql_split[0], file=f)
                 else:
                     for idx, val in enumerate(org_sql_split):
                         self._preprocess_sql(org_sql=val, file=f + "_" + str(idx))
 
     def _preprocess_sql(self, org_sql: Optional[str] = "", file: Optional[str] = "") -> None:
@@ -85,27 +92,29 @@
                         "DATETIME_SUB({},INTERVAL '{}' {})".format(i[0], i[1], i[2]),
                     )
                 else:
                     continue
         if re.search(
             "CREATE VIEW IF NOT EXISTS", ret_sql, flags=re.IGNORECASE
         ) or re.search("CREATE TABLE IF NOT EXISTS", ret_sql, flags=re.IGNORECASE):
-            temp = ret_sql.split(" ")
-            ret_sql = ret_sql[ret_sql.index(temp[7]) :]
-            if temp[5] in self.sql_files_dict.keys():
-                print("WARNING: duplicate script detected for {}".format(temp[5]))
-            self.sql_files_dict[temp[5]] = ret_sql
+            if ret_sql.upper().find("SELECT ") != -1:
+                temp = ret_sql.split(" ")
+                ret_sql = ret_sql[ret_sql.index(temp[7]) :]
+                if temp[5] in self.sql_files_dict.keys():
+                    print("WARNING: duplicate script detected for {}".format(temp[5]))
+                self.sql_files_dict[temp[5]] = ret_sql
         elif re.search("CREATE VIEW", ret_sql, flags=re.IGNORECASE) or re.search(
             "CREATE TABLE", ret_sql, flags=re.IGNORECASE
         ):
-            temp = ret_sql.split(" ")
-            ret_sql = ret_sql[ret_sql.index(temp[4]) :]
-            if temp[2] in self.sql_files_dict.keys():
-                print("WARNING: duplicate script detected for {}".format(temp[2]))
-            self.sql_files_dict[temp[2]] = ret_sql
+            if ret_sql.upper().find("SELECT ") != -1:
+                temp = ret_sql.split(" ")
+                ret_sql = ret_sql[ret_sql.index(temp[4]) :]
+                if temp[2] in self.sql_files_dict.keys():
+                    print("WARNING: duplicate script detected for {}".format(temp[2]))
+                self.sql_files_dict[temp[2]] = ret_sql
         # adjust to INSERT/DELETE/SELECT/
         elif ret_sql.find("INSERT INTO") != -1:
             # find the current name in the insertion dict and how many times it has been inserted
             self.curr_name = re.sub(rem_regex, "", ret_sql.split(" ")[2])
             if self.curr_name not in self.insertion_dict.keys():
                 self.insertion_dict[self.curr_name] = 1
             else:
```

### Comparing `lineagex-0.0.2a2/lineagex/stack.py` & `lineagex-0.0.3a1/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a2/lineagex/utils.py` & `lineagex-0.0.3a1/lineagex/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import os
 import ast
 import json
 from psycopg2.extensions import connection
-from typing import Tuple, List, Optional
+from typing import Tuple, List, Optional, Any
 
 
 def remove_comments(str1: Optional[str] = "") -> str:
     """
     Remove comments/excessive spaces/"create table as"/"create view as" from the sql file
     :param str1: the original sql
     :return: the parsed sql
@@ -23,39 +23,55 @@
     # replace all multiple spaces to one space
     str1 = re.sub("\s\s+", " ", q)
     str1 = str1.replace("\n", " ").strip()
     return str1
 
 
 def find_column(
-    table_name: Optional[str] = "", engine: connection = None, search_schema: Optional[str] = ""
+    table_name: Optional[str] = "", engine: Any = None, search_schema: Optional[str] = ""
 ) -> List:
     """
     Find the columns for the base table in the database
     :param search_schema: the schemas for SET search_path
     :param engine: the connection engine
     :param table_name: the base table name
     :return: the list of columns in the base table
     """
-    cur = engine.cursor()
-    cur.execute("""SET search_path TO {};""".format(search_schema))
-    cur.execute(
-        """SELECT attname AS col
+    if isinstance(engine, connection):
+        # Postgres
+        cur = engine.cursor()
+        cur.execute("""SET search_path TO {};""".format(search_schema))
+        cur.execute(
+            """SELECT attname AS col
+            FROM   pg_attribute
+            WHERE  attrelid = '{}'::regclass  -- table name optionally schema-qualified
+            AND    attnum > 0
+            AND    NOT attisdropped
+            ORDER  BY attnum;
+             ;""".format(
+                table_name
+            )
+        )
+        result = cur.fetchall()
+        cur.close()
+        return [s[0] for s in result]
+    else:
+        # FalDbt
+        cols_fal = engine.execute_sql(
+            """SELECT attname AS col
         FROM   pg_attribute
         WHERE  attrelid = '{}'::regclass  -- table name optionally schema-qualified
         AND    attnum > 0
         AND    NOT attisdropped
         ORDER  BY attnum;
          ;""".format(
-            table_name
+                table_name
+            )
         )
-    )
-    result = cur.fetchall()
-    cur.close()
-    return [s[0] for s in result]
+        return list(cols_fal["col"])
 
 
 def get_files(path: Optional[str] = "") -> List:
     """
     Extracting all files from the directory or just put the file name in a list
     :param path: path to the file/directory
     :return: all the files in the directory and its subdirectory
```

### Comparing `lineagex-0.0.2a2/lineagex/vendor.js` & `lineagex-0.0.3a1/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a2/README.md` & `lineagex-0.0.3a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 
 A Column Level Lineage Graph for Postgres
 
 Have you ever wondered what is the column level relationship among your SQL scripts and base tables? 
 Don't worry, this tool is intended to help you by creating an interactive graph on a webpage to explore the 
 column level lineage among them(Currently only supports Postgres, other connection types or dialects are under development).
 
-What you need is one line of code:
-
+Here is a [demo](https://zshandy.github.io/lineagex-demo/) with the [mimic-iv concepts_postgres](https://github.com/MIT-LCP/mimic-code/tree/main/mimic-iv/concepts_postgres) files([navigation instructions](#how-to-navigate-the-webpage)) and that is created with one line of code:
 ```python
 from lineagex.lineagex import lineagex
 
-lineagex("/path/to/SQL/" or [a_list_of_SQL_string])
+lineagex("/path/to/SQL/", "search, path, schemas", "postgresql://username:password@server:port/database")
 ```
-That is the bare minimum input, the input can be a path to a SQL file, a path to the folder containing many SQL files or 
-simply a list of SQL strings in Python. 
-
-Optionally, you can provide more information such as the schemas to the "search_path" in Postgres and 
-the connection string to the database to achieve a better result. 
+The input can be a path to a SQL file, a path to the folder containing many SQL files or simply a list of SQL strings in Python.
+Optionally, you can provide less information with only the SQLs, but providing the "search_path" and database connection is highly recommended for the best result. 
 ```python
 from lineagex.lineagex import lineagex
 
-lineagex("/path/to/SQL/", "search, path, schemas", "postgresql://username:password@server:port/database")
+lineagex("/path/to/SQL/" or [a_list_of_SQL_string])
 ```
 
 The output would be a output.json and a index.html file in the folder. Start a local http server and you would be able
 to see the interactive graph.
 
 ## Installation
 
@@ -72,15 +68,15 @@
     table_name: table2
   }, 
 }
 ```
 
 ## How to Navigate the Webpage
 ![Alt text](/tests/example.png?raw=true "example")
-- Start by clicking the star on the right(select) and input a model name that you want to start with.
+- Start by clicking the star on the right(select) and input a SQL name that you want to start with.
 - It should show a table on the canvas with table names and its columns, by clicking the "explore" button on the top right, it will show all the downstream and upstream tables that are related to the columns.
 - Hovering over a column will highlight its downstream and upstream columns as well.
 - You can navigate through the canvas by clicking "explore" on other tables.
 - The buttons on the right from top to bottom are: 
   - center the lineage to the middle
   - zoom out
   - zoom in
```

### Comparing `lineagex-0.0.2a2/PKG-INFO` & `lineagex-0.0.3a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.2a2
+Version: 0.0.3a1
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,30 +22,26 @@
 
 A Column Level Lineage Graph for Postgres
 
 Have you ever wondered what is the column level relationship among your SQL scripts and base tables? 
 Don't worry, this tool is intended to help you by creating an interactive graph on a webpage to explore the 
 column level lineage among them(Currently only supports Postgres, other connection types or dialects are under development).
 
-What you need is one line of code:
-
+Here is a [demo](https://zshandy.github.io/lineagex-demo/) with the [mimic-iv concepts_postgres](https://github.com/MIT-LCP/mimic-code/tree/main/mimic-iv/concepts_postgres) files([navigation instructions](#how-to-navigate-the-webpage)) and that is created with one line of code:
 ```python
 from lineagex.lineagex import lineagex
 
-lineagex("/path/to/SQL/" or [a_list_of_SQL_string])
+lineagex("/path/to/SQL/", "search, path, schemas", "postgresql://username:password@server:port/database")
 ```
-That is the bare minimum input, the input can be a path to a SQL file, a path to the folder containing many SQL files or 
-simply a list of SQL strings in Python. 
-
-Optionally, you can provide more information such as the schemas to the "search_path" in Postgres and 
-the connection string to the database to achieve a better result. 
+The input can be a path to a SQL file, a path to the folder containing many SQL files or simply a list of SQL strings in Python.
+Optionally, you can provide less information with only the SQLs, but providing the "search_path" and database connection is highly recommended for the best result. 
 ```python
 from lineagex.lineagex import lineagex
 
-lineagex("/path/to/SQL/", "search, path, schemas", "postgresql://username:password@server:port/database")
+lineagex("/path/to/SQL/" or [a_list_of_SQL_string])
 ```
 
 The output would be a output.json and a index.html file in the folder. Start a local http server and you would be able
 to see the interactive graph.
 
 ## Installation
 
@@ -92,15 +88,15 @@
     table_name: table2
   }, 
 }
 ```
 
 ## How to Navigate the Webpage
 ![Alt text](/tests/example.png?raw=true "example")
-- Start by clicking the star on the right(select) and input a model name that you want to start with.
+- Start by clicking the star on the right(select) and input a SQL name that you want to start with.
 - It should show a table on the canvas with table names and its columns, by clicking the "explore" button on the top right, it will show all the downstream and upstream tables that are related to the columns.
 - Hovering over a column will highlight its downstream and upstream columns as well.
 - You can navigate through the canvas by clicking "explore" on other tables.
 - The buttons on the right from top to bottom are: 
   - center the lineage to the middle
   - zoom out
   - zoom in
```

