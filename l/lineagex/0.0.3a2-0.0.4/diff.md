# Comparing `tmp/lineagex-0.0.3a2.tar.gz` & `tmp/lineagex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.3a2.tar", max compression
+gzip compressed data, was "lineagex-0.0.4.tar", max compression
```

## Comparing `lineagex-0.0.3a2.tar` & `lineagex-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.3a2/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.3a2/lineagex/app.js
--rw-r--r--   0        0        0    35055 2023-05-19 22:35:36.782021 lineagex-0.0.3a2/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    19121 2023-05-18 23:32:07.683255 lineagex-0.0.3a2/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     1632 2023-05-18 22:35:28.479396 lineagex-0.0.3a2/lineagex/lineagex.py
--rw-r--r--   0        0        0     2375 2023-05-18 23:33:22.199597 lineagex-0.0.3a2/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    10065 2023-05-19 21:57:37.156213 lineagex-0.0.3a2/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7176 2023-05-18 22:43:15.279746 lineagex-0.0.3a2/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.3a2/lineagex/stack.py
--rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.3a2/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.3a2/lineagex/vendor.js
--rw-r--r--   0        0        0      443 2023-05-19 22:36:07.268033 lineagex-0.0.3a2/pyproject.toml
--rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.3a2/README.md
--rw-r--r--   0        0        0     4858 1970-01-01 00:00:00.000000 lineagex-0.0.3a2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.4/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.4/lineagex/app.js
+-rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.4/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    22869 2023-05-20 01:36:05.905629 lineagex-0.0.4/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1794 2023-05-20 01:36:11.749312 lineagex-0.0.4/lineagex/lineagex.py
+-rw-r--r--   0        0        0     2389 2023-05-20 01:36:16.471395 lineagex-0.0.4/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    13474 2023-05-20 01:36:19.877229 lineagex-0.0.4/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-18 22:43:15.279746 lineagex-0.0.4/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.4/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.4/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.4/lineagex/vendor.js
+-rw-r--r--   0        0        0      448 2023-05-20 01:53:08.141075 lineagex-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.4/README.md
+-rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 lineagex-0.0.4/PKG-INFO
```

### Comparing `lineagex-0.0.3a2/lineagex/app.js` & `lineagex-0.0.4/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/lineagex/ColumnLineage.py` & `lineagex-0.0.4/lineagex/ColumnLineage.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class ColumnLineage:
     def __init__(
         self,
         plan: Optional[dict] = None,
         sql: Optional[str] = "",
         columns: Optional[List] = None,
         conn: Any = None,
-        part_tables: Optional[str] = None,
+        part_tables: Optional[dict] = None,
         search_schema: Optional[str] = "",
     ) -> None:
         self.split_regex = re.compile(r"[^a-zA-Z0-9._]")
         self.all_used_col = []
         self.possible_columns = []
         self.table_alias = {}
         self.table_alias_reversed = {}
@@ -47,75 +47,14 @@
         # print(self.table_alias)
         # print(self.cte_dict)
         # print(self.all_used_col)
         # print(self.possible_columns)
         # print("columns: ", self.column_dict)
         # print("table: ", self.table_list)
 
-    def _find_final_column(self) -> List[str]:
-        """
-        Find all the column names in the final projection
-        :return: the list of column names in the final projection
-        """
-        # Pop all CTE and Subquery trees
-        for with_sql in self.sql_ast.find_all(exp.With):
-            with_sql.pop()
-        for sub_sql in self.sql_ast.find_all(exp.Subquery):
-            sub_sql.pop()
-        final_column_list = []
-        for projection in self.sql_ast.find(exp.Select).expressions:
-            col_name = projection.alias_or_name
-            # Resolve aggregations with no alias
-            if isinstance(projection, exp.Count):
-                col_name = "count"
-            elif isinstance(projection, exp.Avg):
-                col_name = "avg"
-            elif isinstance(projection, exp.Max):
-                col_name = "max"
-            elif isinstance(projection, exp.Min):
-                col_name = "min"
-            # Resolve * and check if it is from a previous CTE or check database for the table
-            elif (
-                isinstance(projection, exp.Column) and projection.find(exp.Star)
-            ) or col_name == "*":
-                main_table_list = []
-                for table in self.sql_ast.find_all(exp.Table):
-                    table_def_split = re.split(" AS ", table.sql(), flags=re.IGNORECASE)
-                    main_table_list.append(table_def_split[0])
-                # if the * has a prefix
-                if projection.find(exp.Identifier):
-                    t_name = projection.find(exp.Identifier).text("this")
-                    if table_alias_dict[t_name] in self.cte_column.keys():
-                        col_name = self.cte_column[table_alias_dict[t_name]]
-                    else:
-                        col_name = find_column(
-                            table_name=table_alias_dict[t_name],
-                            engine=self.conn,
-                            search_schema=self.search_schema,
-                        )
-                # if * has no prefix
-                else:
-                    for t_name in main_table_list:
-                        if t_name in self.cte_column.keys():
-                            final_column_list.extend(self.cte_column[t_name])
-                        else:
-                            final_column_list.extend(
-                                find_column(
-                                    table_name=t_name,
-                                    engine=self.conn,
-                                    search_schema=self.search_schema,
-                                )
-                            )
-            if isinstance(col_name, list):
-                final_column_list.extend(col_name)
-            else:
-                if col_name != "*":
-                    final_column_list.append(col_name)
-        return final_column_list
-
     def _resolve_column_dict(self, cols: Optional[List] = None) -> None:
         """
         Insert into column_dict using the column names as keys and its dependencies as child
         :param cols: the columns for the final output
         :return: None
         """
         if len(self.final_output) > len(cols):
