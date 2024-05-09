# Comparing `tmp/ecoviewer-0.0.9.tar.gz` & `tmp/ecoviewer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoviewer-0.0.9.tar", last modified: Thu Apr 11 16:53:04 2024, max compression
+gzip compressed data, was "ecoviewer-0.1.0.tar", last modified: Thu May  9 21:19:50 2024, max compression
```

## Comparing `ecoviewer-0.0.9.tar` & `ecoviewer-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.000462 ecoviewer-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/config/configutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/display/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/displayutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/graphutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-11 16:53:04.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/ecoviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/ecoviewer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/config/configutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/src/ecoviewer/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/displayutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23365 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/graphutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/src/ecoviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/top_level.txt
```

### Comparing `ecoviewer-0.0.9/LICENSE` & `ecoviewer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.9/PKG-INFO` & `ecoviewer-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecoviewer-0.0.9/setup.cfg` & `ecoviewer-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoviewer
-version = 0.0.9
+version = 0.1.0
 authors = ["Ecotope"]
 description = Contains functions for use in HVAC Dash applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoviewer-0.0.9/src/ecoviewer/config/configutils.py` & `ecoviewer-0.1.0/src/ecoviewer/config/configutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from plotly.subplots import make_subplots
 import plotly.colors
 import mysql.connector
 import math
 import numpy as np
 from datetime import datetime
 
-def get_user_permissions_from_db(user_email : str, sql_dash_config):
+def get_user_permissions_from_db(user_email : str, sql_dash_config, exclude_csv_only_fields : bool = True):
     email_groups = [user_email, user_email.split('@')[-1]]
     
     cnx = mysql.connector.connect(**sql_dash_config)
     cursor = cnx.cursor() 
 
     site_query = """
         SELECT *
@@ -35,43 +35,47 @@
 
         cursor.execute("SELECT * FROM graph_display")
         result = cursor.fetchall()
         column_names = [desc[0] for desc in cursor.description]
         graph_df = pd.DataFrame(result, columns=column_names)
         graph_df = graph_df.set_index('graph_id')
 
-        field_query = site_query = """
+        field_query = """
             SELECT * FROM field
             WHERE site_name IN ({})
         """.format(', '.join(['%s'] * len(table_names)))
+        if exclude_csv_only_fields:
+            field_query = f"{field_query} AND graph_id IS NOT NULL" 
+        
         cursor.execute(field_query, table_names)
         result = cursor.fetchall()
         column_names = [desc[0] for desc in cursor.description]
         field_df = pd.DataFrame(result, columns=column_names)
+        print("field df length", len(field_df.index))
 
     cursor.close()
     cnx.close()
 
     display_drop_down = []
     for name in table_names:
         display_drop_down.append({'label': site_df.loc[name, "pretty_name"], 'value' : name})
     return site_df, graph_df, field_df, display_drop_down
 
-def get_organized_mapping(df_columns, graph_df : pd.DataFrame, field_df : pd.DataFrame, selected_table : str):
+def get_organized_mapping(df_columns, graph_df : pd.DataFrame, field_df : pd.DataFrame, selected_table : str, all_fields : bool = False):
     returnDict = {}
     site_fields = field_df[field_df['site_name'] == selected_table]
     site_fields = site_fields.set_index('field_name')
     for index, row in graph_df.iterrows():
         # Extract the y-axis units
         y1_units = row["y_1_title"] if row["y_1_title"] != None else ""
         y2_units = row["y_2_title"] if row["y_2_title"] != None else ""
         y1_fields = []
         y2_fields = []
         for field_name, field_row in site_fields[site_fields['graph_id'] == index].iterrows():
-            if field_name in df_columns:
+            if all_fields or field_name in df_columns:
                 column_details = {}
                 column_details["readable_name"] = field_row['pretty_name']
                 column_details["column_name"] = field_name
                 column_details["description"] = field_row["description"]
                 # if not math.isnan(field_row["lower_bound"]):
                 if field_row["lower_bound"] is not None and not math.isnan(field_row["lower_bound"]):
                     column_details["lower_bound"] = field_row["lower_bound"]
