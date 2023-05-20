# Comparing `tmp/lightweight_charts-1.0.5.tar.gz` & `tmp/lightweight_charts-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.5.tar", last modified: Thu May 18 22:31:05 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.6.tar", last modified: Sat May 20 00:45:54 2023, max compression
```

## Comparing `lightweight_charts-1.0.5.tar` & `lightweight_charts-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.310106 lightweight_charts-1.0.5/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.5/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-18 22:31:05.309531 lightweight_charts-1.0.5/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     5569 2023-05-16 14:49:40.000000 lightweight_charts-1.0.5/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.305142 lightweight_charts-1.0.5/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.5/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     9887 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    30005 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.5/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2535 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/pywebview.py
--rw-r--r--   0 louis      (501) staff       (20)     2133 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     1940 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/widgets.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.308864 lightweight_charts-1.0.5/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-18 22:31:05.310319 lightweight_charts-1.0.5/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-18 22:01:10.000000 lightweight_charts-1.0.5/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.438778 lightweight_charts-1.0.6/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.6/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     6069 2023-05-20 00:45:54.438517 lightweight_charts-1.0.6/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     5723 2023-05-20 00:24:46.000000 lightweight_charts-1.0.6/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.435255 lightweight_charts-1.0.6/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.6/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    10197 2023-05-19 22:53:50.000000 lightweight_charts-1.0.6/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    31274 2023-05-20 00:36:42.000000 lightweight_charts-1.0.6/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.6/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2546 2023-05-19 22:53:50.000000 lightweight_charts-1.0.6/lightweight_charts/pywebview.py
+-rw-r--r--   0 louis      (501) staff       (20)     2133 2023-05-18 22:28:08.000000 lightweight_charts-1.0.6/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     2347 2023-05-19 23:40:38.000000 lightweight_charts-1.0.6/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.437962 lightweight_charts-1.0.6/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     6069 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-20 00:45:54.438876 lightweight_charts-1.0.6/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-20 00:24:46.000000 lightweight_charts-1.0.6/setup.py
```

### Comparing `lightweight_charts-1.0.5/LICENSE` & `lightweight_charts-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.5/PKG-INFO` & `lightweight_charts-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight_charts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,29 +14,30 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-
+![cover](cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
 4. Support for PyQt and wxPython.
+5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
```

### Comparing `lightweight_charts-1.0.5/README.md` & `lightweight_charts-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-
+![cover](cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
 4. Support for PyQt and wxPython.
+5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
```

### Comparing `lightweight_charts-1.0.5/lightweight_charts/chart.py` & `lightweight_charts-1.0.6/lightweight_charts/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         :param series: labels: date/time, price
         """
         self._chart._go('_update_line_data', self.id, series)
 
 
 class Chart:
     def __init__(self, volume_enabled: bool = True, width: int = 800, height: int = 600, x: int = None, y: int = None,
-                 on_top: bool = False, debug: bool = False, sub: bool = False, inner_width=1, inner_height=1):
+                 on_top: bool = False, debug: bool = False, sub: bool = False,
+                 inner_width: float = 1.0, inner_height: float = 1.0):
         self.debug = debug
         self.volume_enabled = volume_enabled
         self.width = width
         self.height = height
         self.x = x
         self.y = y
         self.on_top = on_top
@@ -175,14 +176,20 @@
     def layout(self, background_color: str = None, text_color: str = None, font_size: int = None,
                font_family: str = None):
         """
         Global layout options for the chart.
         """
         self._go('layout', background_color, text_color, font_size, font_family)
 
+    def grid(self, vert_enabled: bool = True, horz_enabled: bool = True, color: str = 'rgba(29, 30, 38, 5)', style: LINE_TYPE = 'solid'):
+        """
+        Grid styling for the chart.
+        """
+        self._go('grid', vert_enabled, horz_enabled, color, style)
+
     def candle_style(self, up_color: str = 'rgba(39, 157, 130, 100)', down_color: str = 'rgba(200, 97, 100, 100)',
                      wick_enabled: bool = True, border_enabled: bool = True, border_up_color: str = '',
                      border_down_color: str = '', wick_up_color: str = '', wick_down_color: str = ''):
         """
         Candle styling for each of its parts.
         """
         self._go('candle_style', up_color, down_color, wick_enabled, border_enabled,
@@ -227,16 +234,16 @@
         """
         Subscribes the given function to a chart 'click' event.
         The event returns a dictionary containing the bar object at the time clicked.
         """
         self._go('subscribe_click', function)
 
     def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
-                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
-        c_id = self._go_return('create_sub_chart', volume_enabled, position, width, height, sync)
+                         width: float = 0.5, height: float = 0.5, sync: Union[bool, UUID] = False):
+        c_id = self._go_return('create_subchart', volume_enabled, position, width, height, sync)
         return SubChart(self, c_id)
 
 
 class SubChart(Chart):
     def __init__(self, parent, c_id):
         self._parent = parent._parent if isinstance(parent, SubChart) else parent
```

### Comparing `lightweight_charts-1.0.5/lightweight_charts/js.py` & `lightweight_charts-1.0.6/lightweight_charts/js.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             data['time'] = datetime.fromtimestamp(data['time'])
         else:
             data['time'] = datetime(data['time']['year'], data['time']['month'], data['time']['day'])
         click_func(data) if click_func else None
 
 
 class LWC:
-    def __init__(self, volume_enabled, inner_width=1, inner_height=1):
+    def __init__(self, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0):
         self.id = uuid4()
         self.js_queue = []
         self.loaded = False
 
         self._rand = IDGen()
         self._chart_var = 'chart'
 
@@ -293,15 +293,15 @@
 
         var = self._rand.generate()
         self.run_script(f"""
                let priceLine{var} = {{
                    price: {price},
                    color: '{color}',
                    lineWidth: {width},
-                   lineStyle: LightweightCharts.LineStyle.{style},
+                   lineStyle: LightweightCharts.LineStyle.{_line_type(style)},
                    axisLabelVisible: {'true' if axis_label_visible else 'false'},
                    title: '{text}',
                }};
                let line{var} = {{
                    line: {self._chart_var}.series.createPriceLine(priceLine{var}),
                    price: {price},
                }};
@@ -327,15 +327,15 @@
         :param mode: Chart price scale mode.
         :param title: Last price label text.
         :param right_padding: How many bars of empty space to the right of the last bar.
         """
         if self._stored('config', mode, title, right_padding):
             return None
 
-        self.run_script(f'{self._chart_var}.chart.timeScale().scrollToPosition({right_padding}, false)') if right_padding else None
+        self.run_script(f'{self._chart_var}.chart.timeScale().scrollToPosition({right_padding}, false)') if right_padding is not None else None
         self.run_script(f'{self._chart_var}.series.applyOptions({{title: "{title}"}})') if title else None
         self.run_script(
             f"{self._chart_var}.chart.priceScale().applyOptions({{mode: LightweightCharts.PriceScaleMode.{_price_scale_mode(mode)}}})") if mode else None
 
     def time_scale(self, visible: bool = True, time_visible: bool = True, seconds_visible: bool = False):
         """
         Options for the time scale of the chart.
@@ -374,30 +374,55 @@
             layout: {{
                 {f'backgroundColor: "{background_color}",' if background_color else ''}
                 {f'textColor: "{text_color}",' if text_color else ''}
                 {f'fontSize: {font_size},' if font_size else ''}
                 {f'fontFamily: "{font_family}",' if font_family else ''}
             }}}})""")
 
+    def grid(self, vert_enabled: bool = True, horz_enabled: bool = True, color: str = 'rgba(29, 30, 38, 5)', style: LINE_TYPE = 'solid'):
+        """
+        Grid styling for the chart.
+        """
+        if self._stored('grid', vert_enabled, horz_enabled, color, style):
+            return None
+
+        self.run_script(f"""
+        {self._chart_var}.chart.applyOptions({{
+        grid: {{
+            {f'''vertLines: {{
+                {f'visible: {_js_bool(vert_enabled)},' if vert_enabled is not None else ''}
+                {f'color: "{color}",' if color else ''}
+                {f'style: LightweightCharts.LineStyle.{_line_type(style)},' if style else ''}
+            }},''' if vert_enabled is not None or color or style else ''}
+            
+            {f'''horzLines: {{
+                {f'visible: {_js_bool(horz_enabled)},' if horz_enabled is not None else ''}
+                {f'color: "{color}",' if color else ''}
+                {f'style: LightweightCharts.LineStyle.{_line_type(style)},' if style else ''}
+            }},''' if horz_enabled is not None or color or style else ''}
+        }}
+        }})
+        """)
+
     def candle_style(self, up_color: str = 'rgba(39, 157, 130, 100)', down_color: str = 'rgba(200, 97, 100, 100)',
                      wick_enabled: bool = True, border_enabled: bool = True, border_up_color: str = '',
                      border_down_color: str = '', wick_up_color: str = '', wick_down_color: str = ''):
         """
         Candle styling for each of its parts.
         """
         if self._stored('candle_style', up_color, down_color, wick_enabled, border_enabled,
                         border_up_color, border_down_color, wick_up_color, wick_down_color):
             return None
 
         self.run_script(f"""
             {self._chart_var}.series.applyOptions({{
                 {f'upColor: "{up_color}",' if up_color else ''}
                 {f'downColor: "{down_color}",' if down_color else ''}
-                {f'wickVisible: {_js_bool(wick_enabled)},' if wick_enabled else ''}
-                {f'borderVisible: {_js_bool(border_enabled)},' if border_enabled else ''}
+                {f'wickVisible: {_js_bool(wick_enabled)},' if wick_enabled is not None else ''}
+                {f'borderVisible: {_js_bool(border_enabled)},' if border_enabled is not None else ''}
                 {f'borderUpColor: "{border_up_color}",' if border_up_color else ''}
                 {f'borderDownColor: "{border_down_color}",' if border_down_color else ''}
                 {f'wickUpColor: "{wick_up_color}",' if wick_up_color else ''}
                 {f'wickDownColor: "{wick_down_color}",' if wick_down_color else ''}
             }})""")
 
     def volume_config(self, scale_margin_top: float = 0.8, scale_margin_bottom: float = 0.0,
@@ -520,34 +545,34 @@
                     low: prices{var}.low,
                     close: prices{var}.close,
                     id: '{self.id}'
                     }}
                 {self._js_api_code}(data{var})
                 }})''')
 
-    def create_sub_chart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
-                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
+    def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: Union[bool, UUID] = False):
         subchart = SubChart(self, volume_enabled, position, width, height, sync)
         self._subcharts[subchart.id] = subchart
         return subchart
 
-    def _pywebview_sub_chart(self, volume_enabled, position, width, height, sync, parent=None):
+    def _pywebview_subchart(self, volume_enabled, position, width, height, sync, parent=None):
         subchart = PyWebViewSubChart(self if not parent else parent, volume_enabled, position, width, height, sync)
         self._subcharts[subchart.id] = subchart
         return subchart.id
 
 
 class SubChart(LWC):
     def __init__(self, parent, volume_enabled, position, width, height, sync):
         super().__init__(volume_enabled, width, height)
         self._chart = parent._chart if isinstance(parent, SubChart) else parent
         self._parent = parent
 
         self._rand = self._chart._rand
-        self._chart_var = self._rand.generate()
+        self._chart_var = f'window.{self._rand.generate()}'
         self._js_api = self._chart._js_api
         self._js_api_code = self._chart._js_api_code
 
         self.position = position
 
         self._create_panel(sync)
 
@@ -570,23 +595,23 @@
             sync_parent_var = self._chart._subcharts[sync]._chart_var if isinstance(sync, UUID) else self._parent._chart_var
             sub_sync = f'''
                 {sync_parent_var}.chart.timeScale().subscribeVisibleLogicalRangeChange((timeRange) => {{
                     {self._chart_var}.chart.timeScale().setVisibleLogicalRange(timeRange)
                 }});
             '''
         self.run_script(f'''
-            var {self._chart_var}div = document.createElement('div')
+            {self._chart_var}div = document.createElement('div')
             //{self._chart_var}div.style.position = 'relative'
             {self._chart_var}div.style.float = "{self.position}"
             
             //chartsDiv.style.display = 'inline-block'
             chartsDiv.style.float = 'left'
             
-            var {self._chart_var} = {{}}
-            {self._chart_var}.scale= {{
+            {self._chart_var} = {{}}
+            {self._chart_var}.scale = {{
                 width: {self.inner_width},
                 height: {self.inner_height}
             }}
             {self._chart_var}.chart = makeChart(window.innerWidth*{self._chart_var}.scale.width,
                                         window.innerHeight*{self._chart_var}.scale.height, {self._chart_var}div)
             {self._chart_var}.series = makeCandlestickSeries({self._chart_var}.chart)
             {self._chart_var}.volumeSeries = makeVolumeSeries({self._chart_var}.chart)
@@ -612,17 +637,17 @@
                 }}
             }});
             {sub_sync}
             ''')
 
 
 class PyWebViewSubChart(SubChart):
-    def create_sub_chart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
-                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
-        return self._chart._pywebview_sub_chart(volume_enabled, position, width, height, sync, parent=self)
+    def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: Union[bool, UUID] = False):
+        return self._chart._pywebview_subchart(volume_enabled, position, width, height, sync, parent=self)
 
     def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
         return super().create_line(color, width).id
 
 
 SCRIPT = """
 document.body.style.backgroundColor = '#000000'