@@ -698,59 +637,60 @@
         :param cte_col_dict: the dict that stores the column names for the previous cte
         :return: the dict that contains column names with the current cte
         """
         # Find each CTE
         cte_name = cte.find(exp.TableAlias).alias_or_name
         cte_col_dict[cte_name] = []
         # Iterate column for each CTE
-        for projection in cte.find(exp.Select).expressions:
-            col_name = projection.alias_or_name
-            # Resolve aggregations with no alias
-            if isinstance(projection, exp.Count):
-                col_name = "count"
-            elif isinstance(projection, exp.Avg):
-                col_name = "avg"
-            elif isinstance(projection, exp.Max):
-                col_name = "max"
-            elif isinstance(projection, exp.Min):
-                col_name = "min"
-            elif isinstance(projection, exp.Sum):
-                col_name = "sum"
-            # Resolve * and check if it is from a previous CTE or check database for the table
-            elif (
-                isinstance(projection, exp.Column) and projection.find(exp.Star)
-            ) or col_name == "*":
-                table_alias_dict, cte_table_list = self._find_table(cte=cte)
-                # if the * has a prefix
-                if projection.find(exp.Identifier):
-                    t_name = projection.find(exp.Identifier).text("this")
-                    if table_alias_dict[t_name] in cte_col_dict.keys():
-                        col_name = cte_col_dict[table_alias_dict[t_name]]
-                    else:
-                        col_name = find_column(
-                            table_name=table_alias_dict[t_name],
-                            engine=self.conn,
-                            search_schema=self.search_schema,
-                        )
-                # if * has no prefix
-                else:
-                    for t_name in cte_table_list:
-                        if t_name in cte_col_dict.keys():
-                            cte_col_dict[cte_name].extend(cte_col_dict[t_name])
+        if cte.find(exp.Select):
+            for projection in cte.find(exp.Select).expressions:
+                col_name = projection.alias_or_name
+                # Resolve aggregations with no alias
+                if isinstance(projection, exp.Count):
+                    col_name = "count"
+                elif isinstance(projection, exp.Avg):
+                    col_name = "avg"
+                elif isinstance(projection, exp.Max):
+                    col_name = "max"
+                elif isinstance(projection, exp.Min):
+                    col_name = "min"
+                elif isinstance(projection, exp.Sum):
+                    col_name = "sum"
+                # Resolve * and check if it is from a previous CTE or check database for the table
+                elif (
+                    isinstance(projection, exp.Column) and projection.find(exp.Star)
+                ) or col_name == "*":
+                    table_alias_dict, cte_table_list = self._find_table(cte=cte)
+                    # if the * has a prefix
+                    if projection.find(exp.Identifier):
+                        t_name = projection.find(exp.Identifier).text("this")
+                        if table_alias_dict[t_name] in cte_col_dict.keys():
+                            col_name = cte_col_dict[table_alias_dict[t_name]]
                         else:
-                            cte_col_dict[cte_name].extend(
-                                find_column(
-                                    table_name=t_name,
-                                    engine=self.conn,
-                                    search_schema=self.search_schema,
-                                )
+                            col_name = find_column(
+                                table_name=table_alias_dict[t_name],
+                                engine=self.conn,
+                                search_schema=self.search_schema,
                             )
-            if isinstance(col_name, list):
-                cte_col_dict[cte_name].extend(col_name)
-            else:
-                if col_name != "*":
-                    cte_col_dict[cte_name].append(col_name)
+                    # if * has no prefix
+                    else:
+                        for t_name in cte_table_list:
+                            if t_name in cte_col_dict.keys():
+                                cte_col_dict[cte_name].extend(cte_col_dict[t_name])
+                            else:
+                                cte_col_dict[cte_name].extend(
+                                    find_column(
+                                        table_name=t_name,
+                                        engine=self.conn,
+                                        search_schema=self.search_schema,
+                                    )
+                                )
+                if isinstance(col_name, list):
+                    cte_col_dict[cte_name].extend(col_name)
+                else:
+                    if col_name != "*":
+                        cte_col_dict[cte_name].append(col_name)
         return cte_col_dict
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `lineagex-0.0.3a2/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.4/lineagex/ColumnLineageNoConn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from sqlglot import parse_one, exp
 from sqlglot import expressions
 from typing import Optional, List, Tuple
 import os
 
 shared_conditions = [exp.Where, exp.EQ, exp.Group, exp.Having, exp.Order]
-shared_conditions_with_table = [exp.Where, exp.EQ, exp.Group, exp.Having, exp.Order, exp.From, exp.Join]
+shared_conditions_with_table = [
+    exp.Where,
+    exp.EQ,
+    exp.Group,
+    exp.Having,
+    exp.Order,
+    exp.From,
+    exp.Join,
+]
 
 
 class ColumnLineageNoConn:
-    def __init__(self, sql: Optional[str] = "", input_table_dict: Optional[dict] = None):
+    def __init__(
+        self, sql: Optional[str] = "", input_table_dict: Optional[dict] = None
+    ):
         self.column_dict = {}
         self.table_alias_dict = {}
         self.cte_table_dict = {}
         self.cte_dict = {}
         self.input_table_dict = input_table_dict
         self.sql_ast = parse_one(sql, read="postgres")
         self.all_used_col = []
@@ -22,102 +32,138 @@
         self.sub_cols = []
         self._run_cte_lineage()
         # Everything other than CTEs, and pop the CTE tree
         for with_sql in self.sql_ast.find_all(exp.With):
             with_sql.pop()
         self._sub_shared_col_conds(sql_ast=self.sql_ast)
         self._run_lineage(self.sql_ast, False)
-        #print(self.cte_dict)
-        #print(self.column_dict)
-        #print(self.table_list)
-
-    def _run_lineage(self, sql_ast: expressions = None, subquery_flag: bool = False) -> None:
+        # print(self.cte_dict)
+        # print(self.column_dict)
+        # print(self.table_list)
+
+    def _run_lineage(
+        self, sql_ast: expressions = None, subquery_flag: bool = False
+    ) -> None:
         """
         Run the lineage after all the cte and subquery are resolved
         :param sql_ast: the ast for the sql
         :param subquery_flag: check if it is a subquery
         """
         if not subquery_flag:
             self.all_used_col = []
-            if isinstance(sql_ast, exp.Union) or isinstance(sql_ast, exp.Except) or isinstance(sql_ast, exp.Intersect):
+            if (
+                isinstance(sql_ast, exp.Union)
+                or isinstance(sql_ast, exp.Except)
+                or isinstance(sql_ast, exp.Intersect)
+            ):
                 self._handle_union(sql_ast=sql_ast)
             main_tables = self._resolve_table(part_ast=sql_ast)
             self.table_list = self._find_all_tables(temp_table_list=main_tables)
             self.table_list.extend(self.all_subquery_table)
             self._shared_col_conds(part_ast=sql_ast, used_tables=main_tables)
             self.all_used_col.extend(self.sub_cols)
             self.all_used_col = set(self.all_used_col)
             if sql_ast.find(exp.Select):
                 for projection in sql_ast.find(exp.Select).expressions:
                     col_name = projection.alias_or_name
-                    self.column_dict = self._resolve_proj(projection=projection, col_name=col_name, target_dict=self.column_dict, source_table=main_tables)
+                    self.column_dict = self._resolve_proj(
+                        projection=projection,
+                        col_name=col_name,
+                        target_dict=self.column_dict,
+                        source_table=main_tables,
+                    )
             self.table_list = list(set(self.table_list))
         else:
             temp_sub_cols = []
             for col in sql_ast.find_all(exp.Column):
-                temp_sub_cols.extend(self._find_alias_col(col_sql=col.sql(), temp_table=self.sub_tables))
+                temp_sub_cols.extend(
+                    self._find_alias_col(col_sql=col.sql(), temp_table=self.sub_tables)
+                )
             self.sub_cols.extend(temp_sub_cols)
-            #print(temp_sub_cols)
+            # print(temp_sub_cols)
 
     def _handle_union(self, sql_ast: expressions = None) -> None:
-        if isinstance(sql_ast, exp.Union) or isinstance(sql_ast, exp.Except) or isinstance(sql_ast, exp.Intersect):
+        if (
+            isinstance(sql_ast, exp.Union)
+            or isinstance(sql_ast, exp.Except)
+            or isinstance(sql_ast, exp.Intersect)
+        ):
             self._handle_union(sql_ast=sql_ast.left)
             self._handle_union(sql_ast=sql_ast.right)
         else:
             main_tables = self._resolve_table(part_ast=sql_ast)
             self._shared_col_conds(part_ast=sql_ast, used_tables=main_tables)
             for col in sql_ast.find_all(exp.Column):
-                self.all_used_col.extend(self._find_alias_col(col_sql=col.sql(), temp_table=main_tables))
+                self.all_used_col.extend(
+                    self._find_alias_col(col_sql=col.sql(), temp_table=main_tables)
+                )
             return
 
     def _sub_shared_col_conds(self, sql_ast: expressions = None) -> None:
         """
         After the cte are resolved, run the subquery ast that is with the shared conditions(WHERE, GROUP BY, etc)
         :param sql_ast: the ast without the cte
         """
         # add in more conditions, including FROM/JOIN
         for cond in shared_conditions_with_table:
             for cond_sql in sql_ast.find_all(cond):
                 for sub_ast in cond_sql.find_all(exp.Subquery):
                     self.sub_tables = self._resolve_table(part_ast=sub_ast)
-                    self.all_subquery_table.extend(self._find_all_tables(temp_table_list=self.sub_tables))
+                    self.all_subquery_table.extend(
+                        self._find_all_tables(temp_table_list=self.sub_tables)
+                    )
                     self._run_lineage(sub_ast, True)
                     sub_ast.pop()
 
-    def _sub_shared_col_conds_cte(self, sql_ast: expressions = None) -> Tuple[List, List]:
+    def _sub_shared_col_conds_cte(
+        self, sql_ast: expressions = None
+    ) -> Tuple[List, List]:
         """
         Run the subquery inside the cte first that is with the shared conditions(WHERE, GROUP BY, etc)
         :param sql_ast: the ast for the cte
         """
         all_cte_sub_table = []
         all_cte_sub_cols = []
         # add in more conditions, including FROM/JOIN
         for cond in shared_conditions_with_table:
             for cond_sql in sql_ast.find_all(cond):
                 for sub_ast in cond_sql.find_all(exp.Select):
                     temp_sub_table = self._resolve_table(part_ast=sub_ast)
                     temp_sub_cols = []
                     for col in sub_ast.find_all(exp.Column):
-                        temp_sub_cols.extend(self._find_alias_col(col_sql=col.sql(), temp_table=temp_sub_table))
-                    all_cte_sub_table.extend(self._find_all_tables(temp_table_list=temp_sub_table))
+                        temp_sub_cols.extend(
+                            self._find_alias_col(
+                                col_sql=col.sql(), temp_table=temp_sub_table
+                            )
+                        )
+                    all_cte_sub_table.extend(
+                        self._find_all_tables(temp_table_list=temp_sub_table)
+                    )
                     all_cte_sub_cols.extend(temp_sub_cols)
                     sub_ast.pop()
         return all_cte_sub_table, all_cte_sub_cols
 
     def _run_cte_lineage(self):
         """
         Run the lineage information for all the cte
         """
         for cte in self.sql_ast.find_all(exp.CTE):
-            all_cte_sub_table, all_cte_sub_cols = self._sub_shared_col_conds_cte(sql_ast=cte)
+            all_cte_sub_table, all_cte_sub_cols = self._sub_shared_col_conds_cte(
+                sql_ast=cte
+            )
             self.all_used_col = []
             temp_cte_dict = {}
             temp_cte_table = self._resolve_table(part_ast=cte)
             cte_name = cte.find(exp.TableAlias).alias_or_name
-            self.cte_table_dict[cte_name] = list(set(self._find_all_tables(temp_table_list=temp_cte_table) + all_cte_sub_table))
+            self.cte_table_dict[cte_name] = list(
+                set(
+                    self._find_all_tables(temp_table_list=temp_cte_table)
+                    + all_cte_sub_table
+                )
+            )
             # Resolving shared conditions
             if cte.find(exp.Union):
                 if cte.find(exp.Union).depth == cte.depth + 1:
                     self._handle_union(sql_ast=cte.find(exp.Union))
             elif cte.find(exp.Except):
                 if cte.find(exp.Except).depth == cte.depth + 1:
                     self._handle_union(sql_ast=cte.find(exp.Union))
@@ -127,113 +173,188 @@
             else:
                 self._shared_col_conds(part_ast=cte, used_tables=temp_cte_table)
                 self.all_used_col.extend(all_cte_sub_cols)
             self.all_used_col = set(self.all_used_col)
             # Resolving the projection
             for projection in cte.find(exp.Select).expressions:
                 col_name = projection.alias_or_name
-                temp_cte_dict = self._resolve_proj(projection=projection, col_name=col_name, target_dict=temp_cte_dict, source_table=temp_cte_table)
+                temp_cte_dict = self._resolve_proj(
+                    projection=projection,
+                    col_name=col_name,
+                    target_dict=temp_cte_dict,
+                    source_table=temp_cte_table,
+                )
             self.cte_dict[cte_name] = temp_cte_dict
 
-    def _resolve_proj(self, projection: expressions = None, col_name: Optional[str] = "", target_dict: Optional[dict] = None, source_table: Optional[List] = None) -> dict:
+    def _resolve_proj(
+        self,
+        projection: expressions = None,
+        col_name: Optional[str] = "",
+        target_dict: Optional[dict] = None,
+        source_table: Optional[List] = None,
+    ) -> dict:
         """
         Resolve the projection given the projection expression
         :param projection: the given projection
         :param col_name: the column name
         :param target_dict: the dict it is outputting to
         :param source_table: all the source tables that this column might originate from
         """
         # Resolve count(*) with no alias, potentially other aggregations, MIN, MAX, SUM
         if projection.find(exp.Star):
             if isinstance(projection, exp.Count):
                 col_name = "count"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection,
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
             elif isinstance(projection, exp.Avg):
                 col_name = "avg"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection,
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
             elif isinstance(projection, exp.Max):
                 col_name = "max"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection,
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
             elif isinstance(projection, exp.Min):
                 col_name = "min"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection,
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
             elif isinstance(projection, exp.Sum):
                 col_name = "sum"
-                self._resolve_agg_star(col_name=col_name, projection=projection, used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection,
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
             else:
-                self._resolve_agg_star(col_name=col_name, projection=projection.unalias(), used_tables=source_table, target_dict=target_dict)
+                self._resolve_agg_star(
+                    col_name=col_name,
+                    projection=projection.unalias(),
+                    used_tables=source_table,
+                    target_dict=target_dict,
+                )
         else:
             proj_columns = []
             # Resolve only *
             if not isinstance(projection, exp.Column) and projection.find(exp.Star):
                 for t_name in source_table:
                     if t_name in self.input_table_dict.keys():
                         star_cols = self.input_table_dict[t_name]
                         # every column from there will be a column with that name
                         for per_star_col in star_cols:
                             target_dict[per_star_col] = sorted(
-                                list(set(self._find_alias_col(col_sql=per_star_col, temp_table=source_table)).union(
-                                    self.all_used_col)))
+                                list(
+                                    set(
+                                        self._find_alias_col(
+                                            col_sql=per_star_col,
+                                            temp_table=source_table,
+                                        )
+                                    ).union(self.all_used_col)
+                                )
+                            )
                     elif t_name in self.cte_dict.keys():
                         star_cols = list(self.cte_dict[t_name].keys())
                         for per_star_col in star_cols:
                             target_dict[per_star_col] = sorted(
-                                list(set(self.cte_dict[t_name][per_star_col]).union(self.all_used_col)))
+                                list(
+                                    set(self.cte_dict[t_name][per_star_col]).union(
+                                        self.all_used_col
+                                    )
+                                )
+                            )
             # Resolve projections that have many columns, some of which could be *
             for p in projection.find_all(exp.Column):
                 # Resolve * with other columns
                 if isinstance(p, exp.Column) and p.find(exp.Star):
                     t_name = p.find(exp.Identifier).text("this")
                     # Resolve alias
                     if t_name in self.table_alias_dict.keys():
                         t_name = self.table_alias_dict[t_name]
                     # If from input table, get all columns from there
                     if t_name in self.input_table_dict.keys():
                         star_cols = self.input_table_dict[t_name]
                         # every column from there will be a column with that name
                         for per_star_col in star_cols:
                             target_dict[per_star_col] = sorted(
-                                list(set(self._find_alias_col(col_sql=per_star_col, temp_table=source_table)).union(
-                                    self.all_used_col)))
+                                list(
+                                    set(
+                                        self._find_alias_col(
+                                            col_sql=per_star_col,
+                                            temp_table=source_table,
+                                        )
+                                    ).union(self.all_used_col)
+                                )
+                            )
                     # If from another CTE, get all columns from there
                     elif t_name in self.cte_dict.keys():
                         star_cols = list(self.cte_dict[t_name].keys())
                         for per_star_col in star_cols:
                             target_dict[per_star_col] = sorted(
-                                list(set(self.cte_dict[t_name][per_star_col]).union(self.all_used_col)))
+                                list(
+                                    set(self.cte_dict[t_name][per_star_col]).union(
+                                        self.all_used_col
+                                    )
+                                )
+                            )
                     # If from an unknown table, leave it with a STAR as temporary name
                     else:
                         target_dict[p.sql()] = [p.sql()] + (list(self.all_used_col))
                 else:
                     # one projection can have many columns, append first
-                    proj_columns.extend(self._find_alias_col(col_sql=p.sql(), temp_table=source_table))
+                    proj_columns.extend(
+                        self._find_alias_col(col_sql=p.sql(), temp_table=source_table)
+                    )
             if proj_columns:
-                target_dict[col_name] = sorted(list(set(proj_columns).union(self.all_used_col)))
+                target_dict[col_name] = sorted(
+                    list(set(proj_columns).union(self.all_used_col))
+                )
             # If the column only uses literals, like MAX(1)
             if not projection.find(exp.Column):
                 target_dict[col_name] = sorted(list(self.all_used_col))
         return target_dict
 
     def _resolve_table(self, part_ast: expressions = None) -> List:
         """
         Find the tables in the given ast
         :param part_ast: the ast to find the table
         """
         temp_table_list = []
         # Resolve FROM
         for table_sql in part_ast.find_all(exp.From):
             for table in table_sql.find_all(exp.Table):
-                temp_table_list = self._find_table(table=table, temp_table_list=temp_table_list)
+                temp_table_list = self._find_table(
+                    table=table, temp_table_list=temp_table_list
+                )
         # Resolve JOIN
         for table_sql in part_ast.find_all(exp.Join):
             for table in table_sql.find_all(exp.Table):
-                temp_table_list = self._find_table(table=table, temp_table_list=temp_table_list)
+                temp_table_list = self._find_table(
+                    table=table, temp_table_list=temp_table_list
+                )
         return temp_table_list
 
-    def _find_table(self, table: expressions = None, temp_table_list: Optional[List] = None) -> List:
+    def _find_table(
+        self, table: expressions = None, temp_table_list: Optional[List] = None
+    ) -> List:
         """
         Update table alias and find all aliased used table names
         :param table: the expression with the table
         :param temp_table_list: temporary list of tables for appending the used tables
         :return:
         """
         if table.alias == "":
@@ -259,27 +380,35 @@
                 table_name = self.table_alias_dict[i]
             if table_name in self.cte_table_dict.keys():
                 ret_table.extend(self.cte_table_dict[table_name])
             else:
                 ret_table.append(table_name)
         return ret_table
 
-    def _shared_col_conds(self, part_ast: expressions = None, used_tables: Optional[List] = None):
+    def _shared_col_conds(
+        self, part_ast: expressions = None, used_tables: Optional[List] = None
+    ):
         """
         Extract all the columns in the shared conditions(WHERE, GROUP BY, etc)
         :param part_ast: the ast of the sql to extract
         :param used_tables: the tables that this sql uses
         """
         # COMBINE THE CONDITIONS
         for cond in shared_conditions:
             for cond_sql in part_ast.find_all(cond):
                 for cond_col in cond_sql.find_all(exp.Column):
-                    self.all_used_col.extend(self._find_alias_col(col_sql=cond_col.sql(), temp_table=used_tables))
-
-    def _find_alias_col(self, col_sql: Optional[str] = "", temp_table: Optional[List] = None) -> List:
+                    self.all_used_col.extend(
+                        self._find_alias_col(
+                            col_sql=cond_col.sql(), temp_table=used_tables
+                        )
+                    )
+
+    def _find_alias_col(
+        self, col_sql: Optional[str] = "", temp_table: Optional[List] = None
+    ) -> List:
         """
         Find the columns and its alias and dependencies if it is from a cte
         :param col_sql: the sql to the column
         :param temp_table: the table that the sql uses
         :return:
         """
         temp = col_sql.split(".")
@@ -307,15 +436,21 @@
                 t = temp[0]
             if t in self.cte_dict.keys():
                 return self.cte_dict[t][temp[1]]
             else:
                 return [t + "." + temp[1]]
         return [col_sql]
 
-    def _resolve_agg_star(self, col_name: Optional[str] = "", projection: expressions = None, used_tables: Optional[List] = None, target_dict: Optional[dict] = None):
+    def _resolve_agg_star(
+        self,
+        col_name: Optional[str] = "",
+        projection: expressions = None,
+        used_tables: Optional[List] = None,
+        target_dict: Optional[dict] = None,
+    ):
         """
         Trying to resolve the * and append appropriate columns if the table is able to resolved
         :param col_name: the name of the column
         :param projection: the expression of the sql
         :param used_tables: the tables that are used
         """
         if projection.find(exp.Star):
@@ -325,31 +460,58 @@
                 # Resolve alias
                 if t_name in self.table_alias_dict.keys():
                     t_name = self.table_alias_dict[t_name]
                 if col_name == "*":
                     if t_name in self.input_table_dict.keys():
                         for s in self.input_table_dict[t_name]:
                             self.all_used_col.add(s)
-                            target_dict[s] = sorted(list(set(self._find_alias_col(col_sql=t_name + "." + s, temp_table=used_tables)).union(self.all_used_col)))
+                            target_dict[s] = sorted(
+                                list(
+                                    set(
+                                        self._find_alias_col(
+                                            col_sql=t_name + "." + s,
+                                            temp_table=used_tables,
+                                        )
+                                    ).union(self.all_used_col)
+                                )
+                            )
                     elif t_name in self.cte_dict.keys():
                         for s in list(self.cte_dict[t_name].keys()):
-                            target_dict[s] = sorted(list(set(self._find_alias_col(col_sql=t_name + "." + s, temp_table=used_tables)).union(self.all_used_col)))
+                            target_dict[s] = sorted(
+                                list(
+                                    set(
+                                        self._find_alias_col(
+                                            col_sql=t_name + "." + s,
+                                            temp_table=used_tables,
+                                        )
+                                    ).union(self.all_used_col)
+                                )
+                            )
                     else:
                         target_dict[t_name + ".*"] = sorted(self.all_used_col)
                 else:
                     if t_name in self.input_table_dict.keys():
                         star_cols = []
                         for s in self.input_table_dict[t_name]:
-                            star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
+                            star_cols.extend(
+                                self._find_alias_col(col_sql=s, temp_table=used_tables)
+                            )
                     elif t_name in self.cte_dict.keys():
                         star_cols = []
                         for s in list(self.cte_dict[t_name].keys()):
-                            star_cols.extend(self._find_alias_col(col_sql=s, temp_table=used_tables))
+                            star_cols.extend(
+                                self._find_alias_col(col_sql=s, temp_table=used_tables)
+                            )
                     else:
                         star_cols = [t_name + ".*"]
-                    target_dict[col_name] = sorted(list(set(star_cols).union(self.all_used_col)))
+                    target_dict[col_name] = sorted(
+                        list(set(star_cols).union(self.all_used_col))
+                    )
             # only star, like count(*)
             else:
-                target_dict[col_name] = sorted(list(self.all_used_col) + [t + ".*" for t in used_tables])
+                target_dict[col_name] = sorted(
+                    list(self.all_used_col) + [t + ".*" for t in used_tables]
+                )
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `lineagex-0.0.3a2/lineagex/lineagex.py` & `lineagex-0.0.4/lineagex/lineagex.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,50 @@
 
 from .LineageXWithConn import LineageXWithConn
 from .LineageXNoConn import LineageXNoConn
 
 
 class lineagex:
     def __init__(
-            self,
-            sql: Optional[Union[List, str]] = None,
-            target_schema: Optional[str] = "public",
-            conn_string: Optional[str] = None,
-            search_path_schema: Optional[str] = "public",
+        self,
+        sql: Optional[Union[List, str]] = None,
+        target_schema: Optional[str] = "public",
+        conn_string: Optional[str] = None,
+        search_path_schema: Optional[str] = "public",
     ) -> None:
         if sql is None:
-            raise ValueError("the SQL input cannot be empty, please input a list of sql or path to sql")
+            raise ValueError(
+                "the SQL input cannot be empty, please input a list of sql or path to sql"
+            )
         elif not isinstance(sql, list) and not isinstance(sql, str):
-            raise ValueError("wrong SQL input format, please input a list of sql or path to sql")
+            raise ValueError(
+                "wrong SQL input format, please input a list of sql or path to sql"
+            )
         if conn_string:
-            lx = LineageXWithConn(path=sql, target_schema=target_schema, conn_string=conn_string, search_path_schema=search_path_schema)
+            lx = LineageXWithConn(
+                sql=sql,
+                target_schema=target_schema,
+                conn_string=conn_string,
+                search_path_schema=search_path_schema,
+            )
             self._save_js_file()
             self.output_dict = lx.output_dict
         else:
-            lx = LineageXNoConn(path=sql, search_path_schema=target_schema+","+search_path_schema)
+            lx = LineageXNoConn(
+                sql=sql, search_path_schema=target_schema + "," + search_path_schema
+            )
             self._save_js_file()
             self.output_dict = lx.output_dict
 
     def _save_js_file(self):
         data = pkgutil.get_data(__name__, "app.js")
         js_file = open("app.js", "w", encoding="utf-8")
-        js_file.write(data.decode("utf-8") )
+        js_file.write(data.decode("utf-8"))
         js_file.close()
         data = pkgutil.get_data(__name__, "vendor.js")
         js_file = open("vendor.js", "w", encoding="utf-8")
-        js_file.write(data.decode("utf-8") )
+        js_file.write(data.decode("utf-8"))
         js_file.close()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     pass
```

### Comparing `lineagex-0.0.3a2/lineagex/LineageXNoConn.py` & `lineagex-0.0.4/lineagex/LineageXNoConn.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from .utils import produce_json
 from .SqlToDict import SqlToDict
 from .ColumnLineageNoConn import ColumnLineageNoConn
 
 
 class LineageXNoConn:
-    def __init__(self, path: Optional[str] = "", search_path_schema: Optional[str] = "public") -> None:
+    def __init__(
+        self, sql: Optional[str] = "", search_path_schema: Optional[str] = "public"
+    ) -> None:
         self.output_dict = {}
         search_path_schema = [x.strip() for x in search_path_schema.split(",")]
-        self.sql_files_dict = SqlToDict(path, search_path_schema).sql_files_dict
+        self.sql_files_dict = SqlToDict(sql, search_path_schema).sql_files_dict
         self.input_table_dict = {}
         self._run_lineage_no_conn()
 
     def _run_lineage_no_conn(self):
         """
         The driver function to extract the table lineage information
         :return: output an interactive html for the table lineage information