@@ -176,7 +180,32 @@
 
     cursor.execute(insert_query)
     
     # Commit the changes
     cnx.commit()
     cursor.close()
     cnx.close()
+
+def parse_checklists_from_div(div_children : list) -> list:
+    ret_list = []
+    for element in div_children:
+        if 'type' in element:
+            if element['type'] == 'Checklist':
+                ret_list = ret_list + element['props']['value']
+            elif element['type'] == 'Div':
+                ret_list = ret_list + parse_checklists_from_div(element['props']['children'])
+    return ret_list
+
+def get_df_from_query(query : str, cursor) -> pd.DataFrame:
+    cursor.execute(query)
+    result = cursor.fetchall()
+    column_names = [desc[0] for desc in cursor.description]
+    df = pd.DataFrame(result, columns=column_names)
+
+    # round float columns to 3 decimal places
+    df = round_df_to_3_decimal(df)
+    return df
+
+def round_df_to_3_decimal(df : pd.DataFrame) -> pd.DataFrame:
+    float_cols = df.select_dtypes(include=['float64'])
+    df[float_cols.columns] = float_cols.round(3)
+    return df
```

### Comparing `ecoviewer-0.0.9/src/ecoviewer/display/graphutils.py` & `ecoviewer-0.1.0/src/ecoviewer/display/graphutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from dash import dcc, html
 from plotly.subplots import make_subplots
 import plotly.colors
 import numpy as np
+import math
+from ecoviewer.config import get_organized_mapping, round_df_to_3_decimal
+from datetime import datetime
 
 state_colors = {
     "loadUp" : "green",
     "shed" : "blue"
 }
 
 def get_state_colors():
@@ -22,43 +25,15 @@
         dff = df.loc[start_date:end_date, value]
     else:
         dff = df[value]
     fig = px.line(dff, x=dff.index, y=dff.columns)
     fig.update_layout(xaxis_title = 'Timestamp', yaxis_title = unit)
     return fig
 
-def create_data_dictionary(organized_mapping):
-    returnStr = [html.H2('Variable Definitions', style={'font-size': '24px'})]
-    for key, value in organized_mapping.items():
-        returnStr.append(html.H3(value["title"], style={'font-size': '18px'}))
-        y1_fields = value["y1_fields"]
-        y2_fields = value["y2_fields"]
-        for field_dict in y1_fields:
-            name = field_dict["readable_name"]
-            descr = field_dict["description"]
-            if descr is None:
-                descr = ''
-            returnStr.append(html.P([
-                html.Span(''+name+'',style={"font-weight": "bold"}),
-                html.Span(' : '+descr,style={"font-weight": "normal"}),
-                ],
-                style={'font-size': '14px', 'text-indent': '40px'}
-            ))
-        for field_dict in y2_fields:
-            name = field_dict["readable_name"]
-            descr = field_dict["description"]
-            returnStr.append(html.P([
-                html.Span(''+name+'',style={"font-weight": "bold"}),
-                html.Span(' : '+descr,style={"font-weight": "normal"}),
-                ],
-                style={'font-size': '14px', 'text-indent': '40px'}
-            ))
-    return returnStr
-
-def create_date_note(site_name, cursor):
+def create_date_note(site_name, cursor, pretty_name):
     """
     returns [date_note, first_date, last_date]
     """
     query = f"SELECT time_pt FROM {site_name} ORDER BY time_pt ASC LIMIT 1"
     cursor.execute(query)
     result = cursor.fetchall()
     if len(result) == 0 or len(result[0]) == 0:
@@ -67,15 +42,15 @@
 
     query = f"SELECT time_pt FROM {site_name} ORDER BY time_pt DESC LIMIT 1"
     cursor.execute(query)
     result = cursor.fetchall()
     last_date = result[0][0]
 
     return [
-            f"Possible range for {site_name}:",
+            f"Possible range for {pretty_name}:",
             html.Br(),
             f"{first_date.strftime('%m/%d/%y')} - {last_date.strftime('%m/%d/%y')}"
     ]
 
 def clean_df(df : pd.DataFrame, organized_mapping):
     for key, value in organized_mapping.items():
         fields = value["y1_fields"] + value["y2_fields"]