@@ -694,22 +719,22 @@
     priceScaleId: '',
 });
 }
 
 const chartsDiv = document.createElement('div')
 
 var chart = {}
-
-chart.chart = makeChart(window.innerWidth, window.innerHeight, chartsDiv)
-chart.series = makeCandlestickSeries(chart.chart)
-chart.volumeSeries = makeVolumeSeries(chart.chart)
 chart.scale = {
     width: __INNER_WIDTH__,
     height: __INNER_HEIGHT__
 }
+chart.chart = makeChart(window.innerWidth*chart.scale.width, window.innerHeight*chart.scale.height, chartsDiv)
+chart.series = makeCandlestickSeries(chart.chart)
+chart.volumeSeries = makeVolumeSeries(chart.chart)
+
             
 document.body.appendChild(chartsDiv)
 
 chart.legend = document.createElement('div')
 chart.legend.style.position = 'absolute'
 chart.legend.style.zIndex = 1000
 chart.legend.style.width = `${(chart.scale.width*100)-8}vw`
```

### Comparing `lightweight_charts-1.0.5/lightweight_charts/pkg.py` & `lightweight_charts-1.0.6/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.5/lightweight_charts/pywebview.py` & `lightweight_charts-1.0.6/lightweight_charts/pywebview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Union
 from uuid import UUID
 import webview
 from multiprocessing import Queue
 
 from lightweight_charts.js import LWC
 
 _q = Queue()