@@ -38,15 +40,15 @@
 
     def _guess_schema_name(self):
         """
         Try to guess the schema names for the sql provided for a more accurate depiction
         """
         all_tables = []
         for key, val in self.output_dict.items():
-            all_tables.extend(val['tables'])
+            all_tables.extend(val["tables"])
         all_tables = list(set(all_tables))
         tables_dict = {}
         for t in all_tables:
             tables_dict[t.split(".")[-1]] = t
         for key, val in self.output_dict.copy().items():
             if key in tables_dict.keys():
                 if tables_dict[key] != key:
```

### Comparing `lineagex-0.0.3a2/lineagex/LineageXWithConn.py` & `lineagex-0.0.4/lineagex/LineageXWithConn.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,51 +10,119 @@
 from .stack import *
 from .ColumnLineage import ColumnLineage
 
 
 class LineageXWithConn:
     def __init__(
         self,
-        path: Optional[Union[List, str]] = None,
+        sql: Optional[Union[List, str]] = None,
         target_schema: Optional[str] = "public",
         conn_string: Optional[str] = "",
         search_path_schema: Optional[str] = "public",
     ) -> None:
         self.part_tables = None
         self.df = None
         self.schema = target_schema
         self.search_schema = target_schema + "," + search_path_schema
         self.new_view_list = []
         self.s = Stack()