@@ -85,28 +60,28 @@
             column_name = field_dict["column_name"]
             if 'lower_bound' in field_dict:
                 df[column_name] = np.where(df[column_name] < field_dict["lower_bound"], np.nan, df[column_name])
 
             if 'upper_bound' in field_dict:
                 df[column_name] = np.where(df[column_name] > field_dict["upper_bound"], np.nan, df[column_name])
 
-def create_conjoined_graphs(df : pd.DataFrame, organized_mapping, add_state_shading = False):
+def create_conjoined_graphs(df : pd.DataFrame, organized_mapping, add_state_shading : bool = False):
     clean_df(df, organized_mapping)
     graph_components = []
     # Load the JSON data from the file
     subplot_titles = []
     for key, value in organized_mapping.items():
         # Extract the category (e.g., Temperature or Power)
         category = value["title"]
         subplot_titles.append(f"<b>{category}</b>")
     # Create a new figure for the category
     fig = make_subplots(rows = len(organized_mapping.items()), cols = 1, 
                 specs=[[{"secondary_y": True}]]*len(organized_mapping.items()),
                 shared_xaxes=True,
-                vertical_spacing = 0.05,
+                vertical_spacing = 0.1/max(1, len(organized_mapping.items())),
                 subplot_titles = subplot_titles)
     
     row = 0
     cop_columns = []
 
     for key, value in organized_mapping.items():
         row += 1
@@ -123,23 +98,53 @@
 
         # Iterate over the values and add traces to the figure
         for field_dict in y1_fields:
             name = field_dict["readable_name"]
             column_name = field_dict["column_name"]
             y_axis = 'y1'
             secondary_y = False
-            fig.add_trace(go.Scatter(x=df.index, y=df[column_name], name=name, yaxis=y_axis, mode='lines'), row=row, col = 1, secondary_y=secondary_y)
+            fig.add_trace(
+                go.Scatter(
+                    x=df.index, 
+                    y=df[column_name], 
+                    name=name, 
+                    yaxis=y_axis, 
+                    mode='lines',
+                    hovertemplate="<br>".join([
+                        f"{name}",
+                        "time_pt=%{x}",
+                        "value=%{y}",
+                    ])
+                ), 
+                row=row, 
+                col = 1, 
+                secondary_y=secondary_y)
         for field_dict in y2_fields:
             name = field_dict["readable_name"]
             column_name = field_dict["column_name"]
             if 'COP' in column_name:
                 cop_columns.append(column_name)
             y_axis = 'y2'
             secondary_y = True