@@ -48,17 +48,17 @@
     def exit(self):
         self.webview.destroy()
         del self
 
     def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
         return super().create_line(color, width).id
 
-    def create_sub_chart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
-                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
-        return super()._pywebview_sub_chart(volume_enabled, position, width, height, sync)
+    def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: Union[bool, UUID] = False):
+        return super()._pywebview_subchart(volume_enabled, position, width, height, sync)
 
 
 def _loop(chart, controller=None):
     wv = Webview(chart) if not controller else controller
     chart._result_q.put(wv.id)
     while 1:
         obj = wv
```

### Comparing `lightweight_charts-1.0.5/lightweight_charts/util.py` & `lightweight_charts-1.0.6/lightweight_charts/util.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.5/lightweight_charts/widgets.py` & `lightweight_charts-1.0.6/lightweight_charts/widgets.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,47 +9,52 @@
 except ImportError:
     pass
 
 from lightweight_charts.js import LWC
 
 
 class WxChart(LWC):
-    def __init__(self, parent, volume_enabled=True):
+    def __init__(self, parent, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0):
         try:
             self.webview: wx.html2.WebView = wx.html2.WebView.New(parent)
         except NameError:
             raise ModuleNotFoundError('wx.html2 was not found, and must be installed to use WxChart.')
 