-        self.path = path
+        self.sql = sql
         self.sql_files_dict = {}
         self.creation_list = []
         self.finished_list = []
         self.output_dict = {}
         self.conn = self._check_db_connection(conn_string)
         self.conn.autocommit = True
         self._run_table_lineage()
 
     def _run_table_lineage(self) -> None:
         """
         The driver function to extract the table lineage information
         :return: output an interactive html for the table lineage information
         """
         self.part_tables, self.schema_list = self._get_part_tables()
-        self.sql_files_dict = SqlToDict(self.path, self.schema_list).sql_files_dict
-        for name, sql in self.sql_files_dict.items():
-            try:
-                if name not in self.finished_list:
-                    self._explain_sql(name=name, sql=sql)
-                else:
+        # If the input is a list with no SELECT , assume it to be a list of views/schema
+        if isinstance(self.sql, List) and not any(
+            "SELECT " in s.upper() for s in self.sql
+        ):
+            cur = self.conn.cursor()
+            cur.execute("""SET search_path TO {};""".format(self.search_schema))
+            for t in self.sql:
+                temp = t.split(".")
+                if len(temp) == 2:
+                    cur.execute(
+                        "SELECT concat_ws('.',schemaname,viewname) AS view_name, definition FROM pg_catalog.pg_views WHERE schemaname = '{}' and viewname = '{}';".format(
+                            temp[0], temp[1]
+                        )
+                    )
+                    view_ret = cur.fetchall()
+                    if view_ret:
+                        self.sql_files_dict[view_ret[0][0]] = view_ret[0][1]
+                    else:
+                        print(
+                            "{} is skipped because database returned no result on it".format(
+                                t
+                            )
+                        )
+                elif len(temp) == 1:
+                    cur.execute(
+                        "SELECT concat_ws('.',schemaname,viewname) AS view_name, definition FROM pg_catalog.pg_views WHERE schemaname = '{}';".format(
+                            temp[0]
+                        )
+                    )
+                    schema_ret = cur.fetchall()
+                    if schema_ret:
+                        for s in schema_ret:
+                            self.sql_files_dict[s[0]] = s[1]
+                    else:
+                        print(
+                            "{} is skipped because database returned no result on it".format(
+                                t
+                            )
+                        )
+            cur.close()
+            for name, sql in self.sql_files_dict.items():
+                try:
+                    col_lineage = ColumnLineage(
+                        plan=self._get_plan(sql=sql),
+                        sql=sql,
+                        columns=find_column(
+                            table_name=name,
+                            engine=self.conn,
+                            search_schema=self.search_schema,
+                        ),
+                        conn=self.conn,
+                        part_tables=self.part_tables,
+                        search_schema=self.search_schema,
+                    )
+                    self.output_dict[name] = {
+                        "tables": col_lineage.table_list,
+                        "columns": col_lineage.column_dict,
+                        "table_name": name,
+                    }
+                except Exception as e:
+                    print("{} is not processed because it countered {}".format(name, e))
+                    continue
+        # path or a list of SQL that at least one element contains
+        else:
+            self.sql_files_dict = SqlToDict(self.sql, self.schema_list).sql_files_dict
+            for name, sql in self.sql_files_dict.items():
+                try:
+                    if name not in self.finished_list:
+                        self._explain_sql(name=name, sql=sql)
+                    else:
+                        continue
+                except Exception as e:
+                    print("{} is not processed because it countered {}".format(name, e))
                     continue