-            fig.add_trace(go.Scatter(x=df.index, y=df[column_name], name=name, yaxis=y_axis, mode='lines'), row=row, col = 1, secondary_y=secondary_y)
+            fig.add_trace(
+                go.Scatter(
+                    x=df.index, 
+                    y=df[column_name], 
+                    name=name, 
+                    yaxis=y_axis, 
+                    mode='lines',
+                    hovertemplate="<br>".join([
+                        f"{name}",
+                        "time_pt=%{x}",
+                        "value=%{y}",
+                    ])
+                ), 
+                row=row, 
+                col = 1, 
+                secondary_y=secondary_y)
 
         fig.update_yaxes(title_text="<b>"+y1_units+"</b>", row=row, col = 1, secondary_y = False)
         fig.update_yaxes(title_text="<b>"+y2_units+"</b>", row=row, col = 1, secondary_y = True)
 
     fig.update_xaxes(title_text="<b>Time</b>", row = row, col = 1)
     fig.update_layout(
         width=1500,
@@ -188,76 +193,158 @@
 
     figure = go.Figure(fig)
 
     # Add the figure to the array of graph objects
     graph_components.append(dcc.Graph(figure=figure))
     return graph_components
 
-def _create_summary_bar_graph(df):
+def _format_x_axis_date_str(dt_1 : datetime, dt_2 : datetime = None) -> str:
+    months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+    
+    # Extract date components
+    day_1 = dt_1.day
+    month_1 = months[dt_1.month - 1]
+    year_1 = dt_1.year
+
+    if dt_2 is None:
+        return f"{month_1} {day_1}, {year_1}"
+    
+    day_2 = dt_2.day
+    month_2 = months[dt_2.month - 1]
+    year_2 = dt_2.year
+    
+    # Check if the two dates are in the same year
+    if year_1 == year_2:
+        # Check if the two dates are in the same month
+        if month_1 == month_2:
+            return f"{month_1} {day_1} - {day_2}, {year_1}"
+        else:
+            return f"{month_1} {day_1} - {month_2} {day_2}, {year_1}"
+    else:
+        return f"{month_1} {day_1}, {year_1} - {month_2} {day_2}, {year_2}"
+
+def _create_summary_bar_graph(og_df : pd.DataFrame):
     # Filter columns with the prefix "PowerIn_" and exclude "PowerIn_Total"
-    # powerin_columns = [col for col in df.columns if col.startswith('PowerIn_') and col != 'PowerIn_Total' and df[col].dtype == "float64"]
-    powerin_columns = [col for col in df.columns if col.startswith('PowerIn_') and 'PowerIn_Total' not in col and df[col].dtype == "float64"]
-    energy_dataframe = df[powerin_columns].copy()
+    powerin_columns = [col for col in og_df.columns if col.startswith('PowerIn_') and 'PowerIn_Total' not in col and og_df[col].dtype == "float64"]
+    cop_columns = [col for col in og_df.columns if 'COP' in col]
+    df = og_df[powerin_columns+cop_columns].copy()
+
+    # compress to weeks if more than 3 weeks selected
+    compress_to_weeks = False
+    formatting_time_delta = min(4, math.floor(24/(len(cop_columns) +1))) # TODO error if there are more than 23 cop columns
+    if df.index[-1] - df.index[0] >= pd.Timedelta(weeks=3):
+        compress_to_weeks = True
+        # calculate weekly COPs
+        sum_df = df.copy()
+        sum_df['power_sum'] = sum_df[powerin_columns].sum(axis=1)
+        for cop_column in cop_columns:
+            sum_df[f'heat_out_{cop_column}'] = sum_df['power_sum'] * sum_df[cop_column]
+        sum_df = sum_df.resample('W').sum()
+        df = df.resample('W').mean()
+        for cop_column in cop_columns:
+            df[cop_column] = sum_df[f'heat_out_{cop_column}'] / sum_df['power_sum']
+        df = round_df_to_3_decimal(df)
+
+        formatting_time_delta = formatting_time_delta * 7
+
+    # x_axis_ticktext = []
+    x_axis_tick_val = []
+    x_axis_tick_text = []
+    x_val = df.index[0]
+    while x_val <= df.index[-1]:
+        x_axis_tick_val.append(x_val)# + pd.Timedelta(hours=(formatting_time_delta * math.floor(len(cop_column)/2))))
+        if compress_to_weeks:
+            first_date = x_val - pd.Timedelta(days=6)
+            last_date = x_val
+            if first_date < og_df.index[0]:
+                first_date = og_df.index[0]
+            if x_val > og_df.index[-1]:
+                last_date = og_df.index[-1]
+            x_axis_tick_text.append(_format_x_axis_date_str(first_date, last_date))
+            x_val += pd.Timedelta(weeks=1)
+        else:
+            x_axis_tick_text.append(_format_x_axis_date_str(x_val))
+            x_val += pd.Timedelta(days=1)
 
+    energy_dataframe = df[powerin_columns].copy()
     # Multiply all values in the specified columns by 24
     energy_dataframe[powerin_columns] = energy_dataframe[powerin_columns].apply(lambda x: x * 24)
 
     # TODO error for no power columns
 
 
     # Create a stacked bar graph using Plotly Express
     stacked_fig = px.bar(energy_dataframe, x=energy_dataframe.index, y=powerin_columns, title='Energy and COP',
                 labels={'index': 'Data Point'}, height=400)
     
     num_data_points = len(df)
-    x_shift = pd.Timedelta(hours=4)  # Adjust this value to control the horizontal spacing between the bars
+    x_shift = pd.Timedelta(hours=formatting_time_delta)  # Adjust this value to control the horizontal spacing between the bars
     x_positions_shifted = [x + x_shift for x in df.index]
     # create fake bar for spacing
     stacked_fig.add_trace(go.Bar(x=x_positions_shifted, y=[0]*num_data_points, showlegend=False))
     stacked_fig.update_layout(
         # width=1300,
         yaxis1=dict(
-            title='kWh',
+            title='Avg. Daily kWh' if compress_to_weeks else 'kWh',
         ),
         xaxis=dict(
-            title='Day',
+            title='Week' if compress_to_weeks else 'Day',
+            tickmode = 'array',
+            tickvals = x_axis_tick_val,
+            ticktext = x_axis_tick_text  
         ),
         margin=dict(l=10, r=10),
         legend=dict(x=1.1)
     )
 
     # Add the additional columns as separate bars next to the stacks
-    cop_columns = [col for col in df.columns if 'COP' in col]
     if len(cop_columns) > 0:
         for col in cop_columns:
             x_positions_shifted = [x + x_shift for x in df.index]
-            stacked_fig.add_trace(go.Bar(x=x_positions_shifted, y=df[col], name=col, yaxis = 'y2'))
-            x_shift += pd.Timedelta(hours=4)
+            stacked_fig.add_trace(go.Bar(
+                x=x_positions_shifted, 
+                y=df[col], 
+                name=col, 
+                yaxis = 'y2',
+                customdata=np.transpose([x_axis_tick_text, [col]*len(x_axis_tick_text)]),
+                hovertemplate="<br>".join([
+                    "variable=%{customdata[1]}",
+                    "time_pt=%{customdata[0]}",
+                    "value=%{y}",
+                ])
+                ))
+            x_shift += pd.Timedelta(hours=formatting_time_delta)
         # create fake bar for spacing
         stacked_fig.add_trace(go.Bar(x=df.index, y=[0]*num_data_points, showlegend=False, yaxis = 'y2'))
         # Create a secondary y-axis
         stacked_fig.update_layout(
             yaxis2=dict(
                 title='COP',
                 overlaying='y',
                 side='right'
             ),
         )
 
     return dcc.Graph(figure=stacked_fig)
 
-def _create_summary_Hourly_graph(df, hourly_df):
+def _create_summary_Hourly_graph(df : pd.DataFrame, hourly_df : pd.DataFrame):
     powerin_columns = [col for col in df.columns if col.startswith('PowerIn_') and df[col].dtype == "float64"]
 
     nls_df = hourly_df[hourly_df['load_shift_day'] == 0]
     ls_df = hourly_df[hourly_df['load_shift_day'] == 1]
 
     ls_df = ls_df.groupby('hr').mean(numeric_only = True)
+    ls_df = round_df_to_3_decimal(ls_df)
+
     nls_df = nls_df.groupby('hr').mean(numeric_only = True)
+    nls_df = round_df_to_3_decimal(nls_df)
+
     power_df = hourly_df.groupby('hr').mean(numeric_only = True)
+    power_df = round_df_to_3_decimal(power_df)
+
     power_fig = px.line(title = "Average Daily Power")
     
     for column_name in powerin_columns:
         if column_name in power_df.columns:
             trace = go.Scatter(x=power_df.index, y=power_df[column_name], name=f"{column_name}", mode='lines')
             power_fig.add_trace(trace)
             trace = go.Scatter(x=ls_df.index, y=ls_df[column_name], name=f"Load Shift Day {column_name}", mode='lines')
@@ -330,34 +417,39 @@
         if site_df_row["summary_pie_chart"]:
             graph_components.append(_create_summary_pie_graph(group_df))
         if site_df_row["summary_gpdpp_histogram"]:
             graph_components.append(_create_summary_gpdpp_histogram(group_df, site_df_row))
 
     return graph_components
 
-def create_hourly_shapes(df, organized_mapping):
-
+def create_hourly_shapes(df : pd.DataFrame, graph_df : pd.DataFrame, field_df : pd.DataFrame, selected_table : str):
+    hourly_only_field_df = field_df
+    if 'hourly_shapes_display' in field_df.columns:
+        hourly_only_field_df = field_df[field_df['hourly_shapes_display'] == True]
+    organized_mapping = get_organized_mapping(df.columns, graph_df, hourly_only_field_df, selected_table)
     graph_components = []
     weekday_df = df[df['weekday'] == True]
     weekend_df = df[df['weekday'] == False]
     weekday_df = weekday_df.groupby('hr').mean(numeric_only = True)
+    weekday_df = round_df_to_3_decimal(weekday_df)
     weekend_df = weekend_df.groupby('hr').mean(numeric_only = True)
+    weekend_df = round_df_to_3_decimal(weekend_df)
     subplot_titles = []
     for key, value in organized_mapping.items():
         # Extract the category (e.g., Temperature or Power)
         category = value["title"]
         subplot_titles.append(f"<b>{category} weekday</b>")
         subplot_titles.append(f"<b>{category} weekend</b>")
 
     
     # Create a new figure for the category
     fig = make_subplots(rows = len(organized_mapping.items())*2, cols = 1, 
                 specs=[[{"secondary_y": True}]]*len(organized_mapping.items())*2,
                 shared_xaxes=True,
-                vertical_spacing = 0.025,
+                vertical_spacing = 0.1/max(1, len(organized_mapping.items())),
                 subplot_titles = subplot_titles)
     
     row = 1
     colors = plotly.colors.DEFAULT_PLOTLY_COLORS
     color_num = 0
 
     for key, value in organized_mapping.items():
@@ -376,31 +468,51 @@
         y_axis = 'y1'
         secondary_y = False
         for field_dict in y1_fields:
             name = field_dict["readable_name"]
             column_name = field_dict["column_name"]
             if column_name in weekday_df.columns:
                 weekday_trace = go.Scatter(x=weekday_df.index, y=weekday_df[column_name], name=name, legendgroup=name, yaxis=y_axis, mode='lines',
+                                            hovertemplate="<br>".join([
+                                                f"{name}",
+                                                "hour=%{x}",
+                                                "value=%{y}",
+                                            ]), 
                                             line=dict(color = colors[color_num]))
                 weekend_trace = go.Scatter(x=weekend_df.index, y=weekend_df[column_name], name=name, legendgroup=name, yaxis=y_axis, mode='lines', 
+                                            hovertemplate="<br>".join([
+                                                f"{name}",
+                                                "hour=%{x}",
+                                                "value=%{y}",
+                                            ]), 
                                             showlegend=False, line=dict(color = colors[color_num]))
                 fig.add_trace(weekday_trace, row=row, col = 1, secondary_y=secondary_y)
                 fig.add_trace(weekend_trace, row=row+1, col = 1, secondary_y=secondary_y)
                 color_num += 1
                 color_num = color_num % len(colors)
 
         y_axis = 'y2'
         secondary_y = True
         for field_dict in y2_fields:
             name = field_dict["readable_name"]
             column_name = field_dict["column_name"]
             if column_name in weekday_df.columns:
                 weekday_trace = go.Scatter(x=weekday_df.index, y=weekday_df[column_name], name=name, legendgroup=name, yaxis=y_axis, mode='lines',
+                                            hovertemplate="<br>".join([
+                                                f"{name}",
+                                                "hour=%{x}",
+                                                "value=%{y}",
+                                            ]),
                                             line=dict(color = colors[color_num]))
-                weekend_trace = go.Scatter(x=weekend_df.index, y=weekend_df[column_name], name=name, legendgroup=name, yaxis=y_axis, mode='lines', 
+                weekend_trace = go.Scatter(x=weekend_df.index, y=weekend_df[column_name], name=name, legendgroup=name, yaxis=y_axis, mode='lines',
+                                            hovertemplate="<br>".join([
+                                                f"{name}",
+                                                "hour=%{x}",
+                                                "value=%{y}",
+                                            ]), 
                                             showlegend=False, line=dict(color = colors[color_num]))
                 fig.add_trace(weekday_trace, row=row, col = 1, secondary_y=secondary_y)
                 fig.add_trace(weekend_trace, row=row+1, col = 1, secondary_y=secondary_y)
                 color_num += 1
                 color_num = color_num % len(colors)
 
         fig.update_yaxes(title_text="<b>"+y1_units+"</b>", row=row, col = 1, secondary_y = False)
```

### Comparing `ecoviewer-0.0.9/src/ecoviewer.egg-info/PKG-INFO` & `ecoviewer-0.1.0/src/ecoviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