-        super().__init__(volume_enabled)
+        super().__init__(volume_enabled, inner_width=inner_width, inner_height=inner_height)
 
         self.webview.AddScriptMessageHandler('wx_msg')
         self._js_api_code = 'window.wx_msg.postMessage'
         self.webview.Bind(wx.html2.EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED, lambda e: self._js_api.onClick(eval(e.GetString())))
 
         self.webview.Bind(wx.html2.EVT_WEBVIEW_LOADED, self._on_js_load)
         self.webview.SetPage(self._html, '')
 
     def run_script(self, script): self.webview.RunScript(script)
 
     def _on_js_load(self, e):
         self.loaded = True
         for func, args, kwargs in self.js_queue:
-            getattr(super(), func)(*args, **kwargs)
+            if 'SUB' in func:
+                c_id = args[0]
+                args = args[1:]
+                getattr(self._subcharts[c_id], func.replace('SUB', ''))(*args)
+            else:
+                getattr(self, func)(*args)
 
     def get_webview(self): return self.webview
 
 
 class QtChart(LWC):
-    def __init__(self, widget=None, volume_enabled=True):
+    def __init__(self, widget=None, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0):
         try:
             self.webview = QWebEngineView(widget)
         except NameError:
             raise ModuleNotFoundError('QWebEngineView was not found, and must be installed to use QtChart.')
 
-        super().__init__(volume_enabled)
+        super().__init__(volume_enabled, inner_width=inner_width, inner_height=inner_height)
 
         self.webview.loadFinished.connect(self._on_js_load)
         self.webview.page().setHtml(self._html)
 
     def run_script(self, script): self.webview.page().runJavaScript(script)
 
     def _on_js_load(self):
```

### Comparing `lightweight_charts-1.0.5/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.6/lightweight_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,29 +14,30 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-
+![cover](cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
 4. Support for PyQt and wxPython.
+5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
```

### Comparing `lightweight_charts-1.0.5/setup.py` & `lightweight_charts-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