-            except Exception as e:
-                print("{} is not processed because it countered {}".format(name, e))
-                continue
-        produce_json(output_dict=self.output_dict, engine=self.conn, search_schema=self.search_schema)
+        produce_json(
+            output_dict=self.output_dict,
+            engine=self.conn,
+            search_schema=self.search_schema,
+        )
         self._delete_view()
         self.conn.close()
 
     def _delete_view(self) -> None:
         """
         Delete all temporary tables in the new_view_list
         :return: None
@@ -91,38 +159,46 @@
                 """CREATE TABLE {}.{} AS {} WITH NO DATA;""".format(
                     self.schema, name, sql
                 )
             )
         cur.close()
         print(self.schema + "." + name + " created")
 
+    def _get_plan(self, sql: Optional[str] = "") -> dict:
+        """
+        Get the plan by providing the sql
+        :param sql: the sql for getting the plan
+        :return: the physical plan of the sql
+        """
+        cur = self.conn.cursor()
+        cur.execute("""SET search_path TO {};""".format(self.search_schema))
+        cur.execute(
+            """EXPLAIN (VERBOSE TRUE, FORMAT JSON, COSTS FALSE) {}""".format(sql)
+        )
+        log_plan = cur.fetchall()
+        cur.close()
+        while True:
+            if isinstance(log_plan, list) or isinstance(log_plan, tuple):
+                log_plan = log_plan[0]
+            elif isinstance(log_plan, dict):
+                log_plan = log_plan["Plan"]
+                break
+        return log_plan
+
     def _explain_sql(self, name: Optional[str] = "", sql: Optional[str] = "") -> None:
         """
         Main function for extracting the table name from the sql. It tries to explain the current file's sql by
         analyzing the logical plan. But if its dependency is missing, the current one is put onto a stack and checking
         on the dependency table, then pops the stack when the current one is done.
         :param name: name of the file
         :param sql: the sql from the file
         :return: updates file_list, sql_list, table_list, new_view_list
         """
         try:
-            print(name)
-            cur = self.conn.cursor()
-            cur.execute("""SET search_path TO {};""".format(self.search_schema))
-            cur.execute(
-                """EXPLAIN (VERBOSE TRUE, FORMAT JSON, COSTS FALSE) {}""".format(sql)
-            )
-            log_plan = cur.fetchall()
-            cur.close()
-            while True:
-                if isinstance(log_plan, list) or isinstance(log_plan, tuple):
-                    log_plan = log_plan[0]
-                elif isinstance(log_plan, dict):
-                    log_plan = log_plan["Plan"]
-                    break
+            print(name + " processing")
             if name in self.creation_list:
                 self._create_view(name=name, sql=sql)
                 self.new_view_list.append(self.schema + "." + name)
                 self.creation_list.pop(self.creation_list.index(name))
             else:
                 cur = self.conn.cursor()
                 cur.execute("""SET search_path TO {};""".format(self.search_schema))
@@ -133,17 +209,21 @@
                 )
                 table_result = cur.fetchone()
                 cur.close()
                 if not table_result:
                     self._create_view(name=name, sql=sql)
                     self.new_view_list.append(self.schema + "." + name)
             table_name = self.schema + "." + name
-            cols = find_column(table_name=table_name, engine=self.conn, search_schema=self.search_schema)
+            cols = find_column(
+                table_name=table_name,
+                engine=self.conn,
+                search_schema=self.search_schema,
+            )
             col_lineage = ColumnLineage(
-                plan=log_plan,
+                plan=self._get_plan(sql=sql),
                 sql=sql,
                 columns=cols,
                 conn=self.conn,
                 part_tables=self.part_tables,
                 search_schema=self.search_schema,
             )
             self.output_dict[table_name] = {
@@ -162,17 +242,17 @@
         except psycopg2.ProgrammingError as e:
             # does not exist error code
             if e.pgcode == "42P01":
                 error_msg = e.pgerror
                 no_find_idx = error_msg.find("does not exist")
                 relation_idx = error_msg.find("relation")
                 schema_table = error_msg[relation_idx:no_find_idx]
-                table_name = schema_table.split(" ")[-2].split(".")[-1].strip('\"')
+                table_name = schema_table.split(" ")[-2].split(".")[-1].strip('"')
                 self.s.push(name)
-                #print(table_name, self.sql_files_dict)
+                # print(table_name, self.sql_files_dict)
                 if table_name in self.sql_files_dict.keys():
                     if self.schema + "." + table_name in self.new_view_list:
                         print(
                             "{}.{} is already created, but the created schema is different from the queried schema for {} in {}.sql".format(
                                 self.schema, table_name, table_name, name
                             )
                         )
```

### Comparing `lineagex-0.0.3a2/lineagex/SqlToDict.py` & `lineagex-0.0.4/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/lineagex/stack.py` & `lineagex-0.0.4/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/lineagex/utils.py` & `lineagex-0.0.4/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/lineagex/vendor.js` & `lineagex-0.0.4/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/README.md` & `lineagex-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.3a2/PKG-INFO` & `lineagex-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.3a2
+Version: 0.0.4
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: sqlglot (>=12.3.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 # LineageX
 
 A Column Level Lineage Graph for Postgres
```

