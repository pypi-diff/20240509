# Comparing `tmp/stimulsoft_dashboards-2024.2.4.tar.gz` & `tmp/stimulsoft_dashboards-2024.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimulsoft_dashboards-2024.2.4.tar", last modified: Thu Apr 18 09:32:54 2024, max compression
+gzip compressed data, was "stimulsoft_dashboards-2024.2.5.tar", last modified: Wed May  8 10:58:04 2024, max compression
```

## Comparing `stimulsoft_dashboards-2024.2.4.tar` & `stimulsoft_dashboards-2024.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/
--rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.4/LICENSE.md
--rw-rw-rw-   0        0        0     8477 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1217 2024-04-16 11:07:52.000000 stimulsoft_dashboards-2024.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.175079 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.177280 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/
--rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/StiDashboard.py
--rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.178107 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/
--rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/StiResourcesHelper.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.180113 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/
--rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/__init__.py
--rw-rw-rw-   0        0        0   703179 2024-04-18 06:24:26.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
--rw-rw-rw-   0        0        0   195252 2024-04-18 06:27:06.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
-drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.176229 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/
--rw-rw-rw-   0        0        0     8477 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/
+-rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0     8477 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2024-05-08 10:57:58.000000 stimulsoft_dashboards-2024.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.514111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.517111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/
+-rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/StiDashboard.py
+-rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.518111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/
+-rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/StiResourcesHelper.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.520111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/
+-rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/__init__.py
+-rw-rw-rw-   0        0        0   703489 2024-05-06 08:25:08.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
+-rw-rw-rw-   0        0        0   195363 2024-05-06 08:27:54.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
+drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.516111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/
+-rw-rw-rw-   0        0        0     8477 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/top_level.txt
```

### Comparing `stimulsoft_dashboards-2024.2.4/LICENSE.md` & `stimulsoft_dashboards-2024.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.4/PKG-INFO` & `stimulsoft_dashboards-2024.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft_dashboards
-Version: 2024.2.4
+Version: 2024.2.5
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.4/README.md` & `stimulsoft_dashboards-2024.2.5/README.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.4/setup.py` & `stimulsoft_dashboards-2024.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as file:
     readmeFile = file.read()
 
 setup(
     name = 'stimulsoft_dashboards',
-    version = '2024.2.4',
+    version = '2024.2.5',
     author = 'Stimulsoft',
     author_email = 'info@stimulsoft.com',
     description = 'Data visualization in Python applications.',
     long_description = readmeFile,
     long_description_content_type = 'text/markdown',
     url = 'https://www.stimulsoft.com/en/products/dashboards-python',
     license = 'https://www.stimulsoft.com/en/licensing/developers',
@@ -20,12 +20,12 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Office/Business',
         'Topic :: Software Development'
     ],
-    install_requires = ['stimulsoft-reports==2024.2.4'],
+    install_requires = ['stimulsoft-reports==2024.2.5'],
     packages = find_packages(include=['stimulsoft_dashboards', 'stimulsoft_dashboards.*']),
     package_data = {'stimulsoft_dashboards': ['**/scripts/*.js']},
     python_requires = '>=3.10'
 )
```

### Comparing `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/StiResourcesHelper.py` & `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/StiResourcesHelper.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js` & `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 /*
 Stimulsoft.Dashboards.JS
-Version: 2024.2.4
-Build date: 2024.04.18
+Version: 2024.2.5
+Build date: 2024.05.06
 License: https://www.stimulsoft.com/en/licensing/reports
 */
 ! function(t) {
     var e;
     "undefined" != typeof process && process.__nwjs || "object" != typeof exports || "undefined" == typeof module ? "function" == typeof define && define.amd ? define(["./stimulsoft.reports"], e => Object.assign(e, t(e.Stimulsoft))) : window.Stimulsoft ? window.Stimulsoft.Report && window.Stimulsoft.Report.StiReport ? Object.assign(window, t(window.Stimulsoft)) : window.Stimulsoft.dashboardsFactory = t : window.Stimulsoft = {
         dashboardsFactory: t
     } : module.exports = (e = require("./stimulsoft.reports"), Object.assign(e, t(e.Stimulsoft)))
 }(function(L) {
     var Z = L.StiOptions;
 
     function y(e, t) {
         for (var r in t) r in e ? y(e[r], t[r]) : e[r] = t[r];
         return e
     }
-    L && (L.__engineVersion && "2024.2.4" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.4", L.__engineVersion) : "2024.2.4" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.4", L.__reportsVersion));
+    L && (L.__engineVersion && "2024.2.5" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.5", L.__engineVersion) : "2024.2.5" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.5", L.__reportsVersion));
     var L = y(L || {}, {
             Dashboard: {
                 Components: {
                     Panel: {},
                     Button: {},
                     Cards: {},
                     Helpers: {},
@@ -157,17 +157,17 @@
         Re = L.Report.Components.StiDashboardViewMode,
         Ee = L.Report.Dashboard.IStiAltProperties,
         Oe = L.Report.Dashboard.IStiTitleElement,
         Ve = L.System.Drawing.Rectangle,
         ke = L.Report.Dashboard.StiDashboardContentAlignment,
         Ne = L.Report.IStiGlobalizationProvider;
     {
-        class Im extends Ie {
+        class Dm extends Ie {
             implements() {
-                return Im.ImplementsStiDashboard || (Im.ImplementsStiDashboard = super.implements().concat([Ae, ue, Ne, ...ge, ...oe, l])), Im.ImplementsStiDashboard
+                return Dm.ImplementsStiDashboard || (Dm.ImplementsStiDashboard = super.implements().concat([Ae, ue, Ne, ...ge, ...oe, l])), Dm.ImplementsStiDashboard
             }
             clone() {
                 var e;
                 let t = super.clone();
                 return t.dashboardWatermark = null == (e = this.dashboardWatermark) ? void 0 : e.clone(), t
             }
             meta() {
@@ -374,39 +374,39 @@
             get isMobileSurfacePresent() {
                 return !this.altSize.isEmpty
             }
             constructor(e = null) {
                 super(e), this.backColor = N.transparent, this.margins = new be(10, 10, 10, 10), this._style = o.Blue, this.customStyleName = "", this.dashboardWatermark = new he, this.refreshingEvent = new te, this._width2 = 1200, this._height2 = 600, this._altSize = De.empty, this._dashboardViewMode = Re.Desktop, this._contentAlignment = ke.StretchXY, this._altContentAlignment = ke.StretchXY, this._deviceWidth = 480, this.key = pe.generateKey(), this.width = 1200, this.height = 600
             }
         }
-        F.e.StiDashboard = Im
+        F.e.StiDashboard = Dm
     }
     let u = L.Base.Meta.StiMetaHelper,
         Le = L.System.Type,
         Be = L.Base.Meters.IStiLocalizedMeter,
         Pe = L.Base.Meters.IStiMeter,
         je = L.Base.StiJsonSaveMode,
         He = L.Base.StiJson;
     {
-        class mg {
+        class cg {
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
             is2(e) {
                 return this.is(e)
             }
             as(e) {
                 if (this.is(e)) return this;
                 return null
             }
             implements() {
-                return mg.ImplementsStiMeter || (mg.ImplementsStiMeter = [Pe, Be, l]), mg.ImplementsStiMeter
+                return cg.ImplementsStiMeter || (cg.ImplementsStiMeter = [Pe, Be, l]), cg.ImplementsStiMeter
             }
             clone(e = !0, t = !0) {
                 let r = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return r.key = pe.generateKey(), r
             }
             saveToString() {
                 return this.saveToJsonObject(je.Report).serialize()
@@ -441,27 +441,27 @@
                 let e = this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName();
                 return B.isNullOrWhiteSpace(this.expression) ? e : e + `-"{Expression}"`
             }
             constructor(e, t, r) {
                 this.expression = "", this.label = "", null == e && (e = pe.generateKey()), this.key = e, null != t && (this.expression = t), null != r && (this.label = r)
             }
         }
-        F.e.StiMeter = mg
+        F.e.StiMeter = cg
     }
     let ze = L.Base.Meters.IStiDimensionMeter;
     {
-        class cg extends F.e.StiMeter {
+        class dg extends F.e.StiMeter {
             implements() {
-                return cg.ImplementsStiDimensionMeter || (cg.ImplementsStiDimensionMeter = super.implements().concat([ze])), cg.ImplementsStiDimensionMeter
+                return dg.ImplementsStiDimensionMeter || (dg.ImplementsStiDimensionMeter = super.implements().concat([ze])), dg.ImplementsStiDimensionMeter
             }
             constructor(e, t, r) {
                 super(e, t, r)
             }
         }
-        F.e.StiDimensionMeter = cg
+        F.e.StiDimensionMeter = dg
     }
     let Ge = L.System.Collections.Dictionary,
         Xe = L.System.Attribute;
     {
         class dt extends Xe {
             constructor(e) {
                 super(), this.exportToolTypeName = e
@@ -614,17 +614,17 @@
     }
     let gt = L.Report.Dashboard.ImplementsIStiElement,
         pt = L.Report.Components.ImplementsIStiBackColor,
         St = F.D.StiPanelElement,
         wt = L.Report.Components.IStiBackColor,
         bt = L.Report.Components.StiComponent;
     {
-        class dg extends bt {
+        class gg extends bt {
             implements() {
-                return dg.ImplementsStiElement || (dg.ImplementsStiElement = super.implements().concat([Fe, mt, wt, ut, ot, Ee, ...gt, ...pt, ..._e, ...qe, ...et, l])), dg.ImplementsStiElement
+                return gg.ImplementsStiElement || (gg.ImplementsStiElement = super.implements().concat([Fe, mt, wt, ut, ot, Ee, ...gt, ...pt, ..._e, ...qe, ...et, l])), gg.ImplementsStiElement
             }
             meta() {
                 return [...super.meta(), new le(["UseParentStyles", "MinSize", "MaxSize", "Interaction", "PrintOn", "GrowToHeight", "ShiftMode", "CanShrink", "CanGrow", "Printable", "Bookmark", "Hyperlink", "Conditions", "GetBookmarkEvent", "GetHyperlinkEvent", "GetTagEvent", "GetToolTipEvent", "BeforePrintEvent", "AfterPrintEvent", "ClickEvent", "DoubleEvent", "MouseEnterEvent", "MouseLeaveEvent", "GetDrillDownReportEvent"]), new s("Margin").get(e => this.margin.saveToJsonObject(3, 3, 3, 3)), new s("Padding").get(e => this.padding.saveToJsonObject(5, 5, 5, 5)), new n("Border", "border2").get(() => a.Serialize.jBorder2(this.border2)).set(e => this.border2 = a.Deserialize.simpleBorder(e.value)).setXml(e => this.border2 = a.Deserialize.simpleBorder(e.textContent)), new r("BackColor", "", N.transparent), new ne("AltClientRectangle", "", a.Serialize.rectangleD(Ve.empty)).get(() => a.Serialize.rectangleD(this.altClientRectangle)).set(e => this.altClientRectangle = a.Deserialize.rectangleD(e.value)).setXml(e => this.altClientRectangle = this.loadRectangleDFromXml(e.textContent)), new h("AltTitleVisible", "", !0), new n("AltParentKey", "")]
             }
             convert(e, t, r = !1) {}
             fetchAllMeters() {
                 return new P
@@ -692,27 +692,27 @@
             getNestedPages() {
                 return null
             }
             constructor(e = j.empty) {
                 super(e), this.border2 = new st, this._backColor = N.transparent, this.margin = lt.create(3), this.padding = nt.create(5), this.altTitleVisible = !0, this.altClientRectangle = Ve.empty, this.toolboxCategory = it.Dashboards, this.defaultClientRectangle = new j(0, 0, 280, 280), this.key = pe.generateKey(), this.placeOnToolbox = !0
             }
         }
-        F.e.StiElement = dg
+        F.e.StiElement = gg
     }
     let ft = L.Data.Engine.StiDataSorter,
         yt = L.System.Data.DataColumn,
         Ct = L.Report.Dashboard.StiEmptyCellsAs,
         O = L.Report.Dashboard.StiReportParser,
         V = L.Base.Helpers.StiValueHelper,
         xt = L.Data.Engine.StiDataGrouper,
         Mt = L.System.Data.DataTable,
         Tt = L.Data.Engine.StiDataTable,
         Ft = L.Report.Helpers.StiStringsTableHelper;
     {
-        class gg {
+        class pg {
             static getIndicatorDataTable(e, t) {
                 let r = Ft.loadStringRowsFromCache(t),
                     i = (null == r && (r = Ft.loadStringRowsFromPackedString(e, [this.columnValue, this.columnTarget, this.columnSeries])), new P);
                 if (i.add(new F.U.StiValueIndicatorMeter(null, null, A.get("PropertyMain", "Value"))), i.add(new F.U.StiTargetIndicatorMeter(null, null, A.get("PropertyMain", "Target"))), i.add(new F.U.StiSeriesIndicatorMeter(null, null, A.get("Chart", "Series"))), null == r) return new Tt(i, new P);
                 let s = r.groupBy(e => e[2]).select(e => [e.sum(e => this.parseDecimal(e[0], t)), this.sumNullable(e.select(e => this.parseNullableDecimal(e[1], t)).toList()), this.parseString(e.key, t)]);
                 return new Tt(i, s.toList())
             }
@@ -846,27 +846,27 @@
             }
             static parseString(e, t) {
                 if (null == e) return "";
                 let r = "string" == typeof e ? e : null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toString();
                 return null != r && 0 <= r.indexOf("{") ? O.parse2(r, t.report) : r
             }
         }
-        gg.columnValue = "Value", gg.columnEndValue = "EndValue", gg.columnTarget = "Target", gg.columnCloseValue = "CloseValue", gg.columnLowValue = "LowValue", gg.columnHighValue = "HighValue", gg.columnArgument = "Argument", gg.columnWeight = "Weight", gg.columnSeries = "Series", F.e.StiManuallyEnteredDataParser = gg
+        pg.columnValue = "Value", pg.columnEndValue = "EndValue", pg.columnTarget = "Target", pg.columnCloseValue = "CloseValue", pg.columnLowValue = "LowValue", pg.columnHighValue = "HighValue", pg.columnArgument = "Argument", pg.columnWeight = "Weight", pg.columnSeries = "Series", F.e.StiManuallyEnteredDataParser = pg
     }
     let vt = L.Base.Meters.IStiMeasureMeter;
     {
-        class pg extends F.e.StiMeter {
+        class Sg extends F.e.StiMeter {
             implements() {
-                return pg.ImplementsStiMeasureMeter || (pg.ImplementsStiMeasureMeter = super.implements().concat([vt])), pg.ImplementsStiMeasureMeter
+                return Sg.ImplementsStiMeasureMeter || (Sg.ImplementsStiMeasureMeter = super.implements().concat([vt])), Sg.ImplementsStiMeasureMeter
             }
             constructor(e, t, r) {
                 super(e, t, r)
             }
         }
-        F.e.StiMeasureMeter = pg
+        F.e.StiMeasureMeter = Sg
     }
     let At = L.Report.Dashboard.StiTitlePadding,
         It = L.Report.Dashboard.IStiTitlePadding,
         Dt = L.Report.Dashboard.StiTextSizeMode,
         Rt = L.Base.Meta.StiFontMeta,
         Et = L.Report.Dashboard.ImplementsIStiTitle,
         Ot = L.Report.Dashboard.IStiTitle,
@@ -976,17 +976,17 @@
         lr = L.Report.Dashboard.IStiFixedHeightElement,
         ar = L.Report.Components.IStiFont,
         or = L.Report.Components.IStiVertAlignment,
         ur = L.Report.Components.IStiTextHorAlignment;
     {
         let t = L.Base.Drawing.SizeD,
             r = L.Base.Drawing.RectangleD;
-        class mm extends F.e.StiElement {
+        class cm extends F.e.StiElement {
             implements() {
-                return mm.ImplementsStiButtonElement || (mm.ImplementsStiButtonElement = super.implements().concat([er, qt, ur, or, _t, ar, lr, nr, $t, l, ...Qt, ...sr, ...ir, ...rr, ...tr])), mm.ImplementsStiButtonElement
+                return cm.ImplementsStiButtonElement || (cm.ImplementsStiButtonElement = super.implements().concat([er, qt, ur, or, _t, ar, lr, nr, $t, l, ...Qt, ...sr, ...ir, ...rr, ...tr])), cm.ImplementsStiButtonElement
             }
             clone(e) {
                 var t, r, i, s, n, l, a;
                 let o = super.clone(e);
                 return o.brush = null == (t = this.brush) ? void 0 : t.clone(), o.textBrush = null == (r = this.textBrush) ? void 0 : r.clone(), o.iconBrush = null == (i = this.iconBrush) ? void 0 : i.clone(), o.iconSet = null == (s = this.iconSet) ? void 0 : s.clone(), o.shadow = null == (n = this.shadow) ? void 0 : n.clone(), o.font = null == (l = this.font) ? void 0 : l.clone(), o.cornerRadius = null == (a = this.cornerRadius) ? void 0 : a.clone(), o.visualStates = this.visualStates.clone(), o
             }
             meta() {
@@ -1106,20 +1106,20 @@
             set checkedChangedEvent(e) {
                 null != e && e.set(this, e.script)
             }
             constructor(e = j.empty) {
                 super(e), this.checkedValue = !1, this.shapeType = Yt.Rectangle, this._stretch = Kt.StretchXY, this.type = Ut.Button, this.shadow = new Ye, this._style = o.Auto, this._customStyleName = "", this.userFilters = new P, this.textFormat = new Jt, this.font = new H("Arial", 10), this.cornerRadius = new m, this.horAlignment = X.Center, this.vertAlignment = Wt.Center, this.wordWrap = !0, this.brush = new Xt, this.textBrush = new Xt, this.defaultClientRectangle = new r(0, 0, 140, 40), this.helpUrl = "user-manual/dashboards_data_filtering_button.htm", this.text = "Button", this.group = "", this.iconAlignment = Ht.Left, this.iconBrush = new Xt, this.iconSet = new jt, this.visualStates = new F.E.StiButtonVisualStates, this.border2.side = G.All, this.border2.size = 2
             }
         }
-        mm.eventCheckedChanged = {}, F.E.StiButtonElement = mm
+        cm.eventCheckedChanged = {}, F.E.StiButtonElement = cm
     }
     let hr = L.Base.Drawing.StiDefaultBrush,
         mr = L.Report.Dashboard.IStiButtonVisualState;
     {
-        class Sg {
+        class wg {
             constructor() {
                 this.font = null, this.brush = new hr, this.textBrush = new hr, this.border = null, this.iconSet = new F.E.StiButtonElementIconSet, this.iconBrush = new hr
             }
             implements() {
                 return [mr, Vt]
             }
             meta() {
@@ -1131,36 +1131,36 @@
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             static createFromJsonObject(e) {
-                let t = new Sg;
+                let t = new wg;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new Sg;
+                let t = new wg;
                 return t.loadFromXml(e), t
             }
             clone() {
                 var e, t, r, i, s, n;
                 let l = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return l.border = null == (e = this.border) ? void 0 : e.clone(), l.brush = null == (t = this.brush) ? void 0 : t.clone(), l.textBrush = null == (r = this.textBrush) ? void 0 : r.clone(), l.iconBrush = null == (i = this.iconBrush) ? void 0 : i.clone(), l.font = null == (s = this.font) ? void 0 : s.clone(), l.iconSet = null == (n = this.iconSet) ? void 0 : n.clone(), l
             }
             getIconSet() {
                 return this.iconSet
             }
         }
-        F.E.StiButtonVisualState = Sg
+        F.E.StiButtonVisualState = wg
     }
     let cr = L.Base.IStiGetFonts,
         dr = L.Report.Dashboard.IStiButtonVisualStates;
     {
-        class wg {
+        class bg {
             implements() {
                 return [dr, Vt, cr, qt]
             }
             meta() {
                 return [new s("Hover").check(() => null != this.hover).get(() => this.hover.saveToJsonObject(je.Report)).set(e => this.hover = F.E.StiButtonVisualState.createFromJsonObject(e.value)).setXml(e => this.hover = F.E.StiButtonVisualState.createFromXml(e)), new s("Pressed").check(() => null != this.pressed).get(() => this.pressed.saveToJsonObject(je.Report)).set(e => this.pressed = F.E.StiButtonVisualState.createFromJsonObject(e.value)).setXml(e => this.pressed = F.E.StiButtonVisualState.createFromXml(e)), new s("Checked").check(() => null != this.checked).get(() => this.checked.saveToJsonObject(je.Report)).set(e => this.checked = F.E.StiButtonVisualState.createFromJsonObject(e.value)).setXml(e => this.checked = F.E.StiButtonVisualState.createFromXml(e))]
             }
             saveToJsonObject(e) {
@@ -1169,19 +1169,19 @@
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             static createFromJsonObject(e) {
-                let t = new wg;
+                let t = new bg;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new wg;
+                let t = new bg;
                 return t.loadFromXml(e), t
             }
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.hover = this.hover.clone(), e.pressed = this.pressed.clone(), e.checked = this.checked.clone(), e
             }
             getFonts() {
@@ -1221,15 +1221,15 @@
             set checked(e) {
                 this._checked != e && null != (this._checked = e) && (e.parent = this.parent)
             }
             constructor() {
                 this.hover = new F.E.StiButtonVisualState, this.pressed = new F.E.StiButtonVisualState, this.checked = new F.E.StiButtonVisualState
             }
         }
-        F.E.StiButtonVisualStates = wg
+        F.E.StiButtonVisualStates = bg
     }
     let gr = L.Base.Meters.IStiCardsColumn,
         pr = L.Base.Drawing.StiCardsColumnVisibility,
         Sr = L.Report.Components.ImplementsIStiForeColor,
         wr = L.Report.Components.ImplementsIStiHorAlignment,
         br = L.Report.Components.TextFormats.StiFormatService,
         fr = L.Report.Components.IStiForeColor,
@@ -1424,17 +1424,17 @@
         kr = L.Report.Dashboard.StiInteractionOnClick,
         Nr = L.Report.Dashboard.StiInteractionOpenHyperlinkDestination,
         Lr = L.Report.Dashboard.StiInteractionIdent,
         Br = L.Report.Dashboard.StiAvailableInteractionOnClick,
         Pr = L.Report.Dashboard.StiAvailableInteractionOnHover,
         jr = L.Report.Dashboard.StiAvailableInteractionOnDataManipulation;
     {
-        class bg {
+        class fg {
             implements() {
-                return bg.ImplementsStiDashboardInteraction || (bg.ImplementsStiDashboardInteraction = [Or, l]), bg.ImplementsStiDashboardInteraction
+                return fg.ImplementsStiDashboardInteraction || (fg.ImplementsStiDashboardInteraction = [Or, l]), fg.ImplementsStiDashboardInteraction
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
@@ -1472,15 +1472,15 @@
                     t.name = e["name"], t.expression = e["expression"], this.drillDownParameters.add(t)
                 })
             }
             constructor(e, t, r, i, s, n, l) {
                 this.availableOnClick = Br.All, this.availableOnHover = Pr.All, this.availableOnDataManipulation = jr.None, this.onHover = Vr.ShowToolTip, this.onClick = kr.ApplyFilter, this.hyperlinkDestination = Nr.NewTab, this.toolTip = "", this.hyperlink = "", this.drillDownPageKey = "", this.drillDownParameters = new P, null != e && (this.onHover = e), null != t && (this.onClick = t), null != r && (this.hyperlinkDestination = r), null != i && (this.toolTip = i), null != s && (this.hyperlink = s), null != n && (this.drillDownPageKey = n), null != l && (this.drillDownParameters = l)
             }
         }
-        F.g.StiDashboardInteraction = bg
+        F.g.StiDashboardInteraction = fg
     }
     F.g.StiTableColumnDashboardInteraction = class extends F.g.StiDashboardInteraction {
         isDefault() {
             return this.onHover == Vr.None && this.onClick == kr.None && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip)
         }
         constructor(e, t, r, i, s, n, l) {
             super(e, t, r, i, s, n, l), this.ident = Lr.TableColumn, this.availableOnClick = Br.ApplyFilter | Br.ShowDashboard, this.onHover = Vr.None, this.onClick = kr.None
@@ -2476,15 +2476,15 @@
         Ls = F.H.StiArgumentChartMeter,
         Bs = F.H.StiValueChartMeter,
         Ps = F.H.StiSeriesChartMeter,
         js = F.H.StiEndValueChartMeter,
         Hs = L.Base.IStiAppAlias,
         zs = L.Report.Dictionary.StiVariable;
     {
-        class fg {
+        class yg {
             static getValue(e) {
                 if (e.is(Bs)) return e;
                 let t = new Bs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getGanttStartValue(e) {
                 let t = new Bs;
@@ -2599,16 +2599,16 @@
                 return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
             }
             static getIndicatorValue2(e) {
                 let t = new Vi;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.Chart = fg;
-        class yg {
+        F.h.Chart = yg;
+        class Cg {
             static getName(e) {
                 if (e.is2(xs)) return e;
                 let t = new xs;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName2(e) {
                 let t = new xs;
@@ -2620,54 +2620,54 @@
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
                 let t = new Ms;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.ComboBox = yg;
-        class Cg {
+        F.h.ComboBox = Cg;
+        class xg {
             static getFilter2(e) {
                 let t = "",
                     r = (null != e && null != e.type && (Le.isDateType(e.type) ? t = w.now.toString("MM/dd/yyyy") : Le.isNumericType(e.type) && (t = "0")), new f);
                 return r.key = pe.generateKey(), r.condition = Zi.EqualTo, r.path = d.toExpression(e), r.value = t, r.value2 = t, r
             }
             static getFilter(e, t) {
                 let r = ys.getDataColumnFromExpression(t.page.as(F.e.StiDashboard), e.expression),
                     i = "",
                     s = (null != r && null != r.getDataType() && (Le.isDateType(r.getDataType()) ? i = w.now.toString("MM/dd/yyyy") : Le.isNumericType(r.getDataType()) && (i = "0")), new f);
                 return s.key = pe.generateKey(), s.condition = Zi.EqualTo, s.path = Rs.removeFunction(e.expression), s.value = i, s.value2 = i, s
             }
         }
-        F.h.DataFilter = Cg;
-        class xg {
+        F.h.DataFilter = xg;
+        class Mg {
             static getValue(e) {
                 if (e.is2(fs)) return e;
                 let t = new fs;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getValue2(e) {
                 let t = new fs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.DatePicker = xg;
-        class Mg {
+        F.h.DatePicker = Mg;
+        class Tg {
             static getValue(e) {
                 if (e.is2(Oi)) return e;
                 let t = new Oi;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getValue2(e) {
                 let t = new Oi;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.NumberBox = Mg;
-        class Tg {
+        F.h.NumberBox = Tg;
+        class Fg {
             static getSeries(e) {
                 if (e.is2(Ts)) return e;
                 let t = new Ts;
                 return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
                 let t = new Ts;
@@ -2688,16 +2688,16 @@
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
                 let t = new vs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.Gauge = Tg;
-        class Fg {
+        F.h.Gauge = Fg;
+        class vg {
             static getSeries(e) {
                 if (e.is2(As)) return e;
                 let t = new As;
                 return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
                 let t = new As;
@@ -2718,16 +2718,16 @@
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
                 let t = new Ds;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.Indicator = Fg;
-        class vg {
+        F.h.Indicator = vg;
+        class Ag {
             static getName(e) {
                 if (e.is2(bs)) return e;
                 let t = new bs;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName2(e) {
                 let t = new bs;
@@ -2739,16 +2739,16 @@
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
                 let t = new ws;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.ListBox = vg;
-        class Ag {
+        F.h.ListBox = Ag;
+        class Ig {
             static getLatitude(e) {
                 if (e.is2(ps)) return e;
                 let t = new ps;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getLongitude(e) {
                 if (e.is2(Ss)) return e;
@@ -2788,16 +2788,16 @@
             static getLocationValue2(e) {
                 return new Ui(null, d.toExpression(e), d.toAlias(e))
             }
             static getLocationArgument2(e) {
                 return new Xi(null, d.toExpression(e), d.toAlias(e))
             }
         }
-        F.h.OnlineMap = Ag;
-        class Ig {
+        F.h.OnlineMap = Ig;
+        class Dg {
             static getColumn(e) {
                 if (e.is(cs)) return e;
                 let t = new cs;
                 return t.expression = e.expression, t.label = e.label, t.textFormat = this.getFormat(e), t.topN = this.getTopN(e), t.horAlignment = e.is(Cr) ? e.as(Cr).horAlignment : z.Center, t.size = e.is(mi) ? e.size : new hi, t.totalLabel = this.getTotalLabel(e), t.showTotal = this.getShowTotal(e), t.sortDirection = this.getSortDirection(e), t.expandExpression = this.getExpandExpression(e), t
             }
             static getRow(e) {
                 if (e.is(ds)) return e;
@@ -2846,16 +2846,16 @@
             }
             static getTopN(e) {
                 if (e.is(cs)) return e.topN;
                 if (e.is(ds)) return e.topN;
                 return new Fi
             }
         }
-        F.h.Pivot = Ig;
-        class Dg {
+        F.h.Pivot = Dg;
+        class Rg {
             static getSeries(e) {
                 if (e.is2(ms)) return e;
                 let t = new ms;
                 return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
                 let t = new ms;
@@ -2876,16 +2876,16 @@
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
                 let t = new hs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.Progress = Dg;
-        class Rg {
+        F.h.Progress = Rg;
+        class Eg {
             static getKey(e) {
                 if (e.is2(os)) return e;
                 let t = new os;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName(e) {
                 if (e.is2(as)) return e;
@@ -2924,16 +2924,16 @@
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getColor2(e) {
                 let t = new ss;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.RegionMap = Rg;
-        class Eg {
+        F.h.RegionMap = Eg;
+        class Og {
             static getColumn(e) {
                 let t = e.as(Cs);
                 return (t = null == t ? new(e.is(vt) ? is : rs) : t).loadFromString(e.saveToString()), t
             }
             static getDimension(e) {
                 let t = new rs;
                 return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
@@ -2987,16 +2987,16 @@
                 if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
                     let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
                     r.expression = Rs.replaceFunction(r.expression, e)
                 }
                 return r.horAlignment = z.Right, r
             }
         }
-        F.h.Table = Eg;
-        class Og {
+        F.h.Table = Og;
+        class Vg {
             static getColumn(e) {
                 let t = e.as(Mr);
                 return (t = null == t ? new(e.is(vt) ? Fr : Hi) : t).loadFromString(e.saveToString()), t
             }
             static getDimension(e) {
                 let t = new Hi;
                 return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
@@ -3050,39 +3050,39 @@
                 if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
                     let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
                     r.expression = Rs.replaceFunction(r.expression, e)
                 }
                 return r.horAlignment = z.Right, r
             }
         }
-        F.h.Cards = Og;
-        class Vg {
+        F.h.Cards = Vg;
+        class kg {
             static getKey(e) {
                 if (e.is2(Ki)) return e;
                 let t = new Ki;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
                 let t = new Ki;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.TreeView = Vg;
-        class kg {
+        F.h.TreeView = kg;
+        class Ng {
             static getKey(e) {
                 if (e.is2(Yi)) return e;
                 let t = new Yi;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
                 let t = new Yi;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
-        F.h.TreeViewBox = kg;
+        F.h.TreeViewBox = Ng;
         class d {
             static toTotalExpression2(e) {
                 let t = null == e ? void 0 : e.as(oi);
                 if (null != t) return zi.isNumericType(t) ? this.toSumExpression2(t) : this.toCountExpression2(t);
                 return null == e ? void 0 : e.getName()
             }
             static toTotalExpression(e) {
@@ -3118,15 +3118,15 @@
             static toDataType(e) {
                 var t, r;
                 let i = null == (t = null == e ? void 0 : e.as(oi)) ? void 0 : t.type;
                 if (null != i) return i;
                 return null == (r = null == e ? void 0 : e.as(zs)) ? void 0 : r.type
             }
         }
-        d.Chart = fg, d.ComboBox = yg, d.DataFilter = Cg, d.DatePicker = xg, d.NumberBox = Mg, d.Gauge = Tg, d.Indicator = Fg, d.ListBox = vg, d.OnlineMap = Ag, d.Pivot = Ig, d.Progress = Dg, d.RegionMap = Rg, d.Table = Eg, d.Cards = Og, d.TreeView = Vg, d.TreeViewBox = kg, F.h.StiMeterHelper = d
+        d.Chart = yg, d.ComboBox = Cg, d.DataFilter = xg, d.DatePicker = Mg, d.NumberBox = Tg, d.Gauge = Fg, d.Indicator = vg, d.ListBox = Ag, d.OnlineMap = Ig, d.Pivot = Dg, d.Progress = Rg, d.RegionMap = Eg, d.Table = Og, d.Cards = Vg, d.TreeView = kg, d.TreeViewBox = Ng, F.h.StiMeterHelper = d
     }
     F.F.StiCardsItem = class {
         constructor() {
             this.cornerRadius = new m(0), this.margin = new lt(12, 12, 12, 12), this.padding = new nt(12, 12, 12, 12), this.colorEach = !1
         }
         meta() {
             return [new s("Margin").get(e => this.margin.saveToJsonObject(12, 12, 12, 12)), new s("Padding").get(e => this.padding.saveToJsonObject(12, 12, 12, 12)), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new h("ColorEach")]
@@ -3185,17 +3185,17 @@
         _s = L.Report.Dashboard.StiElementLayout,
         $s = L.Report.Dashboard.ImplementsIStiTitleElement,
         en = L.Data.Helpers.StiUsedDataHelper,
         tn = L.Report.Dashboard.IStiCardsElement,
         rn = L.Data.Engine.StiDataSortRule,
         sn = L.Data.Engine.StiDataActionRule;
     {
-        class ym extends F.e.StiElement {
+        class Cm extends F.e.StiElement {
             implements() {
-                return ym.ImplementsStiCardsElement || (ym.ImplementsStiCardsElement = super.implements().concat([tn, Ke, Oe, qs, Qr, Ze, Us, Ne, Xs, ...Ks, ...$s, ...Qs, ...Ue, l])), ym.ImplementsStiCardsElement
+                return Cm.ImplementsStiCardsElement || (Cm.ImplementsStiCardsElement = super.implements().concat([tn, Ke, Oe, qs, Qr, Ze, Us, Ne, Xs, ...Ks, ...$s, ...Qs, ...Ue, l])), Cm.ImplementsStiCardsElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.transformActions = this.transformActions.select(e => e.clone()).toList(), s.transformFilters = this.transformFilters.select(e => e.clone()).toList(), s.transformSorts = this.transformSorts.select(e => e.clone()).toList(), s.columns = this.columns.select(e => e.clone()).toList(), s.dashboardInteraction = null == (t = this.dashboardInteraction) ? void 0 : t.clone(), s.dataFilters = this.dataFilters.select(e => e.clone()).toList(), s.title = null != this.title ? this.title.clone() : null, s.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.shadow = null == (i = this.shadow) ? void 0 : i.clone(), s
             }
             meta() {
@@ -3220,15 +3220,15 @@
                 if (this.columns.clear(), null == t) return;
                 t.cast().forEach(e => {
                     let t = null;
                     e.is2(ze) ? t = new Hi : e.is2(si) ? t = new F.F.StiSparklinesCardsColumn : e.is2(ii) ? t = new F.F.StiDataBarsCardsColumn : e.is2(ti) ? t = new F.F.StiIndicatorCardsColumn : e.is2(ri) ? t = new F.F.StiColorScaleCardsColumn : e.is2(Ar) ? t = new F.F.StiBubbleCardsColumn : e.is2(vt) && ((t = new Fr).horAlignment = z.Right), null != t && (t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.columns.add(t))
                 }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new Ws)
             }
             createMeters(e) {
-                let t = e.as(ym);
+                let t = e.as(Cm);
                 this.columns.clear();
                 for (let e of t.columns) this.columns.add(e)
             }
             createMeters2(t) {
                 this.columns.clear();
                 for (let e of t.columns.list) null != e && null != e.type && Le.isNumericType(e.type) ? this.columns.add(d.Cards.getMeasure2(e)) : this.columns.add(d.Cards.getDimension2(e))
             }
@@ -3305,15 +3305,15 @@
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
             constructor(e = j.empty) {
                 super(e), this.helpUrl = "user-manual/dashboards_cards.htm", this.dataFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.group = "", this.title = new F.e.StiTitle, this.crossFiltering = !0, this.shadow = new Ye, this.layout = new _s, this.cornerRadius = new m(0), this.showBlanks = !1, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.orientation = Ys.Horizontal, this.columns = new P, this.cards = new Zs, this.columnCount = 0, this.title.text = this.localizedName, this.dashboardInteraction = new Ws
             }
         }
-        F.F.StiCardsElement = ym
+        F.F.StiCardsElement = Cm
     } {
         let e;
         (D = e = F.H.StiChartLabelsStyle || (F.H.StiChartLabelsStyle = {}))[D["Value"] = 0] = "Value", D[D["PercentOfTotal"] = 1] = "PercentOfTotal", D[D["Category"] = 2] = "Category", D[D["CategoryValue"] = 3] = "CategoryValue", D[D["CategoryPercentOfTotal"] = 4] = "CategoryPercentOfTotal";
         let t;
         (I = t = F.H.StiLegendVisibility || (F.H.StiLegendVisibility = {}))[I["False"] = 0] = "False", I[I["Auto"] = 1] = "Auto", I[I["Always"] = 2] = "Always"
     } {
         class nn {
@@ -3341,17 +3341,17 @@
             }
         }
         F.H.StiChartAreaIndicator = nn
     }
     let nn = F.H.StiChartAreaIndicator,
         ln = L.Report.Dashboard.IStiChartArea;
     {
-        class Ng {
+        class Lg {
             implements() {
-                return Ng.ImplementsStiChartArea || (Ng.ImplementsStiChartArea = [ln, l]), Ng.ImplementsStiChartArea
+                return Lg.ImplementsStiChartArea || (Lg.ImplementsStiChartArea = [ln, l]), Lg.ImplementsStiChartArea
             }
             meta() {
                 return [new h("ColorEach"), new h("SideBySide", "", !1, !0), new s("GridLinesHor"), new s("GridLinesVert"), new s("InterlacingHor"), new s("InterlacingVert"), new h("ReverseHor"), new h("ReverseVert"), new s("XAxis").check(() => !1), new s("XTopAxis").check(() => !1), new s("YAxis").check(() => !1), new s("YRightAxis").check(() => !1), new s("Indicator"), new se("HorSpacing", "", 6), new se("VertSpacing", "", 6)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3377,22 +3377,22 @@
             set vertSpacing(e) {
                 0 <= e && (this._vertSpacing = e)
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m) {
                 this.sideBySide = !0, this.colorEach = !1, this.reverseHor = !1, this.reverseVert = !1, this.interlacingHor = new F.H.StiHorChartInterlacing, this.interlacingVert = new F.H.StiVertChartInterlacing, this.gridLinesHor = new F.H.StiHorChartGridLines, this.gridLinesVert = new F.H.StiVertChartGridLines, this.xAxis = new F.H.StiXChartAxis, this.xTopAxis = new F.H.StiXTopChartAxis, this.yAxis = new F.H.StiYChartAxis, this.yRightAxis = new F.H.StiYRightChartAxis, this.indicator = new nn, this._horSpacing = 6, this._vertSpacing = 6, null != e && (this.colorEach = e), null != t && (this.reverseHor = t), null != r && (this.reverseVert = r), null != i && (this.gridLinesHor = i), null != s && (this.gridLinesVert = s), null != s && (this.interlacingHor = n), null != l && (this.interlacingVert = l), null != a && (this.xAxis = a), null != o && (this.yAxis = o), null != u && (this.xTopAxis = u), null != h && (this.yRightAxis = h), null != m && (this.indicator = m)
             }
         }
-        F.H.StiChartArea = Ng
+        F.H.StiChartArea = Lg
     } {
-        class Lg {
+        class Bg {
             constructor() {
                 this.text = "", this.color = N.transparent
             }
             implements() {
-                return Lg.implementsStiChartAreaIndicatorTitle || (Lg.implementsStiChartAreaIndicatorTitle = [l, Vt]), Lg.implementsStiChartAreaIndicatorTitle
+                return Bg.implementsStiChartAreaIndicatorTitle || (Bg.implementsStiChartAreaIndicatorTitle = [l, Vt]), Bg.implementsStiChartAreaIndicatorTitle
             }
             meta() {
                 return [new ne("Text"), new r("Color", "", N.transparent)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3403,22 +3403,22 @@
                 u.loadFromXml(e, this)
             }
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e
             }
         }
-        F.H.StiChartAreaIndicatorTitle = Lg
+        F.H.StiChartAreaIndicatorTitle = Bg
     } {
-        class Bg {
+        class Pg {
             constructor() {
                 this.color = N.transparent
             }
             implements() {
-                return Bg.implementsStiChartAreaIndicatorValue || (Bg.implementsStiChartAreaIndicatorValue = [l, Vt]), Bg.implementsStiChartAreaIndicatorValue
+                return Pg.implementsStiChartAreaIndicatorValue || (Pg.implementsStiChartAreaIndicatorValue = [l, Vt]), Pg.implementsStiChartAreaIndicatorValue
             }
             meta() {
                 return [new r("Color", "", N.transparent)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3429,15 +3429,15 @@
                 u.loadFromXml(e, this)
             }
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e
             }
         }
-        F.H.StiChartAreaIndicatorValue = Bg
+        F.H.StiChartAreaIndicatorValue = Pg
     }
     let an = L.Report.Chart.StiLabelsPlacement;
     {
         class on {
             implements() {
                 return on.ImplementsStiChartAxisLabels || (on.ImplementsStiChartAxisLabels = [Vt, ar, ...rr, l]), on.ImplementsStiChartAxisLabels
             }
@@ -3461,17 +3461,17 @@
                 this.angle = 0, this.color = N.transparent, this.font = new H("Arial", 8), this.placement = an.AutoRotation, this.textAlignment = z.Right, this.textAfter = "", this.textBefore = "", this.step = 0, this.wordWrap = !1, this.width = 0, null != e && (this.textBefore = e), null != t && (this.textAfter = t), null != r && (this.angle = r), null != i && (this.font = i), null != s && (this.placement = s), null != n && (this.color = n), null != l && (this.textAlignment = l), null != a && (this.width = a), null != o && (this.wordWrap = o)
             }
         }
         F.H.StiChartAxisLabels = on
     }
     let on = F.H.StiChartAxisLabels;
     {
-        class Pg {
+        class jg {
             implements() {
-                return Pg.ImplementsStiChartAxis || (Pg.ImplementsStiChartAxis = [l, Vt]), Pg.ImplementsStiChartAxis
+                return jg.ImplementsStiChartAxis || (jg.ImplementsStiChartAxis = [l, Vt]), jg.ImplementsStiChartAxis
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
@@ -3498,19 +3498,19 @@
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             constructor(e, t, r) {
                 this.labels = new on, this.range = new F.H.StiChartAxisRange, this.visible = !0, null != e && (this.labels = e), null != t && (this.range = t), null != r && (this.visible = r)
             }
         }
-        F.H.StiChartAxis = Pg
+        F.H.StiChartAxis = jg
     } {
-        class jg {
+        class Hg {
             implements() {
-                return jg.ImplementsStiChartAxisRange || (jg.ImplementsStiChartAxisRange = [l, Vt]), jg.ImplementsStiChartAxisRange
+                return Hg.ImplementsStiChartAxisRange || (Hg.ImplementsStiChartAxisRange = [l, Vt]), Hg.ImplementsStiChartAxisRange
             }
             meta() {
                 return [new se("Minimum", "", 0), new se("Maximum", "", 0), new h("Auto", "", !0)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3529,25 +3529,25 @@
             set minimum(e) {
                 this._minimum = e
             }
             constructor(e, t, r) {
                 this._minimum = 0, this.maximum = 0, this.auto = !0, null != e && (this.auto = e), null != t && (this.minimum = t), null != r && (this.maximum = r)
             }
         }
-        F.H.StiChartAxisRange = jg
+        F.H.StiChartAxisRange = Hg
     }
     let un = L.Report.Chart.StiTitlePosition,
         hn = L.System.Drawing.FontStyle,
         mn = L.System.Drawing.StringAlignment;
     {
         let e;
         (R = e = F.H.Order || (F.H.Order = {}))[R["Alignment"] = 1] = "Alignment", R[R["Color"] = 2] = "Color", R[R["Direction"] = 3] = "Direction", R[R["Font"] = 4] = "Font", R[R["Placement"] = 5] = "Placement", R[R["Position"] = 6] = "Position", R[R["Text"] = 7] = "Text", R[R["Visible"] = 8] = "Visible";
-        class Hg {
+        class zg {
             implements() {
-                return Hg.ImplementsStiChartAxisTitle || (Hg.ImplementsStiChartAxisTitle = [l]), Hg.ImplementsStiChartAxisTitle
+                return zg.ImplementsStiChartAxisTitle || (zg.ImplementsStiChartAxisTitle = [l]), zg.ImplementsStiChartAxisTitle
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
@@ -3574,22 +3574,22 @@
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.font = this.font.clone(), e
             }
             constructor(e, t, r, i, s, n) {
                 this.visible = !0, this.alignment = mn.Center, this.color = N.transparent, this.font = new H("Arial", 12, hn.Bold), this.position = un.Outside, this.text = "", null != e && (this.font = e), null != t && (this.text = t), null != r && (this.color = r), null != i && (this.alignment = i), null != s && (this.position = s), null != n && (this.visible = n)
             }
         }
-        F.H.StiChartAxisTitle = Hg
+        F.H.StiChartAxisTitle = zg
     }
     let cn = L.Report.Chart.StiConstantLines_StiTextPosition,
         dn = L.Report.Dashboard.IStiChartConstantLines;
     {
-        class zg {
+        class Gg {
             implements() {
-                return zg.ImplementsStiChartConstantLines || (zg.ImplementsStiChartConstantLines = [Vt, dn, l]), zg.ImplementsStiChartConstantLines
+                return Gg.ImplementsStiChartConstantLines || (Gg.ImplementsStiChartConstantLines = [Vt, dn, l]), Gg.ImplementsStiChartConstantLines
             }
             meta() {
                 return [new n("Text"), new r("LineColor"), new i("LineStyle", "", Ri, Ri.Solid), new se("LineWidth", "", 1), new ne("AxisValue", "", "1"), new i("Position", "", cn, cn.LeftTop)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3599,26 +3599,26 @@
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             static createFromJson(e) {
-                let t = new zg;
+                let t = new Gg;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new zg;
+                let t = new Gg;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n) {
                 this.text = "", this.lineStyle = Ri.Solid, this.lineColor = N.black, this.axisValue = "1", this.lineWidth = 1, this.position = cn.LeftTop, null != e && (this.text = e), null != t && (this.axisValue = t), null != r && (this.lineColor = r), null != i && (this.lineStyle = i), null != s && (this.lineWidth = s), null != n && (this.position = n)
             }
         }
-        F.H.StiChartConstantLines = zg
+        F.H.StiChartConstantLines = Gg
     }
     let gn = L.Report.Chart.StiMarkerType,
         pn = L.Report.Chart.StiExtendedStyleBool;
     {
         class jn {
             implements() {
                 return jn.ImplementsStiChartMarker || (jn.ImplementsStiChartMarker = [Vt, l]), jn.ImplementsStiChartMarker
@@ -3891,17 +3891,17 @@
         $n = L.Report.Dashboard.StiChartGroups,
         el = L.Report.Dashboard.IStiChartElement,
         tl = L.Data.Engine.ImplementsIStiDrillDownElement,
         rl = F.H.StiChartTrendLine,
         il = L.Report.Chart.IStiShowNullsSeries;
     {
         dt.add("StiChartElement", "Stimulsoft.Dashboard.Export.Tools.StiChartElementExportTool");
-        class vm extends F.e.StiElement {
+        class Am extends F.e.StiElement {
             implements() {
-                return vm.ImplementsStiChartElement || (vm.ImplementsStiChartElement = super.implements().concat([el, Ke, Ze, Nn, ye, Oe, qs, Ne, Us, Gn, Xn, Xs, ...Kn, ...Qe, ...Ue, ...Zn, ...Yn, ...$s, ...Qs, ...Wn, ...Jn, ...Un, ...tl, l, Qr, Dn])), vm.ImplementsStiChartElement
+                return Am.ImplementsStiChartElement || (Am.ImplementsStiChartElement = super.implements().concat([el, Ke, Ze, Nn, ye, Oe, qs, Ne, Us, Gn, Xn, Xs, ...Kn, ...Qe, ...Ue, ...Zn, ...Yn, ...$s, ...Qs, ...Wn, ...Jn, ...Un, ...tl, l, Qr, Dn])), Am.ImplementsStiChartElement
             }
             clone(e) {
                 var t, r, i, s, n;
                 let l = super.clone(e);
                 return l.values = this.values.select(e => e.clone()).toList(), l.endValues = this.endValues.select(e => e.clone()).toList(), l.closeValues = this.closeValues.select(e => e.clone()).toList(), l.lowValues = this.lowValues.select(e => e.clone()).toList(), l.highValues = this.highValues.select(e => e.clone()).toList(), l.arguments = this.arguments.select(e => e.clone()).toList(), l.weights = this.weights.select(e => e.clone()).toList(), l.series = null != this.series ? this.series.clone() : null, l.sortBy = null != this.sortBy ? this.sortBy.clone() : null, l.indicatorValue = null == (t = this.indicatorValue) ? void 0 : t.clone(), l.userFilters = this.userFilters.select(e => e.clone()).toList(), l.userSorts = this.userSorts.select(e => e.clone()).toList(), l.userViewStates = this.userViewStates.select(e => e.clone()).toList(), l.transformActions = this.transformActions.select(e => e.clone()).toList(), l.transformFilters = this.transformFilters.select(e => e.clone()).toList(), l.transformSorts = this.transformSorts.select(e => e.clone()).toList(), l.dataFilters = this.dataFilters.select(e => e.clone()).toList(), l.topN = this.topN.clone(), l.argumentFormat = null != this.argumentFormat ? this.argumentFormat.clone() : null, l.valueFormat = null != this.valueFormat ? this.valueFormat.clone() : null, l.title = null != this.title ? this.title.clone() : null, l.layout = null != this.layout ? this.layout.clone() : null, l.dashboardInteraction = this.dashboardInteraction.clone(), l.xAxis = null != this.xAxis ? this.xAxis.clone() : null, l.xTopAxis = null == (r = this.xTopAxis) ? void 0 : r.clone(), l.yAxis = null != this.yAxis ? this.yAxis.clone() : null, l.yRightAxis = null == (i = this.yRightAxis) ? void 0 : i.clone(), l.legend = null != this.legend ? this.legend.clone() : null, l.area = null != this.area ? this.area.clone() : null, l.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.negativeSeriesColors = null != this.negativeSeriesColors ? this.negativeSeriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.paretoSeriesColors = null != this.paretoSeriesColors ? this.paretoSeriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.marker = null != this.marker ? this.marker.clone() : null, l.constantLines = this.constantLines.select(e => e.clone()).toList(), l.trendLines = this.trendLines.select(e => e.clone()).toList(), l.chartConditions = this.chartConditions.select(e => e.clone()).toList(), l.shadow = null == (s = this.shadow) ? void 0 : s.clone(), l.cornerRadius = null == (n = this.cornerRadius) ? void 0 : n.clone(), l
             }
             meta() {
@@ -4619,24 +4619,24 @@
                     return null != this.manuallyEnteredChartMeter && e.add(this.manuallyEnteredChartMeter), e
                 }
             }
             constructor(e = j.empty) {
                 super(e), this.title = new qn, this.layout = new _s, this.group = "", this.crossFiltering = !0, this._style = o.Auto, this._customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.userViewStates = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.dataFilters = new P, this.seriesColors = [], this.negativeSeriesColors = [], this.paretoSeriesColors = [], this.cornerRadius = new m(0), this.showBlanks = !1, this.shadow = new Ye, this.helpUrl = "user-manual/dashboards_chart.htm", this.manuallyEnteredChartMeter = new F.H.StiValueChartMeter, this.values = new P, this.endValues = new P, this.closeValues = new P, this.lowValues = new P, this.highValues = new P, this.arguments = new P, this.weights = new P, this.legend = new Qn, this.area = new F.H.StiChartArea, this._labels = new F.H.StiChartLabels, this.argumentFormat = new Jt, this.valueFormat = new Wr(null, null, null, 0, null, null, null, null, null, Bn.DecimalDigits | Bn.Abbreviation), this.trendLines = new P, this.constantLines = new P, this.chartConditions = new P, this.marker = new jn, this.icon = null, this.roundValues = !0, this.columnShape = En.Box, this.dataMode = Vn.UsingDataFields, this.drillDownFiltersList = new P, this.drillDownFilters = new P, this.drillDownCurrentLevel = 0, this.title.text = this.localizedName, this.dashboardInteraction = new zn, this.labels = new F.H.StiChartLabels, this.previousAnimations = new P, this.options3D = new On
             }
         }
-        F.H.StiChartElement = vm
+        F.H.StiChartElement = Am
     }
     let sl = L.Report.Dashboard.IStiChartElementCondition,
         nl = L.Report.Components.StiFilterCondition,
         ll = L.Report.Components.StiFilterDataType,
         al = L.Report.Chart.StiChartConditionalField;
     {
-        class Gg {
+        class Xg {
             implements() {
-                return Gg.ImplementsStiChartElementCondition || (Gg.ImplementsStiChartElementCondition = [Vt, sl, l]), Gg.ImplementsStiChartElementCondition
+                return Xg.ImplementsStiChartElementCondition || (Xg.ImplementsStiChartElementCondition = [Vt, sl, l]), Xg.ImplementsStiChartElementCondition
             }
             meta() {
                 return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new n("KeyValueMeter"), new i("Condition", "", nl, nl.EqualTo), new i("DataType", "", ll, ll.Numeric), new i("Field", "", al, al.Value), new n("Value"), new r("Color", "", N.white), new i("MarkerType", "", gn, gn.Circle), new se("MarkerAngle", "", 0), new h("IsExpression")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -4646,33 +4646,33 @@
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             static createFromJson(e) {
-                let t = new Gg;
+                let t = new Xg;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new Gg;
+                let t = new Xg;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n, l, a, o) {
                 this.color = N.white, this.markerAngle = 0, this.markerType = gn.Circle, this.condition = nl.EqualTo, this.dataType = ll.Numeric, this.value = "", this.keyValueMeter = "", this.field = al.Value, this.isExpression = !1, null != e && (this.keyValueMeter = e), null != t && (this.color = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.markerType = n), null != l && (this.markerAngle = l), null != a && (this.field = a), null != o && (this.isExpression = o)
             }
         }
-        F.H.StiChartElementCondition = Gg
+        F.H.StiChartElementCondition = Xg
     } {
-        class Xg {
+        class Wg {
             constructor() {
                 this.color = N.transparent
             }
             implements() {
-                return Xg.ImplementsStiChartGridLines || (Xg.ImplementsStiChartGridLines = [Vt, l]), Xg.ImplementsStiChartGridLines
+                return Wg.ImplementsStiChartGridLines || (Wg.ImplementsStiChartGridLines = [Vt, l]), Wg.ImplementsStiChartGridLines
             }
             meta() {
                 return [new r("Color"), new h("Visible")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -4682,15 +4682,15 @@
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
         }
-        F.H.StiChartGridLines = Xg
+        F.H.StiChartGridLines = Wg
     }
     F.H.StiChartInterlacing = class {
         meta() {
             return [new r("Color"), new h("Visible")]
         }
         saveToJsonObject(e) {
             return u.saveToJsonObject(e, this)
@@ -4707,17 +4707,17 @@
         constructor(e, t) {
             this.color = N.transparent, this.visible = !1, null != e && (this.color = e), null != e && (this.visible = t)
         }
     };
     let ol = L.Report.Dashboard.IStiChartLabels,
         p = L.Report.Dashboard.StiChartLabelsPosition;
     {
-        class Wg {
+        class Jg {
             implements() {
-                return Wg.ImplementsStiChartLabels || (Wg.ImplementsStiChartLabels = [ol, l]), Wg.ImplementsStiChartLabels
+                return Jg.ImplementsStiChartLabels || (Jg.ImplementsStiChartLabels = [ol, l]), Jg.ImplementsStiChartLabels
             }
             meta() {
                 return [new Rt("Font", "", "Arial", 8), new n("TextAfter"), new n("TextBefore"), new r("ForeColor", "", N.transparent), new i("Position", "", p), new i("AxisPosition", "", p, p.None), new i("PiePosition", "", p, p.Center), new i("Pie3dPosition", "", p, p.Center), new i("DoughnutPosition", "", p, p.Center), new i("FunnelPosition", "", p, p.Center), new i("PictorialStackedPosition", "", p, p.Right), new i("TreemapPosition", "", p, p.Center), new i("RadarPosition", "", p, p.None), new i("ClusteredColumn3dPosition", "", p, p.Center), new i("Line3dPosition", "", p, p.Center), new i("Style", "", F.H.StiChartLabelsStyle, F.H.StiChartLabelsStyle.CategoryValue), new h("AutoRotate"), new h("WordWrap"), new se("Width")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -4737,15 +4737,15 @@
             set position(e) {
                 this.element.isPieChart ? this.piePosition = e : this.element.isPie3dChart ? this.pie3dPosition = e : this.element.isDoughnutChart || this.element.isSunburstChart ? this.doughnutPosition = e : this.element.isFunnelChart ? this.funnelPosition = e : this.element.isPictorialStackedChart ? this.pictorialStackedPosition = e : this.element.isTreemapChart ? this.treemapPosition = e : this.element.isRadarChart ? this.radarPosition = e : this.element.isAxisAreaChart3D ? this.clusteredColumn3dPosition = e : this.element.isLineChart3D ? this.line3dPosition = e : this.axisPosition = e
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g) {
                 this.axisPosition = p.None, this.piePosition = p.Center, this.pie3dPosition = p.Center, this.clusteredColumn3dPosition = p.Center, this.line3dPosition = p.Center, this.doughnutPosition = p.Center, this.funnelPosition = p.Center, this.pictorialStackedPosition = p.Right, this.treemapPosition = p.Center, this.radarPosition = p.None, this.foreColor = N.transparent, this.font = new H("Arial", 8), this.autoRotate = !1, this.style = F.H.StiChartLabelsStyle.CategoryValue, this.textAfter = "", this.textBefore = "", this.wordWrap = !1, this.width = 0, null != e && (this.axisPosition = e), null != t && (this.piePosition = t), null != r && (this.doughnutPosition = r), null != i && (this.funnelPosition = i), null != s && (this.treemapPosition = s), null != n && (this.radarPosition = n), null != l && (this.clusteredColumn3dPosition = l), null != a && (this.style = a), null != o && (this.font = o), null != u && (this.foreColor = u), null != h && (this.textBefore = h), null != m && (this.textAfter = m), null != c && (this.autoRotate = c), null != d && (this.width = d), null != g && (this.wordWrap = g)
             }
         }
-        F.H.StiChartLabels = Wg
+        F.H.StiChartLabels = Jg
     }
     let ul = L.System.Text.Encoding,
         hl = L.Base.StiPacker,
         ml = (F.H.StiChartUserViewStatesHelper = class {
             static saveToJsonObject(e) {
                 let t = new He,
                     r = je.Report;
@@ -4901,17 +4901,17 @@
         }, F.g.StiFilterDashboardInteraction),
         dl = L.Report.Dashboard.ImplementsIStiComboBoxElement,
         W = L.System.Drawing.Size,
         gl = L.Report.Dashboard.StiItemSelectionMode,
         pl = L.Report.Dashboard.IStiComboBoxElement;
     {
         dt.add("StiComboBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiComboBoxElementExportTool");
-        class dm extends F.e.StiElement {
+        class gm extends F.e.StiElement {
             implements() {
-                return dm.ImplementsStiComboBoxElement || (dm.ImplementsStiComboBoxElement = super.implements().concat([pl, Ke, Ze, lr, Qr, ...dl, ...Qe, ...Ue, ...tr, l])), dm.ImplementsStiComboBoxElement
+                return gm.ImplementsStiComboBoxElement || (gm.ImplementsStiComboBoxElement = super.implements().concat([pl, Ke, Ze, lr, Qr, ...dl, ...Qe, ...Ue, ...tr, l])), gm.ImplementsStiComboBoxElement
             }
             meta() {
                 return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
@@ -5033,15 +5033,15 @@
                 return new W(0, t)
             }
             set maxSize(e) {}
             constructor(e = j.empty) {
                 super(e), this.group = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this._style = o.Auto, this.customStyleName = "", this.font = new H("Arial", 8), this.shadow = new Ye, this.cornerRadius = new m(0), this.foreColor = N.transparent, this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.One, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_combo_box.htm", this.dashboardInteraction = new cl
             }
         }
-        F.S.StiComboBoxElement = dm
+        F.S.StiComboBoxElement = gm
     }
     let Sl = L.Report.Dashboard.StiDataFilterCreator,
         wl = L.System.Data.DBNull,
         bl = L.Report.Dashboard.StiElementDataCache,
         fl = (F.S.StiComboBoxHelper = class {
             static fetchItems(i, e, s) {
                 if (null == e || e == Tt.nullTable || 0 == e.rows.length) return null;
@@ -5130,17 +5130,17 @@
         Tl = L.Report.Dashboard.StiDateCondition,
         Fl = L.Report.Dashboard.IStiDatePickerElement,
         vl = L.Report.DateTimeRange,
         Al = L.Report.Range,
         Il = L.Report.Engine.StiVariableHelper;
     {
         dt.add("StiDatePickerElement", "Stimulsoft.Dashboard.Export.Tools.StiDatePickerElementExportTool");
-        class wm extends F.e.StiElement {
+        class bm extends F.e.StiElement {
             implements() {
-                return wm.ImplementsStiDatePickerElement || (wm.ImplementsStiDatePickerElement = super.implements().concat([Fl, Ke, Ze, lr, at, ...yl, ...Qe, ...Ue, ...tr, ...fl, l])), wm.ImplementsStiDatePickerElement
+                return bm.ImplementsStiDatePickerElement || (bm.ImplementsStiDatePickerElement = super.implements().concat([Fl, Ke, Ze, lr, at, ...yl, ...Qe, ...Ue, ...tr, ...fl, l])), bm.ImplementsStiDatePickerElement
             }
             meta() {
                 return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("Condition", "", Tl, Tl.GreaterThanOrEqualTo), new i("SelectionMode", "", Ml, Ml.Single).set(e => {
                     let t = ve.parse(Ml, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(Ml, e.textContent);
@@ -5240,15 +5240,15 @@
                 return new W(0, t)
             }
             set maxSize(e) {}
             constructor(e = j.empty) {
                 super(e), this.group = "", this.userFilters = new P, this.dataFilters = new P, this._style = o.Auto, this.customStyleName = "", this.font = new H("Arial", 8), this.foreColor = N.transparent, this.shadow = new Ye, this.cornerRadius = new m(0), this.textFormat = new Xr, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_date_picker.htm", this.condition = Tl.GreaterThanOrEqualTo, this.selectionMode = Ml.Single, this.initialRangeSelection = Cl.MonthPrevious, this.initialRangeSelectionSource = xl.Variable
             }
         }
-        F.Q.StiDatePickerElement = wm
+        F.Q.StiDatePickerElement = bm
     }
     let Dl = L.Report.Engine.StiParser.StiParser,
         Rl = L.Report.Dictionary.StiVariableInitBy,
         El = L.Report.StiVariableExpressionHelper,
         Ol = L.System.StimulsoftDateTimeRange,
         Vl = L.System.NullableDateTime,
         kl = (F.Q.StiDatePickerHelper = class {
@@ -6070,20 +6070,21 @@
     }
     let Ma = F.T.StiGaugeTarget,
         Ta = F.g.StiGaugeDashboardInteraction,
         Fa = F.T.StiGaugeRange,
         va = L.Report.Dashboard.ImplementsIStiGaugeElement,
         Aa = F.i.StiGaugeElementBuilder,
         Ia = L.Report.Dashboard.IStiGaugeElement,
-        Da = F.T.StiGaugeLabels;
+        Da = F.T.StiGaugeLabels,
+        Ra = L.Report.Components.IStiNumberFormat;
     {
         dt.add("StiGaugeElement", "Stimulsoft.Dashboard.Export.Tools.StiGaugeElementExportTool");
-        class Fm extends F.e.StiElement {
+        class vm extends F.e.StiElement {
             implements() {
-                return Fm.ImplementsStiGaugeElement || (Fm.ImplementsStiGaugeElement = super.implements().concat([Ia, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, ...va, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, l, Xs])), Fm.ImplementsStiGaugeElement
+                return vm.ImplementsStiGaugeElement || (vm.ImplementsStiGaugeElement = super.implements().concat([Ia, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, ...va, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, l, Xs, Ra])), vm.ImplementsStiGaugeElement
             }
             clone(e) {
                 var t, r, i, s;
                 let n = super.clone(e);
                 return n.value = null != this.value ? this.value.clone() : null, n.series = null != this.series ? this.series.clone() : null, n.target = null != this.target ? this.target.clone() : null, n.valueFormat = null != this.valueFormat ? this.valueFormat.clone() : null, n.userSorts = this.userSorts.select(e => e.clone()).toList(), n.transformActions = this.transformActions.select(e => e.clone()).toList(), n.transformFilters = this.transformFilters.select(e => e.clone()).toList(), n.transformSorts = this.transformSorts.select(e => e.clone()).toList(), n.dataFilters = this.dataFilters.select(e => e.clone()).toList(), n.title = null != this.title ? this.title.clone() : null, n.layout = null != this.layout ? this.layout.clone() : null, n.dashboardInteraction = this.dashboardInteraction.clone(), n.labels = null == (t = this.labels) ? void 0 : t.clone(), n.targetSettings = null == (r = this.targetSettings) ? void 0 : r.clone(), n.shadow = null == (i = this.shadow) ? void 0 : i.clone(), n.cornerRadius = null == (s = this.cornerRadius) ? void 0 : s.clone(), n
             }
             meta() {
@@ -6254,26 +6255,23 @@
             }
             get toolboxPosition() {
                 return tt.GaugeElement
             }
             get localizedName() {
                 return A.get("Components", "StiGauge")
             }
-            static getValueFormatDefault() {
-                return new Wr(null, null, null, 0, null, null, null, null, null, F.a.StiTextFormatState.DecimalDigits | F.a.StiTextFormatState.Abbreviation)
-            }
             constructor(e = j.empty) {
                 super(e), this.dataMode = Vn.UsingDataFields, this.group = "", this.title = new qn, this.layout = new _s, this.crossFiltering = !0, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.helpUrl = "user-manual/dashboards_gauge.htm", this.valueFormat = new Wr(null, null, null, 0, null, null, null, null, null, F.a.StiTextFormatState.DecimalDigits | F.a.StiTextFormatState.Abbreviation), this.shortValue = !0, this.labels = new Da, this.targetSettings = new Ma, this.minimum = 0, this.maximum = 100, this.calculationMode = L.Report["Gauge"].StiGaugeCalculationMode.Auto, this.rangeMode = L.Report["Gauge"].StiGaugeRangeMode.Percentage, this.rangeType = L.Report["Gauge"].StiGaugeRangeType.None, this.type = L.Report["Gauge"].StiGaugeType.FullCircular, this.ranges = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ta, this.previousAnimations = new P
             }
         }
-        F.T.StiGaugeElement = Fm
+        F.T.StiGaugeElement = vm
     }
     F.ab.StiGaugeRangeConverter = class {};
-    let Ra = F.H.StiXChartMeter,
-        Ea = F.H.StiStartValueChartMeter;
+    let Ea = F.H.StiXChartMeter,
+        Oa = F.H.StiStartValueChartMeter;
     F.G.StiMeterCreator = class {
         static neww(e) {
             if (B.isNullOrEmpty(e)) return null;
             let t, r = Zt.tryParse(e);
             return null != (t = r.successfully ? ve.parse(F.e.StiMeterIdent, r.result) : ve.parse(F.e.StiMeterIdent, e)) ? this.neww2(t) : null
         }
         static neww2(e) {
@@ -6285,29 +6283,29 @@
                 case F.e.StiMeterIdent.SortByChartMeter:
                     return new ki;
                 case F.e.StiMeterIdent.IndicatorValueChartMeter:
                     return new Vi;
                 case F.e.StiMeterIdent.ValueChartMeter:
                     return new Bs;
                 case F.e.StiMeterIdent.StartValueChartMeter:
-                    return new Ea;
+                    return new Oa;
                 case F.e.StiMeterIdent.EndValueChartMeter:
                     return new js;
                 case F.e.StiMeterIdent.OpenValueChartMeter:
                     return new Os;
                 case F.e.StiMeterIdent.CloseValueChartMeter:
                     return new Vs;
                 case F.e.StiMeterIdent.LowValueChartMeter:
                     return new ks;
                 case F.e.StiMeterIdent.HighValueChartMeter:
                     return new Ns;
                 case F.e.StiMeterIdent.WeightChartMeter:
                     return new Es;
                 case F.e.StiMeterIdent.XChartMeter:
-                    return new Ra;
+                    return new Ea;
                 case F.e.StiMeterIdent.YChartMeter:
                     return new _n;
                 case F.e.StiMeterIdent.KeyComboBoxMeter:
                     return new Ms;
                 case F.e.StiMeterIdent.NameComboBoxMeter:
                     return new xs;
                 case F.e.StiMeterIdent.MaxGaugeMeter:
@@ -6409,83 +6407,83 @@
             return this.onHover == Vr.ShowToolTip && this.onClick == kr.OpenHyperlink && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip)
         }
         constructor(e, t, r, i, s, n, l) {
             super(e, t, r, i, s, n, l), this.ident = Lr.Image, this.availableOnClick = Br.OpenHyperlink | Br.ShowDashboard, this.onClick = kr.OpenHyperlink
         }
     };
     {
-        class Oa extends F.e.StiDimensionMeter {
+        class Va extends F.e.StiDimensionMeter {
             implements() {
-                return Oa.ImplementsStiImageMeter || (Oa.ImplementsStiImageMeter = super.implements().concat([Er])), Oa.ImplementsStiImageMeter
+                return Va.ImplementsStiImageMeter || (Va.ImplementsStiImageMeter = super.implements().concat([Er])), Va.ImplementsStiImageMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Image")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ImageMeter
             }
         }
-        F.W.StiImageMeter = Oa
+        F.W.StiImageMeter = Va
     }
-    let Oa = F.W.StiImageMeter,
-        Va = L.Report.Helpers.StiHyperlinkProcessor,
-        ka = F.g.StiImageDashboardInteraction,
-        Na = L.System.Drawing.Image,
-        La = L.Report.Dashboard.ImplementsIStiImageElement,
-        Ba = L.Base.Drawing.StiImageConverter,
-        Pa = L.Report.Dashboard.Helpers.StiDashboardImageHyperlinkCache,
-        ja = L.Report.Dashboard.IStiImageElement,
-        Ha = L.Report.StiFontIconsHelper;
+    let Va = F.W.StiImageMeter,
+        ka = L.Report.Helpers.StiHyperlinkProcessor,
+        Na = F.g.StiImageDashboardInteraction,
+        La = L.System.Drawing.Image,
+        Ba = L.Report.Dashboard.ImplementsIStiImageElement,
+        Pa = L.Base.Drawing.StiImageConverter,
+        ja = L.Report.Dashboard.Helpers.StiDashboardImageHyperlinkCache,
+        Ha = L.Report.Dashboard.IStiImageElement,
+        za = L.Report.StiFontIconsHelper;
     {
         dt.add("StiImageElement", "Stimulsoft.Dashboard.Export.Tools.StiImageElementExportTool");
-        class Tm extends F.e.StiElement {
+        class Fm extends F.e.StiElement {
             implements() {
-                return Tm.ImplementsStiImageElement || (Tm.ImplementsStiImageElement = super.implements().concat([Cr, or, ja, Ze, Ke, Oe, Ne, ...wr, ...ir, ...La, ...Ue, ...Qe, ...$s, l, Qr])), Tm.ImplementsStiImageElement
+                return Fm.ImplementsStiImageElement || (Fm.ImplementsStiImageElement = super.implements().concat([Cr, or, Ha, Ze, Ke, Oe, Ne, ...wr, ...ir, ...Ba, ...Ue, ...Qe, ...$s, l, Qr])), Fm.ImplementsStiImageElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(ka)).set(e => {
+                return [...super.meta(), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Na)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(ka);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Na);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(ka);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Na);
                     null != r && (this.dashboardInteraction = r)
-                }), new h("AspectRatio", "", !0), new n("ImageHyperlink"), new i("HorAlignment", "", z, z.Center), new i("VertAlignment", "", Wt, Wt.Center), new n("Group"), new n("Style"), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new s("Padding").get(e => this.padding.saveToJsonObject(0, 0, 0, 0)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new ne("Image").check(() => null != this.image).get(() => Ba.imageToString(this.image)).set(e => this.image = Ba.stringToImage(e.value.toString())).setXml(e => this.image = Ba.stringToImage(e.textContent)), new i("Icon", "", kt).check(() => null != this.icon), new r("IconColor", "", N.fromArgb2(68, 114, 196))]
+                }), new h("AspectRatio", "", !0), new n("ImageHyperlink"), new i("HorAlignment", "", z, z.Center), new i("VertAlignment", "", Wt, Wt.Center), new n("Group"), new n("Style"), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new s("Padding").get(e => this.padding.saveToJsonObject(0, 0, 0, 0)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new ne("Image").check(() => null != this.image).get(() => Pa.imageToString(this.image)).set(e => this.image = Pa.stringToImage(e.value.toString())).setXml(e => this.image = Pa.stringToImage(e.textContent)), new i("Icon", "", kt).check(() => null != this.icon), new r("IconColor", "", N.fromArgb2(68, 114, 196))]
             }
             get isDefined() {
                 return this.isImageDefined || this.isImageHyperlinkDefined || this.isImageIconDefined
             }
             get isQuerable() {
                 return this.isImageHyperlinkDataColumnDefined()
             }
             fetchAllMeters() {
                 return this.getMeters()
             }
             getMeters() {
                 if (!this.isImageHyperlinkDataColumnDefined()) return new P;
-                let e = Va.getRealDataColumnFromHyperlink(this.report, this.imageHyperlink),
+                let e = ka.getRealDataColumnFromHyperlink(this.report, this.imageHyperlink),
                     t = new P;
-                return t.add(new Oa(e, e, e)), t
+                return t.add(new Va(e, e, e)), t
             }
             retrieveUsedDataNames() {
                 return en.getMany2(this.getMeters()).distinct().toList()
             }
             get imageToDraw() {
                 if (this.isImageDefined) return new Promise(e => {
                     e(this.image)
                 });
                 if (this.isImageIconDefined) {
                     let e = this.getPaintRectangle(!0, !1);
-                    return Ha.convertFontIconToImageAsync(this.icon, this.iconColor, e.width, e.height, null, this.horAlignment)
+                    return za.convertFontIconToImageAsync(this.icon, this.iconColor, e.width, e.height, null, this.horAlignment)
                 }
                 if (this.isImageHyperlinkDefined) return new Promise(i => {
                     setTimeout(async () => {
                         if (this.isImageHyperlinkDataColumnDefined()) {
                             let r = await bl.getOrCreate(this);
                             if (null != r) {
                                 let e = r.rows.firstOrDefault(),
@@ -6494,20 +6492,20 @@
                                     let e = new L.System.Drawing.Image;
                                     e.bytes = t, i(e)
                                 } else if ("string" == typeof t && !B.isNullOrEmpty(t)) {
                                     if (t[L.System.StiObject.stimulsoft]().isBase64String()) {
                                         let e = new L.System.Drawing.Image;
                                         e.base64 = t, i(e)
                                     }
-                                    i(Pa.get(t, this.report))
+                                    i(ja.get(t, this.report))
                                 }
                             }
                             i(null)
                         }
-                        i(Pa.get(this.imageHyperlink, this.report))
+                        i(ja.get(this.imageHyperlink, this.report))
                     })
                 });
                 return new Promise(e => {
                     e(null)
                 })
             }
             copyAllImageProperties(e) {
@@ -6548,70 +6546,70 @@
                 let t = this.dashboardInteraction.drillDownPageKey;
                 if (pe.isEmptyKey(t)) return null;
                 let e = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == e) return null;
                 return new P([e])
             }
             resetAllImageProperties() {
-                this.image = new Na, this.imageHyperlink = null, this.icon = null
+                this.image = new La, this.imageHyperlink = null, this.icon = null
             }
             get isImageDefined() {
                 return null != this.image && (null != this.image.bytes || !B.isNullOrEmpty(this.image.url))
             }
             get isImageIconDefined() {
                 return null != this.icon
             }
             get isImageHyperlinkDefined() {
                 return !B.isNullOrWhiteSpace(this.imageHyperlink)
             }
             isImageHyperlinkDataColumnDefined() {
-                return !this.isImageDefined && !this.isImageIconDefined && this.isImageHyperlinkDefined && !B.isNullOrWhiteSpace(Va.getRealDataColumnFromHyperlink(this.report, this.imageHyperlink))
+                return !this.isImageDefined && !this.isImageIconDefined && this.isImageHyperlinkDefined && !B.isNullOrWhiteSpace(ka.getRealDataColumnFromHyperlink(this.report, this.imageHyperlink))
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.title = new F.e.StiTitle, this.image = null, this.aspectRatio = !0, this.icon = null, this.iconColor = N.fromArgb2(68, 114, 196), this.crossFiltering = !0, this.horAlignment = z.Center, this.vertAlignment = Wt.Center, this.shadow = new Ye, this.cornerRadius = new m(0), this.defaultClientRectangle = new j(0, 0, 120, 120), this.helpUrl = "user-manual/dashboards_image.htm", this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new ka
+                super(e), this.group = "", this.title = new F.e.StiTitle, this.image = null, this.aspectRatio = !0, this.icon = null, this.iconColor = N.fromArgb2(68, 114, 196), this.crossFiltering = !0, this.horAlignment = z.Center, this.vertAlignment = Wt.Center, this.shadow = new Ye, this.cornerRadius = new m(0), this.defaultClientRectangle = new j(0, 0, 120, 120), this.helpUrl = "user-manual/dashboards_image.htm", this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new Na
             }
         }
-        F.X.StiImageElement = Tm
+        F.X.StiImageElement = Fm
     }
     F._.StiImageBytesConverter = class {};
     {
-        class Ja extends F.g.StiDashboardInteraction {
+        class Ua extends F.g.StiDashboardInteraction {
             implements() {
-                return Ja.ImplementsIStiIndicatorDashboardInteraction || (Ja.ImplementsIStiIndicatorDashboardInteraction = super.implements().concat([An, l, Gs])), Ja.ImplementsIStiIndicatorDashboardInteraction
+                return Ua.ImplementsIStiIndicatorDashboardInteraction || (Ua.ImplementsIStiIndicatorDashboardInteraction = super.implements().concat([An, l, Gs])), Ua.ImplementsIStiIndicatorDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserDrillDown"), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && !this.allowUserDrillDown && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout && this.onHover == Vr.ShowToolTip && this.onClick == kr.None && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip) && !this.allowUserDrillDown && this.allowUserSorting
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g) {
                 super(), this.ident = Lr.Indicator, this.availableOnClick = Br.OpenHyperlink | Br.ShowDashboard, this.availableOnDataManipulation = jr.AllowDrillDown | jr.AllowSorting, this.allowUserDrillDown = !1, this.allowUserSorting = !0, this.onClick = kr.None, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != e && (this.onHover = e), null != t && (this.onClick = t), null != r && (this.hyperlinkDestination = r), null != i && (this.toolTip = i), null != s && (this.hyperlink = s), null != n && (this.drillDownPageKey = n), null != l && (this.drillDownParameters = l), null != a && (this.allowUserDrillDown = a), null != u && (this.fileName = u), null != h && (this.headerText = h), null != m && (this.footerText = m), null != c && (this.showFullScreenButton = c), null != d && (this.showSaveButton = d), null != o && (this.allowUserSorting = o), null != g && (this.showViewDataButton = g)
             }
         }
-        F.g.StiIndicatorDashboardInteraction = Ja
+        F.g.StiIndicatorDashboardInteraction = Ua
     }
-    let za = L.Report.Dashboard.StiIndicatorIconRangeMode,
-        Ga = L.Report.Dashboard.StiIndicatorIconMode,
-        Xa = L.Data.Engine.IStiAllowSortByVariation,
-        Wa = L.Report.Dashboard.StiTargetMode,
-        Ja = F.g.StiIndicatorDashboardInteraction,
-        Ua = L.Report.Dashboard.ImplementsIStiIndicatorElement,
-        Za = L.Data.Engine.ImplementsIStiAllowSortByVariation,
-        Ya = L.Report.Helpers.StiFontIconSet,
-        Ka = L.Report.Dashboard.IStiIndicatorElement,
-        Qa = L.System.Convert,
-        qa = L.Report.Dashboard.StiFontSizeMode;
+    let Ga = L.Report.Dashboard.StiIndicatorIconRangeMode,
+        Xa = L.Report.Dashboard.StiIndicatorIconMode,
+        Wa = L.Data.Engine.IStiAllowSortByVariation,
+        Ja = L.Report.Dashboard.StiTargetMode,
+        Ua = F.g.StiIndicatorDashboardInteraction,
+        Za = L.Report.Dashboard.ImplementsIStiIndicatorElement,
+        Ya = L.Data.Engine.ImplementsIStiAllowSortByVariation,
+        Ka = L.Report.Helpers.StiFontIconSet,
+        Qa = L.Report.Dashboard.IStiIndicatorElement,
+        qa = L.System.Convert,
+        _a = L.Report.Dashboard.StiFontSizeMode;
     {
-        class bh extends F.e.StiElement {
+        class fh extends F.e.StiElement {
             implements() {
-                return bh.ImplementsStiIndicatorElement || (bh.ImplementsStiIndicatorElement = super.implements().concat([yr, Ka, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, Xa, Xs, ...$r, ...Ua, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, ...Za, l])), bh.ImplementsStiIndicatorElement
+                return fh.ImplementsStiIndicatorElement || (fh.ImplementsStiIndicatorElement = super.implements().concat([yr, Qa, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, Wa, Xs, ...$r, ...Za, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, ...Ya, l])), fh.ImplementsStiIndicatorElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.value = null != this.value ? this.value.clone() : null, i.target = null != this.target ? this.target.clone() : null, i.series = null != this.series ? this.series.clone() : null, i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.topN = this.topN.clone(), i.textFormat = this.textFormat.clone(), i.targetFormat = this.targetFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.indicatorConditions = this.indicatorConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -6629,21 +6627,21 @@
                     null != t && (this.target = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
                     let t = g.loadFromJson(e.value).as(F.U.StiSeriesIndicatorMeter);
                     null != t && (this.series = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.U.StiSeriesIndicatorMeter);
                     null != t && (this.series = t)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new r("GlyphColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new i("Icon", "", kt, kt.Rating4), new i("IconSet", "", Ya, Ya.Rating), new i("IconMode", "", Ga, Ga.Auto), new i("IconRangeMode", "", za, za.Percentage), new ne("CustomIcon").check(() => null != this.customIcon).get(() => Qa.toBase64String(this.customIcon)).set(e => this.customIcon = Qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = Qa.fromBase64String(e.textContent)), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetMode", "", Wa, Wa.Variation), new i("FontSizeMode", "", qa, qa.Auto), new s("IndicatorConditions").get(e => a.Serialize.objectArray(this.indicatorConditions, e)).set(e => this.indicatorConditions.addRange(e.value.properties().select(e => F.U.StiIndicatorElementCondition.createFromJson(e.value)))).setXml(e => this.indicatorConditions.addRange(e.childNodes.select(e => F.U.StiIndicatorElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ja)).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new r("GlyphColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new i("Icon", "", kt, kt.Rating4), new i("IconSet", "", Ka, Ka.Rating), new i("IconMode", "", Xa, Xa.Auto), new i("IconRangeMode", "", Ga, Ga.Percentage), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetMode", "", Ja, Ja.Variation), new i("FontSizeMode", "", _a, _a.Auto), new s("IndicatorConditions").get(e => a.Serialize.objectArray(this.indicatorConditions, e)).set(e => this.indicatorConditions.addRange(e.value.properties().select(e => F.U.StiIndicatorElementCondition.createFromJson(e.value)))).setXml(e => this.indicatorConditions.addRange(e.childNodes.select(e => F.U.StiIndicatorElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ua)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ja);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ua);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ja);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ua);
                     null != r && (this.dashboardInteraction = r)
                 }), new h("ShowBlanks")]
             }
             addValue2(e) {
                 this.value = null != e ? d.Indicator.getValue2(e) : null
             }
             addValue(e) {
@@ -6727,15 +6725,15 @@
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
                     i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new Is : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di))),
                     s = (null != i && (this.target = null == this.target ? new F.U.StiTargetIndicatorMeter : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ii)));
-                null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.U.StiSeriesIndicatorMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Ja)
+                null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.U.StiSeriesIndicatorMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Ua)
             }
             fetchAllMeters() {
                 let e = new P;
                 return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             getMeters() {
                 let e = new P;
@@ -6781,62 +6779,62 @@
                 let t = this.dashboardInteraction.drillDownPageKey;
                 if (pe.isEmptyKey(t)) return null;
                 let e = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == e) return null;
                 return new P([e])
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.showBlanks = !1, this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_indicator.htm", this.glyphColor = N.transparent, this.targetFormat = new Ur, this.icon = kt.Rating4, this.iconSet = Ya.Rating, this.iconAlignment = Ht.Right, this.targetMode = Wa.Variation, this.fontSizeMode = qa.Auto, this.iconMode = Ga.Auto, this.iconRangeMode = za.Percentage, this.iconRanges = new P, this.indicatorConditions = new P, this.crossFiltering = !0, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ja
+                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.showBlanks = !1, this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_indicator.htm", this.glyphColor = N.transparent, this.targetFormat = new Ur, this.icon = kt.Rating4, this.iconSet = Ka.Rating, this.iconAlignment = Ht.Right, this.targetMode = Ja.Variation, this.fontSizeMode = _a.Auto, this.iconMode = Xa.Auto, this.iconRangeMode = Ga.Percentage, this.iconRanges = new P, this.indicatorConditions = new P, this.crossFiltering = !0, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ua
             }
         }
-        F.U.StiIndicatorElement = bh
+        F.U.StiIndicatorElement = fh
     }
-    let _a = L.Report.Dashboard.IStiIndicatorElementCondition,
-        $a = L.Report.Dashboard.StiIndicatorFieldCondition,
-        eo = L.Report.Dashboard.StiIndicatorConditionPermissions;
+    let $a = L.Report.Dashboard.IStiIndicatorElementCondition,
+        eo = L.Report.Dashboard.StiIndicatorFieldCondition,
+        to = L.Report.Dashboard.StiIndicatorConditionPermissions;
     {
-        class Jg {
+        class Ug {
             implements() {
-                return Jg.ImplementsStiIndicatorElementCondition || (Jg.ImplementsStiIndicatorElementCondition = [Vt, _a, l]), Jg.ImplementsStiIndicatorElementCondition
+                return Ug.ImplementsStiIndicatorElementCondition || (Ug.ImplementsStiIndicatorElementCondition = [Vt, $a, l]), Ug.ImplementsStiIndicatorElementCondition
             }
             meta() {
-                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new i("Condition", "", nl, nl.EqualTo), new i("Field", "", $a, $a.Value), new n("Value"), new r("IconColor", "", N.fromArgb2(68, 114, 196)), new i("Icon", "", kt, kt.Rating4), new r("TargetIconColor", "", N.fromArgb2(68, 114, 196)), new i("TargetIcon", "", kt, kt.Rating4), new ne("CustomIcon").check(() => null != this.customIcon).get(() => Qa.toBase64String(this.customIcon)).set(e => this.customIcon = Qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = Qa.fromBase64String(e.textContent)), new i("Permissions", "", eo, eo.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("TextColor", "", N.black), new r("BackColor", "", N.transparent), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetIconAlignment", "", Ht, Ht.Right)]
+                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new i("Condition", "", nl, nl.EqualTo), new i("Field", "", eo, eo.Value), new n("Value"), new r("IconColor", "", N.fromArgb2(68, 114, 196)), new i("Icon", "", kt, kt.Rating4), new r("TargetIconColor", "", N.fromArgb2(68, 114, 196)), new i("TargetIcon", "", kt, kt.Rating4), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new i("Permissions", "", to, to.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("TextColor", "", N.black), new r("BackColor", "", N.transparent), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetIconAlignment", "", Ht, Ht.Right)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             static createFromJson(e) {
-                let t = new Jg;
+                let t = new Ug;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new Jg;
+                let t = new Ug;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d) {
-                this.iconColor = N.fromArgb2(68, 114, 196), this.icon = kt.Rating4, this.targetIconColor = N.fromArgb2(68, 114, 196), this.targetIcon = kt.Rating4, this.condition = nl.EqualTo, this.field = $a.Value, this.permissions = eo.All, this.textColor = N.black, this.backColor = N.transparent, this.font = new H("Arial", 8), this.iconAlignment = Ht.Right, this.targetIconAlignment = Ht.Right, null != e && (this.field = e), null != t && (this.condition = t), null != r && (this.value = r), null != n && (this.targetIcon = n), null != l && (this.targetIconColor = l), null != i && (this.icon = i), null != s && (this.iconColor = s), null != a && (this.customIcon = a), null != o && (this.iconAlignment = o), null != u && (this.targetIconAlignment = u), null != h && (this.permissions = h), null != m && (this.font = m), null != c && (this.textColor = c), null != d && (this.backColor = d)
+                this.iconColor = N.fromArgb2(68, 114, 196), this.icon = kt.Rating4, this.targetIconColor = N.fromArgb2(68, 114, 196), this.targetIcon = kt.Rating4, this.condition = nl.EqualTo, this.field = eo.Value, this.permissions = to.All, this.textColor = N.black, this.backColor = N.transparent, this.font = new H("Arial", 8), this.iconAlignment = Ht.Right, this.targetIconAlignment = Ht.Right, null != e && (this.field = e), null != t && (this.condition = t), null != r && (this.value = r), null != n && (this.targetIcon = n), null != l && (this.targetIconColor = l), null != i && (this.icon = i), null != s && (this.iconColor = s), null != a && (this.customIcon = a), null != o && (this.iconAlignment = o), null != u && (this.targetIconAlignment = u), null != h && (this.permissions = h), null != m && (this.font = m), null != c && (this.textColor = c), null != d && (this.backColor = d)
             }
         }
-        F.U.StiIndicatorElementCondition = Jg
+        F.U.StiIndicatorElementCondition = Ug
     }
-    let to = L.Report.Dashboard.ImplementsStiIndicatorIconRange,
-        ro = L.Report.Dashboard.IStiIndicatorIconRange;
+    let ro = L.Report.Dashboard.ImplementsStiIndicatorIconRange,
+        io = L.Report.Dashboard.IStiIndicatorIconRange;
     {
-        class Ug {
+        class Zg {
             implements() {
-                return Ug.ImplementsStiIndicatorIconRange || (Ug.ImplementsStiIndicatorIconRange = [l, ro, ...to, Vt]), Ug.ImplementsStiIndicatorIconRange
+                return Zg.ImplementsStiIndicatorIconRange || (Zg.ImplementsStiIndicatorIconRange = [l, io, ...ro, Vt]), Zg.ImplementsStiIndicatorIconRange
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             meta() {
                 return [new n("StartExpression"), new n("EndExpression"), new i("Icon", "", kt)]
             }
@@ -6846,55 +6844,55 @@
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             static loadFromJson(e) {
-                let t = new Ug;
+                let t = new Zg;
                 return t.loadFromJsonObject(e), t
             }
             static loadFromXml(e) {
-                let t = new Ug;
+                let t = new Zg;
                 return t.loadFromXml(e), t
             }
             saveToString() {
                 return this.saveToJsonObject(je.Report).serialize()
             }
             getStringRepresentation() {
                 return this.startExpression + ` - ` + this.endExpression
             }
             constructor(e, t, r) {
                 this.icon = kt.Rating4, this.startExpression = "0", this.endExpression = "100", null != e && (this.icon = e), null != t && (this.startExpression = t), null != r && (this.endExpression = r)
             }
         }
-        F.U.StiIndicatorIconRange = Ug
+        F.U.StiIndicatorIconRange = Zg
     }
-    let io = L.Report.Dashboard.StiListBoxSelectionType,
-        so = L.Report.Dashboard.ImplementsIStiListBoxElement,
-        no = L.Report.Dashboard.IStiListBoxElement;
+    let so = L.Report.Dashboard.StiListBoxSelectionType,
+        no = L.Report.Dashboard.ImplementsIStiListBoxElement,
+        lo = L.Report.Dashboard.IStiListBoxElement;
     {
         dt.add("StiListBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiListBoxElementExportTool");
-        class gm extends F.e.StiElement {
+        class pm extends F.e.StiElement {
             implements() {
-                return gm.ImplementsStiListBoxElement || (gm.ImplementsStiListBoxElement = super.implements().concat([no, Ke, Ze, Oe, Ne, ...so, ...Qe, ...Ue, ...$s, l, Qr])), gm.ImplementsStiListBoxElement
+                return pm.ImplementsStiListBoxElement || (pm.ImplementsStiListBoxElement = super.implements().concat([lo, Ke, Ze, Oe, Ne, ...no, ...Qe, ...Ue, ...$s, l, Qr])), pm.ImplementsStiListBoxElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.keyMeter = null != this.keyMeter ? this.keyMeter.clone() : null, s.nameMeter = null != this.nameMeter ? this.nameMeter.clone() : null, s.userFilters = this.userFilters.select(e => e.clone()).toList(), s.transformActions = this.transformActions.select(e => e.clone()).toList(), s.transformFilters = this.transformFilters.select(e => e.clone()).toList(), s.transformSorts = this.transformSorts.select(e => e.clone()).toList(), s.dataFilters = this.dataFilters.select(e => e.clone()).toList(), s.textFormat = this.textFormat.clone(), s.title = null != this.title ? this.title.clone() : null, s.shadow = null == (t = this.shadow) ? void 0 : t.clone(), s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.dashboardInteraction = null == (i = this.dashboardInteraction) ? void 0 : i.clone(), s
             }
             meta() {
                 return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
                     null != t && (this.selectionMode = t)
-                }), new i("Orientation", "", Ys, Ys.Vertical), new i("SelectionType", "", io, io.ListBox), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
+                }), new i("Orientation", "", Ys, Ys.Vertical), new i("SelectionType", "", so, so.ListBox), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(bs);
                     null != t && (this.nameMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(bs);
                     null != t && (this.nameMeter = t)
                 }), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.P.StiKeyListBoxMeter);
@@ -7002,18 +7000,18 @@
             get toolboxPosition() {
                 return tt.ListBoxElement
             }
             get localizedName() {
                 return A.get("Components", "StiListBox")
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this._style = o.Auto, this.customStyleName = "", this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.One, this.orientation = Ys.Vertical, this.selectionType = io.ListBox, this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 300), this.helpUrl = "user-manual/dashboards_data_filtering_list_box.htm", this.title.text = this.localizedName, this.title.visible = !1, this.dashboardInteraction = new cl
+                super(e), this.group = "", this._style = o.Auto, this.customStyleName = "", this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.One, this.orientation = Ys.Vertical, this.selectionType = so.ListBox, this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 300), this.helpUrl = "user-manual/dashboards_data_filtering_list_box.htm", this.title.text = this.localizedName, this.title.visible = !1, this.dashboardInteraction = new cl
             }
         }
-        F.P.StiListBoxElement = gm
+        F.P.StiListBoxElement = pm
     }
     F.P.StiListBoxHelper = class {
         static fetchItems(i, e, s) {
             if (null == e || e == Tt.nullTable || 0 == e.rows.length) return null;
             let n = this.getNameMeterIndex(e),
                 l = this.getKeyMeterIndex(e);
             if (-1 == n && 1 == l) return null; - 1 == l && (l = n), -1 == n && (n = l);
@@ -7087,42 +7085,42 @@
         toString() {
             return null != this.label ? this.label : this.value.toString()
         }
         constructor(e, t = e) {
             this.label = e, this.value = t
         }
     };
-    let lo = L.Report.DecimalRange,
-        ao = L.Report.Dashboard.StiNumberSelectionMode,
-        oo = L.Report.Dashboard.StiNumberCondition,
-        uo = L.Report.Dashboard.StiNumberMinMaxMode,
-        ho = (F.R.StiNumberBoxHelper = class {
+    let ao = L.Report.DecimalRange,
+        oo = L.Report.Dashboard.StiNumberSelectionMode,
+        uo = L.Report.Dashboard.StiNumberCondition,
+        ho = L.Report.Dashboard.StiNumberMinMaxMode,
+        mo = (F.R.StiNumberBoxHelper = class {
             static getInitialValue(e) {
                 return this.isRange(e) ? this.getRangeInitialValue(e) : this.getSingleInitialValue(e)
             }
             static async getRangeInitialValue(e) {
                 let t = V.tryToNumber(O.parse2(e.initialValue, e.report)),
                     r = V.tryToNumber(O.parse2(e.initialToValue, e.report)),
                     i = await this.getMinMaxRange(e);
-                return t = Math.max(t, i.from), t = Math.min(t, i.to), r = Math.max(r, i.from), r = Math.min(r, i.to), new lo(t, r)
+                return t = Math.max(t, i.from), t = Math.min(t, i.to), r = Math.max(r, i.from), r = Math.min(r, i.to), new ao(t, r)
             }
             static async getSingleInitialValue(t) {
                 var e;
                 let r = null,
                     i = null == (e = this.getVariableSpecifiedAsValue(t)) ? void 0 : e.as(zs);
                 if (null != i) {
                     let e = t.report.dictionary.getVariableValueByName(i.name);
                     i.initBy != Rl.Expression || B.isNullOrEmpty(e) || (e = Dl.parseTextValue(`{${e}}`, t)), L.System.Type.isNumericType(i.type) && (r = V.tryToNullableNumber(e))
                 } else B.isNullOrEmpty(t.initialValue) || (r = V.tryToNullableNumber(O.parse2(t.initialValue, t.report, !0)));
                 let s = await this.getMinMaxRange(t);
                 return r = null != r ? (r = Math.max(Zt.getValueOrDefault(r), s.from), Math.min(Zt.getValueOrDefault(r), s.to)) : s.from, Zt.getValueOrDefault(r)
             }
             static async fetchDefaultUserFilters(e) {
                 let t = this.getValueMeterExpression(e);
-                return e.selectionMode == ao.Single ? this.getSingleDefaultUserFilters(e, t) : this.getRangeDefaultUserFilters(e, t)
+                return e.selectionMode == oo.Single ? this.getSingleDefaultUserFilters(e, t) : this.getRangeDefaultUserFilters(e, t)
             }
             static async getSingleDefaultUserFilters(e, t) {
                 let r = await this.getSingleInitialValue(e);
                 return new f("", t, this.getCondition(e), e.textFormat.format(r)).toList()
             }
             static async getRangeDefaultUserFilters(e, t) {
                 let r = await this.getRangeInitialValue(e);
@@ -7130,79 +7128,79 @@
             }
             static async getAutoRange(e) {
                 let t = this.getValueMeterExpression(e);
                 if (!B.isNullOrEmpty(t)) {
                     let t = await bl.getOrCreate(e);
                     if (null != t) {
                         let e = t.rows.select(e => e[0]).where(e => null != e && L.System.Type.isNumericType(L.System.Type.getType(e))).select(e => V.tryToNumber(e));
-                        if (null != e && e.any()) return new lo(e.min(), e.max())
+                        if (null != e && e.any()) return new ao(e.min(), e.max())
                     }
                 }
-                return new lo(0, 65535)
+                return new ao(0, 65535)
             }
             static getValueMeterExpression(e) {
                 var t;
                 return null == (t = e.valueMeter) ? void 0 : t.expression
             }
             static getCondition(e) {
                 switch (e.condition) {
-                    case oo.EqualTo:
+                    case uo.EqualTo:
                         return Zi.EqualTo;
-                    case oo.NotEqualTo:
+                    case uo.NotEqualTo:
                         return Zi.NotEqualTo;
-                    case oo.GreaterThan:
+                    case uo.GreaterThan:
                         return Zi.GreaterThan;
-                    case oo.GreaterThanOrEqualTo:
+                    case uo.GreaterThanOrEqualTo:
                         return Zi.GreaterThanOrEqualTo;
-                    case oo.LessThan:
+                    case uo.LessThan:
                         return Zi.LessThan;
-                    case oo.LessThanOrEqualTo:
+                    case uo.LessThanOrEqualTo:
                         return Zi.LessThanOrEqualTo;
                     default:
                         return Zi.EqualTo
                 }
             }
             static getVariableSpecifiedAsValue(e) {
                 var t;
                 return El.getVariableSpecifiedAsExpression(e, null == (t = e.getValueMeter()) ? void 0 : t.expression)
             }
             static isRange(t) {
                 if (this.isVariableSpecifiedAsValue(t)) {
                     let e = this.getVariableSpecifiedAsValue(t).as(zs);
                     return null != e && Al.isNumericRangeType(e.type)
                 }
-                return t.selectionMode == ao.Range
+                return t.selectionMode == oo.Range
             }
             static isVariableSpecifiedAsValue(e) {
                 var t;
                 return El.isVariableSpecifiedAsExpression(e, null == (t = e.getValueMeter()) ? void 0 : t.expression)
             }
             static async getMinMaxRange(r) {
-                if (r.minMaxMode == uo.Auto) return this.getAutoRange(r);
+                if (r.minMaxMode == ho.Auto) return this.getAutoRange(r);
                 {
                     let e = 0,
                         t = (B.isNullOrWhiteSpace(r.min) || (e = V.tryToNumber(O.parse2(r.min, r.report, !0))), 65535);
-                    return B.isNullOrWhiteSpace(r.max) || (t = V.tryToNumber(O.parse2(r.max, r.report, !0))), new lo(e, t)
+                    return B.isNullOrWhiteSpace(r.max) || (t = V.tryToNumber(O.parse2(r.max, r.report, !0))), new ao(e, t)
                 }
             }
         }, F.R.StiNumberBoxHelper),
-        mo = L.Report.Dashboard.IStiNumberBoxElement,
-        co = L.Report.Dashboard.ImplementsIStiNumberBoxElement;
+        co = L.Report.Dashboard.IStiNumberBoxElement,
+        go = L.Report.Dashboard.ImplementsIStiNumberBoxElement;
     {
         dt.add("StiNumberBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiNumberBoxElementExportTool");
-        class Am extends F.e.StiElement {
+        class Im extends F.e.StiElement {
             implements() {
-                return Am.ImplementsStiNumberBoxElement || (Am.ImplementsStiNumberBoxElement = super.implements().concat([mo, Ke, Ze, lr, at, Cr, ...co, ...Qe, ...Ue, ...tr, ...fl, ...wr, l])), Am.ImplementsStiNumberBoxElement
+                return Im.ImplementsStiNumberBoxElement || (Im.ImplementsStiNumberBoxElement = super.implements().concat([co, Ke, Ze, lr, at, Cr, ...go, ...Qe, ...Ue, ...tr, ...fl, ...wr, l])), Im.ImplementsStiNumberBoxElement
             }
             meta() {
-                return [...super.meta(), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("Condition", "", oo, oo.GreaterThanOrEqualTo), new i("MinMaxMode​", "", uo, uo.Auto), new i("SelectionMode", "", ao, ao.Single).set(e => {
-                    let t = ve.parse(ao, e.value);
+                return [...super.meta(), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("Condition", "", uo, uo.GreaterThanOrEqualTo), new i("MinMaxMode​", "", ho, ho.Auto), new i("SelectionMode", "", oo, oo.Single).set(e => {
+                    let t = ve.parse(oo, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
-                    let t = ve.parse(ao, e.textContent);
+                    let t = ve.parse(oo, e.textContent);
                     null != t && (this.selectionMode = t)
                 }), new n("InitialValue"), new n("InitialToValue"), new n("Min"), new n("Max"), new se("DecimalDigits", "", 0), new i("HorAlignment", "", z, z.Center), new s("ValueMeter").check(() => null != this.valueMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(Oi);
                     null != t && (this.valueMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(Oi);
                     null != t && (this.valueMeter = t)
@@ -7215,17 +7213,17 @@
             }
             getParentKey() {
                 return null
             }
             setParentKey(e) {}
             async applyDefaultFilters() {
                 var e;
-                let i = null == (e = ho.getVariableSpecifiedAsValue(this)) ? void 0 : e.as(zs);
+                let i = null == (e = mo.getVariableSpecifiedAsValue(this)) ? void 0 : e.as(zs);
                 if (null == i) {
-                    let e = await ho.fetchDefaultUserFilters(this);
+                    let e = await mo.fetchDefaultUserFilters(this);
                     null != e && (this.userFilters = e)
                 } else if (Al.isRangeType(i.type)) {
                     let e = 0,
                         t = 0,
                         r = new L.Report.DecimalRange(e, t);
                     Il.setVariableValue(this.report, i, r), i.initBy == Rl.Value && (i.valueObject = r)
                 }
@@ -7296,64 +7294,64 @@
                 let e = null != this.report ? this.report.getCurrentPage() : null;
                 if (null == e) return W.empty;
                 let t = zt.alignToMaxGrid(this.defaultClientRectangle.height, e.gridSize, !0);
                 return new W(0, t)
             }
             set maxSize(e) {}
             constructor(e = j.empty) {
-                super(e), this.group = "", this.userFilters = new P, this.dataFilters = new P, this._style = o.Auto, this.customStyleName = "", this.font = new H("Arial", 8), this.foreColor = N.transparent, this.shadow = new Ye, this.cornerRadius = new m(0), this.horAlignment = z.Center, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_number_box.htm", this.decimalDigits = 0, this.condition = oo.GreaterThanOrEqualTo, this.selectionMode = ao.Single, this.minMaxMode = uo.Auto, this.initialValue = "", this.initialToValue = "", this.min = "", this.max = ""
+                super(e), this.group = "", this.userFilters = new P, this.dataFilters = new P, this._style = o.Auto, this.customStyleName = "", this.font = new H("Arial", 8), this.foreColor = N.transparent, this.shadow = new Ye, this.cornerRadius = new m(0), this.horAlignment = z.Center, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_number_box.htm", this.decimalDigits = 0, this.condition = uo.GreaterThanOrEqualTo, this.selectionMode = oo.Single, this.minMaxMode = ho.Auto, this.initialValue = "", this.initialToValue = "", this.min = "", this.max = ""
             }
         }
-        F.R.StiNumberBoxElement = Am
+        F.R.StiNumberBoxElement = Im
     } {
-        class go extends F.g.StiDashboardInteraction {
+        class po extends F.g.StiDashboardInteraction {
             implements() {
-                return go.ImplementsIStiOnlineMapDashboardInteraction || (go.ImplementsIStiOnlineMapDashboardInteraction = super.implements().concat([l, Gs])), go.ImplementsIStiOnlineMapDashboardInteraction
+                return po.ImplementsIStiOnlineMapDashboardInteraction || (po.ImplementsIStiOnlineMapDashboardInteraction = super.implements().concat([l, Gs])), po.ImplementsIStiOnlineMapDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout
             }
             constructor(e, t, r, i, s, n) {
                 super(), this.ident = Lr.OnlineMap, this.availableOnClick = Br.None, this.availableOnHover = Pr.None, this.availableOnDataManipulation = jr.None, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != e && (this.fileName = e), null != t && (this.headerText = t), null != r && (this.footerText = r), null != i && (this.showFullScreenButton = i), null != s && (this.showSaveButton = s), null != n && (this.showViewDataButton = n)
             }
         }
-        F.g.StiOnlineMapDashboardInteraction = go
+        F.g.StiOnlineMapDashboardInteraction = po
     }
-    let go = F.g.StiOnlineMapDashboardInteraction,
-        po = L.Report.Dashboard.ImplementsIStiOnlineMapElement,
-        So = L.Report.Dashboard.IStiOnlineMapElement,
-        wo = L.Report.Dashboard.StiOnlineMapLocationType,
-        bo = L.Report.Dashboard.StiOnlineMapCulture,
-        fo = L.Report.Dashboard.StiOnlineMapLocationColorType,
-        yo = L.Report.Dashboard.StiOnlineMapValueViewMode;
+    let po = F.g.StiOnlineMapDashboardInteraction,
+        So = L.Report.Dashboard.ImplementsIStiOnlineMapElement,
+        wo = L.Report.Dashboard.IStiOnlineMapElement,
+        bo = L.Report.Dashboard.StiOnlineMapLocationType,
+        fo = L.Report.Dashboard.StiOnlineMapCulture,
+        yo = L.Report.Dashboard.StiOnlineMapLocationColorType,
+        Co = L.Report.Dashboard.StiOnlineMapValueViewMode;
     {
         dt.add("StiOnlineMapElement", "Stimulsoft.Dashboard.Export.Tools.StiOnlineMapElementExportTool");
-        class xm extends F.e.StiElement {
+        class Mm extends F.e.StiElement {
             implements() {
-                return xm.ImplementsStiOnlineMapElement || (xm.ImplementsStiOnlineMapElement = super.implements().concat([So, Ke, Ze, Oe, qs, Qr, Ne, ...po, ...Qe, ...Ue, ...$s, ...Qs, l])), xm.ImplementsStiOnlineMapElement
+                return Mm.ImplementsStiOnlineMapElement || (Mm.ImplementsStiOnlineMapElement = super.implements().concat([wo, Ke, Ze, Oe, qs, Qr, Ne, ...So, ...Qe, ...Ue, ...$s, ...Qs, l])), Mm.ImplementsStiOnlineMapElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
-                return i.latitude = null != this.latitude ? this.latitude.clone() : null, i.longitude = null != this.longitude ? this.longitude.clone() : null, i.location = null != this.location ? this.location.clone() : null, i.locationColorMeter = null != this.locationColorMeter ? this.locationColorMeter.clone() : null, i.locationValue = null != this.locationValue ? this.locationValue.clone() : null, i.locationArgument = null != this.locationArgument ? this.locationArgument.clone() : null, i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.locationType = this.locationType, i.culture = this.culture, i.locationColorType = this.locationColorType, i.locationColor = this.locationColor, i.iconColor = this.iconColor, i.icon = this.icon, i.customIcon = null != this.customIcon ? Qa.fromBase64String(Qa.toBase64String(this.customIcon)) : null, i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i.onePointZoom = this.onePointZoom, i.userBingKey = this.userBingKey, i
+                return i.latitude = null != this.latitude ? this.latitude.clone() : null, i.longitude = null != this.longitude ? this.longitude.clone() : null, i.location = null != this.location ? this.location.clone() : null, i.locationColorMeter = null != this.locationColorMeter ? this.locationColorMeter.clone() : null, i.locationValue = null != this.locationValue ? this.locationValue.clone() : null, i.locationArgument = null != this.locationArgument ? this.locationArgument.clone() : null, i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.locationType = this.locationType, i.culture = this.culture, i.locationColorType = this.locationColorType, i.locationColor = this.locationColor, i.iconColor = this.iconColor, i.icon = this.icon, i.customIcon = null != this.customIcon ? qa.fromBase64String(qa.toBase64String(this.customIcon)) : null, i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i.onePointZoom = this.onePointZoom, i.userBingKey = this.userBingKey, i
             }
             meta() {
-                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("Latitude").check(() => null != this.latitude).set(e => this.latitude = g.loadFromJson(e.value).as(F.O.StiLatitudeMapMeter)).setXml(e => this.latitude = g.loadFromXml(e).as(F.O.StiLatitudeMapMeter)), new s("Longitude").check(() => null != this.longitude).set(e => this.longitude = g.loadFromJson(e.value).as(F.O.StiLongitudeMapMeter)).setXml(e => this.longitude = g.loadFromXml(e).as(F.O.StiLongitudeMapMeter)), new s("Location").check(() => null != this.location).set(e => this.location = g.loadFromJson(e.value).as(F.O.StiLocationMapMeter)).setXml(e => this.location = g.loadFromXml(e).as(F.O.StiLocationMapMeter)), new s("LocationColorMeter").check(() => null != this.locationColorMeter).set(e => this.locationColorMeter = g.loadFromJson(e.value).as(F.O.StiLocationColorMapMeter)).setXml(e => this.locationColorMeter = g.loadFromXml(e).as(F.O.StiLocationColorMapMeter)), new s("LocationArgument").check(() => null != this.locationArgument).set(e => this.locationArgument = g.loadFromJson(e.value).as(F.O.StiLocationArgumentMapMeter)).setXml(e => this.locationArgument = g.loadFromXml(e).as(F.O.StiLocationArgumentMapMeter)), new s("LocationValue").check(() => null != this.locationValue).set(e => this.locationValue = g.loadFromJson(e.value).as(F.O.StiLocationValueMapMeter)).setXml(e => this.locationValue = g.loadFromXml(e).as(F.O.StiLocationValueMapMeter)), new n("Group"), new i("Culture", "", bo).set(e => this.culture = ve.parse(bo, e.value, !1)).setXml(e => this.culture = ve.parse(bo, e.textContent, !1)), new i("LocationType", "", wo), new r("LocationColor", "", N.limeGreen), new i("LocationColorType", "", fo), new i("ValueViewMode", "", yo), new i("Icon", "", kt), new r("IconColor", "", N.limeGreen), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new ne("CustomIcon").check(() => null != this.customIcon).get(() => Qa.toBase64String(this.customIcon)).set(e => this.customIcon = Qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = Qa.fromBase64String(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(go)).set(e => {
+                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("Latitude").check(() => null != this.latitude).set(e => this.latitude = g.loadFromJson(e.value).as(F.O.StiLatitudeMapMeter)).setXml(e => this.latitude = g.loadFromXml(e).as(F.O.StiLatitudeMapMeter)), new s("Longitude").check(() => null != this.longitude).set(e => this.longitude = g.loadFromJson(e.value).as(F.O.StiLongitudeMapMeter)).setXml(e => this.longitude = g.loadFromXml(e).as(F.O.StiLongitudeMapMeter)), new s("Location").check(() => null != this.location).set(e => this.location = g.loadFromJson(e.value).as(F.O.StiLocationMapMeter)).setXml(e => this.location = g.loadFromXml(e).as(F.O.StiLocationMapMeter)), new s("LocationColorMeter").check(() => null != this.locationColorMeter).set(e => this.locationColorMeter = g.loadFromJson(e.value).as(F.O.StiLocationColorMapMeter)).setXml(e => this.locationColorMeter = g.loadFromXml(e).as(F.O.StiLocationColorMapMeter)), new s("LocationArgument").check(() => null != this.locationArgument).set(e => this.locationArgument = g.loadFromJson(e.value).as(F.O.StiLocationArgumentMapMeter)).setXml(e => this.locationArgument = g.loadFromXml(e).as(F.O.StiLocationArgumentMapMeter)), new s("LocationValue").check(() => null != this.locationValue).set(e => this.locationValue = g.loadFromJson(e.value).as(F.O.StiLocationValueMapMeter)).setXml(e => this.locationValue = g.loadFromXml(e).as(F.O.StiLocationValueMapMeter)), new n("Group"), new i("Culture", "", fo).set(e => this.culture = ve.parse(fo, e.value, !1)).setXml(e => this.culture = ve.parse(fo, e.textContent, !1)), new i("LocationType", "", bo), new r("LocationColor", "", N.limeGreen), new i("LocationColorType", "", yo), new i("ValueViewMode", "", Co), new i("Icon", "", kt), new r("IconColor", "", N.limeGreen), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(po)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(go);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(po);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(go);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(po);
                     null != r && (this.dashboardInteraction = r)
                 }), new se("OnePointZoom", "", 1), new ne("UserBingKey", "")]
             }
             fetchAllMeters() {
                 let e = new P;
                 return null != this.latitude && e.add(this.latitude), null != this.longitude && e.add(this.longitude), null != this.location && e.add(this.location), null != this.locationColorMeter && e.add(this.locationColorMeter), null != this.locationValue && e.add(this.locationValue), null != this.locationArgument && e.add(this.locationArgument), e
             }
@@ -7459,15 +7457,15 @@
                 this.locationArgument = null
             }
             createNewLocationArgumentMeter() {
                 this.locationArgument = new F.O.StiLocationArgumentMapMeter
             }
             convertFrom(e) {
                 let t = e.as(F.L.StiRegionMapElement);
-                null == t || null == t.keyMeter || t.keyMeter.isDefault() || (this.location = new F.O.StiLocationMapMeter, this.location.label = t.keyMeter.label, this.location.expression = t.keyMeter.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new go)
+                null == t || null == t.keyMeter || t.keyMeter.isDefault() || (this.location = new F.O.StiLocationMapMeter, this.location.label = t.keyMeter.label, this.location.expression = t.keyMeter.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new po)
             }
             setString(e, t) {
                 switch (e) {
                     case "Title.Text":
                         this.title.text = t;
                         break
                 }
@@ -7491,97 +7489,97 @@
             get onePointZoom() {
                 return this._onePointZoom
             }
             set onePointZoom(e) {
                 this._onePointZoom = Math.max(Math.min(e, 20), 1)
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.shadow = new Ye, this.cornerRadius = new m(0), this.helpUrl = "user-manual/dashboards_maps_online_map.htm", this._onePointZoom = 1, this.userBingKey = "", this.locationType = wo.Auto, this.culture = bo.en_US, this.locationColorType = fo.Single, this.valueViewMode = yo.Bubble, this.locationColor = N.limeGreen, this.icon = kt.MapMarker, this.iconColor = N.maroon, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new go
+                super(e), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.shadow = new Ye, this.cornerRadius = new m(0), this.helpUrl = "user-manual/dashboards_maps_online_map.htm", this._onePointZoom = 1, this.userBingKey = "", this.locationType = bo.Auto, this.culture = fo.en_US, this.locationColorType = yo.Single, this.valueViewMode = Co.Bubble, this.locationColor = N.limeGreen, this.icon = kt.MapMarker, this.iconColor = N.maroon, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new po
             }
         }
-        F.O.StiOnlineMapElement = xm
+        F.O.StiOnlineMapElement = Mm
     }
     F.N.StiPivotTableColumnVisibilityHelper = class {
         static getVisible(e, t) {
             if (e.visibility == Hr.True) return !0;
             if (e.visibility == Hr.False) return !1;
             if (B.isNullOrWhiteSpace(e.visibilityExpression)) return !1;
             let r = O.parse2(e.visibilityExpression, t);
             return V.tryToBool(r)
         }
     };
-    let Co = L.System.Collections.Hashtable;
+    let xo = L.System.Collections.Hashtable;
     {
-        class Fo {
+        class vo {
             static getSelected(e) {
                 let t = this.hash.get(e.key);
                 if (null == t) return null;
                 return t.keys.toList()
             }
             static getSelectedObjects(e) {
                 let t = this.getSelected(e);
                 return null != t ? t.toList() : null
             }
             static isSelected(e, t) {
                 let r = this.hash.get(e.key);
-                return null == r && (r = new Co, this.hash.set(e.key, r)), null != r.get(t)
+                return null == r && (r = new xo, this.hash.set(e.key, r)), null != r.get(t)
             }
             static select(e, t) {
                 let r = this.hash.get(e.key);
-                null == r && (r = new Co, this.hash.set(e.key, r)), r.set(t, t)
+                null == r && (r = new xo, this.hash.set(e.key, r)), r.set(t, t)
             }
             static resetSelection(e) {
                 this.hash.containsKey(e.key) && this.hash.remove(e.key)
             }
         }
-        Fo.hash = new Co, F.h.StiPivotTableElementSelection = Fo
+        vo.hash = new xo, F.h.StiPivotTableElementSelection = vo
     } {
-        class Mo extends F.g.StiDashboardInteraction {
+        class To extends F.g.StiDashboardInteraction {
             implements() {
-                return Mo.ImplementsIStiPivotTableDashboardInteraction || (Mo.ImplementsIStiPivotTableDashboardInteraction = super.implements().concat([l, Gs])), Mo.ImplementsIStiPivotTableDashboardInteraction
+                return To.ImplementsIStiPivotTableDashboardInteraction || (To.ImplementsIStiPivotTableDashboardInteraction = super.implements().concat([l, Gs])), To.ImplementsIStiPivotTableDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout
             }
             constructor(e, t, r, i, s, n) {
                 super(), this.ident = Lr.PivotTable, this.availableOnClick = Br.None, this.availableOnHover = Pr.None, this.availableOnDataManipulation = jr.None, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != e && (this.fileName = e), null != t && (this.headerText = t), null != r && (this.footerText = r), null != i && (this.showFullScreenButton = i), null != s && (this.showSaveButton = s), null != n && (this.showViewDataButton = n)
             }
         }
-        F.g.StiPivotTableDashboardInteraction = Mo
+        F.g.StiPivotTableDashboardInteraction = To
     }
-    let xo = L.Report.CrossTab.Core.StiSummaryDirection,
-        Mo = F.g.StiPivotTableDashboardInteraction,
-        To = L.Report.Dashboard.ImplementsIStiPivotTableElement,
-        Fo = F.h.StiPivotTableElementSelection,
-        vo = L.Report.Dashboard.IStiPivotTableElement;
+    let Mo = L.Report.CrossTab.Core.StiSummaryDirection,
+        To = F.g.StiPivotTableDashboardInteraction,
+        Fo = L.Report.Dashboard.ImplementsIStiPivotTableElement,
+        vo = F.h.StiPivotTableElementSelection,
+        Ao = L.Report.Dashboard.IStiPivotTableElement;
     {
         dt.add("StiPivotTableElement", "Stimulsoft.Dashboard.Export.Tools.StiPivotTableElementExportTool");
-        class Zh extends F.e.StiElement {
+        class Yh extends F.e.StiElement {
             implements() {
-                return Zh.ImplementsStiPivotTableElement || (Zh.ImplementsStiPivotTableElement = super.implements().concat([vo, Ke, Ze, Oe, qs, Qr, Ne, ...To, ...Qe, ...Ue, ...$s, ...Qs, l])), Zh.ImplementsStiPivotTableElement
+                return Yh.ImplementsStiPivotTableElement || (Yh.ImplementsStiPivotTableElement = super.implements().concat([Ao, Ke, Ze, Oe, qs, Qr, Ne, ...Fo, ...Qe, ...Ue, ...$s, ...Qs, l])), Yh.ImplementsStiPivotTableElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.columns = this.columns.select(e => e.clone()).toList(), i.rows = this.rows.select(e => e.clone()).toList(), i.summaries = this.summaries.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.dashboardInteraction = this.dashboardInteraction.clone(), i.pivotTableConditions = this.pivotTableConditions.select(e => e.clone()).toList(), i.totalLabel = this.totalLabel, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Rows").get(e => a.Serialize.objectArray(this.rows, e)).set(e => this.rows.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(F.N.StiPivotRow)).where(e => null != e))).setXml(e => this.rows.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Summaries").get(e => a.Serialize.objectArray(this.summaries, e)).set(e => this.summaries.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(gs)).where(e => null != e))).setXml(e => this.summaries.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("TotalLabel"), new s("PivotTableConditions").get(e => a.Serialize.objectArray(this.pivotTableConditions, e)).set(e => this.pivotTableConditions.addRange(e.value.properties().select(e => F.N.StiPivotTableElementCondition.loadFromJson(e.value).as(F.N.StiPivotTableElementCondition)).where(e => null != e))).setXml(e => this.pivotTableConditions.addRange(e.childNodes.select(e => F.N.StiPivotTableElementCondition.loadFromXml(e)))), new i("SummaryDirection", "", xo, xo.UpToDown), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Mo)).set(e => {
+                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Rows").get(e => a.Serialize.objectArray(this.rows, e)).set(e => this.rows.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(F.N.StiPivotRow)).where(e => null != e))).setXml(e => this.rows.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Summaries").get(e => a.Serialize.objectArray(this.summaries, e)).set(e => this.summaries.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(gs)).where(e => null != e))).setXml(e => this.summaries.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("TotalLabel"), new s("PivotTableConditions").get(e => a.Serialize.objectArray(this.pivotTableConditions, e)).set(e => this.pivotTableConditions.addRange(e.value.properties().select(e => F.N.StiPivotTableElementCondition.loadFromJson(e.value).as(F.N.StiPivotTableElementCondition)).where(e => null != e))).setXml(e => this.pivotTableConditions.addRange(e.childNodes.select(e => F.N.StiPivotTableElementCondition.loadFromXml(e)))), new i("SummaryDirection", "", Mo, Mo.UpToDown), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(To)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Mo);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(To);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Mo);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(To);
                     null != r && (this.dashboardInteraction = r)
                 })]
             }
             retrieveUsedDataNames() {
                 let e = en.getMany2(this.columns);
                 return e.addRange(en.getMany2(this.rows)), e.addRange(en.getMany2(this.summaries)), e
             }
@@ -7699,15 +7697,15 @@
                             let e = new F.N.StiPivotRow;
                             e.loadFromJsonObject(t.saveToJsonObject(je.Report)), this.rows.add(e)
                         }
                     else if (t.is2(vt)) {
                         let e = new gs;
                         e.loadFromJsonObject(t.saveToJsonObject(je.Report)), this.summaries.add(e)
                     }
-                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new Mo)
+                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new To)
             }
             setString(r, i) {
                 switch (r) {
                     case "Title.Text":
                         this.title.text = i;
                         break;
                     case "TotalLabel":
@@ -7752,31 +7750,31 @@
             get toolboxPosition() {
                 return tt.PivotTableElement
             }
             get localizedName() {
                 return b.get("Components", "StiPivotTable")
             }
             getFormatObjects() {
-                return Fo.getSelectedObjects(this)
+                return vo.getSelectedObjects(this)
             }
             constructor(e = j.empty) {
-                super(e), this.maxIconSize = 50, this.shadow = new Ye, this.cornerRadius = new m(0), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.crossFiltering = !0, this._style = o.Auto, this.customStyleName = "", this.summaryDirection = xo.UpToDown, this.helpUrl = "user-manual/dashboards_pivot_table.htm", this.columns = new P, this.rows = new P, this.summaries = new P, this.totalLabel = "", this.pivotTableConditions = new P, this.title.text = this.localizedName, this.dashboardInteraction = new Mo
+                super(e), this.maxIconSize = 50, this.shadow = new Ye, this.cornerRadius = new m(0), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.crossFiltering = !0, this._style = o.Auto, this.customStyleName = "", this.summaryDirection = Mo.UpToDown, this.helpUrl = "user-manual/dashboards_pivot_table.htm", this.columns = new P, this.rows = new P, this.summaries = new P, this.totalLabel = "", this.pivotTableConditions = new P, this.title.text = this.localizedName, this.dashboardInteraction = new To
             }
         }
-        F.N.StiPivotTableElement = Zh
+        F.N.StiPivotTableElement = Yh
     }
-    let Ao = L.Report.Components.StiConditionPermissions,
-        Io = L.Base.StiScale,
-        Do = L.Report.Dashboard.IStiPivotTableElementCondition;
+    let Io = L.Report.Components.StiConditionPermissions,
+        Do = L.Base.StiScale,
+        Ro = L.Report.Dashboard.IStiPivotTableElementCondition;
     {
         let d = F.a.StiFilterDataType,
             g = F.a.StiFilterCondition;
-        class Zg {
+        class Yg {
             implements() {
-                return Zg.ImplementsStiPivotTableElementCondition || (Zg.ImplementsStiPivotTableElementCondition = [Do, l]), Zg.ImplementsStiPivotTableElementCondition
+                return Yg.ImplementsStiPivotTableElementCondition || (Yg.ImplementsStiPivotTableElementCondition = [Ro, l]), Yg.ImplementsStiPivotTableElementCondition
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
@@ -7785,39 +7783,39 @@
             }
             as(e) {
                 if (this.is(e)) return this;
                 return null
             }
             clone() {
                 let e = this.saveToJsonObject(null),
-                    t = new Zg;
+                    t = new Yg;
                 return t.loadFromJsonObject(e), t
             }
             meta() {
-                return [new ne("Ident").get(() => "StiPivotTableElementCondition"), new n("KeyValueMeter"), new n("DestinationValueMeter"), new i("Condition", "", g), new i("DataType", "", d), new n("Value"), new r("TextColor", "", N.black), new r("BackColor", "", N.transparent), new Rt("Font"), new i("Permissions", "", Ao), new i("IconAlignment", "", Ht), new r("IconColor", "", N.maroon), new i("Icon", "", kt), new ne("CustomIcon").check(() => null != this.customIcon).get(() => Qa.toBase64String(this.customIcon)).set(e => this.customIcon = Qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = Qa.fromBase64String(e.textContent))]
+                return [new ne("Ident").get(() => "StiPivotTableElementCondition"), new n("KeyValueMeter"), new n("DestinationValueMeter"), new i("Condition", "", g), new i("DataType", "", d), new n("Value"), new r("TextColor", "", N.black), new r("BackColor", "", N.transparent), new Rt("Font"), new i("Permissions", "", Io), new i("IconAlignment", "", Ht), new r("IconColor", "", N.maroon), new i("Icon", "", kt), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent))]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             static loadFromJson(e) {
-                let t = new Zg;
+                let t = new Yg;
                 return t.loadFromJsonObject(e), t
             }
             static loadFromXml(e) {
-                let t = new Zg;
+                let t = new Yg;
                 return t.loadFromXml(e), t
             }
             get iconFontSize() {
-                return 18 * Io.factor
+                return 18 * Do.factor
             }
             get customIcon() {
                 return this._customIcon
             }
             set customIcon(e) {
                 this._customIcon = e, this._iconSize = null
             }
@@ -7826,65 +7824,65 @@
             }
             set destinationValueMeter(e) {
                 this._destinationValueMeter = e
             }
             get iconSize() {
                 try {
                     if (null == this._iconSize && null != this.customIcon) {
-                        let e = new Na;
+                        let e = new La;
                         e.bytes = this.customIcon, this._iconSize = new W(e.width, e.height)
                     } else null == this._iconSize && (this._iconSize = new W(this.iconFontSize, this.iconFontSize))
                 } catch (e) {}
                 return this._iconSize
             }
             async getIcon() {
                 if (null != this.customIcon) return this.customIcon;
                 {
-                    let e = await Ha.convertFontIconToImageAsync(this.icon, this.iconColor, this.iconFontSize, this.iconFontSize, "0.9em");
+                    let e = await za.convertFontIconToImageAsync(this.icon, this.iconColor, this.iconFontSize, this.iconFontSize, "0.9em");
                     return e.bytes
                 }
             }
             getUniqueCode() {
                 return 0
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
-                this.textColor = N.black, this.backColor = N.transparent, this.font = new H("Arial", 8), this.permissions = Ao.All, this.icon = kt.Adjust, this.iconAlignment = Ht.None, this.condition = g.EqualTo, this.dataType = d.Numeric, this._destinationValueMeter = "", this.iconColor = N.maroon, null != e && (this.keyValueMeter = e), null != t && (this.destinationValueMeter = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.font = n), null != l && (this.textColor = l), null != a && (this.backColor = a), null != o && (this.permissions = o), null != u && (this.icon = u), null != h && (this.iconAlignment = h), null != m && (this.customIcon = m), null != c && (this.iconColor = c)
+                this.textColor = N.black, this.backColor = N.transparent, this.font = new H("Arial", 8), this.permissions = Io.All, this.icon = kt.Adjust, this.iconAlignment = Ht.None, this.condition = g.EqualTo, this.dataType = d.Numeric, this._destinationValueMeter = "", this.iconColor = N.maroon, null != e && (this.keyValueMeter = e), null != t && (this.destinationValueMeter = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.font = n), null != l && (this.textColor = l), null != a && (this.backColor = a), null != o && (this.permissions = o), null != u && (this.icon = u), null != h && (this.iconAlignment = h), null != m && (this.customIcon = m), null != c && (this.iconColor = c)
             }
         }
-        F.N.StiPivotTableElementCondition = Zg
+        F.N.StiPivotTableElementCondition = Yg
     }
     F.ac.StiPivotColumnConverter = class extends ml {}, F.ac.StiPivotRowConverter = class extends ml {}, F.ac.StiPivotSummaryConverter = class extends ml {};
     {
-        class Ro extends F.g.StiDashboardInteraction {
+        class Eo extends F.g.StiDashboardInteraction {
             implements() {
-                return Ro.ImplementsIStiProgressDashboardInteraction || (Ro.ImplementsIStiProgressDashboardInteraction = super.implements().concat([An, l, Gs])), Ro.ImplementsIStiProgressDashboardInteraction
+                return Eo.ImplementsIStiProgressDashboardInteraction || (Eo.ImplementsIStiProgressDashboardInteraction = super.implements().concat([An, l, Gs])), Eo.ImplementsIStiProgressDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout && this.allowUserSorting
             }
             constructor(e, t, r, i, s, n, l) {
                 super(), this.ident = Lr.Progress, this.availableOnClick = Br.None, this.availableOnHover = Pr.None, this.availableOnDataManipulation = jr.AllowSorting, this.allowUserSorting = !0, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != e && (this.fileName = e), null != t && (this.headerText = t), null != r && (this.footerText = r), null != i && (this.showFullScreenButton = i), null != s && (this.showSaveButton = s), null != n && (this.allowUserSorting = n), null != l && (this.showViewDataButton = l)
             }
         }
-        F.g.StiProgressDashboardInteraction = Ro
+        F.g.StiProgressDashboardInteraction = Eo
     }
-    let Ro = F.g.StiProgressDashboardInteraction,
-        Eo = L.Report.Dashboard.ImplementsIStiProgressElement,
-        Oo = L.Report.Dashboard.StiProgressElementMode,
-        Vo = L.Report.Dashboard.IStiProgressElement;
+    let Eo = F.g.StiProgressDashboardInteraction,
+        Oo = L.Report.Dashboard.ImplementsIStiProgressElement,
+        Vo = L.Report.Dashboard.StiProgressElementMode,
+        ko = L.Report.Dashboard.IStiProgressElement;
     {
-        class Cm extends F.e.StiElement {
+        class xm extends F.e.StiElement {
             implements() {
-                return Cm.ImplementsStiProgressElement || (Cm.ImplementsStiProgressElement = super.implements().concat([yr, Ke, Ze, Vo, Oe, ar, fr, qs, Qr, Ne, Us, Xa, Xs, ...$r, ...Qe, ...Ue, ...Eo, ...$s, ...rr, ...Sr, ...Qs, ...Wn, ...Za, l])), Cm.ImplementsStiProgressElement
+                return xm.ImplementsStiProgressElement || (xm.ImplementsStiProgressElement = super.implements().concat([yr, Ke, Ze, ko, Oe, ar, fr, qs, Qr, Ne, Us, Wa, Xs, ...$r, ...Qe, ...Ue, ...Oo, ...$s, ...rr, ...Sr, ...Qs, ...Wn, ...Ya, l])), xm.ImplementsStiProgressElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.value = null != this.value ? this.value.clone() : null, i.target = null != this.target ? this.target.clone() : null, i.series = null != this.series ? this.series.clone() : null, i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()), i.transformFilters = this.transformFilters.select(e => e.clone()), i.transformSorts = this.transformSorts.select(e => e.clone()), i.dataFilters = this.dataFilters.select(e => e.clone()), i.topN = this.topN.clone(), i.textFormat = this.textFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, i.progressConditions = this.progressConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -7902,21 +7900,21 @@
                     null != t && (this.target = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
                     let t = g.loadFromJson(e.value).as(F.M.StiSeriesProgressMeter);
                     null != t && (this.series = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.M.StiSeriesProgressMeter);
                     null != t && (this.series = t)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new s("SeriesColors").get(e => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e)).setXml(e => this.seriesColors = Js.convertStringToColorArray(e.textContent)), new i("Mode", "", Oo, Oo.Circle), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new n("Group"), new h("ColorEach", "", !0), new s("ProgressConditions").get(e => a.Serialize.objectArray(this.progressConditions, e)).set(e => this.progressConditions.addRange(e.value.properties().select(e => F.M.StiProgressElementCondition.createFromJson(e.value)))).setXml(e => this.progressConditions.addRange(e.childNodes.select(e => F.M.StiProgressElementCondition.createFromXml(e)))), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ro)).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new s("SeriesColors").get(e => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e)).setXml(e => this.seriesColors = Js.convertStringToColorArray(e.textContent)), new i("Mode", "", Vo, Vo.Circle), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new n("Group"), new h("ColorEach", "", !0), new s("ProgressConditions").get(e => a.Serialize.objectArray(this.progressConditions, e)).set(e => this.progressConditions.addRange(e.value.properties().select(e => F.M.StiProgressElementCondition.createFromJson(e.value)))).setXml(e => this.progressConditions.addRange(e.childNodes.select(e => F.M.StiProgressElementCondition.createFromXml(e)))), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Eo)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ro);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Eo);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ro);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Eo);
                     null != r && (this.dashboardInteraction = r)
                 }), new h("ShowBlanks")]
             }
             addValue2(e) {
                 this.value = null != e ? d.Progress.getValue2(e) : null
             }
             addValue(e) {
@@ -7976,15 +7974,15 @@
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
                     i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new F.M.StiValueProgressMeter : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di))),
                     s = (null != i && (this.target = null == this.target ? new hs : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ii)));
-                null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.M.StiSeriesProgressMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Ro)
+                null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.M.StiSeriesProgressMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Eo)
             }
             fetchAllMeters() {
                 let e = new P;
                 return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             getMeters() {
                 let e = new P;
@@ -8032,104 +8030,104 @@
                 let e = new P;
                 return null != this.progressConditions && e.addRange(this.progressConditions), e
             }
             clearProgressConditions() {
                 this.progressConditions.clear()
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.title = new F.e.StiTitle, this.layout = new _s, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.crossFiltering = !0, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_progress.htm", this.colorEach = !0, this.mode = Oo.Circle, this.progressConditions = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ro
+                super(e), this.group = "", this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.title = new F.e.StiTitle, this.layout = new _s, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.crossFiltering = !0, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_progress.htm", this.colorEach = !0, this.mode = Vo.Circle, this.progressConditions = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Eo
             }
         }
-        F.M.StiProgressElement = Cm
+        F.M.StiProgressElement = xm
     }
-    let ko = L.Report.Dashboard.IStiProgressElementCondition,
-        No = L.Report.Dashboard.StiProgressFieldCondition,
-        Lo = L.Report.Dashboard.StiProgressConditionPermissions;
+    let No = L.Report.Dashboard.IStiProgressElementCondition,
+        Lo = L.Report.Dashboard.StiProgressFieldCondition,
+        Bo = L.Report.Dashboard.StiProgressConditionPermissions;
     {
-        class Yg {
+        class Kg {
             implements() {
-                return Yg.ImplementsStiProgressElementCondition || (Yg.ImplementsStiProgressElementCondition = [Vt, l, ko]), Yg.ImplementsStiProgressElementCondition
+                return Kg.ImplementsStiProgressElementCondition || (Kg.ImplementsStiProgressElementCondition = [Vt, l, No]), Kg.ImplementsStiProgressElementCondition
             }
             meta() {
-                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new i("Condition", "", nl, nl.EqualTo), new i("Field", "", No, No.Value), new n("Value"), new r("Color", "", N.transparent), new i("Permissions", "", Lo, Lo.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("TextColor", "", N.black), new r("TrackColor", "", N.transparent)]
+                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new i("Condition", "", nl, nl.EqualTo), new i("Field", "", Lo, Lo.Value), new n("Value"), new r("Color", "", N.transparent), new i("Permissions", "", Bo, Bo.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("TextColor", "", N.black), new r("TrackColor", "", N.transparent)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             static createFromJson(e) {
-                let t = new Yg;
+                let t = new Kg;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new Yg;
+                let t = new Kg;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n, l, a) {
-                this.condition = nl.EqualTo, this.field = No.Value, this.permissions = Lo.All, this.textColor = N.black, this.color = N.transparent, this.trackColor = N.transparent, this.font = new H("Arial", 8), null != e && (this.field = e), null != t && (this.condition = t), null != r && (this.value = r), null != i && (this.permissions = i), null != s && (this.font = s), null != n && (this.textColor = n), null != l && (this.color = l), null != a && (this.trackColor = a)
+                this.condition = nl.EqualTo, this.field = Lo.Value, this.permissions = Bo.All, this.textColor = N.black, this.color = N.transparent, this.trackColor = N.transparent, this.font = new H("Arial", 8), null != e && (this.field = e), null != t && (this.condition = t), null != r && (this.value = r), null != i && (this.permissions = i), null != s && (this.font = s), null != n && (this.textColor = n), null != l && (this.color = l), null != a && (this.trackColor = a)
             }
         }
-        F.M.StiProgressElementCondition = Yg
+        F.M.StiProgressElementCondition = Kg
     } {
-        class Po extends F.g.StiDashboardInteraction {
+        class jo extends F.g.StiDashboardInteraction {
             implements() {
-                return Po.ImplementsIStiRegionMapDashboardInteraction || (Po.ImplementsIStiRegionMapDashboardInteraction = super.implements().concat([l, Gs])), Po.ImplementsIStiRegionMapDashboardInteraction
+                return jo.ImplementsIStiRegionMapDashboardInteraction || (jo.ImplementsIStiRegionMapDashboardInteraction = super.implements().concat([l, Gs])), jo.ImplementsIStiRegionMapDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.onHover == Vr.ShowToolTip && this.onClick == kr.ApplyFilter && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip) && this.isDefaultLayout
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 super(e, t, r, i, s, n, l), this.ident = Lr.RegionMap, this.availableOnClick = Br.ApplyFilter | Br.OpenHyperlink | Br.ShowDashboard, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != a && (this.fileName = a), null != o && (this.headerText = o), null != u && (this.footerText = u), null != h && (this.showFullScreenButton = h), null != m && (this.showSaveButton = m), null != c && (this.showViewDataButton = c)
             }
         }
-        F.g.StiRegionMapDashboardInteraction = Po
+        F.g.StiRegionMapDashboardInteraction = jo
     }
-    let Bo = L.Report.Maps.StiMapLabels,
-        Po = F.g.StiRegionMapDashboardInteraction,
-        jo = L.Report.Dashboard.ImplementsIStiRegionMapElement,
-        Ho = L.Report.Maps.StiMap,
-        zo = L.Report.Maps.StiDisplayNameType,
-        Go = L.Report.Maps.StiMapType,
-        Xo = L.Report.Maps.StiMapSource,
-        Wo = L.Report.Dashboard.IStiRegionMapElement;
+    let Po = L.Report.Maps.StiMapLabels,
+        jo = F.g.StiRegionMapDashboardInteraction,
+        Ho = L.Report.Dashboard.ImplementsIStiRegionMapElement,
+        zo = L.Report.Maps.StiMap,
+        Go = L.Report.Maps.StiDisplayNameType,
+        Xo = L.Report.Maps.StiMapType,
+        Wo = L.Report.Maps.StiMapSource,
+        Jo = L.Report.Dashboard.IStiRegionMapElement;
     {
         dt.add("StiRegionMapElement", "Stimulsoft.Dashboard.Export.Tools.StiRegionMapElementExportTool");
-        class Mm extends F.e.StiElement {
+        class Tm extends F.e.StiElement {
             implements() {
-                return Mm.ImplementsStiRegionMapElement || (Mm.ImplementsStiRegionMapElement = super.implements().concat([Wo, Ke, Ze, ye, Oe, qs, ar, Ne, ...jo, ...Qe, ...Ue, ...Yn, ...$s, ...Qs, ...rr, l, Qr])), Mm.ImplementsStiRegionMapElement
+                return Tm.ImplementsStiRegionMapElement || (Tm.ImplementsStiRegionMapElement = super.implements().concat([Jo, Ke, Ze, ye, Oe, qs, ar, Ne, ...Ho, ...Qe, ...Ue, ...Yn, ...$s, ...Qs, ...rr, l, Qr, Ra])), Tm.ImplementsStiRegionMapElement
             }
             clone(e) {
-                var t, r, i;
-                let s = super.clone(e);
-                return s.keyMeter = null != this.keyMeter ? this.keyMeter.clone() : null, s.nameMeter = null != this.nameMeter ? this.nameMeter.clone() : null, s.valueMeter = null != this.valueMeter ? this.valueMeter.clone() : null, s.groupMeter = null != this.groupMeter ? this.groupMeter.clone() : null, s.colorMeter = null != this.colorMeter ? this.colorMeter.clone() : null, s.userFilters = this.userFilters.select(e => e.clone()).toList(), s.transformActions = this.transformActions.select(e => e.clone()).toList(), s.transformFilters = this.transformFilters.select(e => e.clone()).toList(), s.transformSorts = this.transformSorts.select(e => e.clone()).toList(), s.dataFilters = this.dataFilters.select(e => e.clone()).toList(), s.labels = null == (t = this.labels) ? void 0 : t.clone(), s.title = null != this.title ? this.title.clone() : null, s.layout = null != this.layout ? this.layout.clone() : null, s.dashboardInteraction = this.dashboardInteraction.clone(), s.shadow = null == (r = this.shadow) ? void 0 : r.clone(), s.cornerRadius = null == (i = this.cornerRadius) ? void 0 : i.clone(), s
+                var t, r, i, s;
+                let n = super.clone(e);
+                return n.keyMeter = null != this.keyMeter ? this.keyMeter.clone() : null, n.nameMeter = null != this.nameMeter ? this.nameMeter.clone() : null, n.valueMeter = null != this.valueMeter ? this.valueMeter.clone() : null, n.groupMeter = null != this.groupMeter ? this.groupMeter.clone() : null, n.colorMeter = null != this.colorMeter ? this.colorMeter.clone() : null, n.userFilters = this.userFilters.select(e => e.clone()).toList(), n.transformActions = this.transformActions.select(e => e.clone()).toList(), n.transformFilters = this.transformFilters.select(e => e.clone()).toList(), n.transformSorts = this.transformSorts.select(e => e.clone()).toList(), n.dataFilters = this.dataFilters.select(e => e.clone()).toList(), n.valueFormat = null == (t = this.valueFormat) ? void 0 : t.clone(), n.labels = null == (r = this.labels) ? void 0 : r.clone(), n.title = null != this.title ? this.title.clone() : null, n.layout = null != this.layout ? this.layout.clone() : null, n.dashboardInteraction = this.dashboardInteraction.clone(), n.shadow = null == (i = this.shadow) ? void 0 : i.clone(), n.cornerRadius = null == (s = this.cornerRadius) ? void 0 : s.clone(), n
             }
             meta() {
-                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Po)).set(e => {
+                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(jo)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Po);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(jo);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Po);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(jo);
                     null != r && (this.dashboardInteraction = r)
-                }), new s("Labels").check(() => null != this.labels).set(e => this.labels = Bo.createFromJsonObject(e.value)).setXml(e => this.labels = Bo.createFromXml(e)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
+                }), new s("Labels").check(() => null != this.labels).set(e => this.labels = Po.createFromJsonObject(e.value)).setXml(e => this.labels = Po.createFromXml(e)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(os);
                     null != t && (this.keyMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(os);
                     null != t && (this.keyMeter = t)
                 }), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.L.StiNameMapMeter);
@@ -8151,36 +8149,36 @@
                     null != t && (this.groupMeter = t)
                 }), new s("ColorMeter").check(() => null != this.colorMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.L.StiColorMapMeter);
                     null != t && (this.colorMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.L.StiColorMapMeter);
                     null != t && (this.colorMeter = t)
-                }), new i("DataFrom", "", Xo, Xo.Manual), new i("MapType", "", Go, Go.Individual), new n("MapData"), new h("ShowValue", "", !0), new h("ShortValue", "", !0), new h("ShowZeros", "", !0), new h("ColorEach"), new h("ShowBubble"), new i("ShowName", "", zo, zo.Full), new i("Style", "", o, o.Auto), new n("Group"), new n("Language"), new n("CustomStyleName"), new n(["MapIdent", "MapID"]), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new n("ManuallyEnteredData")]
+                }), new i("DataFrom", "", Wo, Wo.Manual), new i("MapType", "", Xo, Xo.Individual), new n("MapData"), new h("ShowValue", "", !0), new h("ShortValue", "", !0), new h("ShowZeros", "", !0), new h("ColorEach"), new h("ShowBubble"), new i("ShowName", "", Go, Go.Full), new i("Style", "", o, o.Auto), new n("Group"), new n("Language"), new n("CustomStyleName"), new n(["MapIdent", "MapID"]), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new n("ManuallyEnteredData"), new s("ValueFormat").check(() => null != this.valueFormat).set(e => this.valueFormat = br.createFromJsonObject(e.value)).setXml(e => this.valueFormat = br.loadFormatFromXml(e))]
             }
             get allowSkipOwnFilter() {
                 return !0
             }
             fetchAllMeters() {
                 let e = new P;
                 return null != this.keyMeter && e.add(this.keyMeter), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && e.add(this.valueMeter), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter && e.add(this.colorMeter), e
             }
             getMeters() {
                 let e = new P;
-                return this.isDefined && this.dataFrom == Xo.DataColumns && (null != this.keyMeter && (Rs.isFunctionPresent(this.keyMeter.expression) ? e.add(this.keyMeter) : e.add(new os(this.keyMeter.key, `Iso2(${this.keyMeter.expression}, "${this.mapIdent}")`))), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && (Rs.isAggregationFunctionPresent(this.valueMeter.expression) ? e.add(this.valueMeter) : e.add(new F.L.StiValueMapMeter(this.valueMeter.key, `First(${this.valueMeter.expression})`))), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter) && e.add(this.colorMeter), e
+                return this.isDefined && this.dataFrom == Wo.DataColumns && (null != this.keyMeter && (Rs.isFunctionPresent(this.keyMeter.expression) ? e.add(this.keyMeter) : e.add(new os(this.keyMeter.key, `Iso2(${this.keyMeter.expression}, "${this.mapIdent}")`))), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && (Rs.isAggregationFunctionPresent(this.valueMeter.expression) ? e.add(this.valueMeter) : e.add(new F.L.StiValueMapMeter(this.valueMeter.key, `First(${this.valueMeter.expression})`))), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter) && e.add(this.colorMeter), e
             }
             retrieveUsedDataNames() {
                 let e = new P;
-                return this.dataFrom == Xo.DataColumns && (e.addRange(en.getMany(this.keyMeter)), e.addRange(en.getMany(this.nameMeter)), e.addRange(en.getMany(this.valueMeter)), e.addRange(en.getMany(this.groupMeter)), e.addRange(en.getMany(this.colorMeter))), e.distinct()
+                return this.dataFrom == Wo.DataColumns && (e.addRange(en.getMany(this.keyMeter)), e.addRange(en.getMany(this.nameMeter)), e.addRange(en.getMany(this.valueMeter)), e.addRange(en.getMany(this.groupMeter)), e.addRange(en.getMany(this.colorMeter))), e.distinct()
             }
             get isDefined() {
-                return this.dataFrom != Xo.DataColumns || null != this.keyMeter || null != this.nameMeter || null != this.valueMeter || null != this.groupMeter || null != this.colorMeter
+                return this.dataFrom != Wo.DataColumns || null != this.keyMeter || null != this.nameMeter || null != this.valueMeter || null != this.groupMeter || null != this.colorMeter
             }
             get isQuerable() {
-                return this.dataFrom == Xo.DataColumns
+                return this.dataFrom == Wo.DataColumns
             }
             get font() {
                 return this.labels.font
             }
             set font(e) {
                 this.labels.font = e
             }
@@ -8266,15 +8264,15 @@
                 this.colorMeter = null
             }
             createNewColorMeter() {
                 this.colorMeter = new F.L.StiColorMapMeter
             }
             convertFrom(e) {
                 let t = e.as(F.O.StiOnlineMapElement);
-                null == t || null == t.location || t.location.isDefault() || (this.keyMeter = new os, this.keyMeter.label = t.location.label, this.keyMeter.expression = t.location.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new Po)
+                null == t || null == t.location || t.location.isDefault() || (this.keyMeter = new os, this.keyMeter.label = t.location.label, this.keyMeter.expression = t.location.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new jo)
             }
             setString(e, t) {
                 switch (e) {
                     case "Title.Text":
                         this.title.text = t;
                         break
                 }
@@ -8298,15 +8296,15 @@
             get dashboardInteraction() {
                 return this._dashboardInteraction
             }
             set dashboardInteraction(e) {
                 this._dashboardInteraction = e
             }
             getManuallyEnteredDataTable() {
-                if (this.dataFrom == Xo.Manual) {
+                if (this.dataFrom == Wo.Manual) {
                     let e = this.getMapData().orderBy(e => e.key).toList(),
                         r = new Tt;
                     r.meters.add(new os("Key", "Key")), r.meters.add(new F.L.StiNameMapMeter("Name", "Name")), r.meters.add(new F.L.StiValueMapMeter("Value", "Value"));
                     for (let t of e) {
                         let e = [];
                         e[0] = t.key, e[1] = t.name, e[2] = t.value, r.rows.add(e)
                     }
@@ -8319,61 +8317,61 @@
                 let t = this.dashboardInteraction.drillDownPageKey;
                 if (pe.isEmptyKey(t)) return null;
                 let e = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == e) return null;
                 return new P([e])
             }
             getMapData() {
-                let e = new Ho;
+                let e = new zo;
                 return e.mapData = this.mapData, e.mapIdent = this.mapIdent, e.page = this.page, e.getMapData()
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.layout = new _s, this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.helpUrl = "user-manual/dashboards_maps_region_map.htm", this.dataMode = Vn.UsingDataFields, this.labels = new Bo, this.mapIdent = "USA", this.dataFrom = Xo.Manual, this.mapType = Go.Individual, this.showValue = !0, this.showZeros = !0, this.shortValue = !0, this.colorEach = !1, this.showBubble = !1, this.showName = zo.Full, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new Po
+                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.valueFormat = new Wr(null, null, null, 1, null, null, null, null, null, L.Report.Components.StiTextFormatState.DecimalDigits | L.Report.Components.StiTextFormatState.Abbreviation), this.layout = new _s, this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.helpUrl = "user-manual/dashboards_maps_region_map.htm", this.dataMode = Vn.UsingDataFields, this.labels = new Po, this.mapIdent = "USA", this.dataFrom = Wo.Manual, this.mapType = Xo.Individual, this.showValue = !0, this.showZeros = !0, this.shortValue = !0, this.colorEach = !1, this.showBubble = !1, this.showName = Go.Full, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new jo
             }
         }
-        F.L.StiRegionMapElement = Mm
+        F.L.StiRegionMapElement = Tm
     } {
-        class Ko extends F.g.StiDashboardInteraction {
+        class Qo extends F.g.StiDashboardInteraction {
             StiShapeDashboardInteraction() {}
             constructor(e, t, r, i, s, n, l) {
                 super(e, t, r, i, s, n, l), this.ident = Lr.Shape, this.availableOnClick = Br.OpenHyperlink | Br.ShowDashboard, this.onClick = kr.OpenHyperlink
             }
         }
-        F.g.StiShapeDashboardInteraction = Ko
+        F.g.StiShapeDashboardInteraction = Qo
     }
-    let Jo = L.Report.Components.StiShapeTypeService,
-        Uo = L.Report.Dashboard.ImplementsIStiShapeElement,
-        Zo = L.Report.Components.StiRectangleShapeType,
-        Yo = L.Report.Dashboard.IStiShapeElement,
-        Ko = F.g.StiShapeDashboardInteraction;
+    let Uo = L.Report.Components.StiShapeTypeService,
+        Zo = L.Report.Dashboard.ImplementsIStiShapeElement,
+        Yo = L.Report.Components.StiRectangleShapeType,
+        Ko = L.Report.Dashboard.IStiShapeElement,
+        Qo = F.g.StiShapeDashboardInteraction;
     {
         dt.add("StiShapeElement", "Stimulsoft.Dashboard.Export.Tools.StiShapeElementExportTool");
-        class cm extends F.e.StiElement {
+        class dm extends F.e.StiElement {
             implements() {
-                return cm.ImplementsStiShapeElement || (cm.ImplementsStiShapeElement = super.implements().concat([Yo, Oe, Qr, Ne, ...Uo, ...$s, l])), cm.ImplementsStiShapeElement
+                return dm.ImplementsStiShapeElement || (dm.ImplementsStiShapeElement = super.implements().concat([Ko, Oe, Qr, Ne, ...Zo, ...$s, l])), dm.ImplementsStiShapeElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shapeType = null == (t = this.shapeType) ? void 0 : t.clone(), i.dashboardInteraction = null == (r = this.dashboardInteraction) ? void 0 : r.clone(), i
             }
             meta() {
                 return [...super.meta(), new s("Title").check(() => null != this.title).set(e => {
                     this.title = new qn, this.title.loadFromJsonObject(e)
                 }).setXml(e => {
                     this.title = new qn, this.title.loadFromXml(e)
-                }), new Pt("Fill"), new r("Stroke", "", N.black), new se("Size", "", 1), new s("ShapeType").set(e => this.shapeType = Jo.createFromJsonObject(e.value)).setXml(e => {
-                    this.shapeType = Jo.convertFromXml(e), this.shapeType.loadFromXml(e)
-                }), new s("Padding").get(e => this.padding.saveToJsonObject(0, 0, 0, 0)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ko)).set(e => {
+                }), new Pt("Fill"), new r("Stroke", "", N.black), new se("Size", "", 1), new s("ShapeType").set(e => this.shapeType = Uo.createFromJsonObject(e.value)).setXml(e => {
+                    this.shapeType = Uo.convertFromXml(e), this.shapeType.loadFromXml(e)
+                }), new s("Padding").get(e => this.padding.saveToJsonObject(0, 0, 0, 0)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Qo)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ko);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Qo);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ko);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Qo);
                     null != r && (this.dashboardInteraction = r)
                 })]
             }
             get toolboxPosition() {
                 return tt.ShapeElement
             }
             get localizedName() {
@@ -8415,81 +8413,81 @@
                 if (pe.isEmptyKey(t)) return null;
                 super.getNestedPages;
                 let r = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == r) return null;
                 return new P([r])
             }
             constructor(e = j.empty) {
-                super(e), this.helpUrl = "user-manual/dashboards_shape.htm", this.title = new qn, this.shapeType = new Zo, this._size = 1, this.fill = new v, this.stroke = N.black, this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new Ko
+                super(e), this.helpUrl = "user-manual/dashboards_shape.htm", this.title = new qn, this.shapeType = new Yo, this._size = 1, this.fill = new v, this.stroke = N.black, this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new Qo
             }
         }
-        F.Y.StiShapeElement = cm
+        F.Y.StiShapeElement = dm
     } {
         let e;
         (K = e = F.K.StiDataBarsDirection || (F.K.StiDataBarsDirection = {}))[K["LeftToRight"] = 0] = "LeftToRight", K[K["RighToLeft"] = 1] = "RighToLeft";
         let t;
         (Y = t = F.K.StiDataBarsBrushType || (F.K.StiDataBarsBrushType = {}))[Y["Solid"] = 0] = "Solid", Y[Y["Gradient"] = 1] = "Gradient";
         let r;
         (k = r = F.K.StiSparklinesType || (F.K.StiSparklinesType = {}))[k["Line"] = 0] = "Line", k[k["Area"] = 1] = "Area", k[k["Column"] = 2] = "Column", k[k["WinLoss"] = 3] = "WinLoss"
     } {
-        class iu {
+        class su {
             static getSelected(e) {
                 let t = this.hash.get(e.key);
                 if (null == t) return null;
                 return t.keys.cast().toList()
             }
             static getSelectedObjects(e) {
                 let t = this.getSelected(e);
                 return null != t ? t.cast() : null
             }
             static isSelected(e, t) {
                 let r = this.hash.get(e.key);
-                return null == r && (r = new Co, this.hash.set(e.key, r)), null != r.get(t)
+                return null == r && (r = new xo, this.hash.set(e.key, r)), null != r.get(t)
             }
             static select(e, t) {
                 let r = this.hash.get(e.key);
-                null == r && (r = new Co, this.hash.set(e.key, r)), r.set(t, t)
+                null == r && (r = new xo, this.hash.set(e.key, r)), r.set(t, t)
             }
             static resetSelection(e) {
                 this.hash.containsKey(e.key) && this.hash.remove(e.key)
             }
         }
-        iu.hash = new Co, F.h.StiTableElementSelection = iu
+        su.hash = new xo, F.h.StiTableElementSelection = su
     }
-    let Qo = L.Report.Dashboard.IStiAllowUserColumnSelectionDashboardInteraction,
-        qo = L.Report.Dashboard.IStiTableDashboardInteraction,
-        _o = L.Report.Dashboard.IStiAllowUserFilteringDashboardInteraction;
+    let qo = L.Report.Dashboard.IStiAllowUserColumnSelectionDashboardInteraction,
+        _o = L.Report.Dashboard.IStiTableDashboardInteraction,
+        $o = L.Report.Dashboard.IStiAllowUserFilteringDashboardInteraction;
     {
-        class eu extends F.g.StiDashboardInteraction {
+        class tu extends F.g.StiDashboardInteraction {
             implements() {
-                return eu.ImplementsIStiTableDashboardInteraction || (eu.ImplementsIStiTableDashboardInteraction = super.implements().concat([qo, An, Qo, _o, l, Gs])), eu.ImplementsIStiTableDashboardInteraction
+                return tu.ImplementsIStiTableDashboardInteraction || (tu.ImplementsIStiTableDashboardInteraction = super.implements().concat([_o, An, qo, $o, l, Gs])), tu.ImplementsIStiTableDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserColumnSelection", "", !0), new h("AllowUserSorting", "", !0), new h("AllowUserFiltering", "", !0), new h("DrillDownFiltered", "", !0), new h("FullRowSelect"), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout && this.allowUserColumnSelection && this.allowUserFiltering && this.allowUserSorting && this.drillDownFiltered && !this.fullRowSelect && super.isDefault()
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g, p, S, w) {
                 super(e, t, r, i, s, n, l), this.allowUserColumnSelection = !0, this.allowUserSorting = !0, this.allowUserFiltering = !0, this.drillDownFiltered = !0, this.fullRowSelect = !1, this.ident = Lr.Table, this.availableOnClick = Br.None, this.availableOnHover = Pr.None, this.availableOnDataManipulation = jr.AllowFiltering | jr.AllowSorting, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != u && (this.allowUserColumnSelection = u), null != a && (this.allowUserFiltering = a), null != o && (this.allowUserSorting = o), null != h && (this.drillDownFiltered = h), null != m && (this.fullRowSelect = m), null != c && (this.fileName = c), null != d && (this.headerText = d), null != g && (this.footerText = g), null != p && (this.showFullScreenButton = p), null != S && (this.showSaveButton = S), null != w && (this.showViewDataButton = w)
             }
         }
-        F.g.StiTableDashboardInteraction = eu
+        F.g.StiTableDashboardInteraction = tu
     }
-    let $o = L.Report.Dashboard.StiTableConditionPermissions;
+    let eu = L.Report.Dashboard.StiTableConditionPermissions;
     {
-        class nu {
+        class lu {
             implements() {
-                return nu.ImplementsStiTableElementCondition || (nu.ImplementsStiTableElementCondition = [Vt, _a, l]), nu.ImplementsStiTableElementCondition
+                return lu.ImplementsStiTableElementCondition || (lu.ImplementsStiTableElementCondition = [Vt, $a, l]), lu.ImplementsStiTableElementCondition
             }
             meta() {
-                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new s("KeyValueMeters").get(() => a.Serialize.stringArray(this.keyValueMeters)).set(e => this.keyValueMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyValueMeters = this.parseStringArray(e)), new s("KeyDataFieldMeters").get(() => a.Serialize.stringArray(this.keyDataFieldMeters)).set(e => this.keyValueMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyValueMeters = this.parseStringArray(e)), new s("KeyDestinationMeters").get(() => a.Serialize.stringArray(this.keyDestinationMeters)).set(e => this.keyDestinationMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyDestinationMeters = this.parseStringArray(e)), new i("DataType", "", F.a.StiFilterDataType, F.a.StiFilterDataType.Numeric), new i("Condition", "", nl, nl.EqualTo), new n("Value"), new h("IsExpression"), new i("Permissions", "", $o, $o.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("ForeColor", "", N.black), new r("BackColor", "", N.transparent)]
+                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new s("KeyValueMeters").get(() => a.Serialize.stringArray(this.keyValueMeters)).set(e => this.keyValueMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyValueMeters = this.parseStringArray(e)), new s("KeyDataFieldMeters").get(() => a.Serialize.stringArray(this.keyDataFieldMeters)).set(e => this.keyValueMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyValueMeters = this.parseStringArray(e)), new s("KeyDestinationMeters").get(() => a.Serialize.stringArray(this.keyDestinationMeters)).set(e => this.keyDestinationMeters = a.Deserialize.stringArray(e.value)).setXml(e => this.keyDestinationMeters = this.parseStringArray(e)), new i("DataType", "", F.a.StiFilterDataType, F.a.StiFilterDataType.Numeric), new i("Condition", "", nl, nl.EqualTo), new n("Value"), new h("IsExpression"), new i("Permissions", "", eu, eu.All), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new r("ForeColor", "", N.black), new r("BackColor", "", N.transparent)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -8510,57 +8508,57 @@
             get keyValueMeters() {
                 return this.keyDataFieldMeters
             }
             set keyValueMeters(e) {
                 this.keyDataFieldMeters = e, this.keyDestinationMeters = e
             }
             static createFromJson(e) {
-                let t = new nu;
+                let t = new lu;
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
-                let t = new nu;
+                let t = new lu;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n, l, a, o, u) {
-                this.keyDataFieldMeters = [], this.keyDestinationMeters = [], this.dataType = L.Report.Components.StiFilterDataType.Numeric, this.condition = L.Report.Components.StiFilterCondition.EqualTo, this.permissions = $o.All, this.font = new H("Arial", 8), this.foreColor = N.black, this.backColor = N.transparent, this.isExpression = !1, null != e && (this.keyDataFieldMeters = e), null != t && (this.keyDestinationMeters = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.permissions = n), null != l && (this.font = l), null != a && (this.foreColor = a), null != o && (this.backColor = o), null != u && (this.isExpression = u)
+                this.keyDataFieldMeters = [], this.keyDestinationMeters = [], this.dataType = L.Report.Components.StiFilterDataType.Numeric, this.condition = L.Report.Components.StiFilterCondition.EqualTo, this.permissions = eu.All, this.font = new H("Arial", 8), this.foreColor = N.black, this.backColor = N.transparent, this.isExpression = !1, null != e && (this.keyDataFieldMeters = e), null != t && (this.keyDestinationMeters = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.permissions = n), null != l && (this.font = l), null != a && (this.foreColor = a), null != o && (this.backColor = o), null != u && (this.isExpression = u)
             }
         }
-        F.K.StiTableElementCondition = nu
+        F.K.StiTableElementCondition = lu
     }
-    let eu = F.g.StiTableDashboardInteraction,
-        tu = L.Report.Dashboard.StiTableSizeMode,
-        ru = L.Report.Dashboard.ImplementsIStiTableElement,
-        iu = F.h.StiTableElementSelection,
-        su = L.Report.Dashboard.IStiTableElement,
-        nu = F.K.StiTableElementCondition;
+    let tu = F.g.StiTableDashboardInteraction,
+        ru = L.Report.Dashboard.StiTableSizeMode,
+        iu = L.Report.Dashboard.ImplementsIStiTableElement,
+        su = F.h.StiTableElementSelection,
+        nu = L.Report.Dashboard.IStiTableElement,
+        lu = F.K.StiTableElementCondition;
     {
         dt.add("StiTableElement", "Stimulsoft.Dashboard.Export.Tools.StiTableElementExportTool");
-        class fm extends F.e.StiElement {
+        class ym extends F.e.StiElement {
             implements() {
-                return fm.ImplementsStiTableElement || (fm.ImplementsStiTableElement = super.implements().concat([su, Ke, Ze, Oe, qs, Ne, ...ru, ...Qe, ...Ue, ...$s, ...Qs, l, Qr, ye])), fm.ImplementsStiTableElement
+                return ym.ImplementsStiTableElement || (ym.ImplementsStiTableElement = super.implements().concat([nu, Ke, Ze, Oe, qs, Ne, ...iu, ...Qe, ...Ue, ...$s, ...Qs, l, Qr, ye])), ym.ImplementsStiTableElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.columns = this.columns.select(e => e.clone()).toList(), i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.tableConditions = this.tableConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(Cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("HeaderForeColor", "", N.transparent), new r("FooterForeColor", "", N.transparent), new r("ForeColor", "", N.transparent), new n("HeaderFont").get(() => a.Serialize.fontArial8(this.headerFont)).set(e => this.headerFont = a.Deserialize.font(e.value, this.headerFont)).setXml(e => this.headerFont = L.System.Convert.toFont(e.textContent)), new n("FooterFont").get(() => a.Serialize.fontArial8(this.footerFont)).set(e => this.footerFont = a.Deserialize.font(e.value, this.footerFont)).setXml(e => this.footerFont = L.System.Convert.toFont(e.textContent)), new Rt("Font", "", "Arial", 10), new h("CrossFiltering", "", !0), new s("TableConditions").get(e => a.Serialize.objectArray(this.tableConditions.select(e => e[L.System.StiObject.stimulsoft]().as(nu)), e)).set(e => this.tableConditions.addRange(e.value.properties().select(e => nu.createFromJson(e.value)))).setXml(e => this.tableConditions.addRange(e.childNodes.select(e => nu.createFromXml(e)))), new s("Title").check(() => null != this.title), new s("Layout").check(() => null != this.layout), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(eu)).set(e => {
+                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(Cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("HeaderForeColor", "", N.transparent), new r("FooterForeColor", "", N.transparent), new r("ForeColor", "", N.transparent), new n("HeaderFont").get(() => a.Serialize.fontArial8(this.headerFont)).set(e => this.headerFont = a.Deserialize.font(e.value, this.headerFont)).setXml(e => this.headerFont = L.System.Convert.toFont(e.textContent)), new n("FooterFont").get(() => a.Serialize.fontArial8(this.footerFont)).set(e => this.footerFont = a.Deserialize.font(e.value, this.footerFont)).setXml(e => this.footerFont = L.System.Convert.toFont(e.textContent)), new Rt("Font", "", "Arial", 10), new h("CrossFiltering", "", !0), new s("TableConditions").get(e => a.Serialize.objectArray(this.tableConditions.select(e => e[L.System.StiObject.stimulsoft]().as(lu)), e)).set(e => this.tableConditions.addRange(e.value.properties().select(e => lu.createFromJson(e.value)))).setXml(e => this.tableConditions.addRange(e.childNodes.select(e => lu.createFromXml(e)))), new s("Title").check(() => null != this.title), new s("Layout").check(() => null != this.layout), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(tu)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(eu);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(tu);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(eu);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(tu);
                     null != r && (this.dashboardInteraction = r)
-                }), new i("Style", "", o, o.Auto), new i("SizeMode", "", tu, tu.AutoSize), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new se("RowsPerPage", "", 0), new se("PageTurnTime", "", 0)]
+                }), new i("Style", "", o, o.Auto), new i("SizeMode", "", ru, ru.AutoSize), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new se("RowsPerPage", "", 0), new se("PageTurnTime", "", 0)]
             }
             createMeters(e) {
-                let t = e.as(fm);
+                let t = e.as(ym);
                 this.columns.clear();
                 for (let e of t.columns) this.columns.add(e)
             }
             createMeters2(t) {
                 this.columns.clear();
                 for (let e of t.columns.list) null != e && null != e.type && Le.isNumericType(e.type) ? this.columns.add(d.Table.getMeasure2(e)) : this.columns.add(d.Table.getDimension2(e))
             }
@@ -8600,15 +8598,15 @@
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (this.columns.clear(), null == t) return;
                 t.cast().forEach(e => {
                     let t = null;
                     e.is2(ze) ? t = new F.K.StiDimensionColumn : e.is2(si) ? t = new F.K.StiSparklinesColumn : e.is2(ii) ? t = new F.K.StiDataBarsColumn : e.is2(ti) ? t = new F.K.StiIndicatorColumn : e.is2(ri) ? t = new F.K.StiColorScaleColumn : e.is2(Ar) ? t = new F.K.StiBubbleColumn : e.is2(vt) && ((t = new F.K.StiMeasureColumn).horAlignment = z.Right), null != t && (t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.columns.add(t))
-                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new eu)
+                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new tu)
             }
             fetchAllMeters() {
                 return this.columns.cast()
             }
             getMeters() {
                 return this.columns.cast()
             }
@@ -8653,15 +8651,15 @@
             }
             getAllStrings() {
                 let t = ["Title.Text"],
                     r = 0;
                 return this.columns.forEach(e => t.push(`Column${r++}.Label`)), t
             }
             addTableCondition(e, t, r, i, s, n, l, a, o, u) {
-                null == this.tableConditions && (this.tableConditions = new P), this.tableConditions.add(new nu(e, t, r, i, s, n, l, a, o, u))
+                null == this.tableConditions && (this.tableConditions = new P), this.tableConditions.add(new lu(e, t, r, i, s, n, l, a, o, u))
             }
             get toolboxPosition() {
                 return tt.TableElement
             }
             get localizedName() {
                 return A.get("Components", "StiTable")
             }
@@ -8676,21 +8674,21 @@
                 for (let e of this.columns)
                     if (null != (null === e || void 0 === e ? void 0 : e.dashboardInteraction) && e.dashboardInteraction.onClick != kr.None && (i = null == (t = null === e || void 0 === e ? void 0 : e.dashboardInteraction) ? void 0 : t.drillDownPageKey, pe.isKey(i))) {
                         let e = this.report.pages.toList().firstOrDefault(e => e.guid == i);
                         null != e && r.add(e)
                     } return 0 == r.length ? null : r.distinct()
             }
             getFormatObjects() {
-                return iu.getSelectedObjects(this)
+                return su.getSelectedObjects(this)
             }
             constructor(e = j.empty) {
-                super(e), this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.layout = new _s, this.group = "", this.foreColor = N.transparent, this.font = new H("Arial", 10), this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.tableConditions = new P, this.crossFiltering = !0, this.helpUrl = "user-manual/dashboards_table.htm", this.columns = new P, this.sizeMode = tu.AutoSize, this.rowsPerPage = 0, this.pageTurnTime = 0, this.currentPageIndex = -1, this.headerForeColor = N.transparent, this.headerFont = new H("Arial", 10), this.footerForeColor = N.transparent, this.footerFont = new H("Arial", 10), this.title.text = this.localizedName, this.dashboardInteraction = new eu
+                super(e), this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.layout = new _s, this.group = "", this.foreColor = N.transparent, this.font = new H("Arial", 10), this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.tableConditions = new P, this.crossFiltering = !0, this.helpUrl = "user-manual/dashboards_table.htm", this.columns = new P, this.sizeMode = ru.AutoSize, this.rowsPerPage = 0, this.pageTurnTime = 0, this.currentPageIndex = -1, this.headerForeColor = N.transparent, this.headerFont = new H("Arial", 10), this.footerForeColor = N.transparent, this.footerFont = new H("Arial", 10), this.title.text = this.localizedName, this.dashboardInteraction = new tu
             }
         }
-        F.K.StiTableElement = fm
+        F.K.StiTableElement = ym
     }
     F.K.StiTableElementConditionHelper = class {
         static async getConditionResult(i, t, s) {
             let e = !1;
             if (null != i) {
                 try {
                     if (t.dataType == L.Report.Components.StiFilterDataType.Numeric) {
@@ -8766,26 +8764,26 @@
             }
             return null
         }
         static async processBackColor(e, t, i, s, n) {
             for (let r of i.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let t = 0; t < n.length; t++) {
                     let e = n[t];
-                    if (0 <= r.keyDataFieldMeters.indexOf(e) && 0 < (r.permissions & $o.BackColor)) {
+                    if (0 <= r.keyDataFieldMeters.indexOf(e) && 0 < (r.permissions & eu.BackColor)) {
                         let e = s[t];
                         if (await this.getConditionResult(e, r, i)) return r.backColor
                     }
                 }
             return e
         }
         static async processForeColor(e, t, i, s, n) {
             for (let r of i.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let t = 0; t < n.length; t++) {
                     let e = n[t];
-                    if (0 <= r.keyDataFieldMeters.indexOf(e) && 0 < (r.permissions & $o.ForeColor)) {
+                    if (0 <= r.keyDataFieldMeters.indexOf(e) && 0 < (r.permissions & eu.ForeColor)) {
                         let e = s[t];
                         if (await this.getConditionResult(e, r, i)) return r.foreColor
                     }
                 }
             return e
         }
         static async processForeAndBackColor(e, t, r, s, n, l) {
@@ -8793,120 +8791,120 @@
                 foreColor: null,
                 backColor: null
             };
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(r)))
                 for (let r = 0; r < l.length; r++) {
                     let e = l[r],
                         t = n[r];
-                    if ((null == a.foreColor || null == a.backColor) && 0 <= i.keyDataFieldMeters.indexOf(e) && await this.getConditionResult(t, i, s) && (0 < (i.permissions & $o.ForeColor) && (a.foreColor = i.foreColor), 0 < (i.permissions & $o.BackColor)) && (a.backColor = i.backColor), null != a.backColor && null != a.foreColor) return a
+                    if ((null == a.foreColor || null == a.backColor) && 0 <= i.keyDataFieldMeters.indexOf(e) && await this.getConditionResult(t, i, s) && (0 < (i.permissions & eu.ForeColor) && (a.foreColor = i.foreColor), 0 < (i.permissions & eu.BackColor)) && (a.backColor = i.backColor), null != a.backColor && null != a.foreColor) return a
                 }
             return null == a.foreColor && (a.foreColor = e), null == a.backColor && (a.backColor = t), a
         }
         static async processFontStyle(e, t, i, s, n) {
             let l = hn.Regular;
             for (let r of i.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let t = 0; t < n.length; t++) {
                     let e = n[t];
                     if (0 <= r.keyDataFieldMeters.indexOf(e)) {
                         let e = s[t];
-                        await this.getConditionResult(e, r, i) && (0 < (r.permissions & $o.FontStyleBold) && r.font.bold && !(l & hn.Bold) && (l ^= hn.Bold), 0 < (r.permissions & $o.FontStyleItalic) && r.font.italic && !(l & hn.Italic) && (l ^= hn.Italic), 0 < (r.permissions & $o.FontStyleUnderline) && r.font.underline && !(l & hn.Underline) && (l ^= hn.Underline), 0 < (r.permissions & $o.FontStyleStrikeout)) && r.font.strikeout && !(l & hn.Strikeout) && (l ^= hn.Strikeout)
+                        await this.getConditionResult(e, r, i) && (0 < (r.permissions & eu.FontStyleBold) && r.font.bold && !(l & hn.Bold) && (l ^= hn.Bold), 0 < (r.permissions & eu.FontStyleItalic) && r.font.italic && !(l & hn.Italic) && (l ^= hn.Italic), 0 < (r.permissions & eu.FontStyleUnderline) && r.font.underline && !(l & hn.Underline) && (l ^= hn.Underline), 0 < (r.permissions & eu.FontStyleStrikeout)) && r.font.strikeout && !(l & hn.Strikeout) && (l ^= hn.Strikeout)
                     }
                 }
             return l
         }
         static async processFontStrikeout(e, t, s, n, l) {
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let r = 0; r < l.length; r++) {
                     let e = l[r],
                         t = n[r];
-                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & $o.FontStyleStrikeout) && await this.getConditionResult(t, i, s)) return i.font.strikeout
+                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & eu.FontStyleStrikeout) && await this.getConditionResult(t, i, s)) return i.font.strikeout
                 }
             return e
         }
         static async processFontUnderline(e, t, s, n, l) {
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let r = 0; r < l.length; r++) {
                     let e = l[r],
                         t = n[r];
-                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & $o.FontStyleUnderline) && await this.getConditionResult(t, i, s)) return i.font.underline
+                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & eu.FontStyleUnderline) && await this.getConditionResult(t, i, s)) return i.font.underline
                 }
             return e
         }
         static async processFontItalic(e, t, s, n, l) {
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let r = 0; r < l.length; r++) {
                     let e = l[r],
                         t = n[r];
-                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & $o.FontStyleItalic) && await this.getConditionResult(t, i, s)) return i.font.italic
+                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & eu.FontStyleItalic) && await this.getConditionResult(t, i, s)) return i.font.italic
                 }
             return e
         }
         static async processFontBold(e, t, s, n, l) {
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let r = 0; r < l.length; r++) {
                     let e = l[r],
                         t = n[r];
-                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & $o.FontStyleBold) && await this.getConditionResult(t, i, s)) return i.font.bold
+                    if (0 <= i.keyDataFieldMeters.indexOf(e) && 0 < (i.permissions & eu.FontStyleBold) && await this.getConditionResult(t, i, s)) return i.font.bold
                 }
             return e
         }
     }, F.ad.StiDataBarsColumnConverter = class extends ml {}, F.ad.StiDimensionColumnConverter = class extends ml {}, F.ad.StiSparklinesColumnConverter = class extends ml {}, F.ad.StiTableColumnConverter = class extends ml {}, F.g.StiTextDashboardInteraction = class extends F.g.StiDashboardInteraction {
         isDefault() {
             return this.onHover == Vr.ShowToolTip && this.onClick == kr.OpenHyperlink && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip)
         }
         constructor(e, t, r, i, s, n, l) {
             super(e, t, r, i, s, n, l), this.ident = Lr.Text, this.availableOnClick = Br.OpenHyperlink | Br.ShowDashboard, this.onClick = kr.OpenHyperlink
         }
     };
-    let lu = L.Report.StiParserType,
-        au = F.g.StiTextDashboardInteraction,
-        ou = L.Report.Dashboard.StiDashboardDesignAssembly,
-        uu = L.Report.Dashboard.ImplementsIStiTextElement,
-        hu = L.Report.Dashboard.IStiTextElement,
-        mu = L.Report.Components.IStiTextFont;
+    let au = L.Report.StiParserType,
+        ou = F.g.StiTextDashboardInteraction,
+        uu = L.Report.Dashboard.StiDashboardDesignAssembly,
+        hu = L.Report.Dashboard.ImplementsIStiTextElement,
+        mu = L.Report.Dashboard.IStiTextElement,
+        cu = L.Report.Components.IStiTextFont;
     {
         dt.add("StiTextElement", "Stimulsoft.Dashboard.Export.Tools.StiTextElementExportTool");
-        class bm extends F.e.StiElement {
+        class fm extends F.e.StiElement {
             implements() {
-                return bm.ImplementsStiTextElement || (bm.ImplementsStiTextElement = super.implements().concat([mu, Ke, Ze, fr, ur, or, hu, Oe, Ne, ...$r, ...Qe, ...Ue, ...Sr, ...sr, ...ir, ...uu, ...$s, l, Qr])), bm.ImplementsStiTextElement
+                return fm.ImplementsStiTextElement || (fm.ImplementsStiTextElement = super.implements().concat([cu, Ke, Ze, fr, ur, or, mu, Oe, Ne, ...$r, ...Qe, ...Ue, ...Sr, ...sr, ...ir, ...hu, ...$s, l, Qr])), fm.ImplementsStiTextElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.title = null != this.title ? this.title.clone() : null, s.shadow = null == (t = this.shadow) ? void 0 : t.clone(), s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.dashboardInteraction = null == (i = this.dashboardInteraction) ? void 0 : i.clone(), s
             }
             meta() {
                 return [...super.meta(), new le("HorAlignment"), new le("Padding"), new n("Group"), new n("Style"), new s("DashboardInteraction").check(() => null != this.dashboardInteraction).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(au);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(ou);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(au);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(ou);
                     null != r && (this.dashboardInteraction = r)
                 }), new s("Padding").get(() => this.padding.saveToJsonObject(0, 0, 0, 0)), new r("ForeColor", "", N.transparent), new n("Text"), new i("VertAlignment", "", Wt, Wt.Center), new i("SizeMode", "", Dt, Dt.Fit), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new h("RightToLeft", "", !1)]
             }
             get isDefined() {
                 return !B.isNullOrWhiteSpace(this.text)
             }
             get isQuerable() {
-                return Z.Engine.dashboardTextElementExpressionParser == lu.DataParser && !B.isNullOrEmpty(this.text) && this.text[L.System.StiObject.stimulsoft]().contains("{")
+                return Z.Engine.dashboardTextElementExpressionParser == au.DataParser && !B.isNullOrEmpty(this.text) && this.text[L.System.StiObject.stimulsoft]().contains("{")
             }
             fetchAllMeters() {
                 return this.getMeters()
             }
             getMeters() {
                 var e;
-                if (Z.Engine.dashboardTextElementExpressionParser == lu.ReportParser) return new P;
+                if (Z.Engine.dashboardTextElementExpressionParser == au.ReportParser) return new P;
                 if (B.isNullOrEmpty(this.text)) return null;
                 return null == (e = Rs.fetchBlocksFromExpression(this.text)) ? void 0 : e.select(e => new F.W.StiTextMeter(e, e, e)).cast().toList();
                 return null
             }
             retrieveUsedDataNames() {
-                return Z.Engine.dashboardTextElementExpressionParser == lu.ReportParser ? super.retrieveUsedDataNames() : en.getMany2(this.getMeters()).distinct().toList()
+                return Z.Engine.dashboardTextElementExpressionParser == au.ReportParser ? super.retrieveUsedDataNames() : en.getMany2(this.getMeters()).distinct().toList()
             }
             getSimpleText() {
                 return this.getHtmlTextHelper().getSimpleText(this.text, J.getForeColor(this))
             }
             getFont() {
                 let e = this.getHtmlTextHelper();
                 if (null == e) return null;
@@ -8986,50 +8984,50 @@
                 let t = this.dashboardInteraction.drillDownPageKey;
                 if (pe.isEmptyKey(t)) return null;
                 let e = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == e) return null;
                 return new P([e])
             }
             getHtmlTextHelper() {
-                return ou.getHtmlTextHelper()
+                return uu.getHtmlTextHelper()
             }
             constructor(e = j.empty) {
-                super(e), this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.text = "", this.rightToLeft = !1, this.group = "", this.foreColor = N.transparent, this.crossFiltering = !0, this.vertAlignment = Wt.Center, this.defaultClientRectangle = new j(0, 0, 100, 40), this.helpUrl = "user-manual/dashboards_text.htm", this.sizeMode = Dt.Fit, this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new au
+                super(e), this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.text = "", this.rightToLeft = !1, this.group = "", this.foreColor = N.transparent, this.crossFiltering = !0, this.vertAlignment = Wt.Center, this.defaultClientRectangle = new j(0, 0, 100, 40), this.helpUrl = "user-manual/dashboards_text.htm", this.sizeMode = Dt.Fit, this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0), this.dashboardInteraction = new ou
             }
         }
-        F.W.StiTextElement = bm
+        F.W.StiTextElement = fm
     } {
-        class Kg extends F.e.StiDimensionMeter {
+        class Qg extends F.e.StiDimensionMeter {
             implements() {
-                return Kg.ImplementsStiTextMeter || (Kg.ImplementsStiTextMeter = super.implements().concat([Er])), Kg.ImplementsStiTextMeter
+                return Qg.ImplementsStiTextMeter || (Qg.ImplementsStiTextMeter = super.implements().concat([Er])), Qg.ImplementsStiTextMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Text")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.TextMeter
             }
         }
-        F.W.StiTextMeter = Kg
+        F.W.StiTextMeter = Qg
     }
     F.aa.StiTextConverter = class {}, F.J.StiTreeItem = class {
         toString() {
             return null == this.key ? "" : this.key.toString()
         }
         constructor(e, t) {
             this.key = e, this.meter = t
         }
     };
-    let cu = L.Report.Dashboard.ImplementsIStiTreeViewElement,
-        du = L.Report.Dashboard.IStiTreeViewElement;
+    let du = L.Report.Dashboard.ImplementsIStiTreeViewElement,
+        gu = L.Report.Dashboard.IStiTreeViewElement;
     {
         dt.add("StiTreeViewElement", "Stimulsoft.Dashboard.Export.Tools.StiTreeViewElementExportTool");
-        class Sm extends F.e.StiElement {
+        class wm extends F.e.StiElement {
             implements() {
-                return Sm.ImplementsStiTreeViewElement || (Sm.ImplementsStiTreeViewElement = super.implements().concat([du, Ke, Ze, Oe, Ne, ...cu, ...Qe, ...Ue, ...$s, l])), Sm.ImplementsStiTreeViewElement
+                return wm.ImplementsStiTreeViewElement || (wm.ImplementsStiTreeViewElement = super.implements().concat([gu, Ke, Ze, Oe, Ne, ...du, ...Qe, ...Ue, ...$s, l])), wm.ImplementsStiTreeViewElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.keyMeters = this.keyMeters.select(e => e.clone()).toList(), i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.textFormat = this.textFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -9120,30 +9118,30 @@
             get localizedName() {
                 return A.get("Components", "StiTreeView")
             }
             constructor(e = j.empty) {
                 super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.Multi, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 300), this.helpUrl = "user-manual/dashboards_data_filtering_tree_view.htm", this.keyMeters = new P, this.title.text = this.localizedName, this.title.visible = !1
             }
         }
-        F.J.StiTreeViewElement = Sm
+        F.J.StiTreeViewElement = wm
     }
-    let gu = F.J.StiTreeItem,
-        pu = (F.J.StiTreeViewHelper = class {
+    let pu = F.J.StiTreeItem,
+        Su = (F.J.StiTreeViewHelper = class {
             static fetchItems(l, a) {
-                let t = new gu;
+                let t = new pu;
                 for (let e of l.rows) {
                     let s = 0,
                         n = t;
                     for (let i of e) {
                         let e = null == i,
                             t = "string" == typeof i ? B.isNullOrEmpty(i) : null == i,
                             r = e || t;
                         if (a || !r) {
                             let e = null != n.items ? n.items.firstOrDefault(e => e.key == i) : null;
-                            null == e && (e = new gu(i, l.meters[s]), null == n.items && (n.items = new P), n.items.add(e)), n = e
+                            null == e && (e = new pu(i, l.meters[s]), null == n.items && (n.items = new P), n.items.add(e)), n = e
                         }
                         s++
                     }
                 }
                 return t.items
             }
             static async fetchDefaultUserFilters(e) {
@@ -9178,21 +9176,21 @@
                 var r;
                 if (t instanceof w && !e.textFormat.is(Xr)) return t.toShortDateString();
                 let i = null == (r = null == e ? void 0 : e.report) ? void 0 : r.getParsedCulture();
                 if (li.isEligable(t, i)) return li.convert(t, i);
                 return e.textFormat.format(t)
             }
         }, L.Report.Dashboard.ImplementsIStiTreeViewBoxElement),
-        Su = F.J.StiTreeViewHelper,
-        wu = L.Report.Dashboard.IStiTreeViewBoxElement;
+        wu = F.J.StiTreeViewHelper,
+        bu = L.Report.Dashboard.IStiTreeViewBoxElement;
     {
         dt.add("StiTreeViewBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiTreeViewBoxElementExportTool");
-        class pm extends F.e.StiElement {
+        class Sm extends F.e.StiElement {
             implements() {
-                return pm.ImplementsStiTreeViewBoxElement || (pm.ImplementsStiTreeViewBoxElement = super.implements().concat([wu, Ke, Ze, lr, ...pu, ...Qe, ...Ue, ...tr, l])), pm.ImplementsStiTreeViewBoxElement
+                return Sm.ImplementsStiTreeViewBoxElement || (Sm.ImplementsStiTreeViewBoxElement = super.implements().concat([bu, Ke, Ze, lr, ...Su, ...Qe, ...Ue, ...tr, l])), Sm.ImplementsStiTreeViewBoxElement
             }
             meta() {
                 return [...super.meta(), new n("ParentKey"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
@@ -9207,15 +9205,15 @@
             getParentKey() {
                 return this.parentKey
             }
             setParentKey(e) {
                 this.parentKey = e
             }
             async applyDefaultFilters() {
-                let e = await Su.fetchDefaultUserFilters(this);
+                let e = await wu.fetchDefaultUserFilters(this);
                 null != e && (this.userFilters = e)
             }
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
@@ -9286,23 +9284,23 @@
                 return new W(0, t)
             }
             set maxSize(e) {}
             constructor(e = j.empty) {
                 super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.Multi, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_tree_view_box.htm", this.keyMeters = new P
             }
         }
-        F.I.StiTreeViewBoxElement = pm
+        F.I.StiTreeViewBoxElement = Sm
     }
-    let bu = L.Report.Dashboard.ImplementsIStiWebContentElement,
-        fu = L.Report.Dashboard.IStiWebContentElement;
+    let fu = L.Report.Dashboard.ImplementsIStiWebContentElement,
+        yu = L.Report.Dashboard.IStiWebContentElement;
     {
         dt.add("StiWebContentElement", "Stimulsoft.Dashboard.Export.Tools.StiWebContentElementExportTool");
-        class hm extends F.e.StiElement {
+        class mm extends F.e.StiElement {
             implements() {
-                return hm.ImplementsStiWebContentElement || (hm.ImplementsStiWebContentElement = super.implements().concat([fu, Ze, Ke, Oe, ...bu, ...Ue, ...Qe, ...$s, l])), hm.ImplementsStiWebContentElement
+                return mm.ImplementsStiWebContentElement || (mm.ImplementsStiWebContentElement = super.implements().concat([yu, Ze, Ke, Oe, ...fu, ...Ue, ...Qe, ...$s, l])), mm.ImplementsStiWebContentElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -9323,217 +9321,217 @@
             get localizedName() {
                 return A.get("Components", "StiWebContent")
             }
             constructor(e = j.empty) {
                 super(e), this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.defaultClientRectangle = new j(0, 0, 120, 120), this.helpUrl = "user-manual/dashboards_image.htm", this.title.text = this.localizedName, this.title.visible = !1, this.padding = nt.create(0)
             }
         }
-        F.Z.StiWebContentElement = hm
+        F.Z.StiWebContentElement = mm
     }
     F.k.StiInplaceDesigner = class {};
     {
         let e;
         (Q = e = F.r.StiRichTextAlignment || (F.r.StiRichTextAlignment = {}))[Q["Left"] = 1] = "Left", Q[Q["Right"] = 2] = "Right", Q[Q["Center"] = 3] = "Center", Q[Q["Justify"] = 4] = "Justify"
     }
-    let yu = L.Base.Drawing.StiFontUtils,
-        Cu = (F.r.StiRichBoxControl = class {
+    let Cu = L.Base.Drawing.StiFontUtils,
+        xu = (F.r.StiRichBoxControl = class {
             selectAll() {
                 this.selectedText = this.text
             }
             select(e, t) {
                 !B.isNullOrEmpty(this.text) && e < this.text.length && (this.selectedText = this.text.substr(e, t))
             }
             beginUpdate() {}
             endUpdate() {}
             setSelectionFont(e) {
-                return this.selectionFont = yu.changeFontName(this.selectionFont, e), !0
+                return this.selectionFont = Cu.changeFontName(this.selectionFont, e), !0
             }
             setSelectionSize(e) {
-                return this.selectionFont = yu.changeFontSize(this.selectionFont, e), !0
+                return this.selectionFont = Cu.changeFontSize(this.selectionFont, e), !0
             }
             setSelectionBold(e) {
-                return this.selectionFont = yu.changeFontStyleBold(this.selectionFont, e), !0
+                return this.selectionFont = Cu.changeFontStyleBold(this.selectionFont, e), !0
             }
             setSelectionItalic(e) {
-                return this.selectionFont = yu.changeFontStyleItalic(this.selectionFont, e), !0
+                return this.selectionFont = Cu.changeFontStyleItalic(this.selectionFont, e), !0
             }
             setSelectionUnderlined(e) {
-                return this.selectionFont = yu.changeFontStyleUnderline(this.selectionFont, e), !0
+                return this.selectionFont = Cu.changeFontStyleUnderline(this.selectionFont, e), !0
             }
             constructor() {
                 this.selectionFont = new H("Arial", 12), this.selectionColor = N.black, this.font = new H("Arial", 12), this.text = "", this.selectedText = ""
             }
         }, L.Base.Drawing.StiTextRenderer),
-        xu = F.r.StiRichTextAlignment,
-        Mu = L.System.Drawing.ColorTranslator,
-        Tu = L.Base.Drawing.StiHtmlState,
-        Fu = L.Base.Drawing.StiHtmlTagsState,
-        vu = F.r.StiRichBoxControl,
-        Au = (F.r.StiHtmlTextHelper = class {
+        Mu = F.r.StiRichTextAlignment,
+        Tu = L.System.Drawing.ColorTranslator,
+        Fu = L.Base.Drawing.StiHtmlState,
+        vu = L.Base.Drawing.StiHtmlTagsState,
+        Au = F.r.StiRichBoxControl,
+        Iu = (F.r.StiHtmlTextHelper = class {
             setFontName(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.setSelectionFont(r), this.getHtmlText(s, i)
             }
             setFontSize(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.setSelectionSize(Math.round(r)), this.getHtmlText(s, i)
             }
             growFontSize(e, t, r) {
-                let i = new vu;
+                let i = new Au;
                 return this.setHtmlText(t, e, i, r), i.selectAll(), i.setSelectionSize(Math.round(i.selectionFont.size + 1)), this.getHtmlText(i, r)
             }
             shrinkFontSize(e, t, r) {
-                let i = new vu;
+                let i = new Au;
                 return this.setHtmlText(t, e, i, r), i.selectAll(), 0 < i.selectionFont.size - 1 && i.setSelectionSize(Math.round(i.selectionFont.size - 1)), this.getHtmlText(i, r)
             }
             setFontBoldStyle(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.setSelectionBold(r), this.getHtmlText(s, i)
             }
             setFontItalicStyle(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.setSelectionItalic(r), this.getHtmlText(s, i)
             }
             setFontUnderlineStyle(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.setSelectionUnderlined(r), this.getHtmlText(s, i)
             }
             setColor(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.selectionColor = r, this.getHtmlText(s, i)
             }
             setHorAlignment(e, t, r, i) {
-                let s = new vu;
+                let s = new Au;
                 return this.setHtmlText(t, e, s, i), s.selectAll(), s.selectionAlignment = this.getAlignment(r), this.getHtmlText(s, i)
             }
             getFont(e, t, r) {
-                let i = new vu;
+                let i = new Au;
                 return this.setHtmlText(t, e, i, r), i.selectAll(), i.selectionFont
             }
             getColor(e, t, r) {
-                let i = new vu;
+                let i = new Au;
                 return this.setHtmlText(t, e, i, r), i.selectAll(), i.selectionColor
             }
             getHorAlign(e, t, r) {
-                let i = new vu;
+                let i = new Au;
                 return this.setHtmlText(t, e, i, r), i.selectAll(), this.getAlignment2(i.selectionAlignment)
             }
             setHtmlText(e, t, l, r) {
                 let i = "Arial",
                     s = 12,
-                    n = (l.selectAll(), l.setSelectionFont(i), l.setSelectionSize(s), new Fu(!1, !1, !1, !1, s, i, r, N.white, !1, !1, 0, 0, 0, X.Center)),
+                    n = (l.selectAll(), l.setSelectionFont(i), l.setSelectionSize(s), new vu(!1, !1, !1, !1, s, i, r, N.white, !1, !1, 0, 0, 0, X.Center)),
                     a = null,
-                    o = new Tu(n, 0),
-                    u = Cu.parseHtmlToStates(e, o, !1);
+                    o = new Fu(n, 0),
+                    u = xu.parseHtmlToStates(e, o, !1);
                 for (let n of u) {
                     let e = l.text.length,
                         t = (l.select(e, 0), null),
                         r = (t = B.isNullOrEmpty(n.ts.href) ? n.text.toString() : `<a href="${n.ts.href}">${n.text.toString()}</a>`, l.text += t, l.select(e, n.text.length), hn.Regular),
                         i = (n.ts.bold && (r |= hn.Bold), n.ts.italic && (r |= hn.Italic), n.ts.underline && (r |= hn.Underline), n.ts.fontName),
                         s = n.ts.fontSize;
-                    null == a && (a = l.font = new H(i, s)), l.selectionFont = yu.changeFontStyle2(i, s, r), l.selectionColor = n.ts.fontColor, l.selectionAlignment = this.getAlignment(n.ts.textAlign)
+                    null == a && (a = l.font = new H(i, s)), l.selectionFont = Cu.changeFontStyle2(i, s, r), l.selectionColor = n.ts.fontColor, l.selectionAlignment = this.getAlignment(n.ts.textAlign)
                 }
                 l.select(0, 0)
             }
             getHtmlText(a, o) {
                 let u = !1,
                     h = !1,
                     m = !1,
                     c = o,
                     d = "",
                     e = (a.selectAll(), null != a.selectionFont ? a.selectionFont.name : "Arial"),
                     t = null != a.selectionFont ? a.selectionFont.sizeInPoints : 12,
-                    r = ve.getName(xu, a.selectionAlignment);
+                    r = ve.getName(Mu, a.selectionAlignment);
                 d = d + `<font face="${e}" size="${t}">` + `<text-align="${r}">`;
                 for (let l = 0; l < a.text.length; l++) {
                     a.select(l, 1);
                     let e = a.selectionFont,
                         t = null != e && e.style & hn.Bold,
                         r = null != e && e.style & hn.Italic,
                         i = null != e && e.style & hn.Underline,
                         s = a.selectionColor,
                         n = "\n" == a.text[l];
-                    n && (d += "<br />"), t && !u && (u = !0, d += "<b>"), !t && u && (u = !1, d += "</b>"), r && !h && (h = !0, d += "<i>"), !r && h && (h = !1, d += "</i>"), i && !m && (m = !0, d += "<u>"), !i && m && (m = !1, d += "</u>"), c.equals(s) || (c = (c.equals(o) ? d += `<font-color="${Mu.toHtml(s)}">` : s.equals(o) ? d += "</font-color>" : d = (d += "</font-color>") + `<font-color="${Mu.toHtml(s)}">`, s)), d += a.text[l]
+                    n && (d += "<br />"), t && !u && (u = !0, d += "<b>"), !t && u && (u = !1, d += "</b>"), r && !h && (h = !0, d += "<i>"), !r && h && (h = !1, d += "</i>"), i && !m && (m = !0, d += "<u>"), !i && m && (m = !1, d += "</u>"), c.equals(s) || (c = (c.equals(o) ? d += `<font-color="${Tu.toHtml(s)}">` : s.equals(o) ? d += "</font-color>" : d = (d += "</font-color>") + `<font-color="${Tu.toHtml(s)}">`, s)), d += a.text[l]
                 }
                 return c.equals(o) || (d += "</font-color>"), m && (d += "</u>"), h && (d += "</i>"), u && (d += "</b>"), (d = d + "</text-align>" + "</font>").toString()
             }
             getAlignment(e) {
                 switch (e) {
                     case X.Left:
-                        return xu.Left;
+                        return Mu.Left;
                     case X.Center:
-                        return xu.Center;
+                        return Mu.Center;
                     case X.Right:
-                        return xu.Right;
+                        return Mu.Right;
                     case X.Width:
-                        return xu.Justify;
+                        return Mu.Justify;
                     default:
                         throw new Error("NotSupportedException")
                 }
             }
             getAlignment2(e) {
                 switch (e) {
-                    case xu.Left:
+                    case Mu.Left:
                         return X.Left;
-                    case xu.Center:
+                    case Mu.Center:
                         return X.Center;
-                    case xu.Right:
+                    case Mu.Right:
                         return X.Right;
-                    case xu.Justify:
+                    case Mu.Justify:
                         return X.Width;
                     default:
                         throw new Error("NotSupportedException")
                 }
             }
             getSimpleText(e, t) {
-                let r = new vu;
+                let r = new Au;
                 return this.setHtmlText(e, null, r, t), r.text
             }
         }, L.Report.Components.StiHtmlTextRender),
-        Iu = L.Report.Components.StiText,
-        Du = L.System.Drawing.StringTrimming,
-        Ru = L.System.Drawing.Text.HotkeyPrefix,
-        Eu = L.Base.Drawing.StiTextOptions,
-        Ou = (F.h.StiAutoSizeHtmlTextHelper = class {
+        Du = L.Report.Components.StiText,
+        Ru = L.System.Drawing.StringTrimming,
+        Eu = L.System.Drawing.Text.HotkeyPrefix,
+        Ou = L.Base.Drawing.StiTextOptions,
+        Vu = (F.h.StiAutoSizeHtmlTextHelper = class {
             static measure(e, t, r, i, s = null) {
                 let n = this.getTextScale(s, i),
                     l = (t.height = 1e3, new H("Arial", 12)),
-                    a = new Iu,
-                    o = (a.font = l, a.clientRectangle = t.clone(), a.text = r, Au.measureString(a));
+                    a = new Du,
+                    o = (a.font = l, a.clientRectangle = t.clone(), a.text = r, Iu.measureString(a));
                 return new W(o.width * n, o.height * n)
             }
             static getDefaultTextOptions() {
-                return new Eu(!1, !1, !1, 0, Ru.None, Du.None)
+                return new Ou(!1, !1, !1, 0, Eu.None, Ru.None)
             }
             static getTextScale(e, t) {
                 if (null != e) return e;
                 let r = t[L.System.StiObject.stimulsoft]().as(Fe);
                 return null != r && r.isDesigning ? t.zoom : 1
             }
         }, L.Base.Drawing.StiTextDrawing),
-        Vu = (F.h.StiAutoSizeTextHelper = class {
+        ku = (F.h.StiAutoSizeTextHelper = class {
             static toAlignment(e) {
                 switch (e) {
                     case z.Left:
                         return X.Left;
                     case z.Center:
                         return X.Center;
                     case z.Right:
                         return X.Right;
                     default:
                         throw new ca(e)
                 }
             }
             static measure(e, t, r) {
-                let i = Ou.measureString(e, t, r);
+                let i = Vu.measureString(e, t, r);
                 return new W(i.width, i.height)
             }
             static measure2(e, t, r, i) {
-                let s = new Eu,
-                    n = (s.angle = 0, s.wordWrap = !0, Ou.measureString(e, t, r, i, s));
+                let s = new Ou,
+                    n = (s.angle = 0, s.wordWrap = !0, Vu.measureString(e, t, r, i, s));
                 return new W(n.width, n.height)
             }
             static measureFontSize(e, t, r, i) {
                 let s = this.measure(e, t, i),
                     n = s.width > r.width ? r.width / s.width : 1,
                     l = s.height > r.height ? r.height / s.height : 1,
                     a = Math.min(Math.abs(n), Math.abs(l));
@@ -9545,59 +9543,59 @@
                 return t.rows.any() ? t.rows.min(e => V.tryToNumber(e[r])) : 0
             }
             static maxDataColumnValue(e, t, r) {
                 if (!(e.is2(Pi) || e.is2(Bi) || e.is2(Li))) return 0;
                 return t.rows.any() ? t.rows.max(e => V.tryToNumber(e[r])) : 0
             }
         }, L.Base.Context.StiLinesSegmentGeom),
-        ku = (F.j.StiVisual = class {
+        Nu = (F.j.StiVisual = class {
             async draw(e, t) {}
             drawArrowMore(e, t, r) {
                 let i = [],
-                    s = (i[0] = new Yl(t.right - 5 * r, t.bottom - 5 * r), i[1] = new Yl(t.right - 5 * r, t.bottom - 15 * r), i[2] = new Yl(t.right - 15 * r, t.bottom - 5 * r), new P([new Vu(i)]));
+                    s = (i[0] = new Yl(t.right - 5 * r, t.bottom - 5 * r), i[1] = new Yl(t.right - 5 * r, t.bottom - 15 * r), i[2] = new Yl(t.right - 15 * r, t.bottom - 5 * r), new P([new ku(i)]));
                 e.fillPath(N.fromArgb2(140, 140, 140), s, t.clone(), null)
             }
         }, L.Base.Context.StiFontGeom),
-        Nu = L.Base.Drawing.StiRotationMode,
-        Lu = (F.h.StiStringFormatHelper = class {
+        Lu = L.Base.Drawing.StiRotationMode,
+        Bu = (F.h.StiStringFormatHelper = class {
             static getStringFormatGeom(e) {
                 let t = e.getGenericStringFormat();
-                return t.trimming = Du.None, t.alignment = mn.Center, t.lineAlignment = mn.Center, t
+                return t.trimming = Ru.None, t.alignment = mn.Center, t.lineAlignment = mn.Center, t
             }
             static measureAlignmentParameters(e, t, r, i) {
                 switch (e) {
                     case z.Left:
-                        r.ref = Nu.LeftCenter, i.ref.x = t.x, i.ref.y = t.y + t.height / 2;
+                        r.ref = Lu.LeftCenter, i.ref.x = t.x, i.ref.y = t.y + t.height / 2;
                         break;
                     case z.Center:
-                        r.ref = Nu.CenterCenter, i.ref.x = t.x + t.width / 2, i.ref.y = t.y + t.height / 2;
+                        r.ref = Lu.CenterCenter, i.ref.x = t.x + t.width / 2, i.ref.y = t.y + t.height / 2;
                         break;
                     case z.Right:
-                        r.ref = Nu.RightCenter, i.ref.x = t.x + t.width, i.ref.y = t.y + t.height / 2;
+                        r.ref = Lu.RightCenter, i.ref.x = t.x + t.width, i.ref.y = t.y + t.height / 2;
                         break
                 }
             }
             static getFontSize(e, t, r, i) {
                 let s = new H(i.fontFamily.name, 25, i.style, i.unit),
-                    n = e.measureString(r, ku.create(s));
+                    n = e.measureString(r, Nu.create(s));
                 if (0 == n.width || 0 == n.height) return 0;
                 let l = t.width / n.width,
                     a = t.height / n.height,
                     o = a < l ? a : l;
                 return 25 * o
             }
         }, L.Report.Components.StiImageHelper),
-        Bu = L.Base.Context.StiLineSegmentGeom,
-        Pu = L.Report.Painters.StiWinLossSparklinesCellPainter,
-        ju = L.Report.Painters.StiLineSparklinesCellPainter,
-        Hu = L.Report.Painters.StiColumnSparklinesCellPainter,
-        zu = F.K.StiSparklinesType,
-        Gu = F.h.StiStringFormatHelper;
+        Pu = L.Base.Context.StiLineSegmentGeom,
+        ju = L.Report.Painters.StiWinLossSparklinesCellPainter,
+        Hu = L.Report.Painters.StiLineSparklinesCellPainter,
+        zu = L.Report.Painters.StiColumnSparklinesCellPainter,
+        Gu = F.K.StiSparklinesType,
+        Xu = F.h.StiStringFormatHelper;
     {
-        class Yu {
+        class Ku {
             static DataBarsDraw(t, e, r, i, s, n, l, a, o, u) {
                 let h = ts.formatBasedOnColumnType2(r, n.textFormat, n, a);
                 if (null == a || 0 == a) return;
                 0 < o && (o = 0), u < 0 && (u = 0);
                 let m = e.clone(),
                     c = (m.inflate(-1 * l, -1 * l), t.fillRectangle(N.fromArgb3(40, i.cellDataBarsPositive), m.clone(), null), u + Math.abs(o)),
                     d = m.width * Math.abs(o) / c,
@@ -9607,22 +9605,22 @@
                 if (S && (p = g), m.x += a < 0 ? d - p : d, m.width = p, 0 < m.width && 0 < m.height) {
                     let e = a < 0 ? i.cellDataBarsNegative : i.cellDataBarsPositive;
                     if (t.fillRectangle(e, m, null), S) {
                         let e = new j(m.right - 6 * l, m.y, 6 * l, m.height);
                         t.fillRectangle(i.cellDataBarsOverlapped, e, null)
                     }
                 }
-                let w = t.measureString(h, new ku(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point));
-                Yu.drawText(t, h, n.font, s, n.horAlignment, n.vertAlignment, e, w, l)
+                let w = t.measureString(h, new Nu(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point));
+                Ku.drawText(t, h, n.font, s, n.horAlignment, n.vertAlignment, e, w, l)
             }
             static colorScaleDraw(e, t, r, i, s, n, l, a, o, u) {
                 let h = ts.formatBasedOnColumnType2(r, n.textFormat, n, a),
                     m = this.getScaleColor(V.tryToNumber(a), o, u, i.cellBackColor, n.minimumColor, n.maximumColor),
                     c = t.clone(),
-                    d = (c.inflate(-1 * l, -1 * l), e.fillRectangle(m, c, null), e.measureString(h, new ku(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point)));
+                    d = (c.inflate(-1 * l, -1 * l), e.fillRectangle(m, c, null), e.measureString(h, new Nu(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point)));
                 this.drawText(e, h, n.font, s, n.horAlignment, n.vertAlignment, t, d, l)
             }
             static getScaleColor(t, r, i, s, n, l) {
                 let a = (i - r) / 2,
                     o = (t = Math.min(t, i), 0),
                     u, h;
                 if (a < (t = Math.max(t, r))) {
@@ -9639,25 +9637,25 @@
                 return e = Math.min(e, 255), m = Math.min(m, 255), c = Math.min(c, 255), d = Math.min(d, 255), e = Math.max(e, 0), m = Math.max(m, 0), c = Math.max(c, 0), d = Math.max(d, 0), N.fromArgb(Math.round(e), Math.round(m), Math.round(c), Math.round(d))
             }
             static sparklinesDraw(t, r, i, e, s) {
                 let n = this.castToArray(e);
                 if (null != n) {
                     let e = n[L.System.StiObject.stimulsoft]().toList();
                     switch (i.type) {
-                        case zu.Column:
-                            Hu.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, i.allowCustomColors ? i.negativeColor : s.cellSparkline);
+                        case Gu.Column:
+                            zu.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, i.allowCustomColors ? i.negativeColor : s.cellSparkline);
                             break;
-                        case zu.Line:
-                            ju.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, !1, i.showFirstLastPoints, i.showHighLowPoints);
+                        case Gu.Line:
+                            Hu.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, !1, i.showFirstLastPoints, i.showHighLowPoints);
                             break;
-                        case zu.Area:
-                            ju.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, !0, i.showFirstLastPoints, i.showHighLowPoints);
+                        case Gu.Area:
+                            Hu.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellSparkline, !0, i.showFirstLastPoints, i.showHighLowPoints);
                             break;
-                        case zu.WinLoss:
-                            Pu.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellWinLossPositive, i.allowCustomColors ? i.negativeColor : s.cellWinLossNegative);
+                        case Gu.WinLoss:
+                            ju.draw(t, r, e, i.allowCustomColors ? i.positiveColor : s.cellWinLossPositive, i.allowCustomColors ? i.negativeColor : s.cellWinLossNegative);
                             break;
                         default:
                             throw new ca(i.type)
                     }
                 }
             }
             static castToArray(e) {
@@ -9666,15 +9664,15 @@
             static bubbleDraw(i, r, e, s, n, l, a, o, t, u, h = !0) {
                 if (0 == o) return;
                 let m = ts.formatBasedOnColumnType2(e, l.textFormat, l, o),
                     c = (0 < t && (t = 0), u < 0 && (u = 0), l.horAlignment),
                     d = r.clone();
                 if (d.inflate(-1, -1), d = this.calculateBubbleRect(d, l, Math.abs(o), t, u, a), h && c != z.Center) {
                     let e = l.horAlignment == z.Left ? z.Right : z.Left,
-                        t = i.measureString(m, new ku(l.font.fontFamily.name, l.font.size, l.font.style, L.System.Drawing.GraphicsUnit.Point));
+                        t = i.measureString(m, new Nu(l.font.fontFamily.name, l.font.size, l.font.style, L.System.Drawing.GraphicsUnit.Point));
                     this.drawText(i, m, l.font, n, e, l.vertAlignment, r, t, a)
                 }
                 if (0 < d.width && 0 < d.height) {
                     let e = l.allowCustomColors ? l.positiveColor : s.cellDataBarsPositive,
                         t = l.allowCustomColors ? l.negativeColor : s.cellDataBarsNegative,
                         r = o < 0 ? t : e;
                     i.fillEllipse(r, d.x, d.y, d.width, d.height, null)
@@ -9698,16 +9696,16 @@
             }
             static indicatorDraw(e, t, r, i, s, n, l) {
                 let a = this.getCellText(r, s, l),
                     o = F.t.StiCardsVisual.getFontGeom(s.font, n),
                     u = e.measureString(a, o).width,
                     h = this.calculateIndicatorRect(t, s, n, u, r.isExporting),
                     m = (this.drawIndicator(e, h, l, i, r.isExporting), this.getColor(s.foreColor, l, i)),
-                    c = Yu.calculateTextRect(t, s, n, u, r.isExporting),
-                    d = e.measureString(a, new ku(s.font.fontFamily.name, s.font.size, s.font.style, L.System.Drawing.GraphicsUnit.Point));
+                    c = Ku.calculateTextRect(t, s, n, u, r.isExporting),
+                    d = e.measureString(a, new Nu(s.font.fontFamily.name, s.font.size, s.font.style, L.System.Drawing.GraphicsUnit.Point));
                 this.drawText(e, a, s.font, m, s.horAlignment, s.vertAlignment, c, d, n)
             }
             static calculateTextRect(e, t, r, i, s) {
                 let n = this.calculateIndicatorRect(e, t, r, i, s),
                     l = 2 * n.width;
                 switch (this.getHorAlignment(t)) {
                     case z.Left:
@@ -9754,40 +9752,40 @@
                 let g = Math.min(m.width, m.height);
                 if (null == c || 0 == c) h.fillRectangle(d.cellIndicatorNeutral, new j(m.x + (m.width - g) / 2, m.y + (m.height - 4) / 2, g, 5), null);
                 else {
                     let e = .75 * g,
                         t = (m = new j(m.x + (m.width - g) / 2, m.y + (m.height - e) / 2, g, e)).width / 2,
                         r, i, s, n = (s = 0 < c ? (r = new Yl(m.left + t, m.top), i = new Yl(m.left, m.bottom), new Yl(m.right, m.bottom)) : (r = new Yl(m.left + t, m.bottom), i = new Yl(m.left, m.top), new Yl(m.right, m.top)), 0 < c ? d.cellIndicatorPositive : d.cellIndicatorNegative),
                         l = new P,
-                        a = new Bu(r, i),
-                        o = new Bu(i, s),
-                        u = new Bu(s, r);
+                        a = new Pu(r, i),
+                        o = new Pu(i, s),
+                        u = new Pu(s, r);
                     l.add(a), l.add(o), l.add(u), h.fillPath(n, l, m, null)
                 }
             }
             static imageDraw(e, t, r) {
-                let i = Lu.getImageBytesFromObject(r);
+                let i = Bu.getImageBytesFromObject(r);
                 e.drawImage(i, t)
             }
             static drawWordWrapText(e, t, r, i, s, n, l, a, o) {
                 let u = e.getGenericStringFormat();
-                switch (u.trimming = Du.None, u.lineAlignment = mn.Center, s) {
+                switch (u.trimming = Ru.None, u.lineAlignment = mn.Center, s) {
                     case z.Left:
                         u.alignment = mn.Near;
                         break;
                     case z.Center:
                         u.alignment = mn.Center;
                         break;
                     case z.Right:
                         u.alignment = mn.Far;
                         break
                 }
                 let h = 0,
                     m = (l.width < a.width ? l : a).width,
-                    c = Nu.CenterCenter;
+                    c = Lu.CenterCenter;
                 switch (s) {
                     case z.Left:
                         h = l.x;
                         break;
                     case z.Center:
                         h = l.x + l.width / 2 - m / 2;
                         break;
@@ -9808,15 +9806,15 @@
                         break
                 }
                 let g = new j(h, d, m, a.height),
                     p = F.t.StiCardsVisual.getFontGeom(r, o);
                 e.drawRotatedString6(t, p, i, g, u, c, 0, !0, l.width)
             }
             static drawText(e, t, r, i, s, n, l, a, o) {
-                let u = Gu.getStringFormatGeom(e),
+                let u = Xu.getStringFormatGeom(e),
                     h = (u.alignment = mn.Far, 0),
                     m = (l.width < a.width ? l : a).width;
                 switch (s) {
                     case z.Left:
                         h = l.x;
                         break;
                     case z.Center:
@@ -9851,29 +9849,29 @@
                             if (4 < e.length) return e.substring(0, e.length - 3) + "...";
                             if (1 < e.length) return e.substring(0, 1) + "..."
                         }
                     }
                 return i
             }
         }
-        F.t.StiCardsCellDrawer = Yu
+        F.t.StiCardsCellDrawer = Ku
     }
-    let Xu = L.Data.Extensions.ListExt,
-        Wu = F.e.StiMeterIdent,
-        Ju = L.Report.Painters.StiContextRoundedRectangleCreator,
-        Uu = L.Base.Context.StiContextPainter,
-        Zu = L.Report.Dashboard.Helpers.StiElementScale,
+    let Wu = L.Data.Extensions.ListExt,
+        Ju = F.e.StiMeterIdent,
+        Uu = L.Report.Painters.StiContextRoundedRectangleCreator,
+        Zu = L.Base.Context.StiContextPainter,
+        Yu = L.Report.Dashboard.Helpers.StiElementScale,
         U = L.Base.Dashboard.StiElementConsts,
-        Yu = F.t.StiCardsCellDrawer,
-        Ku = L.Base.Context.StiPenGeom,
-        Qu = F.F.StiCardsColumnVisibilityHelper,
-        qu = F.h.StiCardsElementHelper,
-        _u = L.Base.Context.StiContext;
+        Ku = F.t.StiCardsCellDrawer,
+        Qu = L.Base.Context.StiPenGeom,
+        qu = F.F.StiCardsColumnVisibilityHelper,
+        _u = F.h.StiCardsElementHelper,
+        $u = L.Base.Context.StiContext;
     {
-        class $u extends F.j.StiVisual {
+        class eh extends F.j.StiVisual {
             async draw(e, t) {
                 this.paintCards(e, t)
             }
             paintCards(s, n) {
                 let l = s.options.zoom,
                     a = this.dataTable.meters.where(e => e.is(Mr)).cast().toList(),
                     o = J.getCardsStyle(this.element),
@@ -9881,53 +9879,53 @@
                     t = {},
                     u = (this.getCardRectanglesList(a, n, l, e, t), e.ref),
                     h = t.ref,
                     m = new P,
                     c = new P;
                 for (let i = 0; i < a.length; i++) {
                     let e = a[i],
-                        t = qu.minDataColumnValue(e, this.dataTable, i),
-                        r = qu.maxDataColumnValue(e, this.dataTable, i);
+                        t = _u.minDataColumnValue(e, this.dataTable, i),
+                        r = _u.maxDataColumnValue(e, this.dataTable, i);
                     m.add(t), c.add(r)
                 }
                 let d;
                 for (let i = 0; i < this.dataTable.rows.length; i++) {
                     let e = this.dataTable.rows[i],
                         t = u[i],
                         r = h[i];
                     !d && (1 < t.right - n.right || 1 < t.bottom - n.bottom) && (d = !0), this.paintCardItem(s, t, this.element, i, r, a, e, m, c, o, l)
                 }
                 if (d) {
-                    let e = Zu.factor(this.element);
+                    let e = Yu.factor(this.element);
                     this.drawArrowMore(s, n, e)
                 }
             }
             getCardRectanglesList(s, e, n, t, r) {
                 let i = new P,
                     l = new P,
-                    a = new Uu,
-                    o = new _u(a, !0, !1, !1, n),
+                    a = new Zu,
+                    o = new $u(a, !0, !1, !1, n),
                     u = 0,
                     h = 0;
                 for (let i of this.dataTable.rows) {
                     let e = {
                             ref: new P
                         },
-                        t = $u.measureCards(o, this.element, s, i, e, n),
+                        t = eh.measureCards(o, this.element, s, i, e, n),
                         r = e.ref;
                     u = Math.max(u, t.width), h = Math.max(h, t.height), l.add(r)
                 }
                 if (0 < this.element.columnCount && this.element.orientation == L.Report.Dashboard.StiItemOrientation.Horizontal ? u = e.width / this.element.columnCount : 0 < this.element.columnCount && this.element.orientation == L.Report.Dashboard.StiItemOrientation.Vertical && (h = e.height / this.element.columnCount), 0 == this.element.columnCount && this.element.orientation == L.Report.Dashboard.StiItemOrientation.Horizontal && (u = Math.max(u, e.width / this.dataTable.rows.length)), s.any(e => e.wordWrap)) {
                     l.clear();
                     for (let i of this.dataTable.rows) {
                         let e = {
                                 ref: new P
                             },
                             t = u - this.element.cards.margin.left * n - this.element.cards.margin.right * n - this.element.cards.padding.left * n - this.element.cards.padding.right * n,
-                            r = $u.measureCards2(o, this.element, s, i, e, n, t);
+                            r = eh.measureCards2(o, this.element, s, i, e, n, t);
                         h = Math.max(h, r.height), l.add(e.ref)
                     }
                 }
                 i = this.element.orientation == L.Report.Dashboard.StiItemOrientation.Horizontal ? this.getRectanglesHorizontalOrientation(e, u, h) : this.getRectanglesVerticalOrientation(e, u, h), t.ref = i, r.ref = l
             }
             getRectanglesHorizontalOrientation(t, r, i) {
                 let s = new P,
@@ -9963,15 +9961,15 @@
                 for (let e of s) n = j.union(e, n);
                 return n
             }
             paintCardItem(g, p, S, t, n, w, b, f, y, C, x) {
                 let r = new j(p.x + S.cards.margin.left * x, p.y + S.cards.margin.top * x, p.width - S.cards.margin.left * x - S.cards.margin.right * x, p.height - S.cards.margin.top * x - S.cards.margin.bottom * x);
                 if (g.pushClip(r), null == S.cards.cornerRadius || S.cards.cornerRadius.isEmpty) g.fillRectangle(this.getColor(t), r, null);
                 else {
-                    let e = Ju.create(r, S.cards.cornerRadius, x);
+                    let e = Uu.create(r, S.cards.cornerRadius, x);
                     g.fillPath(this.getColor(t), e, r, null)
                 }
                 let i = new P,
                     s = new P;
                 for (let t = 0; t < w.length; t++) {
                     let e = w[t];
                     s.add(t), !e.wrapLine && t != w.length - 1 || (i.add(s), s = new P)
@@ -9983,44 +9981,44 @@
                         let e = s[r],
                             t = n[e];
                         M.add(new j(i * r, t.y, i, t.height))
                     }
                 }
                 for (let d = 0; d < b.length; d++) {
                     let n = w[d],
-                        e = Qu.getVisible(n, S.report);
+                        e = qu.getVisible(n, S.report);
                     if (!e) continue;
                     let l = b[d],
                         t = f[d],
                         r = y[d],
-                        a = $u.getForeColor(S, w[d], C),
+                        a = eh.getForeColor(S, w[d], C),
                         o = n.font,
                         i = M[d],
                         s = p.x + S.cards.margin.left * x + S.cards.padding.left * x + i.x,
                         u = p.y + S.cards.margin.top * x + S.cards.padding.top * x + i.y,
                         h = i.width,
                         m = i.height - S.cards.padding.top * x - S.cards.padding.bottom * x,
                         c = new j(s, u, h, m);
                     if (n.is2(Pi)) {
                         let e = n.as(Pi);
-                        Yu.DataBarsDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
+                        Ku.DataBarsDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
                     } else if (n.is2(Bi)) {
                         let e = n.as(Bi);
-                        Yu.colorScaleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
+                        Ku.colorScaleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
                     } else if (n.is2(ji)) {
                         let e = n.as(ji);
-                        Yu.sparklinesDraw(g, c, e, l, C)
+                        Ku.sparklinesDraw(g, c, e, l, C)
                     } else if (n.is2(Li)) {
                         let e = n.as(Li);
-                        Yu.bubbleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
+                        Ku.bubbleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
                     } else if (n.is2(Ni)) {
                         let e = n.as(Ni);
-                        Yu.indicatorDraw(g, c, S, C, e, x, V.tryToNullableNumber(l))
+                        Ku.indicatorDraw(g, c, S, C, e, x, V.tryToNullableNumber(l))
                     } else {
-                        let s = Lu.getImageFromObject(l);
+                        let s = Bu.getImageFromObject(l);
                         if (null != s && null != s.height) {
                             let e = c.height / s.height,
                                 t = s.width * e,
                                 r = 0;
                             switch (n.horAlignment) {
                                 case z.Left:
                                     r = c.x;
@@ -10029,58 +10027,58 @@
                                     r = c.x + (c.width - t) / 2;
                                     break;
                                 case z.Right:
                                     r = c.x + c.width - t;
                                     break
                             }
                             let i = new j(r, c.y, t, c.height);
-                            Yu.imageDraw(g, i, l)
+                            Ku.imageDraw(g, i, l)
                         } else {
                             let e = this.processRowValue(l, n),
                                 r = ts.formatBasedOnColumnType2(S, n.textFormat, n, e),
                                 t = n.as(_t),
-                                i = new ku(o.fontFamily.name, o.size, o.style, L.System.Drawing.GraphicsUnit.Point);
+                                i = new Nu(o.fontFamily.name, o.size, o.style, L.System.Drawing.GraphicsUnit.Point);
                             if (null != t && t.wordWrap) {
                                 let e = g.getGenericStringFormat(),
-                                    t = (e.trimming = Du.None, e.alignment = mn.Center, e.lineAlignment = mn.Center, g.measureString2(r, i, c.width, e));
-                                Yu.drawWordWrapText(g, r, o, a, n.horAlignment, n.vertAlignment, c, t, x)
+                                    t = (e.trimming = Ru.None, e.alignment = mn.Center, e.lineAlignment = mn.Center, g.measureString2(r, i, c.width, e));
+                                Ku.drawWordWrapText(g, r, o, a, n.horAlignment, n.vertAlignment, c, t, x)
                             } else {
                                 let e = g.measureString(r, i);
-                                Yu.drawText(g, r, o, a, n.horAlignment, n.vertAlignment, c, e, x)
+                                Ku.drawText(g, r, o, a, n.horAlignment, n.vertAlignment, c, e, x)
                             }
                         }
                     }
                 }
                 g.popClip();
-                let l = new Ku(C.lineColor, 1);
+                let l = new Qu(C.lineColor, 1);
                 if (null == S.cards.cornerRadius || S.cards.cornerRadius.isEmpty) g.drawRectangle(l, r);
                 else {
-                    let e = Ju.create(r, S.cards.cornerRadius, x);
+                    let e = Uu.create(r, S.cards.cornerRadius, x);
                     g.drawPath(l, e, r)
                 }
             }
             processRowValue(e, t) {
                 var r;
-                let i = t.ident == Wu.SparklinesColumn;
-                return e = Xu.isList(e) ? i ? Xu.toList(e) : null == (r = Xu.toList(e)) ? void 0 : r.firstOrDefault() : e
+                let i = t.ident == Ju.SparklinesColumn;
+                return e = Wu.isList(e) ? i ? Wu.toList(e) : null == (r = Wu.toList(e)) ? void 0 : r.firstOrDefault() : e
             }
             static measureItem(i, s, n, l, a, o) {
                 let u;
                 if (n.is2(Pi) || n.is2(Bi)) u = this.measureDataBarsCell(i, s, n, l, a);
                 else if (n.is2(ji)) {
                     let e = n.as(ji);
                     u = this.measureSparklinesCell(e, a)
                 } else if (n.is2(Ni)) {
                     let e = n.as(Ni);
                     u = this.measureIndicatorCell(i, s, e, l, a)
                 } else if (n.is2(Li)) {
                     let e = n.as(Li);
                     u = this.measureBubbleCell(i, s, e, l, a)
-                } else if (Lu.isImage(l)) {
-                    let e = Lu.getImageFromObject(l),
+                } else if (Bu.isImage(l)) {
+                    let e = Bu.getImageFromObject(l),
                         t = 50 * a,
                         r = t / e.height,
                         i = e.width * r;
                     u = new W(i, t)
                 } else {
                     let t = ts.formatBasedOnColumnType2(s, n.textFormat, n, l),
                         r = this.getFontGeom(n.font, a),
@@ -10106,15 +10104,15 @@
                     let e = n[t];
                     i.add(t), !e.wrapLine && t != l.length - 1 || (r.add(i), i = new P)
                 }
                 let c = new P;
                 for (let i = 0; i < l.length; i++) {
                     let e = n[i],
                         t = l[i],
-                        r = Qu.getVisible(e, o.report);
+                        r = qu.getVisible(e, o.report);
                     r || c.add(W.empty), c.add(this.measureItem(s, o, e, t, u, a))
                 }
                 for (let e = 0; e < r.length; e++) {
                     let s = r[e],
                         i = 0,
                         n = 0;
                     for (let r = 0; r < s.length; r++) {
@@ -10131,26 +10129,26 @@
                         a += t.width, h.add(r)
                     }
                     t = Math.max(t, l.width + o.cards.padding.left * u + o.cards.padding.right * u), m += l.height
                 }
                 return e.ref = h, new W(t, m + o.cards.padding.top * u + o.cards.padding.bottom * u + o.cards.margin.top * u + o.cards.margin.bottom * u)
             }
             static measureDataBarsCell(e, t, r, i, s) {
-                let n = Yu.getCellText(t, r, V.tryToNullableNumber(i)),
+                let n = Ku.getCellText(t, r, V.tryToNullableNumber(i)),
                     l = this.getFontGeom(r.font, s),
                     a = e.measureString(n, l);
                 return new W(a.width, 1.5 * a.height)
             }
             static measureSparklinesCell(e, t) {
                 let r = 0 == e.height ? 20 : e.height;
                 return new W(0, r * t)
             }
             static measureIndicatorCell(e, t, r, i, s) {
                 let n = r.as(Ni),
-                    l = Yu.getCellText(t, n, V.tryToNullableNumber(i)),
+                    l = Ku.getCellText(t, n, V.tryToNullableNumber(i)),
                     a = this.getFontGeom(r.font, s),
                     o = e.measureString(l, a);
                 return new W(o.width, 1.5 * o.height)
             }
             static measureBubbleCell(e, t, r, i, s) {
                 let n = ts.formatBasedOnColumnType2(t, r.textFormat, r, i),
                     l = this.getFontGeom(r.font, s),
@@ -10161,66 +10159,66 @@
                 if (!t.foreColor.equals(N.transparent)) return t.foreColor;
                 let i = J.getForeColor(e);
                 if (!i.equals(N.transparent)) return i;
                 if (null != r) return r.cellForeColor;
                 return U.Table.Font.Color
             }
             static getFontGeom(e, t) {
-                let r = ku.changeFontSize(e, e.size * t);
+                let r = Nu.changeFontSize(e, e.size * t);
                 return r
             }
             getColor(e) {
                 return this.element.cards.colorEach ? this.getStyleColor(e) : this.style.cellBackColor
             }
             getStyleColor(e) {
                 let t = (null != this.element.seriesColors && 0 < this.element.seriesColors.length ? this.element : J.getCardsStyle(this.element)).seriesColors;
                 return t[e %= t.length]
             }
             constructor(e, t) {
                 super(), this.element = e, this.dataTable = t, this.style = J.getCardsStyle(this.element)
             }
         }
-        F.t.StiCardsVisual = $u
+        F.t.StiCardsVisual = eh
     }
-    let $u = F.t.StiCardsVisual,
-        eh = L.Report.Dashboard.Visuals.IStiCardsVisualSvgHelper,
-        th = L.Report.Dashboard.IStiManuallyEnteredData,
-        rh = L.Report.Export.Services.Helpers.StiContextSvgHelper;
+    let eh = F.t.StiCardsVisual,
+        th = L.Report.Dashboard.Visuals.IStiCardsVisualSvgHelper,
+        rh = L.Report.Dashboard.IStiManuallyEnteredData,
+        ih = L.Report.Export.Services.Helpers.StiContextSvgHelper;
     {
-        class Qg {
+        class qg {
             implements() {
-                return Qg.ImplementsStiCardsVisualSvgHelper || (Qg.ImplementsStiCardsVisualSvgHelper = [eh]), Qg.ImplementsStiCardsVisualSvgHelper
+                return qg.ImplementsStiCardsVisualSvgHelper || (qg.ImplementsStiCardsVisualSvgHelper = [th]), qg.ImplementsStiCardsVisualSvgHelper
             }
             async writeCards(e, t, r, i, s) {
                 let n = new j(0, 0, t.width, t.height),
                     l = t.component.as(F.F.StiCardsElement),
-                    a = await Qg.getDataTable(l);
+                    a = await qg.getDataTable(l);
                 if (null == a) return;
-                let o = new Uu,
-                    u = new _u(o, !0, !1, !1, 1),
-                    h = new $u(l, a);
+                let o = new Zu,
+                    u = new $u(o, !0, !1, !1, 1),
+                    h = new eh(l, a);
                 if (r && (r.needToVertScroll || r.needToHorScroll)) {
                     let e = h.getContentRectangle(n);
                     r.needToVertScroll = e.height > n.height + 5, r.needToHorScroll = e.width > n.width + 5, r.needToVertScroll && (n.width -= 15, e = h.getContentRectangle(n), n = e, r.needToHorScroll || (n.height += 10), i.ref = L.System.Convert.toInt32(n.height)), r.needToHorScroll && (n.height -= 15, e = h.getContentRectangle(n), n = e, r.needToVertScroll || (n.height += 10), s.ref = L.System.Convert.toInt32(n.width))
                 }
                 await h.draw(u, n.clone()), e.writeStartElement("g");
                 let m = r && (r.needToVertScroll || r.needToHorScroll) ? 0 : t.x,
                     c = r && (r.needToVertScroll || r.needToHorScroll) ? 0 : t.y;
-                e.writeAttributeString("transform", `translate(${m},${c})`), rh.writeGeoms(e, u, !1), e.writeEndElement()
+                e.writeAttributeString("transform", `translate(${m},${c})`), ih.writeGeoms(e, u, !1), e.writeEndElement()
             }
             static async getDataTable(e) {
                 var t;
-                let r = null == (t = e.as(th)) ? void 0 : t.getManuallyEnteredDataTable();
+                let r = null == (t = e.as(rh)) ? void 0 : t.getManuallyEnteredDataTable();
                 if (null != r) return r;
                 return bl.tryToGetOrCreate(e)
             }
         }
-        F.h.StiCardsVisualSvgHelper = Qg
+        F.h.StiCardsVisualSvgHelper = qg
     } {
-        class Dc {
+        class Rc {
             static getSumRectangle(t) {
                 let r = new j(0, 0, 0, 0);
                 for (let e of t) e.right > r.right && (r = new j(r.x, r.y, e.right - r.x, r.height)), e.bottom > r.bottom && (r = new j(r.x, r.y, r.width, e.bottom - r.y));
                 return r
             }
             static getLocationRectangles(t, r, e) {
                 if (1 == r) return new P([this.checkMinRect(t.clone(), e)]);
@@ -10266,86 +10264,86 @@
                 for (let e = 0; e < i; e++) {
                     let e = new j(n, l, r.width, r.height);
                     a < e.right - t.x && (a = e.right - t.x), o < e.bottom - t.y && (o = e.bottom - t.y), s = new j(t.x, t.y, a, o), n = e.right + e.width <= t.right ? e.right : (l = e.bottom, t.x)
                 }
                 return s
             }
             static checkMinRect(e, t) {
-                let r = Zu.factor(t);
+                let r = Yu.factor(t);
                 return e.width < 80 * r && (e.width = 80 * r), e.height < 50 * r && (e.height = 50 * r), e
             }
             static getSimpleRect(e, t, r) {
                 let i = this.getMinRectangle(e.clone(), t),
                     s = (i = this.checkMinRect(i, r), {
                         ref: 0
                     }),
                     n = {
                         ref: 0
                     },
                     l = (this.prepareColumnRow(s, n, e.clone(), i, t), this.getUsingRect(e.clone(), i, t));
                 return l.width < e.width && (i = new j(e.x, e.y, i.width + (e.width - l.width) / s.ref, i.height)), i = l.height < e.height ? new j(e.x, e.y, i.width, i.height + (e.height - l.height) / n.ref) : i
             }
         }
-        Dc.hashLocations = new Co, F.h.StiElementLocationHelper = Dc
+        Rc.hashLocations = new xo, F.h.StiElementLocationHelper = Rc
     }
-    let ih = L.Report.Components.Gauge.StiRadialTickLabelCustomValue,
-        sh = L.Report.Components.Gauge.StiLinearTickLabelCustomValue,
-        nh = L.System.Drawing.Orientation,
-        lh = L.Report.Export.StiGaugeSvgHelper,
-        ah = L.System.Drawing.Graphics,
-        oh = L.Report.Export.StiSvgData,
-        uh = L.Report.Dashboard.Visuals.IStiGaugeVisualSvgHelper;
+    let sh = L.Report.Components.Gauge.StiRadialTickLabelCustomValue,
+        nh = L.Report.Components.Gauge.StiLinearTickLabelCustomValue,
+        lh = L.System.Drawing.Orientation,
+        ah = L.Report.Export.StiGaugeSvgHelper,
+        oh = L.System.Drawing.Graphics,
+        uh = L.Report.Export.StiSvgData,
+        hh = L.Report.Dashboard.Visuals.IStiGaugeVisualSvgHelper;
     {
-        class ad {
+        class od {
             implements() {
-                return ad.ImplementsStiGaugeVisualSvgHelper || (ad.ImplementsStiGaugeVisualSvgHelper = [uh]), ad.ImplementsStiGaugeVisualSvgHelper
+                return od.ImplementsStiGaugeVisualSvgHelper || (od.ImplementsStiGaugeVisualSvgHelper = [hh]), od.ImplementsStiGaugeVisualSvgHelper
             }
             async writeGauge(s, e, n, t, r) {
                 let i = new j(e.x, e.y, e.width, e.height),
                     l = e.component,
-                    a = await ad.getDataTable(l);
+                    a = await od.getDataTable(l);
                 if (null == a) return;
                 let o = new W(e.width, e.height),
                     u = (new F.i.StiGaugeElementBuilder).render2(l, o, a),
                     h = F.h.StiElementLocationHelper.getLocationRectangles(i.clone(), (await u()).count2(), l);
                 if (null == (u = 1 < (await u()).count2() ? (new F.i.StiGaugeElementBuilder).render2(l, new W(h[0].width, h[0].height), a) : u) || !(await u()).any()) return;
-                let m = await ad.getTitleHeight(null, u, i.clone(), l, null),
+                let m = await od.getTitleHeight(null, u, i.clone(), l, null),
                     c = null != m ? m : 0,
                     d = h[0].clone(),
-                    g = await ad.getTitleMinFontSize(null, u, l.font, d.width, d.height),
-                    p = (g < l.font.size && (m = await ad.getTitleHeight(null, u, i.clone(), l, g), c = null != m ? m : 0), 0);
+                    g = await od.getTitleMinFontSize(null, u, l.font, d.width, d.height),
+                    p = (g < l.font.size && (m = await od.getTitleHeight(null, u, i.clone(), l, g), c = null != m ? m : 0), 0);
                 if (t && t.needToVertScroll) {
                     let e = F.h.StiElementLocationHelper.getSumRectangle(h);
                     t.needToVertScroll = e.height > i.height + i.top + 5, t.needToVertScroll && (i.width -= 15, h = F.h.StiElementLocationHelper.getLocationRectangles(i.clone(), (await u()).count2(), l), u = (new F.i.StiGaugeElementBuilder).render2(l, new W(h[0].width, h[0].height), a), i = F.h.StiElementLocationHelper.getSumRectangle(h), r.ref = L.System.Convert.toInt32(i.height), c = 0)
                 }
                 for (let i of await u()) {
                     let t = h[p].clone();
                     if (null != m) {
                         let e = new j(t.x, t.y, t.width, c);
                         this.paintTitle(l, null, s, e, i.series, g)
                     }
-                    let r = new oh;
+                    let r = new uh;
                     if (r.x = t.x / 2, r.y = (t.y + c) / 2, r.width = t.width, r.height = t.height - c, r.component = i.gauge, this.isEmptyData(l, a) && !l["isSampleForStyles"]) {
                         let e = this.getEmptyDataGauge(l);
                         null != e && (r.component = e)
                     }
-                    lh.writeGauge(s, r, 1, n, l["isSampleForStyles"]), l.previousAnimations = r.component.previousAnimations, p++
+                    ah.writeGauge(s, r, 1, n, l["isSampleForStyles"]), l.previousAnimations = r.component.previousAnimations, p++
                 }
             }
             paintTitle(s, e, n, l, a, o) {
                 if (B.isNullOrEmpty(a)) return;
-                let u = yu.changeFontSize(s.font, o),
+                let u = Cu.changeFontSize(s.font, o),
                     t = F.h.StiTitleMeasureHelper.measureTitle4(e, l.clone(), s.font, a),
                     h = new j(l.x, l.y, l.width, t.height);
                 if (!B.isNullOrWhiteSpace(a)) {
                     let e = jl.getForeColor(s, s.foreColor),
                         t = N.transparent.equals(e) ? J.getForeColor(s) : e,
-                        r = ah.measureString(a, u),
+                        r = oh.measureString(a, u),
                         i = new Yl(h.x + l.width / 2 - .39 * r.width, h.y + r.height / 2);
-                    lh.writeText(n, a, u, new v(t), i, o)
+                    ah.writeText(n, a, u, new v(t), i, o)
                 }
                 l.y += h.height, l.height -= h.height
             }
             static async getTitleMinFontSize(r, e, i, t, s) {
                 let n = null,
                     l = new j(0, 0, t, s);
                 for (let t of await e()) {
@@ -10363,15 +10361,15 @@
                 return a
             }
             isEmptyData(e, t) {
                 return null != t && t.isEmpty && e.isQuerable
             }
             static async getDataTable(e) {
                 var t;
-                let r = null == (t = e.as(th)) ? void 0 : t.getManuallyEnteredDataTable();
+                let r = null == (t = e.as(rh)) ? void 0 : t.getManuallyEnteredDataTable();
                 if (null != r) return r;
                 return bl.tryToGetOrCreate(e)
             }
             getEmptyDataGauge(e) {
                 switch (e.type) {
                     case _l.FullCircular:
                         return this.getFullCircularEmptyDataGauge(e);
@@ -10387,110 +10385,110 @@
                 return null
             }
             getBulletEmptyDataGauge(e) {
                 let t = J.getDataEmptyColor(e),
                     r = J.getDataEmptyForeColor(e),
                     i = new $l,
                     s = new sa,
-                    n = (s.allowApplyStyle = !1, s.relativeHeight = .85, s.orientation = nh.Horizontal, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
+                    n = (s.allowApplyStyle = !1, s.relativeHeight = .85, s.orientation = lh.Horizontal, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
                 if (n.allowApplyStyle = !1, n.textBrush = new v(r), s.items.add(n), e.showBlanks) {
                     let e = new Bl;
-                    e.offset = .1, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Inside, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new sh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
+                    e.offset = .1, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Inside, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new nh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
                 }
                 return i.scales.add(s), i
             }
             getHorizontalLinearEmptyDataGauge(e) {
                 let t = J.getDataEmptyColor(e),
                     r = J.getDataEmptyForeColor(e),
                     i = new $l,
                     s = new sa,
-                    n = (s.allowApplyStyle = !1, s.relativeHeight = .92, s.orientation = nh.Horizontal, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
+                    n = (s.allowApplyStyle = !1, s.relativeHeight = .92, s.orientation = lh.Horizontal, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
                 if (n.allowApplyStyle = !1, n.textBrush = new v(r), s.items.add(n), e.showBlanks) {
                     let e = new Bl;
-                    e.offset = .1, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Inside, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new sh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
+                    e.offset = .1, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Inside, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new nh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
                 }
                 return i.scales.add(s), i
             }
             getLinearEmptyDataGauge(e) {
                 let t = J.getDataEmptyColor(e),
                     r = J.getDataEmptyForeColor(e),
                     i = new $l,
                     s = new sa,
-                    n = (s.allowApplyStyle = !1, s.relativeHeight = .84, s.orientation = nh.Vertical, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
+                    n = (s.allowApplyStyle = !1, s.relativeHeight = .84, s.orientation = lh.Vertical, s.startWidth = .1, s.endWidth = .1, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new Ul);
                 if (n.allowApplyStyle = !1, n.textBrush = new v(r), s.items.add(n), e.showBlanks) {
                     let e = new Bl;
-                    e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new sh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
+                    e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.textObj = A.get("Dashboard", "Blank"), e.values.add(new nh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
                 }
                 return i.scales.add(s), i
             }
             getHalfCircularEmptyDataGauge(e) {
                 let t = J.getDataEmptyColor(e),
                     r = J.getDataEmptyForeColor(e),
                     i = new $l,
                     s = new ma,
                     n = (s.allowApplyStyle = !1, s.startAngle = 180, s.sweepAngle = 180, s.startWidth = .13, s.endWidth = .13, s.minimum = 0, s.maximum = 1, s.radius = .92, s.majorInterval = 1, s.center = new Yl(.5, .7), s.borderBrush = new rt, s.brush = new v(t), new ua);
                 if (n.allowApplyStyle = !1, n.textBrush = new v(r), s.items.add(n), e.showBlanks) {
                     let e = new Pl;
-                    e.offset = .8, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.values.add(new ih(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
+                    e.offset = .8, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.values.add(new sh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
                 }
                 return i.scales.add(s), i
             }
             getFullCircularEmptyDataGauge(e) {
                 let t = J.getDataEmptyColor(e),
                     r = J.getDataEmptyForeColor(e),
                     i = new $l,
                     s = new ma,
                     n = (s.allowApplyStyle = !1, s.startAngle = 120, s.sweepAngle = 300, s.startWidth = .13, s.endWidth = .13, s.minimum = 0, s.maximum = 1, s.majorInterval = 1, s.borderBrush = new rt, s.brush = new v(t), new ua);
                 if (n.allowApplyStyle = !1, n.textBrush = new v(r), s.items.add(n), i.scales.add(s), e.showBlanks) {
                     let e = new Pl;
-                    e.offset = .8, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.values.add(new ih(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
+                    e.offset = .8, e.font = new H("Arial", 14), e.textBrush = new v(r), e.placement = ea.Overlay, e.values.add(new sh(.5, A.get("Dashboard", "Blank"))), s.items.add(e)
                 }
                 return i.scales.add(s), i
             }
         }
-        F.h.StiGaugeVisualSvgHelper = ad
+        F.h.StiGaugeVisualSvgHelper = od
     }
     F.u.StiIndicatorIteration = class {
         constructor(e, t, r) {
             this.series = e, this.value = t, this.target = r
         }
     };
-    let hh = L.Data.Engine.StiDataSortDirection,
-        mh = L.Data.Engine.StiDataSortVariation,
-        ch = L.Data.Engine.StiDataTopNMode,
-        dh = F.u.StiIndicatorIteration;
+    let mh = L.Data.Engine.StiDataSortDirection,
+        ch = L.Data.Engine.StiDataSortVariation,
+        dh = L.Data.Engine.StiDataTopNMode,
+        gh = F.u.StiIndicatorIteration;
     {
-        class yh extends F.i.StiElementBuilder {
+        class Ch extends F.i.StiElementBuilder {
             async render(l, a) {
                 this.storedCulture = ai.set(l.report);
                 try {
                     let t = this.getValueMeterIndex(a),
                         r = this.getTargetMeterIndex(a),
                         i = this.getSeriesMeterIndex(a),
                         e = this.getSeriesKeys(a, i, this.getSeriesKeysLimitCount(l)),
                         s = e.count2(),
-                        n = e.select(e => new dh(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
-                    return n = yh.processVariationSort(l, n), await yh.processTopNElements(l, n)
+                        n = e.select(e => new gh(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
+                    return n = Ch.processVariationSort(l, n), await Ch.processTopNElements(l, n)
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static processVariationSort(e, t) {
                 let r = e.userSorts;
-                return t = null != r && r.any(e => e.key == mh.ident) ? r.firstOrDefault().direction == hh.Ascending ? t.orderBy(e => 0 != e.target ? e.value / e.target : 0) : t.orderByDescending(e => 0 != e.target ? e.value / e.target : 0) : t
+                return t = null != r && r.any(e => e.key == ch.ident) ? r.firstOrDefault().direction == mh.Ascending ? t.orderBy(e => 0 != e.target ? e.value / e.target : 0) : t.orderByDescending(e => 0 != e.target ? e.value / e.target : 0) : t
             }
             static async processTopNElements(s, n) {
-                if (s.topN.mode == ch.None) return n;
-                let l = (n = s.topN.mode == ch.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).take(s.topN.count);
+                if (s.topN.mode == dh.None) return n;
+                let l = (n = s.topN.mode == dh.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).take(s.topN.count);
                 if (n.count2() > s.topN.count && s.topN.showOthers) {
                     let e = n.skip(s.topN.count).sum(e => V.tryToNumber(e.value)),
                         t = n.skip(s.topN.count),
                         r = t.all(e => null != e ? null == e.target : null) ? null : t.sum(e => V.tryToNullableNumber(e.target)),
                         i = B.isNullOrEmpty(s.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(s.topN.othersText, s);
-                    l.add(new dh(i, e, r))
+                    l.add(new gh(i, e, r))
                 }
                 return l
             }
             getValueMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(Is));
                 return null != t ? e.meters.indexOf(t) : -1
@@ -10502,21 +10500,21 @@
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(As));
                 return null != t ? e.meters.indexOf(t) : -1
             }
         }
-        F.i.StiIndicatorElementBuilder = yh
+        F.i.StiIndicatorElementBuilder = Ch
     }
-    let gh = L.Report.Components.TextFormats.StiNegativeColorChecker,
-        ph = L.System.Drawing.GraphicsUnit,
-        Sh = L.Base.Context.StiInteractionDataGeom,
-        wh = L.Base.Context.StiIndicatorInteractionData,
-        bh = (F.u.StiIndicatorVisual = class extends F.j.StiVisual {
+    let ph = L.Report.Components.TextFormats.StiNegativeColorChecker,
+        Sh = L.System.Drawing.GraphicsUnit,
+        wh = L.Base.Context.StiInteractionDataGeom,
+        bh = L.Base.Context.StiIndicatorInteractionData,
+        fh = (F.u.StiIndicatorVisual = class extends F.j.StiVisual {
             async draw(e, t) {
                 let r = .06 * t.width,
                     i = (12 < (r = r < 4 ? 4 : r) && (r = 12), new j(t.x + r / 2, t.y + r / 2, t.width - r, t.height - r));
                 try {
                     e.pushClip(t), 1 == this.iterations.length ? this.drawSingleMode(e, t, i) : 1 < this.iterations.length && await this.drawMultiMode(e, i), e.popClip()
                 } finally {}
             }
@@ -10553,172 +10551,172 @@
                     b = this.processIconAlignment(this.iterations[0]),
                     f = this.processCustomIcon(this.iterations[0]);
                 if (null != g && a.fillRectangle(g, t, null), !this.element.report.isDesigning) {
                     let e = J.getHotBackColor(this.element);
                     null == g && (g = N.transparent), a.fillRectangle3(g, e, t, this.getInteractionDataGeom(this.iterations[0]))
                 }
                 let y = p;
-                if (this.iterations[0].value < 0 && gh.isNegativeInRed(this.element.textFormat) && (y = Z.Engine.negativeColor), this.drawTextIcon(a, h, d, Ha.getContent(w), y, S, i, b, f), r) {
+                if (this.iterations[0].value < 0 && ph.isNegativeInRed(this.element.textFormat) && (y = Z.Engine.negativeColor), this.drawTextIcon(a, h, d, za.getContent(w), y, S, i, b, f), r) {
                     let e = this.getVariation(this.iterations[0]),
                         t = J.getIndicatorStyle(this.element),
                         r = 0 <= e ? t.positiveColor : t.negativeColor,
                         i = (r = this.processTargetIconColor(r, this.iterations[0]), 0 <= e ? kt.ArrowUp : kt.ArrowDown),
                         s = (i = this.processTargetIcon(i, this.iterations[0]), ts.formatAsPercentage2(this.element.report, this.element.targetFormat, e)),
                         n = 0 == e ? Ht.None : Ht.Right,
                         l = this.processTargetIconAlignment(n, this.iterations[0]);
-                    this.drawTextIcon(a, s, d, Ha.getContent(i), r, r, o, l, null)
+                    this.drawTextIcon(a, s, d, za.getContent(i), r, r, o, l, null)
                 }
                 let C = null,
                     x = {
                         ref: C
                     };
                 if (this.measureFontSize(a, s, this.iterations[0].series, x), null != (C = .88 * x.ref) && 0 < C) {
                     let e = new H(m, C, c),
-                        t = ku.create(e);
-                    a.drawRotatedString5(this.iterations[0].series, t, p, s, Gu.getStringFormatGeom(a), Nu.CenterCenter, 0, !0)
+                        t = Nu.create(e);
+                    a.drawRotatedString5(this.iterations[0].series, t, p, s, Xu.getStringFormatGeom(a), Lu.CenterCenter, 0, !0)
                 }
             }
             getVariation(e) {
                 let t = e.value,
                     r = V.tryToNumber(e.target),
                     i = 0;
                 if (0 != r) switch (this.element.targetMode) {
-                    case Wa.Variation:
+                    case Ja.Variation:
                         i = t / r - 1, r < 0 && (i = -i);
                         break;
-                    case Wa.Percentage:
+                    case Ja.Percentage:
                         i = t / r;
                         break
                 }
                 return i
             }
             getFactorByFontSize(t, r, i, s) {
                 switch (i.fontSizeMode) {
-                    case qa.Auto:
+                    case _a.Auto:
                         return .7;
-                    case qa.Value:
-                    case qa.Target: {
-                        let e = t.measureString(r, ku.create(i.font));
+                    case _a.Value:
+                    case _a.Target: {
+                        let e = t.measureString(r, Nu.create(i.font));
                         return e.height / s.height
                     }
                 }
                 return 0
             }
             getRectanglesSingleMode(e, t, r, i, s, n) {
                 let l = this.iterations[0].target,
                     a = null != l,
                     o = !B.isNullOrEmpty(this.iterations[0].series),
                     u = .7,
                     h = (1 - u) / 2,
                     m = 1 - h - u,
                     c = r.y;
-                !o && a ? (this.element.fontSizeMode == qa.Value ? (u = this.getFactorByFontSize(e, t, this.element, r), h = 1 - u) : this.element.fontSizeMode == qa.Target && (h = this.getFactorByFontSize(e, t, this.element, r), u = 1 - h), m = 0) : o && !a ? (h = 0, m = 1 - u) : o || a || (this.element.fontSizeMode != qa.Value ? u = 1 : (u = this.getFactorByFontSize(e, t, this.element, r), c = r.y + (r.height - r.height * u) / 2), h = 0, m = 0), i.ref = new j(r.x, c, r.width, r.height * u), s.ref = new j(i.ref.x, i.ref.bottom, r.width, r.height * h), n.ref = new j(i.ref.x, s.ref.bottom, r.width, r.height * m)
+                !o && a ? (this.element.fontSizeMode == _a.Value ? (u = this.getFactorByFontSize(e, t, this.element, r), h = 1 - u) : this.element.fontSizeMode == _a.Target && (h = this.getFactorByFontSize(e, t, this.element, r), u = 1 - h), m = 0) : o && !a ? (h = 0, m = 1 - u) : o || a || (this.element.fontSizeMode != _a.Value ? u = 1 : (u = this.getFactorByFontSize(e, t, this.element, r), c = r.y + (r.height - r.height * u) / 2), h = 0, m = 0), i.ref = new j(r.x, c, r.width, r.height * u), s.ref = new j(i.ref.x, i.ref.bottom, r.width, r.height * h), n.ref = new j(i.ref.x, s.ref.bottom, r.width, r.height * m)
             }
             processFontStyle(e, t) {
                 let r = this.processFontBold(e.bold, t),
                     i = this.processFontItalic(e.italic, t),
                     s = this.processFontUnderline(e.underline, t),
                     n = this.processFontStrikeout(e.strikeout, t),
                     l = hn.Regular;
                 return r && (l ^= hn.Bold), i && (l ^= hn.Italic), s && (l ^= hn.Underline), n && (l ^= hn.Strikeout), l
             }
             processFontStrikeout(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
+                    if (0 < (e.permissions & to.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
                 return e
             }
             processFontUnderline(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.FontStyleUnderline) && this.getConditionResult(t, e)) return e.font.underline;
+                    if (0 < (e.permissions & to.FontStyleUnderline) && this.getConditionResult(t, e)) return e.font.underline;
                 return e
             }
             processFontItalic(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.FontStyleItalic) && this.getConditionResult(t, e)) return e.font.italic;
+                    if (0 < (e.permissions & to.FontStyleItalic) && this.getConditionResult(t, e)) return e.font.italic;
                 return e
             }
             processFontBold(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.FontStyleBold) && this.getConditionResult(t, e)) return e.font.bold;
+                    if (0 < (e.permissions & to.FontStyleBold) && this.getConditionResult(t, e)) return e.font.bold;
                 return e
             }
             processFontName(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.Font) && this.getConditionResult(t, e)) return e.font.name;
+                    if (0 < (e.permissions & to.Font) && this.getConditionResult(t, e)) return e.font.name;
                 return e
             }
             processIcon(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.Icon) && this.getConditionResult(t, e)) return e.icon;
+                    if (0 < (e.permissions & to.Icon) && this.getConditionResult(t, e)) return e.icon;
                 return e
             }
             processTargetIcon(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.TargetIcon) && this.getConditionResult(t, e)) return e.targetIcon;
+                    if (0 < (e.permissions & to.TargetIcon) && this.getConditionResult(t, e)) return e.targetIcon;
                 return e
             }
             processCustomIcon(t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.Icon) && this.getConditionResult(t, e)) return e.customIcon;
+                    if (0 < (e.permissions & to.Icon) && this.getConditionResult(t, e)) return e.customIcon;
                 return this.element.customIcon
             }
             processIconAlignment(t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.Icon) && this.getConditionResult(t, e)) return e.iconAlignment;
+                    if (0 < (e.permissions & to.Icon) && this.getConditionResult(t, e)) return e.iconAlignment;
                 return this.element.iconAlignment
             }
             processTargetIconAlignment(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.TargetIcon) && this.getConditionResult(t, e)) return e.targetIconAlignment;
+                    if (0 < (e.permissions & to.TargetIcon) && this.getConditionResult(t, e)) return e.targetIconAlignment;
                 return e
             }
             processBackColor(t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.BackColor) && this.getConditionResult(t, e)) return e.backColor;
+                    if (0 < (e.permissions & to.BackColor) && this.getConditionResult(t, e)) return e.backColor;
                 return null
             }
             processForeColor(t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.TextColor) && this.getConditionResult(t, e)) return e.textColor;
+                    if (0 < (e.permissions & to.TextColor) && this.getConditionResult(t, e)) return e.textColor;
                 return J.getForeColor(this.element)
             }
             processGlyphColor(t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.Icon) && this.getConditionResult(t, e)) return e.iconColor;
+                    if (0 < (e.permissions & to.Icon) && this.getConditionResult(t, e)) return e.iconColor;
                 return J.getGlyphColor(this.element)
             }
             processTargetIconColor(e, t) {
                 for (let e of this.element.indicatorConditions)
-                    if (0 < (e.permissions & eo.TargetIcon) && this.getConditionResult(t, e)) return e.targetIconColor;
+                    if (0 < (e.permissions & to.TargetIcon) && this.getConditionResult(t, e)) return e.targetIconColor;
                 return e
             }
             getConditionResult(i, t) {
                 let s = null;
                 switch (t.field) {
-                    case $a.Value:
+                    case eo.Value:
                         s = i.value;
                         break;
-                    case $a.Series:
+                    case eo.Series:
                         s = i.series;
                         break;
-                    case $a.Target:
+                    case eo.Target:
                         s = i.target;
                         break;
-                    case $a.Variation: {
+                    case eo.Variation: {
                         let e = this.getVariation(i),
                             t = new Ur,
                             r = (t.decimalDigits = 3, ts.formatAsPercentage2(this.element.report, t, e));
                         s = r.replace("%", "")[L.System.StiObject.stimulsoft]().toNumber();
                         break
                     }
                 }
                 let e = !1,
                     r = this.getConditionValue(t);
                 if (null != s) {
-                    let e = s = t.field != $a.Value && t.field != $a.Target && t.field != $a.Variation ? s : null == s ? 0 : s[L.System.StiObject.stimulsoft]().toNumber();
+                    let e = s = t.field != eo.Value && t.field != eo.Target && t.field != eo.Variation ? s : null == s ? 0 : s[L.System.StiObject.stimulsoft]().toNumber();
                     if (null != e && null != r) {
                         s[L.System.StiObject.stimulsoft]().getType() != r[L.System.StiObject.stimulsoft]().getType() && (s = s.toString(), r = r[L.System.StiObject.stimulsoft]().toString(), e = s);
                         try {
                             switch (t.condition) {
                                 case L.Report.Components.StiFilterCondition.EqualTo:
                                     return 0 == e[L.System.StiObject.stimulsoft]().compareTo(r);
                                 case L.Report.Components.StiFilterCondition.NotEqualTo:
@@ -10756,17 +10754,17 @@
                     }
                 }
                 return e
             }
             getConditionValue(e) {
                 if (B.isNullOrEmpty(e.value)) return null;
                 switch (e.field) {
-                    case $a.Value:
-                    case $a.Target:
-                    case $a.Variation:
+                    case eo.Value:
+                    case eo.Target:
+                    case eo.Variation:
                         return e.value[L.System.StiObject.stimulsoft]().toNumber();
                     default:
                         return e.value.toString()
                 }
             }
             async drawMultiMode(e, t) {
                 if (0 == this.iterations.length) return;
@@ -10778,86 +10776,86 @@
                     t = e.max(),
                     s = e.min(),
                     n = t - s,
                     c = g.height / this.iterations.length,
                     p = (c < this.minSide && (c = this.minSide), new P),
                     S = new P,
                     w = new P,
-                    l = Ha.getFontIcons(this.element.iconSet),
+                    l = za.getFontIcons(this.element.iconSet),
                     a = new P;
-                if (this.element.iconMode == Ga.Auto) {
+                if (this.element.iconMode == Xa.Auto) {
                     let i = 1 / l.length;
                     for (let r = 0; r < l.length; r++) {
                         let e = s + r * i * n,
                             t = s + (1 + r) * i * n;
                         a.add(new F.u.StiIndicatorIconRangeValue(e, t, l[r]))
                     }
                 } else
                     for (let r of this.element.iconRanges) {
                         let e = V.tryToNumber(await O.parseAsync(r.startExpression, this.element)),
                             t = V.tryToNumber(await O.parseAsync(r.endExpression, this.element));
-                        this.element.iconRangeMode == za.Percentage && (e = s + e / 100 * n, t = s + t / 100 * n), a.add(new F.u.StiIndicatorIconRangeValue(e, t, r.icon))
+                        this.element.iconRangeMode == Ga.Percentage && (e = s + e / 100 * n, t = s + t / 100 * n), a.add(new F.u.StiIndicatorIconRangeValue(e, t, r.icon))
                     }
                 for (let t of this.iterations) {
                     p.add(t.series), S.add(ts.format(this.element.report, this.element.textFormat, t.value));
                     let e = a.where(e => e.isBetween(t.value)).firstOrDefault();
                     null != e ? w.add(e.icon) : w.add(null)
                 }
                 let b = this.element.font,
                     o = null,
                     u = new H(b.fontFamily.name, 1, b.style, b.unit);
                 for (let i = 0; i < this.iterations.length; i++) {
                     let e = p[i] + S[i] + "Icon",
                         t = new j(g.x, g.y, g.width, c),
-                        r = Gu.getFontSize(d, t, e, u);
+                        r = Xu.getFontSize(d, t, e, u);
                     (null == o || o > r) && (o = r)
                 }
-                let f = Gu.getStringFormatGeom(d),
+                let f = Xu.getStringFormatGeom(d),
                     y = this.element.font.size / 13 * o;
                 if ((y = y > o ? o : y) < 1) return;
                 let C = new P,
                     x = null,
-                    M = new ku("Stimulsoft", .6 * y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point);
+                    M = new Nu("Stimulsoft", .6 * y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point);
                 for (let m = 0; m < this.iterations.length; m++) {
                     let e = this.processFontName(b.fontFamily.name, this.iterations[m]),
                         t = this.processFontStyle(b, this.iterations[m]),
                         r = new H(e, y, t),
-                        i = ku.create(r),
+                        i = Nu.create(r),
                         s = new P,
                         n = g.y + c * m,
                         l = new j(g.x, n, g.width, c),
                         a = (s.add(l), d.measureString(p[m], i)),
                         o = new j(l.x, l.y, a.width, c),
-                        u = (s.add(o), d.measureString(Ha.getContent(w[m]), M)),
+                        u = (s.add(o), d.measureString(za.getContent(w[m]), M)),
                         h = ((null == x || x > g.right - u.width - this.indent) && (x = g.right - u.width - this.indent), new j(x, l.y, u.width, c));
                     s.add(h), C.add(s)
                 }
                 for (let c = 0; c < this.iterations.length; c++) {
                     let e = this.processFontName(b.fontFamily.name, this.iterations[c]),
                         t = this.processFontStyle(b, this.iterations[c]),
                         r = new H(e, y, t),
-                        i = ku.create(r),
+                        i = Nu.create(r),
                         s = C[c],
                         n = s[0];
                     if (!n.intersectsWith(g)) return;
                     let l = this.processBackColor(this.iterations[c]);
                     if (null != l && d.fillRectangle(l, n, null), !this.element.report.isDesigning) {
                         let e = J.getHotBackColor(this.element);
                         null == l && (l = N.transparent), d.fillRectangle3(l, e, n, this.getInteractionDataGeom(this.iterations[c]))
                     }
                     let a = new j(s[1].x + this.indent, s[1].y, s[1].width, s[1].height),
                         o = this.processForeColor(this.iterations[c]),
-                        u = (d.drawRotatedString5(p[c], i, o, a, f, Nu.CenterCenter, 0, !0), s[2]),
+                        u = (d.drawRotatedString5(p[c], i, o, a, f, Lu.CenterCenter, 0, !0), s[2]),
                         h = this.processGlyphColor(this.iterations[c]),
                         m = w[c];
                     if (null != m) {
                         let e = this.processIcon(m, this.iterations[c]);
-                        d.drawRotatedString5(Ha.getContent(e), M, h, u, Gu.getStringFormatGeom(d), Nu.CenterCenter, 0, !0)
+                        d.drawRotatedString5(za.getContent(e), M, h, u, Xu.getStringFormatGeom(d), Lu.CenterCenter, 0, !0)
                     }
-                    d.drawRotatedString4(S[c], i, o, new Yl(x - 4, u.y + u.height / 2), f, Nu.RightCenter, 0, !0)
+                    d.drawRotatedString4(S[c], i, o, new Yl(x - 4, u.y + u.height / 2), f, Lu.RightCenter, 0, !0)
                 }
             }
             drawMultiModeWithTarget(f, y, e) {
                 let C = y.height / this.iterations.length,
                     x = (C < this.minSide && (C = this.minSide), new P),
                     M = new P,
                     T = new P,
@@ -10872,81 +10870,81 @@
                 }
                 let s = null,
                     A = this.element.font,
                     n = new H(A.fontFamily.name, 1, A.style, A.unit);
                 for (let i = 0; i < this.iterations.length; i++) {
                     let e = x[i] + M[i] + T[i] + "DeltaIcon",
                         t = new j(y.x, y.y, y.width, C),
-                        r = Gu.getFontSize(f, t, e, n);
+                        r = Xu.getFontSize(f, t, e, n);
                     (null == s || s > r) && (s = r)
                 }
-                let I = Gu.getStringFormatGeom(f),
+                let I = Xu.getStringFormatGeom(f),
                     D = this.element.font.size / 13 * s;
                 if ((D = D > s ? s : D) < 1) return;
-                let R = new ku(A.fontFamily.name, D, A.style, A.unit),
-                    E = new ku("Stimulsoft", .99 * D, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point),
+                let R = new Nu(A.fontFamily.name, D, A.style, A.unit),
+                    E = new Nu("Stimulsoft", .99 * D, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point),
                     O = null;
                 for (let e = 0; e < this.iterations.length; e++) {
                     let t = F[e];
                     if (null != t) {
-                        let e = f.measureString(Ha.getContent(t), E);
+                        let e = f.measureString(za.getContent(t), E);
                         (null == O || O > y.right - e.width - +this.indent) && (O = y.right - e.width - +this.indent)
                     }
                 }
                 let V = null;
                 for (let t = 0; t < this.iterations.length; t++) {
                     let e = f.measureString(T[t], R);
                     (null == V || V > O - e.width) && (V = O - e.width)
                 }
                 let k = J.getIndicatorStyle(this.element);
                 for (let b = 0; b < this.iterations.length; b++) {
                     let e = this.processForeColor(this.iterations[b]),
                         t = this.processFontName(A.fontFamily.name, this.iterations[b]),
                         r = this.processFontStyle(A, this.iterations[b]),
                         i = new H(t, D, r),
-                        s = (R = ku.create(i), y.y + C * b),
+                        s = (R = Nu.create(i), y.y + C * b),
                         n = new j(y.x, s, y.width, C);
                     if (!n.intersectsWith(y)) return;
                     let l = this.processBackColor(this.iterations[b]);
                     if (null != l && f.fillRectangle(l, n, null), !this.element.report.isDesigning) {
                         let e = J.getHotBackColor(this.element);
                         null == l && (l = N.transparent), f.fillRectangle3(l, e, n, this.getInteractionDataGeom(this.iterations[b]))
                     }
                     let a = f.measureString(x[b], R),
                         o = new j(n.x + this.indent, n.y, a.width, C),
                         u = (f.drawString(x[b], R, e, o, I), F[b] == kt.ArrowUp ? k.positiveColor : k.negativeColor),
-                        h = (u = this.processTargetIconColor(u, this.iterations[b]), f.measureString(Ha.getContent(F[b]), E)),
+                        h = (u = this.processTargetIconColor(u, this.iterations[b]), f.measureString(za.getContent(F[b]), E)),
                         m = new j(O, n.y, h.width, C),
                         c = f.measureString(T[b], R),
                         d = new j(O - c.width, n.y, c.width, C),
                         g = F[b],
-                        p = (g = this.processTargetIcon(g, this.iterations[b]), f.drawRotatedString5(T[b], R, u, d, I, Nu.CenterCenter, 0, !0), this.processTargetIconAlignment(v[b], this.iterations[b])),
-                        S = (p != Ht.None && f.drawRotatedString5(Ha.getContent(g), E, u, m, Gu.getStringFormatGeom(f), Nu.CenterCenter, 0, !0), this.iterations[b].value < 0 && gh.isNegativeInRed(this.element.textFormat) && (e = Z.Engine.negativeColor), f.measureString(M[b], R)),
+                        p = (g = this.processTargetIcon(g, this.iterations[b]), f.drawRotatedString5(T[b], R, u, d, I, Lu.CenterCenter, 0, !0), this.processTargetIconAlignment(v[b], this.iterations[b])),
+                        S = (p != Ht.None && f.drawRotatedString5(za.getContent(g), E, u, m, Xu.getStringFormatGeom(f), Lu.CenterCenter, 0, !0), this.iterations[b].value < 0 && ph.isNegativeInRed(this.element.textFormat) && (e = Z.Engine.negativeColor), f.measureString(M[b], R)),
                         w = new j(V - S.width, s, S.width, C);
-                    f.drawRotatedString4(M[b], R, e, new Yl(w.right, w.y + w.height / 2), I, Nu.RightCenter, 0, !0)
+                    f.drawRotatedString4(M[b], R, e, new Yl(w.right, w.y + w.height / 2), I, Lu.RightCenter, 0, !0)
                 }
             }
             getInteractionDataGeom(e) {
-                let t = new wh,
-                    r = (t.value = e.value, t.seriesText = e.series, t.target = e.target, new Sh);
+                let t = new bh,
+                    r = (t.value = e.value, t.seriesText = e.series, t.target = e.target, new wh);
                 return r.interactionToolTip = this.getToolTip(t), r.interactionHyperlink = this.getHyperlink(t), r.interactionData = t, r
             }
             getToolTip(e) {
                 var t;
                 let r = null == (t = this.element.dashboardInteraction) ? void 0 : t.toolTip;
                 return B.isNullOrEmpty(r) ? r : this.parseConstants(r, e)
             }
             getHyperlink(e) {
                 var t;
                 let r = null == (t = this.element.dashboardInteraction) ? void 0 : t.hyperlink;
                 return B.isNullOrEmpty(r) ? r : this.parseConstants(r, e)
             }
             parseConstants(t, r) {
                 if (!B.isNullOrEmpty(t)) {
-                    let e = new Co;
+                    let e = new xo;
                     return e.set("Value", r.value), e.set("Series", r.seriesText), e.set("Target", r.target), O.parse(t, this.element, !1, e)
                 }
                 return t
             }
             getMaxValue() {
                 let t = 0;
                 for (let e of this.iterations) t < e.value && (t = e.value);
@@ -10966,16 +10964,16 @@
                     };
                     this.measureFontSize(c, f.clone(), d, e), y = e.ref
                 } else if (w == Ht.Right || w == Ht.Left) {
                     let e = {
                         ref: y
                     };
                     if (this.measureFontSize(c, S.clone(), d, e), null == (y = e.ref) && y <= 0) return;
-                    let t = new ku("Stimulsoft", y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point),
-                        r = new ku(g.fontFamily.name, y, g.style, L.System.Drawing.GraphicsUnit.Point),
+                    let t = new Nu("Stimulsoft", y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point),
+                        r = new Nu(g.fontFamily.name, y, g.style, L.System.Drawing.GraphicsUnit.Point),
                         i = c.measureString(d, r),
                         s = c.measureString(p, t),
                         n = i.width + s.width > S.width ? S.width / (i.width + s.width) : 1,
                         l = (y *= n, new W(i.width * n, i.height * n)),
                         a = new W(s.width * n, s.height * n),
                         o = w == Ht.Right ? S.x + (S.width - l.width - a.width) / 2 : S.x + (S.width - l.width - a.width) / 2 + a.width,
                         u = S.y + (S.height - l.height) / 2,
@@ -10986,25 +10984,25 @@
                     f = w == Ht.Bottom ? new j(S.x, S.y, S.width, S.height / 2) : new j(S.x, S.y + S.height / 2, S.width, S.height / 2), b = w == Ht.Bottom ? new j(S.x, S.y + S.height / 2, S.width, S.height / 2) : new j(S.x, S.y, S.width, S.height / 2);
                     let e = {
                         ref: y
                     };
                     this.measureFontSize(c, f, d, e), y = e.ref
                 }
                 if (null != y && 0 < y) {
-                    let e = new ku(g.fontFamily.name, y, g.style, ph.Pixel);
-                    c.drawRotatedString5(d, e, t, f, Gu.getStringFormatGeom(c), Nu.CenterCenter, 0, !0)
+                    let e = new Nu(g.fontFamily.name, y, g.style, Sh.Pixel);
+                    c.drawRotatedString5(d, e, t, f, Xu.getStringFormatGeom(c), Lu.CenterCenter, 0, !0)
                 }
                 if (null != y && 0 < y && w != Ht.None)
                     if (null == e || 0 == e.length) {
-                        let e = new ku("Stimulsoft", .6 * y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point);
-                        c.drawRotatedString5(p, e, r, b, Gu.getStringFormatGeom(c), Nu.CenterCenter, 0, !0)
+                        let e = new Nu("Stimulsoft", .6 * y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point);
+                        c.drawRotatedString5(p, e, r, b, Xu.getStringFormatGeom(c), Lu.CenterCenter, 0, !0)
                     } else c.drawImage(e, b)
             }
             getFontGeom(e) {
-                return new ku("Arial", e, hn.Bold, ph.Point)
+                return new Nu("Arial", e, hn.Bold, Sh.Point)
             }
             measureFontSize(e, t, r, i) {
                 let s = e.measureString(r, this.getFontGeom(1e3));
                 if (0 == s.width || 0 == s.height) return void(i.ref = 0);
                 let n = t.width / s.width * 1e3,
                     l = t.height / s.height * 1e3,
                     a = l < n ? l : n;
@@ -11016,81 +11014,81 @@
                     s = r / this.iterations.length;
                 return s = s > i ? i : s
             }
             constructor(e, t) {
                 super(), this.indent = 4, this.minSide = 20, this.element = e, this.iterations = t
             }
         }, F.U.StiIndicatorElement),
-        fh = L.Report.Dashboard.Visuals.IStiIndicatorVisualSvgHelper,
-        yh = F.i.StiIndicatorElementBuilder,
-        Ch = F.u.StiIndicatorVisual;
+        yh = L.Report.Dashboard.Visuals.IStiIndicatorVisualSvgHelper,
+        Ch = F.i.StiIndicatorElementBuilder,
+        xh = F.u.StiIndicatorVisual;
     {
-        class qg {
+        class _g {
             implements() {
-                return qg.ImplementsStiIndicatorVisualSvgHelper || (qg.ImplementsStiIndicatorVisualSvgHelper = [fh]), qg.ImplementsStiIndicatorVisualSvgHelper
+                return _g.ImplementsStiIndicatorVisualSvgHelper || (_g.ImplementsStiIndicatorVisualSvgHelper = [yh]), _g.ImplementsStiIndicatorVisualSvgHelper
             }
             async writeIndicator(e, t, r, i) {
                 let s = new j(0, 0, t.width, t.height),
                     n = t.component.as(F.U.StiIndicatorElement),
-                    l = await qg.getDataTable(n);
+                    l = await _g.getDataTable(n);
                 if (null == l) return;
-                let a = await (new yh).render(n, l);
+                let a = await (new Ch).render(n, l);
                 if (n["isSampleForStyles"] ? a = this.getStyleSampleIterations() : this.isEmptyData(n, l) && (a = this.getEmptyDataIterations(n), n = this.getEmptyDataIndicatorElement(n)), null == a || !a.any()) return;
-                let o = new Uu,
-                    u = new _u(o, !0, !1, !1, 1),
-                    h = new Ch(n, a.toList());
+                let o = new Zu,
+                    u = new $u(o, !0, !1, !1, 1),
+                    h = new xh(n, a.toList());
                 if (r && r.needToVertScroll) {
                     let e = h.getContentRectangle(s);
                     r.needToVertScroll = e.height > s.height + 5, r.needToVertScroll && (s.width -= 15, e = h.getContentRectangle(s), (s = e).height += 10, i.ref = L.System.Convert.toInt32(s.height))
                 }
                 await h.draw(u, s.clone()), e.writeStartElement("g");
                 let m = r && r.needToVertScroll ? 0 : t.x,
                     c = r && r.needToVertScroll ? 0 : t.y;
-                e.writeAttributeString("transform", B.format("translate({0},{1})", this.p(m), this.p(c))), rh.writeGeoms(e, u, !1), e.writeEndElement()
+                e.writeAttributeString("transform", B.format("translate({0},{1})", this.p(m), this.p(c))), ih.writeGeoms(e, u, !1), e.writeEndElement()
             }
             p(e) {
                 return e.toString().split(",").join(".")
             }
             isEmptyData(e, t) {
                 return null != t && t.isEmpty && e.isQuerable
             }
             getStyleSampleIterations() {
                 let e = new P,
-                    t = new dh;
+                    t = new gh;
                 return t.value = 100, e.add(t), e
             }
             getEmptyDataIterations(e) {
                 let t = new P,
-                    r = new dh;
+                    r = new gh;
                 return r.value = 0, e.showBlanks && (r.series = A.get("Dashboard", "Blank")), t.add(r), t
             }
             getEmptyDataIndicatorElement(e) {
-                let t = e.clone(!0).as(bh);
+                let t = e.clone(!0).as(fh);
                 return t.glyphColor = N.fromArgb2(240, 240, 240), t
             }
             static async getDataTable(e) {
                 var t;
-                let r = null == (t = e.as(th)) ? void 0 : t.getManuallyEnteredDataTable();
+                let r = null == (t = e.as(rh)) ? void 0 : t.getManuallyEnteredDataTable();
                 if (null != r) return r;
                 return bl.tryToGetOrCreate(e)
             }
         }
-        F.h.StiIndicatorVisualSvgHelper = qg
+        F.h.StiIndicatorVisualSvgHelper = _g
     }
-    let xh = L.Data.Comparers.StiArrayEqualityComparer,
-        Mh = L.Base.Helpers.StiBingMapHelper,
-        Th = L.Base.Drawing.StiColorUtils,
-        Fh = L.Report.Maps.StiMapHelper;
+    let Mh = L.Data.Comparers.StiArrayEqualityComparer,
+        Th = L.Base.Helpers.StiBingMapHelper,
+        Fh = L.Base.Drawing.StiColorUtils,
+        vh = L.Report.Maps.StiMapHelper;
     {
-        class zd {
+        class Gd {
             static get ICON() {
-                return null == this._ICON && (this._ICON = Qa.toBase64String(ul.UTF8.getBytes('<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z" fill="#af6682" stroke="#663a4c"/><circle cx="12" cy="9" r="3" fill="#f7f4f2"/></svg>'))), this._ICON
+                return null == this._ICON && (this._ICON = qa.toBase64String(ul.UTF8.getBytes('<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z" fill="#af6682" stroke="#663a4c"/><circle cx="12" cy="9" r="3" fill="#f7f4f2"/></svg>'))), this._ICON
             }
             static get EMPTY_ICON() {
-                return null == this._EMPTY_ICON && (this._EMPTY_ICON = Qa.toBase64String(ul.UTF8.getBytes('<svg xmlns="http://www.w3.org/2000/svg" width="1" height="1" ></svg>'))), this._EMPTY_ICON
+                return null == this._EMPTY_ICON && (this._EMPTY_ICON = qa.toBase64String(ul.UTF8.getBytes('<svg xmlns="http://www.w3.org/2000/svg" width="1" height="1" ></svg>'))), this._EMPTY_ICON
             }
             static async getBingMapScript(o, e) {
                 let t = await bl.tryToGetOrCreate(o),
                     u = this.calculateMapData(t, o);
                 if (e) {
                     u["outerStyle"] = "display: table;";
                     let a = o.title;
@@ -11099,21 +11097,21 @@
                         if (a.font.bold && (t += "font-weight: bold;"), a.font.italic && (t += "font-style: italic;"), a.font.strikeout || a.font.underline) {
                             let e = a.font.underline ? a.font.strikeout ? "underline line-through" : "underline" : a.font.strikeout ? "line-through" : "none";
                             t += `text-decoration: ${e};`
                         }
                         let e = a.sizeMode == Dt.WordWrap ? "normal" : "nowrap",
                             r = a.sizeMode == Dt.Trimming ? ";text-overflow:ellipsis; overflow:hidden; display:table-caption; width:{}" : "",
                             i = a.sizeMode == Dt.Fit ? "font-size:measure" : `font-size: ${a.font.size.toString().replace(",",".")}pt`,
-                            s = Mu.toHtml(N.transparent.equals(a.foreColor) ? J.getTitleForeColor(o) : a.foreColor),
-                            n = Mu.toHtml(N.transparent.equals(a.backColor) ? J.getBackColor(o) : a.backColor),
+                            s = Tu.toHtml(N.transparent.equals(a.foreColor) ? J.getTitleForeColor(o) : a.foreColor),
+                            n = Tu.toHtml(N.transparent.equals(a.backColor) ? J.getBackColor(o) : a.backColor),
                             l = ve.getName(z, a.horAlignment).toLowerCase();
                         u["title"] = `font-family: ${a.font.name}; ${i}; color: ${s};` + `${t}background-color:${n};white-space:${e}${r};text-align:${l}'>${a.text}</div>`
                     }
                 }
-                return Mh.getScript(u)
+                return Th.getScript(u)
             }
             static calculateMapData(d, g) {
                 let r = {},
                     a = this.getLongitudeMeterIndex(d),
                     o = this.getLatitudeMeterIndex(d),
                     s = this.getLocationMeterIndex(d),
                     n = this.getLocationColorMeterIndex(d),
@@ -11130,36 +11128,36 @@
                                 t = s[a];
                             if (null == e || null == t) continue;
                             let r = V.tryToNumber(e).toString().replace(",", "."),
                                 i = V.tryToNumber(t).toString().replace(",", ".");
                             if (null == g.customIcon ? n.push({
                                     lat: r,
                                     lon: i,
-                                    fontIcon: Ha.getContent(g.icon).charCodeAt(0),
+                                    fontIcon: za.getContent(g.icon).charCodeAt(0),
                                     fontIconColor: `rgb(${g.iconColor.r}, ${g.iconColor.g}, ${g.iconColor.b})`
                                 }) : n.push({
                                     lat: r,
                                     lon: i,
                                     anchorX: this.MAX_RADIUS,
                                     anchorY: 2 * this.MAX_RADIUS
                                 }), l > this.MAX_LOCATIONS) break
                         }
                         r["pushpins"] = n
                     } else if (-1 != s) {
                     let e = null,
                         i = null;
-                    if (g.locationColorType == fo.ColorEach) e = this.getColors(Math.min(d.rows.length, this.MAX_LOCATIONS));
-                    else if (g.locationColorType == fo.Group && -1 != n) {
+                    if (g.locationColorType == yo.ColorEach) e = this.getColors(Math.min(d.rows.length, this.MAX_LOCATIONS));
+                    else if (g.locationColorType == yo.Group && -1 != n) {
                         let r = [];
                         for (let t = 0; t < d.rows.length; t++) {
                             let e = null != d.rows[t][n] ? d.rows[t][n].toString() : "";
                             r[L.System.StiObject.stimulsoft]().contains(e) || r.push(e)
                         }
                         let t = this.getColors(r.length);
-                        i = new Co;
+                        i = new xo;
                         for (let e = 0; e < r.length; e++) i.set(r[e], t[e])
                     }
                     let t = new P;
                     if (0 <= p)
                         for (let e = 0; e < Math.min(d.rows.length, this.MAX_LOCATIONS); e++) t.add(V.tryToNumber(d.rows[e][p]));
                     Ln.sort(t);
                     let h = t,
@@ -11169,51 +11167,51 @@
                         let a = d.rows[c][s];
                         if (null == a) {
                             c++;
                             continue
                         }
                         let o = N.limeGreen,
                             u = null;
-                        if (g.locationColorType == fo.Single) o = g.locationColor, u = N.transparent.equals(g.locationColor) ? "Transparent" : null;
-                        else if (g.locationColorType == fo.ColorEach) o = e[c];
-                        else if ((g.locationColorType == fo.Group || g.locationColorType == fo.Value) && 0 <= n) {
+                        if (g.locationColorType == yo.Single) o = g.locationColor, u = N.transparent.equals(g.locationColor) ? "Transparent" : null;
+                        else if (g.locationColorType == yo.ColorEach) o = e[c];
+                        else if ((g.locationColorType == yo.Group || g.locationColorType == yo.Value) && 0 <= n) {
                             let e = null != d.rows[c][n] ? d.rows[c][n].toString() : "";
-                            g.locationColorType == fo.Group && i.containsKey(e) && (o = i.get(e)), g.locationColorType != fo.Value || B.isNullOrEmpty(e) || (u = e)
+                            g.locationColorType == yo.Group && i.containsKey(e) && (o = i.get(e)), g.locationColorType != yo.Value || B.isNullOrEmpty(e) || (u = e)
                         }
                         if (m[a] = {
                                 fillStyle: null != u ? u : `rgba(${o.r}, ${o.g}, ${o.b}, 0.5)`,
                                 strokeStyle: "Transparent" == u ? u : "#d3d3d3"
-                            }, 0 <= p || g.valueViewMode == yo.Icon)
-                            if (g.valueViewMode == yo.Bubble) {
+                            }, 0 <= p || g.valueViewMode == Co.Icon)
+                            if (g.valueViewMode == Co.Bubble) {
                                 let e = h.indexOf(V.tryToNumber(d.rows[c][p])) / h.length,
                                     t = 2 * this.MAX_RADIUS + 2,
                                     r = this.MIN_RADIUS + Math.ceil(e * this.DELTA_RADIUS),
                                     i = this.MAX_RADIUS + 1,
-                                    s = Th.dark(null != u ? this.parseColor(u) : o, 70),
+                                    s = Fh.dark(null != u ? this.parseColor(u) : o, 70),
                                     n = null != u ? u : `rgba(${o.r}, ${o.g}, ${o.b}, 0.5)`,
                                     l = `<svg xmlns="http://www.w3.org/2000/svg" width="${t}" height="${t}">` + `<circle cx="${i}" cy="${i}" r="${r}" stroke="rgba(${s.r}, ${s.g}, ${s.b}, ${s.a})" ` + `stroke-width="1" fill="${n}"/>` + "</svg>";
-                                m[a]["icon"] = Qa.toBase64String(ul.UTF8.getBytes(l)), m[a]["anchorX"] = i, m[a]["anchorY"] = i
-                            } else g.valueViewMode == yo.Value ? (m[a]["icon"] = this.EMPTY_ICON, m[a]["title"] = null != d.rows[c][p] ? d.rows[c][p].toString() : "", m[a]["anchorX"] = 1, m[a]["anchorY"] = 7) : g.valueViewMode == yo.Icon ? (null == g.customIcon && (m[a]["fontIcon"] = Ha.getContent(g.icon).charCodeAt(0), m[a]["fontIconColor"] = `rgb(${g.iconColor.r}, ${g.iconColor.g}, ${g.iconColor.b})`), 0 < p && (m[a]["title"] = null != d.rows[c][p] ? d.rows[c][p].toString() : "")) : g.valueViewMode == yo.Chart && (m[a]["chart"] = this.getChartData(d, s, p, l, d.rows[c][s]), m[a]["icon"] = this.EMPTY_ICON);
+                                m[a]["icon"] = qa.toBase64String(ul.UTF8.getBytes(l)), m[a]["anchorX"] = i, m[a]["anchorY"] = i
+                            } else g.valueViewMode == Co.Value ? (m[a]["icon"] = this.EMPTY_ICON, m[a]["title"] = null != d.rows[c][p] ? d.rows[c][p].toString() : "", m[a]["anchorX"] = 1, m[a]["anchorY"] = 7) : g.valueViewMode == Co.Icon ? (null == g.customIcon && (m[a]["fontIcon"] = za.getContent(g.icon).charCodeAt(0), m[a]["fontIconColor"] = `rgb(${g.iconColor.r}, ${g.iconColor.g}, ${g.iconColor.b})`), 0 < p && (m[a]["title"] = null != d.rows[c][p] ? d.rows[c][p].toString() : "")) : g.valueViewMode == Co.Chart && (m[a]["chart"] = this.getChartData(d, s, p, l, d.rows[c][s]), m[a]["icon"] = this.EMPTY_ICON);
                         c++
                     }
-                    r["locations"] = m, r["locationType"] = ve.getName(wo, g.locationType)
-                }(g.valueViewMode == yo.Icon || -1 != o && -1 != a) && null != g.customIcon && this.getCustomIcon(g.customIcon, r), r["theme"] = e ? "canvasDark" : "canvasLight", r["culture"] = bo[g.culture].toString().replace("_", "-");
+                    r["locations"] = m, r["locationType"] = ve.getName(bo, g.locationType)
+                }(g.valueViewMode == Co.Icon || -1 != o && -1 != a) && null != g.customIcon && this.getCustomIcon(g.customIcon, r), r["theme"] = e ? "canvasDark" : "canvasLight", r["culture"] = fo[g.culture].toString().replace("_", "-");
                 let t = J.getBackColor(g);
-                return N.transparent.equals(t) && null != g.report && g.report.info.fillComponent && g.isDesigning && (t = N.fromArgb3(153, N.white)), r["backgroundColor"] = Mu.toHtml(t), r["onePointZoom"] = g.onePointZoom, r["userBingKey"] = g.userBingKey, r
+                return N.transparent.equals(t) && null != g.report && g.report.info.fillComponent && g.isDesigning && (t = N.fromArgb3(153, N.white)), r["backgroundColor"] = Tu.toHtml(t), r["onePointZoom"] = g.onePointZoom, r["userBingKey"] = g.userBingKey, r
             }
             static getChartData(t, r, i, s, y) {
-                let n = new Co;
+                let n = new xo;
                 try {
                     if (0 <= r && 0 <= i && 0 <= s) {
                         let h = this.CHART_RADIUS,
                             m = t.meters[s],
                             c = t.meters[i],
                             d = t.meters[r],
                             e = t.rows.where(e => e[r] == y),
-                            g = e.groupBy2(e => [e[s]], new xh).select(e => e.key[L.System.StiObject.stimulsoft]().toArray()[0]).toList(),
+                            g = e.groupBy2(e => [e[s]], new Mh).select(e => e.key[L.System.StiObject.stimulsoft]().toArray()[0]).toList(),
                             p = new P;
                         for (let t of g) p.add(e.where(e => e[s] == t).select(e => e[i]).sum(e => V.tryToNumber(e)));
                         let S = p.sum(),
                             w = this.getColors(Math.min(g.countItems, this.MAX_CHART_SECTORS)),
                             b = 0,
                             f = [];
                         for (let u = 0; u < Math.min(g.countItems, this.MAX_CHART_SECTORS); u++) {
@@ -11221,19 +11219,19 @@
                                 t = p[u],
                                 r = t / S * 6.28318530716,
                                 i = h + 1 + h * Math.cos(b),
                                 s = h + 1 + h * Math.sin(b),
                                 n = h + 1 + h * Math.cos(b + r),
                                 l = h + 1 + h * Math.sin(b + r),
                                 a = .5 < t / S ? 1 : 0,
-                                o = Th.dark(w[u], 100);
+                                o = Fh.dark(w[u], 100);
                             f.push({
                                 stroke: `rgb(${o.r}, ${o.g}, ${o.b})`,
                                 fill: `rgb(${w[u].r}, ${w[u].g}, ${w[u].b})`,
-                                _color: Mu.toHtml(w[u]),
+                                _color: Tu.toHtml(w[u]),
                                 d: `M ${h+1} ${h+1} L ${this.toUnits(i)} ${this.toUnits(s)} A ${h} ${h} 0 ${a} 1 ${this.toUnits(n)} ${this.toUnits(l)}z`,
                                 _text0: d.label,
                                 _text1: null != y ? y.toString() : null,
                                 _text2: m.label,
                                 _text3: null != e ? e.toString() : null,
                                 _text4: c.label,
                                 _text5: t.toString
@@ -11249,39 +11247,39 @@
                     r = ae.round2(e, t).toString().replace(",", ".");
                 return r
             }
             static getCustomIcon(s, n) {
                 try {
                     let t, r = 0,
                         i = 0;
-                    if (!Lu.isSvg(s)) {
-                        t = Ba.bytesToImage(s);
+                    if (!Bu.isSvg(s)) {
+                        t = Pa.bytesToImage(s);
                         let e = Math.min(1, 2 * this.MAX_RADIUS / Math.max(t.width, t.height));
                         r = Math.round(t.width * e), i = Math.round(t.height * e)
                     }
                     n["customIconAnchorX"] = r / 2, n["customIconAnchorY"] = i;
                     let e = `<svg xmlns="http://www.w3.org/2000/svg" width="${r}" height="${i}"><image width="${r}" height="${i}" href="${this.imageBytesToBase64String(s)}"></image></svg>`;
-                    n["customIcon"] = Qa.toBase64String(ul.UTF8.getBytes(e))
+                    n["customIcon"] = qa.toBase64String(ul.UTF8.getBytes(e))
                 } catch (e) {}
             }
             static imageBytesToBase64String(e) {
                 let t = "data:image/png;base64,";
-                return Lu.isBmp(e) ? t = "data:image/bmp;base64," : Lu.isJpeg(e) ? t = "data:image/jpeg;base64," : Lu.isGif(e) ? t = "data:image/gif;base64," : Lu.isSvg(e) && (t = "data:image/svg+xml;base64,"), t + Qa.toBase64String(e)
+                return Bu.isBmp(e) ? t = "data:image/bmp;base64," : Bu.isJpeg(e) ? t = "data:image/jpeg;base64," : Bu.isGif(e) ? t = "data:image/gif;base64," : Bu.isSvg(e) && (t = "data:image/svg+xml;base64,"), t + qa.toBase64String(e)
             }
             static getColors(e) {
                 let t = new P,
                     r = 10,
                     i = !0,
-                    s = Fh.getColors();
+                    s = vh.getColors();
                 t.addRange(s[L.System.StiObject.stimulsoft]().toList());
                 while (t.length < e) {
                     if (i)
-                        for (let e of s) t.add(Th.dark(e, r));
+                        for (let e of s) t.add(Fh.dark(e, r));
                     else {
-                        for (let e of s) t.add(Th.light(e, r));
+                        for (let e of s) t.add(Fh.light(e, r));
                         r += 10
                     }
                     i = !i
                 }
                 return t
             }
             static getLongitudeMeterIndex(e) {
@@ -11322,15 +11320,15 @@
                             let r = t.substring(1).toLowerCase(),
                                 i = "";
                             for (let t = 0; t < r.length; t++) {
                                 let e = r.charAt(t);
                                 "0" != e && "1" != e && "2" != e && "3" != e && "4" != e && "5" != e && "6" != e && "7" != e && "8" != e && "9" != e && "a" != e && "b" != e && "c" != e && "d" != e && "e" != e && "f" != e || (i += e)
                             }
                             if (6 == (r = 3 == i.length ? B.format("{0}{0}{1}{1}{2}{2}", i[0], i[1], i[2]) : i).length) {
-                                let e = Qa.toInt32(r, 16);
+                                let e = qa.toInt32(r, 16);
                                 s = N.fromArgb(255, e >> 16 & 255, e >> 8 & 255, 255 & e)
                             }
                         } else if (t[L.System.StiObject.stimulsoft]().startsWith("rgb")) {
                             let r = t.trim().substring(4, t.length - 1).split(",");
                             if (3 == r.length) {
                                 let e = [0, 0, 0];
                                 r[0][L.System.StiObject.stimulsoft]().endsWith("%") ? e[0] = Math.round(2.55 * V.tryToNumber(r[0].substring(0, r[0].length - 1))) : e[0] = V.tryToNumber(r[0]), r[1][L.System.StiObject.stimulsoft]().endsWith("%") ? e[1] = Math.round(2.55 * V.tryToNumber(r[1].substring(0, r[1].length - 1))) : e[1] = V.tryToNumber(r[1]), r[2][L.System.StiObject.stimulsoft]().endsWith("%") ? e[2] = Math.round(2.55 * V.tryToNumber(r[2].substring(0, r[2].length - 1))) : e[2] = V.tryToNumber(r[2]), s = N.fromArgb(255, e[0], e[1], e[2])
@@ -11485,112 +11483,112 @@
                                 ["Violet", "#EE82EE"],
                                 ["Wheat", "#F5DEB3"],
                                 ["White", "#FFFFFF"],
                                 ["WhiteSmoke", "#F5F5F5"],
                                 ["Yellow", "#FFFF00"],
                                 ["YellowGreen", "#9ACD32"]
                             ];
-                            this.htmlNameToColor = new Co;
+                            this.htmlNameToColor = new xo;
                             for (let i = 0; i < 2; i++) {
                                 let e = s[i][0].toLowerCase(),
-                                    t = Qa.toInt32(s[i][1].substring(1), 16),
+                                    t = qa.toInt32(s[i][1].substring(1), 16),
                                     r = N.fromArgb(255, t >> 16 & 255, t >> 8 & 255, 255 & t);
                                 this.htmlNameToColor.set(e, r)
                             }
                         }
                         let e = t.toLowerCase();
                         this.htmlNameToColor.containsKey(e) && (s = this.htmlNameToColor.get(e))
                     }
                 } catch (e) {}
                 return s
             }
         }
-        zd.MAX_LOCATIONS = 1e3, zd.MAX_CHART_SECTORS = 100, zd.MIN_RADIUS = 3, zd.MAX_RADIUS = 15, zd.CHART_RADIUS = 26, zd.DELTA_RADIUS = 12, zd.lockHtmlNameToColor = new Object, F.h.StiOnlineMapHelper = zd
+        Gd.MAX_LOCATIONS = 1e3, Gd.MAX_CHART_SECTORS = 100, Gd.MIN_RADIUS = 3, Gd.MAX_RADIUS = 15, Gd.CHART_RADIUS = 26, Gd.DELTA_RADIUS = 12, Gd.lockHtmlNameToColor = new Object, F.h.StiOnlineMapHelper = Gd
     }
-    let vh = L.Report.Dictionary.StiDataTableSource,
-        Ah = L.Report.Engine.StiAsmCommandType,
-        Ih = L.Report.Engine.StiParserParameters,
-        Dh = F.N.StiPivotTableColumnVisibilityHelper,
-        Rh = L.Report.CrossTab.Core.StiCellType,
-        Eh = L.Report.Components.StiDataHelper,
-        Oh = L.Report.Components.StiFilter,
-        Vh = L.Report.Components.StiCondition,
-        kh = L.Data.Helpers.StiLabelHelper,
-        Nh = L.Report.Engine.StiEngine,
-        Lh = L.System.Drawing.ContentAlignment,
-        Bh = L.Report.Components.StiIconSetIndicator,
-        Ph = L.Report.Dashboard.StiPivotToConvertedStateCache,
-        jh = L.Report.Dashboard.StiPivotTableToCrossTabCache,
-        Hh = L.Report.CrossTab.StiCrossTotal,
-        zh = L.Report.CrossTab.StiCrossRowTotal,
-        Gh = L.Report.CrossTab.StiCrossTab,
-        Xh = L.Report.CrossTab.StiCrossTitle,
-        Wh = L.Report.Components.StiComponentsCollection,
-        Jh = L.Report.CrossTab.StiCrossColumnTotal,
-        Uh = L.Report.CrossTab.StiCrossSummary,
-        Zh = F.N.StiPivotTableElement,
-        Yh = L.Report.CrossTab.Core.StiCell,
-        Kh = L.Report.CrossTab.StiCrossColumn,
-        Qh = L.Report.StiReportUnitType,
-        qh = L.Report.StiReport,
-        _h = L.Report.CrossTab.StiCrossRow,
-        $h = L.Report.CrossTab.StiCrossSummaryHeader,
-        em = L.System.Guid,
-        tm = L.Report.CrossTab.StiCrossHeader,
-        rm = L.Report.CrossTab.Core.StiSummaryType,
-        im = L.Report.CrossTab.StiCrossCell,
-        sm = L.Report.CrossTab.Core.StiCross,
-        nm = L.Report.CrossTab.StiCrossTabHelper;
+    let Ah = L.Report.Dictionary.StiDataTableSource,
+        Ih = L.Report.Engine.StiAsmCommandType,
+        Dh = L.Report.Engine.StiParserParameters,
+        Rh = F.N.StiPivotTableColumnVisibilityHelper,
+        Eh = L.Report.CrossTab.Core.StiCellType,
+        Oh = L.Report.Components.StiDataHelper,
+        Vh = L.Report.Components.StiFilter,
+        kh = L.Report.Components.StiCondition,
+        Nh = L.Data.Helpers.StiLabelHelper,
+        Lh = L.Report.Engine.StiEngine,
+        Bh = L.System.Drawing.ContentAlignment,
+        Ph = L.Report.Components.StiIconSetIndicator,
+        jh = L.Report.Dashboard.StiPivotToConvertedStateCache,
+        Hh = L.Report.Dashboard.StiPivotTableToCrossTabCache,
+        zh = L.Report.CrossTab.StiCrossTotal,
+        Gh = L.Report.CrossTab.StiCrossRowTotal,
+        Xh = L.Report.CrossTab.StiCrossTab,
+        Wh = L.Report.CrossTab.StiCrossTitle,
+        Jh = L.Report.Components.StiComponentsCollection,
+        Uh = L.Report.CrossTab.StiCrossColumnTotal,
+        Zh = L.Report.CrossTab.StiCrossSummary,
+        Yh = F.N.StiPivotTableElement,
+        Kh = L.Report.CrossTab.Core.StiCell,
+        Qh = L.Report.CrossTab.StiCrossColumn,
+        qh = L.Report.StiReportUnitType,
+        _h = L.Report.StiReport,
+        $h = L.Report.CrossTab.StiCrossRow,
+        em = L.Report.CrossTab.StiCrossSummaryHeader,
+        tm = L.System.Guid,
+        rm = L.Report.CrossTab.StiCrossHeader,
+        im = L.Report.CrossTab.Core.StiSummaryType,
+        sm = L.Report.CrossTab.StiCrossCell,
+        nm = L.Report.CrossTab.Core.StiCross,
+        lm = L.Report.CrossTab.StiCrossTabHelper;
     {
-        class Ud {
+        class Zd {
             static getHeadersBounds(i) {
                 let s = -1,
                     n = -1,
                     l = -1,
                     a = -1;
                 for (let r = 0; r < i.length; r++)
                     for (let t = 0; t < i[r].length; t++) {
                         let e = i[r][t];
-                        e.cellType != Rh.HeaderColMain && e.cellType != Rh.HeaderColSummaryTotal || (s = -1 == s ? t : s, n = Math.max(t, n)), e.cellType != Rh.HeaderRowMain && e.cellType != Rh.HeaderRowSummaryTotal || (l = -1 == l ? r : l, a = Math.max(r, a))
+                        e.cellType != Eh.HeaderColMain && e.cellType != Eh.HeaderColSummaryTotal || (s = -1 == s ? t : s, n = Math.max(t, n)), e.cellType != Eh.HeaderRowMain && e.cellType != Eh.HeaderRowSummaryTotal || (l = -1 == l ? r : l, a = Math.max(r, a))
                     }
                 return new j(l, s, a - l, n - s)
             }
             static async getViewerData(e) {
                 let t = {},
-                    r = e.as(Zh),
-                    i = r.columns.where(e => Dh.getVisible(e, r.report)).toList(),
-                    s = r.rows.where(e => Dh.getVisible(e, r.report)).toList(),
-                    n = r.summaries.where(e => Dh.getVisible(e, r.report)).toList(),
-                    l = jh.get(r);
+                    r = e.as(Yh),
+                    i = r.columns.where(e => Rh.getVisible(e, r.report)).toList(),
+                    s = r.rows.where(e => Rh.getVisible(e, r.report)).toList(),
+                    n = r.summaries.where(e => Rh.getVisible(e, r.report)).toList(),
+                    l = Hh.get(r);
                 if (null == l) {
                     let e = await bl.getOrCreate(r);
-                    l = await Ud.convertToCrossTab(r, e), jh.put(r, l), Ph.putFalse(r)
+                    l = await Zd.convertToCrossTab(r, e), Hh.put(r, l), jh.putFalse(r)
                 }
                 let a = 0 == s.length && 0 == i.length && 0 < n.length,
                     o = l.crossTabInfo.cross.cells,
                     u = this.getHeadersBounds(o),
                     h = u.bottom + 1,
                     m = u.right + 1,
-                    c = (t["headerHeight"] = h, t["headerWidth"] = m, t["onlySummaries"] = a, t["pivotColumnsCount"] = i.length, t["pivotRowsCount"] = s.length, t["pivotSummariesCount"] = n.length, t["pivotSummaryDirection"] = ve.getName(xo, r.summaryDirection), []);
+                    c = (t["headerHeight"] = h, t["headerWidth"] = m, t["onlySummaries"] = a, t["pivotColumnsCount"] = i.length, t["pivotRowsCount"] = s.length, t["pivotSummariesCount"] = n.length, t["pivotSummaryDirection"] = ve.getName(Mo, r.summaryDirection), []);
                 if (0 < o.length) {
-                    let l = new Co;
+                    let l = new xo;
                     for (let r = 0; r < o.length; r++)
                         for (let t = 0; t < o[r].length; t++) {
                             let e = o[r][t];
                             B.isNullOrEmpty(e.parentGuid) || e.parentCell != e || (l.containsKey(e.parentGuid) || l.set(e.parentGuid, new P), l.get(e.parentGuid).add(e))
                         }
                     let a = [];
                     for (let n = 0; n < o.length; n++) {
                         let s = [];
                         for (let e = 0; e < o[0].length; e++) {
                             let t = o[n][e],
                                 r = new P,
                                 i = null;
                             if (t.parentCell == t && !B.isNullOrEmpty(t.guid) && l.containsKey(t.guid))
-                                for (let e of l.get(t.guid)) e.field.is(Hh) && e.parentCell == e ? i = e.guid : r.add(e.guid);
+                                for (let e of l.get(t.guid)) e.field.is(zh) && e.parentCell == e ? i = e.guid : r.add(e.guid);
                             s.push(this.cellItem(o[n][e], n, e, r, i, n < m || e < h, a, n >= m))
                         }
                         c.push(s)
                     }
                     t["cells"] = c, t["sizes"] = a
                 }
                 return t
@@ -11599,35 +11597,35 @@
                 var o, u, h, m, c, d;
                 let g = null == (u = null == (o = s.field) ? void 0 : o.report) ? void 0 : u.unit,
                     p = -1;
                 if (s.field && null != g) {
                     let e = `${g.convertToHInches(null==(h=s.field)?void 0:h.minSize.width)};${g.convertToHInches(null==(m=s.field)?void 0:m.maxSize.width)};` + (null != (c = s.field) && c.wordWrap ? "True" : "False"); - 1 == l.indexOf(e) && l.push(e), p = l.indexOf(e)
                 }
                 let S = {};
-                if (S["rowSpan"] = s.height, S["colSpan"] = s.width, S["row"] = t, S["column"] = e, S["text"] = s.text, S["isColumn"] = a, S["s"] = p, S["l"] = s.level, null != (d = s.field) && d.is(tm) && (S["o"] = s.field.isExpanded), n && (B.isNullOrEmpty(s.guid) && (s.guid = em.newGuid().toString()), B.isNullOrEmpty(s.parentGuid) || (S["parentGuid"] = s.parentGuid), null != s.parentCell && s.parentCell == s && (S["parentCellGuid"] = s.parentCell.guid), null != s.field && (S["isTotal"] = s.field.is(Hh) && s.parentCell == s), S["guid"] = s.guid, 0 < r.length && (S["dependedCellGuis"] = r), null != i) && (S["totalCellGuid"] = i), null != s.field && null != s.field.indicator && s.field.indicator[L.System.StiObject.stimulsoft]().is(Bh)) {
-                    let e = s.field.indicator.as(Bh),
-                        t = ve.getName(Lh, e.alignment),
+                if (S["rowSpan"] = s.height, S["colSpan"] = s.width, S["row"] = t, S["column"] = e, S["text"] = s.text, S["isColumn"] = a, S["s"] = p, S["l"] = s.level, null != (d = s.field) && d.is(rm) && (S["o"] = s.field.isExpanded), n && (B.isNullOrEmpty(s.guid) && (s.guid = tm.newGuid().toString()), B.isNullOrEmpty(s.parentGuid) || (S["parentGuid"] = s.parentGuid), null != s.parentCell && s.parentCell == s && (S["parentCellGuid"] = s.parentCell.guid), null != s.field && (S["isTotal"] = s.field.is(zh) && s.parentCell == s), S["guid"] = s.guid, 0 < r.length && (S["dependedCellGuis"] = r), null != i) && (S["totalCellGuid"] = i), null != s.field && null != s.field.indicator && s.field.indicator[L.System.StiObject.stimulsoft]().is(Ph)) {
+                    let e = s.field.indicator.as(Ph),
+                        t = ve.getName(Bh, e.alignment),
                         r = 0 == t.indexOf("Top") ? "top" : 0 == t.indexOf("Bottom") ? "bottom" : "middle",
-                        i = `<img src='data:image/png;base64,${Qa.toBase64String(e.customIcon)}' style='vertical-align: ${r};'>`;
+                        i = `<img src='data:image/png;base64,${qa.toBase64String(e.customIcon)}' style='vertical-align: ${r};'>`;
                     delete S["text"], 0 < t.indexOf("Left") ? S["text"] = i + s.text : S["text"] = s.text + i
                 }
                 let w = null != s.field ? s.field.conditionPermissions : null,
                     b = {};
                 if (s.isNegativeColor) {
                     let e = Z.Engine.negativeColor;
                     b["color"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                 }
-                if (w != Ao.None) {
-                    if (0 < (w & Ao.BackColor)) {
+                if (w != Io.None) {
+                    if (0 < (w & Io.BackColor)) {
                         let e = s.field.conditionBrush.color;
                         b["backgroundColor"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                     }
-                    0 < (w & Ao.Font) && (b["fontFamily"] = s.field.font.name), 0 < (w & Ao.FontSize) && (b["fontSize"] = s.field.font.sizeInPoints + `pt`), 0 < (w & Ao.FontStyleBold) && (b["fontWeight"] = 0 < (s.field.font.style & hn.Bold) ? "bold" : "normal"), 0 < (w & Ao.FontStyleItalic) && (b["fontStyle"] = 0 < (s.field.font.style & hn.Italic) ? "italic " : "normal");
+                    0 < (w & Io.Font) && (b["fontFamily"] = s.field.font.name), 0 < (w & Io.FontSize) && (b["fontSize"] = s.field.font.sizeInPoints + `pt`), 0 < (w & Io.FontStyleBold) && (b["fontWeight"] = 0 < (s.field.font.style & hn.Bold) ? "bold" : "normal"), 0 < (w & Io.FontStyleItalic) && (b["fontStyle"] = 0 < (s.field.font.style & hn.Italic) ? "italic " : "normal");
                     let e = "";
-                    if (0 < (w & Ao.FontStyleStrikeout) && 0 < (s.field.font.style & hn.Strikeout) && (e += "line-through "), 0 < (w & Ao.FontStyleUnderline) && 0 < (s.field.font.style & hn.Underline) && (e += "underline"), B.isNullOrEmpty(e) || (b["textDecoration"] = e), 0 < (w & Ao.TextColor)) {
+                    if (0 < (w & Io.FontStyleStrikeout) && 0 < (s.field.font.style & hn.Strikeout) && (e += "line-through "), 0 < (w & Io.FontStyleUnderline) && 0 < (s.field.font.style & hn.Underline) && (e += "underline"), B.isNullOrEmpty(e) || (b["textDecoration"] = e), 0 < (w & Io.TextColor)) {
                         let e = s.field.conditionTextBrush.color;
                         b["color"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                     }
                 }
                 if (null != s.field) switch (s.field.horAlignment) {
                     case X.Left:
                         b["text-align"] = "left";
@@ -11643,77 +11641,77 @@
                         break
                 }
                 return S["style"] = b, S
             }
             static applyStyle(e, t, s) {
                 let n = J.getPivotTableStyle(e),
                     l = t.crossTabInfo.cross.cells,
-                    a = e.columns.length + (0 < e.rows.length ? 1 : 0) + (1 < e.summaries.length && e.summaryDirection == xo.LeftToRight ? 1 : 0),
-                    o = (0 == e.rows.length ? 1 : e.rows.length) + (1 < e.summaries.length && e.summaryDirection == xo.UpToDown ? 1 : 0);
+                    a = e.columns.length + (0 < e.rows.length ? 1 : 0) + (1 < e.summaries.length && e.summaryDirection == Mo.LeftToRight ? 1 : 0),
+                    o = (0 == e.rows.length ? 1 : e.rows.length) + (1 < e.summaries.length && e.summaryDirection == Mo.UpToDown ? 1 : 0);
                 for (let i = 0; i < l.length; i++)
                     for (let r = 0; r < l[i].length; r++)
                         if (null != l[i][r].field) {
                             let e = l[i][r],
-                                t = !(e.isCrossSummary || e.field.is2(Uh) || (e.field.is2(zh) || e.field.is2(Jh)) && null == e.guid);
+                                t = !(e.isCrossSummary || e.field.is2(Zh) || (e.field.is2(Gh) || e.field.is2(Uh)) && null == e.guid);
                             s ? (e.field.font = new H("Arial", 10, t ? hn.Bold : hn.Regular), e.field.brush = new v(N.transparent), e.field.textBrush = new v(N.black)) : t ? (i < o && r >= a ? e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.rowHeaderBackColor) : e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.columnHeaderBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(n.columnHeaderForeColor)) : (e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(r % 2 != 0 ? n.alternatingCellBackColor : n.cellBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(r % 2 != 0 ? n.alternatingCellForeColor : n.cellForeColor)), e.field.border.color = n.lineColor
                         }
             }
             static buildCross(l, n, t) {
-                let a = new Co;
+                let a = new xo;
                 for (let e = 0; e < n.meters.length; e++) a.set(n.meters[e].expression, e);
                 l.crossTabInfo.startRow = 0, l.crossTabInfo.startCol = 0;
-                let u = new Wh(null),
-                    h = new Wh(null),
-                    m = new Wh(null),
-                    c = new Wh(null),
-                    d = new Wh(null),
-                    g = new Wh(null),
-                    i = t.columns.where(e => Dh.getVisible(e, t.report)).toList(),
-                    s = t.rows.where(e => Dh.getVisible(e, t.report)).toList(),
-                    o = t.summaries.where(e => Dh.getVisible(e, t.report)).toList(),
+                let u = new Jh(null),
+                    h = new Jh(null),
+                    m = new Jh(null),
+                    c = new Jh(null),
+                    d = new Jh(null),
+                    g = new Jh(null),
+                    i = t.columns.where(e => Rh.getVisible(e, t.report)).toList(),
+                    s = t.rows.where(e => Rh.getVisible(e, t.report)).toList(),
+                    o = t.summaries.where(e => Rh.getVisible(e, t.report)).toList(),
                     p = null,
                     S = null,
                     w = null,
                     b = new Mt;
                 for (let n of l.components.list)
-                    if (n.is(im) || n.is(Xh) || n.is($h)) {
-                        let e = n.as(_h),
-                            t = n.as(Kh),
-                            o = n.as(Uh),
-                            r = n.as($h),
-                            i = n.as(Xh);
+                    if (n.is(sm) || n.is(Wh) || n.is(em)) {
+                        let e = n.as($h),
+                            t = n.as(Qh),
+                            o = n.as(Zh),
+                            r = n.as(em),
+                            i = n.as(Wh);
                         if (null != i) {
                             i.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Row:") && d.add(i), i.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Col:") && g.add(i), i.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("LeftTitle") && (p = i), i.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("RightTitle") && (S = i), i.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("SummaryTitle") && (w = i);
                             continue
                         }
                         if (null != e && (h.add(e), e.isTotalVisible || (e.total.height = 0)), null != t && (u.add(t), t.isTotalVisible || (t.total.width = 0)), null != o && !o.disabledByCondition && o.enabled) {
                             m.add(o), o.arguments.clear(), o.report.dictionary.dataSources.cachedDataSources = {};
                             for (let e of o.report.dictionary.dataSources.list) 0 < e.name.indexOf(" ") && (o.report.dictionary.dataSources.cachedDataSources[e.name.toLowerCase().split(" ").join("")] = e);
                             try {
-                                let e = new Ih,
+                                let e = new Dh,
                                     t = (e.returnAsmList = !0, Dl.parseTextValue2(o.value, o, null, e)),
-                                    r = t.where(e => e.type == Ah.PushDataSourceField);
+                                    r = t.where(e => e.type == Ih.PushDataSourceField);
                                 1 < r.length && (r.forEach(e => {
                                     let t = e.parameter1;
                                     if (!o.arguments.containsKey(t)) {
                                         o.arguments.add(t, o.summary + `(${t})`);
                                         let e = new yt(t, Object);
                                         b.columns.add(e)
                                     }
                                 }), o.complexExpression = !0)
                             } catch (e) {}
                             o.conditions.toList().cast().forEach(l => {
                                 let a = `{${l.expression}}`;
                                 try {
-                                    let e = new Ih,
+                                    let e = new Dh,
                                         t = (e.returnAsmList = !0, Dl.parseTextValue2(a, o, null, e)),
                                         s = new P,
-                                        r = (t.where(e => e.type == Ah.PushValue).forEach(e => {
+                                        r = (t.where(e => e.type == Ih.PushValue).forEach(e => {
                                             var t, r;
-                                            let i = null == (r = null == (t = e.parameter1) ? void 0 : t[L.System.StiObject.stimulsoft]().as(P)) ? void 0 : r.where(e => e.Type == Ah.PushDataSourceField);
+                                            let i = null == (r = null == (t = e.parameter1) ? void 0 : t[L.System.StiObject.stimulsoft]().as(P)) ? void 0 : r.where(e => e.Type == Ih.PushDataSourceField);
                                             null != i && s.addRange(i)
                                         }), o.report.engine.parserConversionStore.get("*StiConditionExpression*" + o.name)),
                                         i = r.findIndex(e => e.key == l),
                                         n = r[i].value;
                                     s.forEach(e => {
                                         let t = e.parameter1;
                                         if (!o.arguments.containsKey(t)) {
@@ -11727,139 +11725,139 @@
                                         value: n
                                     })
                                 } catch (e) {}
                             }), o.report.dictionary.dataSources.cachedDataSources = {}
                         }
                         null != r && c.add(r);
                         let s = new yt(n.name, Object);
-                        b.columns.add(s), n.is(tm) && (s = new yt("Display__" + n.name, Object), b.columns.add(s))
+                        b.columns.add(s), n.is(rm) && (s = new yt("Display__" + n.name, Object), b.columns.add(s))
                     } for (let s of n.rows) {
                     let i = b.newRow();
                     for (let r of l.components.list) {
-                        if (r.is($h)) continue;
-                        let t = r.as(im);
+                        if (r.is(em)) continue;
+                        let t = r.as(sm);
                         if (null != t) {
                             let e = a.contains(r.alias) ? s[a.get(r.alias)] : null;
-                            if ("number" == typeof(e = Ln.isArray(e) ? new P(e).firstOrDefault() : e) && (e = e[L.System.StiObject.stimulsoft]().toNumber()), i.sett(t.name, e), t.is(tm) && i.sett("Display__" + r.name, s[a.get(r.alias)]), t.is(Uh))
+                            if ("number" == typeof(e = Ln.isArray(e) ? new P(e).firstOrDefault() : e) && (e = e[L.System.StiObject.stimulsoft]().toNumber()), i.sett(t.name, e), t.is(rm) && i.sett("Display__" + r.name, s[a.get(r.alias)]), t.is(Zh))
                                 for (let e of t.arguments) i.sett(e.key, a.contains(e.value) ? s[a.get(e.value)] : null)
-                        } else if (r.is(Xh) && !B.isNullOrEmpty(r.alias)) {
+                        } else if (r.is(Wh) && !B.isNullOrEmpty(r.alias)) {
                             let e = s[a.get(r.alias)];
                             r.setTextInternal(e.toString())
                         }
                     }
                     b.rows.add(i), l.next()
                 }
-                let f = new sm,
-                    r = (l.crossTabInfo.cross = f, l.crossTabInfo.cross.designTime = !1, l.crossTabInfo.cross.colFields = u, l.crossTabInfo.cross.rowFields = h, l.crossTabInfo.cross.sumFields = m, l.crossTabInfo.cross.sumHeaderFields = c, l.crossTabInfo.cross.colTitleFields = g, l.crossTabInfo.cross.rowTitleFields = d, l.crossTabInfo.cross.leftCrossTitle = p, l.crossTabInfo.cross.rightCrossTitle = S, l.crossTabInfo.cross.summaryCrossTitle = w, (l.crossTabInfo.cross.crossTab = l).dataSourceName = "pivot", new vh("pivot", "pivot"));
+                let f = new nm,
+                    r = (l.crossTabInfo.cross = f, l.crossTabInfo.cross.designTime = !1, l.crossTabInfo.cross.colFields = u, l.crossTabInfo.cross.rowFields = h, l.crossTabInfo.cross.sumFields = m, l.crossTabInfo.cross.sumHeaderFields = c, l.crossTabInfo.cross.colTitleFields = g, l.crossTabInfo.cross.rowTitleFields = d, l.crossTabInfo.cross.leftCrossTitle = p, l.crossTabInfo.cross.rightCrossTitle = S, l.crossTabInfo.cross.summaryCrossTitle = w, (l.crossTabInfo.cross.crossTab = l).dataSourceName = "pivot", new Ah("pivot", "pivot"));
                 r.dictionary = l.report.dictionary;
                 for (let e of b.columns.list) r.columns.add(new oi(e.columnName, e.columnName, e.columnName));
-                r.dataTable = b, l.report.dictionary.dataSources.add(r), l.summaryDirection = 1 < (null == o ? void 0 : o.length) ? t.summaryDirection : xo.UpToDown, l.crossTabInfo.cross.create(b, l.report, l.summaryDirection, l.emptyValue), l.crossTabInfo.cross.crossTab = null;
+                r.dataTable = b, l.report.dictionary.dataSources.add(r), l.summaryDirection = 1 < (null == o ? void 0 : o.length) ? t.summaryDirection : Mo.UpToDown, l.crossTabInfo.cross.create(b, l.report, l.summaryDirection, l.emptyValue), l.crossTabInfo.cross.crossTab = null;
                 let y = J.getPivotTableStyle(t),
                     e = 0 == s.length && 0 == i.length && 0 < o.length;
                 if (e) {
                     f.init(2, o.length);
                     for (let i = 0; i < o.length; i++) {
                         let e = o[i],
-                            t = new Kh,
-                            r = (t.alias = e.expression, t.name = "CrossTab_Sum" + i.toString(), t.page = l.page, t.horAlignment = X.Center, t.textFormat = e.textFormat.clone(), t.guid = em.newGuidString(), t.font = U.Table.Font.getCachedGdiFont(), t.brush = new v(y.cellBackColor), t.hideZeros = e.hideZeros, t.border = new ie(i == o.length - 1 ? G.Right | G.Top : 0 == i ? G.Right | G.Bottom : G.Right | G.Bottom | G.Top, y.lineColor, 1, Ri.Solid), t.height = U.Table.getHeight(t.font), f.cells[0][i] = new Yh, f.cells[0][i].text = this.getLabel(e), f.cells[0][i].field = t, f.cells[0][i].parentCell = f.cells[0][i], new Uh);
-                        r.name = "CrossTab_Sum" + i.toString(), r.value = 0 < n.rows.length ? n.rows[0][i].toString() : "", r.page = l.page, r.horAlignment = X.Right, r.textFormat = e.textFormat.clone(), r.guid = em.newGuidString(), r.font = U.Table.Font.getCachedGdiFont(), r.border = new ie(G.None, y.lineColor, 1, Ri.Solid), r.height = U.Table.getHeight(r.font), f.cells[1][i] = new Yh, f.cells[1][i].field = r, f.cells[1][i].text = 0 < n.rows.length ? n.rows[0][i].toString() : "", f.cells[1][i].parentCell = f.cells[1][i]
+                            t = new Qh,
+                            r = (t.alias = e.expression, t.name = "CrossTab_Sum" + i.toString(), t.page = l.page, t.horAlignment = X.Center, t.textFormat = e.textFormat.clone(), t.guid = tm.newGuidString(), t.font = U.Table.Font.getCachedGdiFont(), t.brush = new v(y.cellBackColor), t.hideZeros = e.hideZeros, t.border = new ie(i == o.length - 1 ? G.Right | G.Top : 0 == i ? G.Right | G.Bottom : G.Right | G.Bottom | G.Top, y.lineColor, 1, Ri.Solid), t.height = U.Table.getHeight(t.font), f.cells[0][i] = new Kh, f.cells[0][i].text = this.getLabel(e), f.cells[0][i].field = t, f.cells[0][i].parentCell = f.cells[0][i], new Zh);
+                        r.name = "CrossTab_Sum" + i.toString(), r.value = 0 < n.rows.length ? n.rows[0][i].toString() : "", r.page = l.page, r.horAlignment = X.Right, r.textFormat = e.textFormat.clone(), r.guid = tm.newGuidString(), r.font = U.Table.Font.getCachedGdiFont(), r.border = new ie(G.None, y.lineColor, 1, Ri.Solid), r.height = U.Table.getHeight(r.font), f.cells[1][i] = new Kh, f.cells[1][i].field = r, f.cells[1][i].text = 0 < n.rows.length ? n.rows[0][i].toString() : "", f.cells[1][i].parentCell = f.cells[1][i]
                     }
                 }
-                if (l.rightToLeft && nm.makeRightToLeft(l), l.crossTabInfo.cross.doAutoSize(), !e) {
+                if (l.rightToLeft && lm.makeRightToLeft(l), l.crossTabInfo.cross.doAutoSize(), !e) {
                     for (let t = 0; t < f.cells.length; t++)
                         for (let e = 0; e < f.cells[t].length; e++) null != f.cells[t][e].field && (f.cells[t][e].field.margins = f.cells[t][e].field.margins.clone(), 0 == t && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Left), 0 == e && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Top), t == f.cells.length - 1 && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Right), e == f.cells[t].length - 1) && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Bottom);
                     let e = i.length + (0 < s.length ? 1 : 0),
                         r = (0 == s.length ? 1 : s.length) + (1 < o.length ? 1 : 0);
                     for (let t = e; t < f.cells[0].length; t++)
                         for (let e = r; e < f.cells.length; e++) null != f.cells[e][t].field && (f.cells[e][t].field.border.side = G.Left | G.Right);
                     if (1 < f.sumFields.count)
                         for (let e = 0; e < f.cells[0].length; e++) null != f.cells[r - 1][e].field && (f.cells[r - 1][e].field.border = new ie(G.All, y.lineColor, 1, Ri.Solid));
                     null != f.cells[0][0].field && (f.cells[0][0].field.border.side = G.Right | G.Bottom)
                 }
                 l.report.dictionary.dataSources.remove(r)
             }
             static async convertToCrossTab(e, t) {
-                let r = new qh,
-                    i = (r.info.zoom = 1, r.reportUnit = null != e && null != e.report ? e.report.reportUnit : Qh.HundredthsOfInch, new Nh(r)),
+                let r = new _h,
+                    i = (r.info.zoom = 1, r.reportUnit = null != e && null != e.report ? e.report.reportUnit : qh.HundredthsOfInch, new Lh(r)),
                     s = (r.engine = i, new Ie),
-                    n = (r.pages.add(s), r.dictionary.variables = e.report.dictionary.variables, r.dictionary.dataSources = e.report.dictionary.dataSources, new Gh);
+                    n = (r.pages.add(s), r.dictionary.variables = e.report.dictionary.variables, r.dictionary.dataSources = e.report.dictionary.dataSources, new Xh);
                 return n.name = "CrossTab", n.crossTabStyle = null, n.crossTabStyleIndex = 9, s.components.add(n), await this.updateCrossTab(n, e, t), s.components.remove(n), new Promise(e => {
                     e(n)
                 })
             }
             static async updateCrossTab(c, i, e, t = !0) {
-                let s = new Co,
+                let s = new xo,
                     n = new P,
                     l = new P,
                     r = new P,
                     a = "",
-                    o = new Co,
-                    u = new Co,
+                    o = new xo,
+                    u = new xo,
                     h = (n.clear(), l.clear(), new P),
                     m = new P,
-                    d = new Co,
+                    d = new xo,
                     g = J.getPivotTableStyle(i),
-                    p = i.columns.where(e => Dh.getVisible(e, i.report)).toList(),
-                    S = i.rows.where(e => Dh.getVisible(e, i.report)).toList(),
-                    w = i.summaries.where(e => Dh.getVisible(e, i.report)).toList(),
+                    p = i.columns.where(e => Rh.getVisible(e, i.report)).toList(),
+                    S = i.rows.where(e => Rh.getVisible(e, i.report)).toList(),
+                    w = i.summaries.where(e => Rh.getVisible(e, i.report)).toList(),
                     b = 0;
                 for (let r of S) {
-                    let e = new _h,
-                        t = (e.showTotal = r.showTotal, e.alias = r.expression, e.displayValue = "{" + r.expression + "}", e.value = e.displayValue, B.isNullOrEmpty(a) && 0 < r.expression.length && 0 <= r.expression.indexOf(".") && (a = r.expression.substring(0, r.expression.indexOf("."))), e.page = null, e.name = c.name + "_Row" + (b + 1).toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, r.horAlignment)), e.textFormat = r.textFormat.clone(), e.guid = em.newGuidString(), e.wordWrap = r.size.wordWrap, e.margins = new be(this.FieldMargin), e.sortDirection = r.sortDirection, e.expandExpression = r.expandExpression, 0 < r.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.maxWidth), 0)), 0 < r.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(r.size.minWidth), 0)), 0 < r.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(r.size.width), 0)), await this.getCondition(i, r, e), await this.setTopN(e, r.topN, i), this.setupTitle(e, g), o.add(r, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), d.set(e, e), h.add(e), e.total);
+                    let e = new $h,
+                        t = (e.showTotal = r.showTotal, e.alias = r.expression, e.displayValue = "{" + r.expression + "}", e.value = e.displayValue, B.isNullOrEmpty(a) && 0 < r.expression.length && 0 <= r.expression.indexOf(".") && (a = r.expression.substring(0, r.expression.indexOf("."))), e.page = null, e.name = c.name + "_Row" + (b + 1).toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, r.horAlignment)), e.textFormat = r.textFormat.clone(), e.guid = tm.newGuidString(), e.wordWrap = r.size.wordWrap, e.margins = new be(this.FieldMargin), e.sortDirection = r.sortDirection, e.expandExpression = r.expandExpression, 0 < r.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.maxWidth), 0)), 0 < r.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(r.size.minWidth), 0)), 0 < r.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(r.size.width), 0)), await this.getCondition(i, r, e), await this.setTopN(e, r.topN, i), this.setupTitle(e, g), o.add(r, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), d.set(e, e), h.add(e), e.total);
                     null == t && (t = this.createRowTotal(i, e, s, g), B.isNullOrWhiteSpace(r.totalLabel) || (t.text = r.totalLabel), e.totalGuid = t.guid, c.components.add(t)), d.set(t, t), n.add(t), b++
                 }
                 let f = 0;
                 for (let r of p) {
-                    let e = new Kh,
-                        t = (e.showTotal = r.showTotal, e.alias = r.expression, e.displayValue = "{" + r.expression + "}", e.value = e.displayValue, e.page = null, e.name = c.name + "_Column" + (f + 1).toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, r.horAlignment)), e.guid = em.newGuidString(), e.wordWrap = r.size.wordWrap, e.margins = new be(this.FieldMargin), e.sortDirection = r.sortDirection, e.expandExpression = r.expandExpression, 0 < r.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(r.size.minWidth), 0)), 0 < r.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.maxWidth), 0)), 0 < r.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(r.size.width), 0)), await this.getCondition(i, r, e), await this.setTopN(e, r.topN, i), B.isNullOrEmpty(a) && 0 < r.expression.length && 0 <= r.expression.indexOf(".") && (a = r.expression.substring(0, r.expression.indexOf("."))), e.textFormat = r.textFormat.clone(), this.setupTitle(e, g), u.add(r, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), d.set(e, e), m.add(e), e.total);
+                    let e = new Qh,
+                        t = (e.showTotal = r.showTotal, e.alias = r.expression, e.displayValue = "{" + r.expression + "}", e.value = e.displayValue, e.page = null, e.name = c.name + "_Column" + (f + 1).toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, r.horAlignment)), e.guid = tm.newGuidString(), e.wordWrap = r.size.wordWrap, e.margins = new be(this.FieldMargin), e.sortDirection = r.sortDirection, e.expandExpression = r.expandExpression, 0 < r.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(r.size.minWidth), 0)), 0 < r.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.maxWidth), 0)), 0 < r.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(r.size.width), 0)), await this.getCondition(i, r, e), await this.setTopN(e, r.topN, i), B.isNullOrEmpty(a) && 0 < r.expression.length && 0 <= r.expression.indexOf(".") && (a = r.expression.substring(0, r.expression.indexOf("."))), e.textFormat = r.textFormat.clone(), this.setupTitle(e, g), u.add(r, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), d.set(e, e), m.add(e), e.total);
                     null == t && (t = this.createColTotal(i, e, s, l, g), B.isNullOrWhiteSpace(r.totalLabel) || (t.text = r.totalLabel), e.totalGuid = t.guid, c.components.add(t)), d.set(t, t), l.add(t), f++
                 }
                 let y = 1;
                 for (let t of w) {
-                    let e = new Uh;
-                    e.alias = t.expression, this.setSummaryType(e, t.expression), e.page = null, e.name = c.name + "_Sum" + y.toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), e.textFormat = t.textFormat.clone(), e.guid = em.newGuidString(), await this.getCondition(i, t, e), e.font = U.Table.Font.getCachedGdiFont(), e.border = new ie(G.All, g.lineColor, 1, Ri.Solid), e.height = U.Table.getHeight(e.font), e.hideZeros = t.hideZeros, 0 < t.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(t.size.minWidth), 0)), 0 < t.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.maxWidth), 0)), 0 < t.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(t.size.width), 0)), d.set(e, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), y++
+                    let e = new Zh;
+                    e.alias = t.expression, this.setSummaryType(e, t.expression), e.page = null, e.name = c.name + "_Sum" + y.toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), e.textFormat = t.textFormat.clone(), e.guid = tm.newGuidString(), await this.getCondition(i, t, e), e.font = U.Table.Font.getCachedGdiFont(), e.border = new ie(G.All, g.lineColor, 1, Ri.Solid), e.height = U.Table.getHeight(e.font), e.hideZeros = t.hideZeros, 0 < t.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(t.size.minWidth), 0)), 0 < t.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.maxWidth), 0)), 0 < t.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(t.size.width), 0)), d.set(e, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), y++
                 }
                 if (w.length < 2) {
                     for (let e of r) c.components.contains(e) && c.components.remove(e);
                     r.clear()
                 } else if (r.length > w.length)
                     while (r.length > w.length) {
                         let e = r[r.length - 1];
                         c.components.contains(e) && c.components.remove(e), r.removeAt(r.length - 1)
                     } else if (r.length < w.length)
                         while (r.length < w.length) {
-                            let e = new $h;
+                            let e = new em;
                             e.text = B.isNullOrEmpty(w.getByIndex(r.length).label) ? (r.length + 1).toString() : w.getByIndex(r.length).label, e.page = null, e.name = c.name + "_SumHeader" + (r.length + 1).toString(), e.page = c.page, c.applyFieldStyle(e), c.components.add(e), r.add(e)
                         }
                 for (let e of r) d.set(e, e);
                 let C = 1;
                 for (let e of n) e.page = null, e.name = c.name + "_RowTotal" + (C++).toString(), e.page = c.page;
                 let x = 1;
                 for (let e of l) e.page = null, e.name = c.name + "_ColTotal" + (x++).toString(), e.page = c.page;
                 let M = 0 < p.length && 0 < S.length,
                     T = [],
                     F = [],
                     v = null,
                     A = null,
                     I = null;
                 for (let t of c.components.list)
-                    if (t.is(Xh)) {
+                    if (t.is(Wh)) {
                         let e = t;
                         e.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Col:") && T.push(e), e.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Row:") && F.push(e), e.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("LeftTitle") && (v = e), e.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("RightTitle") && (A = e), e.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("SummaryTitle") && (I = e)
                     } if (0 == S.length)
                     for (let i of m) {
                         let t = "Col:" + i.name,
                             r = !1;
                         for (let e of T)
                             if (e.typeOfComponent == t) {
                                 T[L.System.StiObject.stimulsoft]().remove(e), r = !0, d.set(e, e);
                                 break
                             } if (!r) {
                             let t = "",
-                                r = new Xh;
+                                r = new Wh;
                             r.name = i.name + "_Title", r.typeOfComponent = "Col:" + i.name;
                             for (let e of p) u.get(e) == i && (t = this.getLabel(e), r.horAlignment = X.Center, r.textFormat = e.textFormat.clone());
                             r.text = t, this.setupField(r), this.setupTitle(r, g), c.components.add(r), d.set(r, r)
                         }
                     }
                 for (let i of h) {
                     let t = "Row:" + i.name,
@@ -11867,174 +11865,174 @@
                     for (let e of F) {
                         if (e.typeOfComponent != t) continue;
                         F[L.System.StiObject.stimulsoft]().remove(e), r = !0, d.set(e, e);
                         break
                     }
                     if (!r) {
                         let t = "",
-                            r = new Xh;
+                            r = new Wh;
                         for (let e of S) o.get(e) == i && (t = this.getLabel(e), r.horAlignment = X.Center, r.textFormat = e.textFormat.clone());
                         this.setupField(r), r.name = i.name + "_Title", r.text = t, r.typeOfComponent = "Row:" + i.name, this.setupTitle(r, g), c.components.add(r), d.set(r, r)
                     }
                 }
-                if (null == v ? M && ((v = new Xh).name = c.name + "_LeftTitle", this.setupField(v), null != i.title && (v.text = i.title.text), v.typeOfComponent = "LeftTitle", this.setupTitle(v, g), c.components.add(v), d.set(v, v)) : M && d.set(v, v), null == A) {
+                if (null == v ? M && ((v = new Wh).name = c.name + "_LeftTitle", this.setupField(v), null != i.title && (v.text = i.title.text), v.typeOfComponent = "LeftTitle", this.setupTitle(v, g), c.components.add(v), d.set(v, v)) : M && d.set(v, v), null == A) {
                     if (M) {
                         let t = "",
                             r = !0;
                         for (let e of p) r || (t += ", "), t += this.getLabel(e), r = !1;
-                        (A = new Xh).name = c.name + "_RightTitle", A.text = t, A.typeOfComponent = "RightTitle", this.setupField(A), this.setupTitle(A, g), c.components.add(A), d.set(A, A)
+                        (A = new Wh).name = c.name + "_RightTitle", A.text = t, A.typeOfComponent = "RightTitle", this.setupField(A), this.setupTitle(A, g), c.components.add(A), d.set(A, A)
                     }
                 } else M && d.set(A, A);
                 let D = (0 == p.length || 0 == S.length) && 0 < w.length,
                     R = B.join(", ", w.select(e => e.label)[L.System.StiObject.stimulsoft]().toArray()),
-                    E = (null == I ? D && ((I = new Xh).name = c.name + "_SummaryTitle", I.text = R, I.typeOfComponent = "SummaryTitle", this.setupField(I), this.setupTitle(I, g), c.components.add(I), d.set(I, I)) : D && ((B.isNullOrEmpty(I.text) || I.text[L.System.StiObject.stimulsoft]().startsWith(R) || R[L.System.StiObject.stimulsoft]().startsWith(I.text)) && (I.text = R), d.set(I, I)), 0);
+                    E = (null == I ? D && ((I = new Wh).name = c.name + "_SummaryTitle", I.text = R, I.typeOfComponent = "SummaryTitle", this.setupField(I), this.setupTitle(I, g), c.components.add(I), d.set(I, I)) : D && ((B.isNullOrEmpty(I.text) || I.text[L.System.StiObject.stimulsoft]().startsWith(R) || R[L.System.StiObject.stimulsoft]().startsWith(I.text)) && (I.text = R), d.set(I, I)), 0);
                 while (E < c.components.count) {
                     let e = c.components.getByIndex(E);
                     null == d.get(e) ? c.components.removeAt(E) : E++
                 }
                 let O = Ve.empty;
                 if (c.dataSourceName = a, !t) return;
                 this.buildCross(c, e, i);
                 for (let t of c.components.toCast())
                     if (c.crossTabInfo.cross.fields.contains(t)) {
                         let e = c.crossTabInfo.cross.fields.get(t);
                         c.crossTabInfo.cross.setTextOfCell(e.x, e.y, t.cellText)
                     } c.crossTabInfo.cross.maxWidth = c.page.width, c.crossTabInfo.cross.maxHeight = c.page.height, c.crossTabInfo.cross.doAutoSize();
-                let V = new Co;
+                let V = new xo;
                 for (let t of c.components.toCast()) {
-                    let e = t.as(tm);
+                    let e = t.as(rm);
                     null == e || e.isTotalVisible || V.set(e.total, e.total)
                 }
                 let k = c.report.unit.convertFromHInches(2),
                     N = c.report.unit.convertFromHInches(2);
                 for (let m of c.components.toCast())
                     if (c.crossTabInfo.cross.fields.contains(m)) {
                         let e = c.crossTabInfo.cross.fields.get(m),
                             t = c.report.unit.convertRectangleToHInches(L.Report.CrossTab.StiCrossTabHelper.getCellRect(c, e.x, e.y)),
                             r = (O.width = Math.max(O.width, t.right), O.height = Math.max(O.height, t.bottom), t = c.report.unit.convertRectangleFromHInches(t), null != V.get(m) && (t.width = 0, t.height = 0), 0),
                             i = 0,
-                            s = m.as(Xh),
-                            n = (null != s && (s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("LeftTitle") && (r = 0, i = 0), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("RightTitle") && (r = k, i = 0), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("SummaryTitle") && (0 == S.length && (r = 0, i = 2 * N), 0 == p.length) && (r = k, i = N), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Row:") && (r = 0, i = N), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Col:")) && (r = 0, i = N), m.as(_h)),
-                            l = (null != n && (r = 0, i = 2 * N), m.as(zh)),
-                            a = (null != l && (r = 0, i = 2 * N), m.as(Kh)),
-                            o = (null != a && (r = k, i = N), m.as(Jh)),
-                            u = (null != o && (r = k, i = N), m.as(Uh)),
-                            h = (null != u && (r = k, i = 2 * N), m.as($h));
-                        null != h && (i = c.summaryDirection == xo.LeftToRight ? (r = k, N) : (r = 0, 2 * N)), t.x += r, t.y += i, m.clientRectangle = t.clone()
+                            s = m.as(Wh),
+                            n = (null != s && (s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("LeftTitle") && (r = 0, i = 0), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("RightTitle") && (r = k, i = 0), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("SummaryTitle") && (0 == S.length && (r = 0, i = 2 * N), 0 == p.length) && (r = k, i = N), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Row:") && (r = 0, i = N), s.typeOfComponent[L.System.StiObject.stimulsoft]().startsWith("Col:")) && (r = 0, i = N), m.as($h)),
+                            l = (null != n && (r = 0, i = 2 * N), m.as(Gh)),
+                            a = (null != l && (r = 0, i = 2 * N), m.as(Qh)),
+                            o = (null != a && (r = k, i = N), m.as(Uh)),
+                            u = (null != o && (r = k, i = N), m.as(Zh)),
+                            h = (null != u && (r = k, i = 2 * N), m.as(em));
+                        null != h && (i = c.summaryDirection == Mo.LeftToRight ? (r = k, N) : (r = 0, 2 * N)), t.x += r, t.y += i, m.clientRectangle = t.clone()
                     }
             }
             static async getCondition(a, o, u) {
                 let t = new P;
-                for (let e of a.pivotTableConditions) e.destinationValueMeter != kh.getLabel(o) && e.destinationValueMeter != o.key || t.add(e);
+                for (let e of a.pivotTableConditions) e.destinationValueMeter != Nh.getLabel(o) && e.destinationValueMeter != o.key || t.add(e);
                 if (null != t && 0 < t.length)
                     for (let l of t) {
-                        let e = new Vh,
-                            t = new Oh,
-                            r = (t.condition = l.condition, t.dataType = l.dataType, t.value1 = l.value, a.getAllMeters().find(e => l.keyValueMeter == e.key || l.keyValueMeter == kh.getLabel(e))),
+                        let e = new kh,
+                            t = new Vh,
+                            r = (t.condition = l.condition, t.dataType = l.dataType, t.value1 = l.value, a.getAllMeters().find(e => l.keyValueMeter == e.key || l.keyValueMeter == Nh.getLabel(e))),
                             i = null == r || r == o ? "value2" : r.expression,
-                            s = Eh.getFilterExpression(t, i, u.report),
-                            n = (l.dataType != L.Report.Components.StiFilterDataType.String && (s = `value2 == null ? False : (value2.ToString().Length > 0 ? ${s} : False)`), e.expression = s, e.permissions = l.permissions, e.permissions &= ~Ao.Borders, e.backColor = l.backColor, e.font = l.font, e.textColor = l.textColor, l.iconAlignment != Ht.None && (e.icon = await l.getIcon(), e.iconSize = l.iconSize, e.iconAlignment = l.iconAlignment == Ht.Right ? Lh.MiddleRight : Lh.MiddleLeft), {
+                            s = Oh.getFilterExpression(t, i, u.report),
+                            n = (l.dataType != L.Report.Components.StiFilterDataType.String && (s = `value2 == null ? False : (value2.ToString().Length > 0 ? ${s} : False)`), e.expression = s, e.permissions = l.permissions, e.permissions &= ~Io.Borders, e.backColor = l.backColor, e.font = l.font, e.textColor = l.textColor, l.iconAlignment != Ht.None && (e.icon = await l.getIcon(), e.iconSize = l.iconSize, e.iconAlignment = l.iconAlignment == Ht.Right ? Bh.MiddleRight : Bh.MiddleLeft), {
                                 key: e,
                                 value: `{${s}}`
                             });
                         if (null == u.report.engine.parserConversionStore.get("*StiConditionExpression*" + u.name)) {
                             let e = [];
                             u.report.engine.parserConversionStore.set("*StiConditionExpression*" + u.name, e)
                         }
                         u.report.engine.parserConversionStore.get("*StiConditionExpression*" + u.name).push(n), u.conditions.add(e)
                     }
             }
             static setupTitle(e, t) {
                 e.border = new ie(G.All, t.lineColor, 1, Ri.Solid), e.font = U.Table.Font.getCachedGdiFont(), e.height = U.Table.getHeight(e.font)
             }
             static setupField(e) {
-                e.margins.left = 0, e.margins.right = 0, e.guid = em.newGuidString()
+                e.margins.left = 0, e.margins.right = 0, e.guid = tm.newGuidString()
             }
             static createRowTotal(e, t, r, i) {
                 let s = t.guid,
                     n = r.get(s);
-                return null == n && ((n = new zh).text = B.isNullOrEmpty(e.totalLabel) ? b.get("PropertyMain", "Total") : e.totalLabel, n.wordWrap = t.wordWrap, n.minSize = t.minSize, n.maxSize = t.maxSize, this.setupField(n), this.setupTitle(n, i)), r.set(s, n), n
+                return null == n && ((n = new Gh).text = B.isNullOrEmpty(e.totalLabel) ? b.get("PropertyMain", "Total") : e.totalLabel, n.wordWrap = t.wordWrap, n.minSize = t.minSize, n.maxSize = t.maxSize, this.setupField(n), this.setupTitle(n, i)), r.set(s, n), n
             }
             static createColTotal(e, t, r, i, s) {
                 let n = t.guid,
                     l = r.get(n);
-                return null == l && ((l = new Jh).text = B.isNullOrEmpty(e.totalLabel) ? b.get("PropertyMain", "Total") : e.totalLabel, l.wordWrap = t.wordWrap, l.minSize = t.minSize, l.maxSize = t.maxSize, this.setupField(l), this.setupTitle(l, s)), r.set(n, l), i.add(l), l
+                return null == l && ((l = new Uh).text = B.isNullOrEmpty(e.totalLabel) ? b.get("PropertyMain", "Total") : e.totalLabel, l.wordWrap = t.wordWrap, l.minSize = t.minSize, l.maxSize = t.maxSize, this.setupField(l), this.setupTitle(l, s)), r.set(n, l), i.add(l), l
             }
             static getLabel(e) {
                 return B.isNullOrEmpty(e.label) ? e.expression.substr(e.expression.lastIndexOf(".") + 1)[L.System.StiObject.stimulsoft]().replaceAll("]", "")[L.System.StiObject.stimulsoft]().replaceAll(")", "") : e.label
             }
             static getSummaryTypes() {
                 return 0 == this.summaryTypes.count && (this.summaryTypes.add("None", "None"), this.summaryTypes.add("Sum", "Sum"), this.summaryTypes.add("Avg", "Average"), this.summaryTypes.add("Min", "Min"), this.summaryTypes.add("Max", "Max"), this.summaryTypes.add("DistinctCount", "CountDistinct"), this.summaryTypes.add("Count", "Count"), this.summaryTypes.add("Median", "Median"), this.summaryTypes.add("First", ""), this.summaryTypes.add("Last", "")), this.summaryTypes
             }
             static async setTopN(t, e, r) {
-                let i = r.summaries.where(e => Dh.getVisible(e, r.report)).toList();
-                if (t.topN = e.clone(), t.topN.mode != ch.None) {
+                let i = r.summaries.where(e => Rh.getVisible(e, r.report)).toList();
+                if (t.topN = e.clone(), t.topN.mode != dh.None) {
                     t.topN.showOthers && (t.topN.othersText = B.isNullOrEmpty(t.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(t.topN.othersText, r));
                     for (let e of i) {
-                        if (!B.isNullOrEmpty(e.label) && e.label != t.topN.measureField || kh.getLabel(e) != t.topN.measureField) continue;
+                        if (!B.isNullOrEmpty(e.label) && e.label != t.topN.measureField || Nh.getLabel(e) != t.topN.measureField) continue;
                         e.label != t.topN.measureField || B.isNullOrEmpty(e.expression) || -1 == e.expression.indexOf("(") || -1 == e.expression.indexOf(")") || (t.topN.measureField = e.expression.substr(e.expression.indexOf("(") + 1)[L.System.StiObject.stimulsoft]().replaceAll(")", ""))
                     }
                 }
             }
             static setSummaryType(t, s) {
                 if (B.isNullOrEmpty(s)) return;
                 let n = this.getSummaryTypes();
                 for (let e of n.keys) {
                     let i = e + `(`;
                     if (0 <= s.indexOf(i)) {
-                        "First" == e || "Last" == e ? t.summary = rm.None : t.summary = "Count" != e && "DistinctCount" != e ? rm[n.get(e)] : rm.Sum;
+                        "First" == e || "Last" == e ? t.summary = im.None : t.summary = "Count" != e && "DistinctCount" != e ? im[n.get(e)] : im.Sum;
                         let r = s.indexOf(i);
                         while (0 <= r) {
                             let e = r + i.length,
                                 t = 1;
                             while (e < s.length && 0 != t) t += "(" == s[e] ? 1 : ")" == s[e] ? -1 : 0, e++;
                             s = s.substr(0, r) + s.substr(r + i.length, e - r - i.length - 1) + s.substr(e, s.length - e), r = s.indexOf(i)
                         }
                     }
                 }
                 t.value = `{${s}}`
             }
         }
-        Ud.summaryTypes = new Co, Ud.FieldMargin = 1.5, F.h.StiPivotTableHelper = Ud
+        Zd.summaryTypes = new xo, Zd.FieldMargin = 1.5, F.h.StiPivotTableHelper = Zd
     }
     F.v.StiProgressIteration = class {
         constructor(e = "", t, r) {
             this.series = e, this.value = t, this.target = r
         }
     };
-    let lm = F.v.StiProgressIteration;
+    let am = F.v.StiProgressIteration;
     {
-        class am extends F.i.StiElementBuilder {
+        class om extends F.i.StiElementBuilder {
             async render(l, a) {
                 this.storedCulture = ai.set(l.report);
                 try {
                     let t = this.getValueMeterIndex(a),
                         r = this.getTargetMeterIndex(a),
                         i = this.getSeriesMeterIndex(a),
                         e = this.getSeriesKeys(a, i),
                         s = e.count2(),
-                        n = e.select(e => new lm(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
-                    return n = am.processVariationSort(l, n), await am.processTopNElements(l, n)
+                        n = e.select(e => new am(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
+                    return n = om.processVariationSort(l, n), await om.processTopNElements(l, n)
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static processVariationSort(e, t) {
                 let r = e.userSorts;
-                return t = null != r && r.any(e => e.key == mh.ident) ? r.firstOrDefault().direction == hh.Ascending ? t.orderBy(e => 0 != e.target ? e.value / e.target : 0) : t.orderByDescending(e => 0 != e.target ? e.value / e.target : 0) : t
+                return t = null != r && r.any(e => e.key == ch.ident) ? r.firstOrDefault().direction == mh.Ascending ? t.orderBy(e => 0 != e.target ? e.value / e.target : 0) : t.orderByDescending(e => 0 != e.target ? e.value / e.target : 0) : t
             }
             static async processTopNElements(s, n) {
-                if (s.topN.mode == ch.None) return n;
-                let l = (n = (s.topN.mode == ch.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).toList()).take(s.topN.count).toList();
+                if (s.topN.mode == dh.None) return n;
+                let l = (n = (s.topN.mode == dh.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).toList()).take(s.topN.count).toList();
                 if (n.count2() > s.topN.count && s.topN.showOthers) {
                     let e = n.skip(s.topN.count).sum(e => V.tryToNumber(e.value)),
                         t = n.skip(s.topN.count),
                         r = t.all(e => null == e.target) ? null : t.sum(e => V.tryToNullableNumber(e.target)),
                         i = B.isNullOrEmpty(s.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(s.topN.othersText, s);
-                    l.add(new lm(i, e, r))
+                    l.add(new am(i, e, r))
                 }
                 return l
             }
             getValueMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(us));
                 return null != t ? e.meters.indexOf(t) : -1
@@ -12046,81 +12044,81 @@
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(ms));
                 return null != t ? e.meters.indexOf(t) : -1
             }
         }
-        F.i.StiProgressElementBuilder = am
+        F.i.StiProgressElementBuilder = om
     }
     F.w.StiProgressVisualCreator = class {
         static createProgressVisual(e, t) {
             switch (e.mode) {
-                case Oo.DataBars:
+                case Vo.DataBars:
                     return new F.v.StiDataBarsProgressVisual(e, t);
-                case Oo.Circle:
+                case Vo.Circle:
                     return new F.v.StiCircleProgressVisual(e, t);
-                case Oo.Pie:
+                case Vo.Pie:
                     return new F.v.StiPieProgressVisual(e, t);
                 default:
                     throw new ca(e.mode)
             }
         }
     };
-    let am = F.i.StiProgressElementBuilder,
-        om = L.Report.Dashboard.Visuals.IStiProgressVisualSvgHelper,
-        um = F.w.StiProgressVisualCreator;
+    let om = F.i.StiProgressElementBuilder,
+        um = L.Report.Dashboard.Visuals.IStiProgressVisualSvgHelper,
+        hm = F.w.StiProgressVisualCreator;
     {
-        class _g {
+        class $g {
             implements() {
-                return _g.ImplementsStiProgressVisualSvgHelper || (_g.ImplementsStiProgressVisualSvgHelper = [om]), _g.ImplementsStiProgressVisualSvgHelper
+                return $g.ImplementsStiProgressVisualSvgHelper || ($g.ImplementsStiProgressVisualSvgHelper = [um]), $g.ImplementsStiProgressVisualSvgHelper
             }
             async writeProgress(e, t, r, i) {
                 let s = new j(0, 0, t.width, t.height),
                     n = t.component,
-                    l = await _g.getDataTable(n);
+                    l = await $g.getDataTable(n);
                 if (null == l) return;
-                let a = await (new am).render(n, l);
+                let a = await (new om).render(n, l);
                 if (n["isSampleForStyles"] ? a = this.getStyleSampleIterations() : this.isEmptyData(n, l) && (a = this.getEmptyDataIterations(n)), null == a || !a.any()) return;
-                let o = new Uu,
-                    u = new _u(o, !0, !1, !1, 1),
-                    h = um.createProgressVisual(n, a.toList());
+                let o = new Zu,
+                    u = new $u(o, !0, !1, !1, 1),
+                    h = hm.createProgressVisual(n, a.toList());
                 if (r && r.needToVertScroll) {
                     let e = h.getContentRectangle(s.clone());
                     r.needToVertScroll = e.height > s.height + 5, r.needToVertScroll && (s.width -= 15, e = h.getContentRectangle(s.clone()), s = e, i.ref = L.System.Convert.toInt32(s.height))
                 }
                 await h.draw(u, s.clone()), e.writeStartElement("g");
                 let m = r && r.needToVertScroll ? 0 : t.x,
                     c = r && r.needToVertScroll ? 0 : t.y;
-                e.writeAttributeString("transform", B.format("translate({0},{1})", this.p(m), this.p(c))), rh.writeGeoms(e, u, !1), e.writeEndElement()
+                e.writeAttributeString("transform", B.format("translate({0},{1})", this.p(m), this.p(c))), ih.writeGeoms(e, u, !1), e.writeEndElement()
             }
             p(e) {
                 return e.toString().split(",").join(".")
             }
             isEmptyData(e, t) {
                 return null != t && t.isEmpty && e.isQuerable
             }
             getStyleSampleIterations() {
                 let e = new P,
-                    t = new lm;
+                    t = new am;
                 return t.value = 75, t.target = 100, e.add(t), e
             }
             getEmptyDataIterations(e) {
                 let t = new P,
-                    r = new lm;
+                    r = new am;
                 return r.value = 0, e.showBlanks && (r.series = A.get("Dashboard", "Blank")), t.add(r), t
             }
             static async getDataTable(e) {
                 var t;
-                let r = null == (t = e.as(th)) ? void 0 : t.getManuallyEnteredDataTable();
+                let r = null == (t = e.as(rh)) ? void 0 : t.getManuallyEnteredDataTable();
                 if (null != r) return r;
                 return bl.tryToGetOrCreate(e)
             }
         }
-        F.h.StiProgressVisualSvgHelper = _g
+        F.h.StiProgressVisualSvgHelper = $g
     }
     F.h.StiTableAlignmentHelper = class {
         static getHorAlign(e) {
             let t = F.h.StiMeterHelper.toDataType(e);
             if (Le.isNumericType(t)) return z.Right;
             if (Le.isDateType(t)) return z.Center;
             return z.Left
@@ -12159,29 +12157,29 @@
         }
         static measureTitle2(e, t) {
             return this.measureTitle3(null, null, e, t)
         }
         static measureTitle3(e, t, r, i) {
             var s;
             if (null == r || !r.visible) return W.empty;
-            let n = Io.yy(30),
+            let n = Do.yy(30),
                 l = null != (s = null == t ? void 0 : t.width) ? s : j.empty.width;
             if (B.isNullOrWhiteSpace(i)) return new W(l, n);
             let a = r.sizeMode == Dt.WordWrap ? F.h.StiAutoSizeTextHelper.measure2(e, i, r.font, l) : F.h.StiAutoSizeTextHelper.measure(e, i, r.font);
             return n = Math.max(n, a.height), null != t && (n = Math.min(n, t.height)), new W(a.width, n)
         }
         static measureTitle4(e, t, r, i) {
-            let s = Io.yy(30);
+            let s = Do.yy(30);
             if (B.isNullOrWhiteSpace(i)) return new W(t.width, s);
             let n = F.h.StiAutoSizeTextHelper.measure(e, i, r);
             return s = Math.max(s, n.height), null != t && (s = Math.min(s, t.height)), new W(n.width, s)
         }
     };
     {
-        class $g {
+        class ep {
             static loadReport(e, t) {
                 switch (t) {
                     case "Financial":
                         e.loadPacked(this.financial);
                         break;
                     case "Orders":
                         e.loadPacked(this.orders);
@@ -12200,19 +12198,19 @@
                         break;
                     case "WebsiteAnalytics":
                         e.loadPacked(this.websiteAnalytics);
                         break
                 }
             }
         }
-        $g.financial = "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", $g.orders = "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", $g.salesOverview = "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", $g.ticketsStatistics = "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", $g.trafficAnalytics = "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", $g.vehicleProduction = "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", $g.websiteAnalytics = "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", F.d.StiWizardDashboardsHelper = $g
+        ep.financial = "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", ep.orders = "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", ep.salesOverview = "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", ep.ticketsStatistics = "H4sIAAAAAAAEAO1b628iObb/vtL+Dyj7ZUbpaWyXy2VPz12JQCAkISRAnmrpyk+oUA+6qghJRv2/rwsC4R3S3Xd2Z+8QJYHysX3O8c/nZfP73/9WKOy19CBOsiudpH4c7f1a2EMAwY/4o/MR7H2Yo6gNfZU3a/uikGJXc4ghVwy7mEspuIJcImoWOp3xUOedOr7s6yxtZzzz08yX6QJVKfB5OkdW2EQ3zHpxkhO2Mz8cBmlssgWCcqJ5psdsFiv23U9gHzgA/FxcpOrxqDtPBYlDsMtcCAj0FnscRl0/0nPaeXmAXtrLPJDDwHIbR41YjWWtR5lOBonOxk8XZr6M/GxCInt6Ktt5oh98PWrrLPOjbq4HZDmhjMFJe4WnPRHzRF1ZKp0s0OEJSVsm/mA88jC1bYX2U5rp8NPn5HM0/+BjJeEj+3G14dqPVDxKP1bjJEzX9OMZn3860/7HchxlSRyk61sPeKrXTfpKMdHLtraPFZ8HcXfDDC805TgcxJGOsglZ/htZ6KUDLnVhQpPmD3/P/xTsazAUgS8LMuBpWlhBZ+HXNXPYJ5N30zFmg80NuDLUTz9PKRbI81fW89OPdQsJK6D/rGcy/PTzp3nSr1OJpg/+keiuRVZhxlCholO/G+mk0NX2b74FCtKisfBLQcWFKM4KYax88zQeKPuc/UNH6nvGmHE1/jNDuNGJjqRWpTTVodWGzjH6e95om8F4277AKQgmnexzOP98gpSFdjTXvoDSBSpnfhQL1oVGPNd4EwYLbe6iNZnheYGILBFNYD1H4C0RTJFrSXKKry8b2Ze5ReDJ05xeWjqNh4mc19WLtmaf7OclOzqdeNy2bD0XGjtPg3HHcvqw8Lwe8u64oRnCLuwNmle9bnxSfBjeu83hCb8/ury6aD525VWvFrpCFn11Hlye3HcxPD3rV27dk/Se88OnULAiqezXfXT44ApcrQ66uHs3UKiq7zzWRMb30kd+BoemcV72GuC2TJLH48ssRUc3ncsmvynSUemu/nhUDE3J51759uq+1KuNwGnmH3X2/U5ThajdLO7v0+OkenPoZKxZcjUonz53ApPio+uufwiLTjBMTs8fdXpzg+Jy7/T5vkef9q+O+WlZlPpNcwG7cnhyaRxBq/VB/YqSR3Sf3g1rh8HoIb6h10VJvVpfPiSRaF4NHrPo/LkSjPDgmbThl+MrWa7FVdlPjiuVYqV0deHSknsvS0cVxNp+v13utEbPxVaplUok2k0UDfm9igDoghg/xOenbFQ9hpVHR2LuPh47w7BlwpPHc3kzuLsVI++xdtrM5OjYnJij22jYAPX2AwrdW9ZjX27btZPMfegH6KxyGWadkyG7cM7P+5eNgHQbSXXQV73SXWUUd2pVcXRdcUivyS6GF4f+TeC3kjS8CwaDLIv9/VOumtcgBgl6ejRB9tTRAeJDYLIq7p0els9BtWTKMJZP5asHYlpaw4p6fr4/CHqt/mgo8OikBentQS00tZrnHD1EDLndsgm+jDrDyzP3rt7dN0yexqZW7ap61Rm2Gk8XvW6/37l/UPLu7A4lQVJ0q0T7jU7j6LlaAcnj4FpkzeFddLZf7Tai+kUYPfn7zeNRsV8ZDpqqislAiWr/eFTx8X75uuapy/7FTa+tjm/k8/FtGB4wOPpyHJ6ehrR8/djJDiMAi0MYZI6oOWbE62Fw1X5+9mHxsdZ/9kKPFWFrdPhw3r0GLYjZXR8kznUDHiuKbx/NAUuv7tLro3C/0zJfLm/PG4cP/auzpxY+OYVJA94/meSgs9/octiNnH5oTs6e1Qk4bVhvX24FZ97l+WG52z9IcMgaYdNisUPKPcDJARzQy4pblcGRf94Y2Z9aNTwp0qdS47B+O+iXGA17D0eOXwfHiJ0QcnJYue3ibNSq8bSelEJx4jpSsVFml9Mp9g1rVYonKumB+6daJEgZj/ggOnKSFMnr04eDQem6PvpSjG46/Zszlg27g/6X50qEZAJavIJTTW6DGjDnD/X7gwbPOg+XHvMGHScN+xLHo1O/TVSjy4rNEQpr144T3FSv7irwmHVGGbghV7KvYvFF1XitgX1yU/5yf3581SPP6rneVr0KeaqZm+x5pIvDqEoeO152dBQc6Pv4plcOnQgMT6KT0egUk+D29pofH9fBVSDvKtcXzu0zv2Lyzt+/Ywejc7ttO7hf7l6Kx0PcLB6WOp2b68dj2IbJ6dFT9eyAfWHyuHV+cNFKnbQZtg6P7qU8vQ/rI3Rw4UYI7wtwcX3RcyveILt5viv2PFjbmxrCr5M3X6d2PHcd7R3McV1ZN/1i8/M+HS4CPem4YGW/2Wyf6NxH7FHkOq7ENjr1CNZE5yEqx9zGhgZBAtyFPuU4GIZRusjqKvMLjOVxygLLE/EipR9t8y9wuSXvV49eJN3Yfyba+uapT3pxye0ssU5/hepFBYRD7RgBpQOxzTkIpRoR6ipGOYLayL35bl8XBhnHFpskH///dsHXdp/Jvbb1XWILjwjmCUcbhTGggkPEsZICIaYFFGyb2GiL2LUkHg7qle+QfNMIM+E3EbxLfqA4toIagQ3GXAhBHSMdRajmWDoe3Ca/s0V+6/X0oGfD7O/QwOYxXvf0RpJ3aUEpDxJuMYCM3fbGFYQZ5TpKSSYcSMg2LeAtWsiDzuDBpsDfroSNQ8x0sJHifftfCaQ0I4B6DhaMUOYKI7hyASIIs637390GhIRHNmFJvksJWwZ5hcJmmncpgkNr9SAw3GCBqWcYU1QooJB2qafQ1h1BtmIhGybRd2JhwxBzWNhA8S4VGEaZIB6TAiCMmNWDka7nuA4BUgNltqnA26KCevS/50lsnX66bvLd9bB9nJkytpO9SyOOo7GHOAOMCsyAQ6liDHFptONYxWzdHXTb7ogzHnzPxljb/3VPrG1+l+SeotYqeB7QHsIEGeF4NrviwNOSU+spFyV//TCvhFW2J6HYx2lIti1OFDx9R5Ro8+9ppx8aIVpfSDWxdkAQaR2jI7R1mNpqwroMarRc6HPOs17ORd4xeak7/FosbpJ2rnRxzrsr1ZxXwRfD4Zdq5evMMyFnbRvKwWPiaZ2ZOdhafY4xxS4mhjAbAEhhKONSCdfguS5v1o/HVAfJMO3lVNYt+erXuZbX6uHSCq6Ezgui2k3ctWpMDwMd5k8Xt9dU6CkVWmqf1dMdoQwTyCWMYukh4RltAz9pbJRjt7ZZ6lYOfDtXS8uMR91gPAP44CDwAVPwAWKwRH4QJ0qPS+af7GupsRRka4cb/yzRztZuXN7m40rWGgMy089U7JX924yO4ocJS+1ePOrEcdDxB2vILGuyn5OVBoPgqeoHdt4VsiNrM5LAj/oVbdc74i9s7Z3pkU3Ktpm/Kx4M9TYJxgRTMWyCv2b2qWvWgEPpGaMNxHblGJFKA2MIEDZ49VaDwMPHQT7oC6/tYfjT1PJMHeXP21jv8KSrs228Tyh2Yh5zgKHnSaRtpqGEYNQoIyl3qVJQeasuezPzY7O+lfO2Tny9kqIu7KsxxU6cQwOE4g6iUjLMhMepa7WvrBcE0LgKvMH5lOvxRt2mbT8L1gGlox+zrbFNNZ6K1I114bL+CbofPXd5F+YgjhNrwrpR+KKDss732DaepkN/gs6ngzhQyzt7ehaVW/sDnqTLRiQO4uSQy9wcZslQb3CPK/nzgvnL5d9u+nIKuMHsSYfZRRJCGgCwI4CwmZ1hOfSgcBxFdzF71uAhYC3fDzJ6uQVdGcuSjwFw5ae+GNMaHqR6CSIvUPjN2HWxBFL/z+fZsn/eK6T+c/7EIZ/3/vlbZol/4fl620eTpbaPJ2gce670t+IrzT9/K+aD/nPvfaAc/1/G2ZIMW/D1Xmu/drr3W/rmQEczi/5dtn4DoldKI4uIzst4b0A6J9mEaQ85RFv8SqMEBtLaIRcQh2MEsHXrDtsF0/iHevLpaOibYL2horguMFrUZcW3Kszt7GSE5ZV8NeEUQ+za5E262sOQcy6h0vat9UFUSbbiObcb8VXi3XC8yPx4iTcxvgjrszUVnheaGaY30rwDzvnr6+KDr8u7Y02xc2FJXjzBWyviMG7RktcUoMQQSG5DA0AAxogDqjF8c0UWo5lJCejnNb1yk5Ef5PI1gcwi63Znng1DoZMJuY0QHny5Xqdnumv1+KBtpmPXO+dnOVUdk1W09EMeVPyuP475wTqicR2zrQc84dnk1smHtXNOity/Lo+6sn7/3ehclW45qmn53V629waK19Su56VvaJ4Ok43yz4oDCDApiEN4flzCFDdcea6rGWXS4Ry9E8TTkHxXGf8C+3852N8A8ZoDiG8AsYDGoQSDvNhp8xpImUuIgppBj2mg8btAvFBzXIfkUy50MKlOFjZXJ/+C/F+QXyfsutOmb4A8hFq7kFDoUBsDKpdRoaUnuWvze44NfRfkX6oRf04Efx84PxRKQuTXSifL+v8bqlvS3CPNVb5o02IKWEmsqnGcbad4MxN/qUn7UeH3hh2nl6cqP3VixZ9+/loQT4X2wC6dzfXTNxP2P7DA9O4CQI6Ff2+td0U7wyBoxaO2DmxOvFLoWi1N+s96Wjar+vOB6kIFYcW3Lx7z9HjyRlFsTLKpgkCJwR72DFIYYeEgqrXjcgRdhaHmejmLX5Pz5+l+fhxgQ+APiP6QIgIkkyoCWqlJjEvk31AfGPcbK2JtgffVIRhAjYNcLCDTmHmaIxdoCIFRrot+ZDY6KTtPTyAPhiKH8+6GpJR0h+HqAdIuuph23UUdVEmNHEY4Jw42hAuHIQxdj1NglYLJ94SEuwt7rXOH+Q2iTjruIqigVEhNsZXTxYpgJj3IXIow4oQb+r51f72B8R4p32sBx2L9x552veWlSkFQ2Oqp/sjTjQaPhjwIng5zQq3mAPPWcd1mbM1KAwIpql0lBDLKIdRI+wlil2rm2Nxq6x2SXU+v3uaCSY4lkEYyG9cKi2/EsLXxEilr9AHjP+joampbNkWxC76rNv7eR7AYwm4ZfKzwnUbeITbeIS5+M6vbJWjeJZtbkvOm9OivW/QNW2o1bNvd5tz+cVOVEs3XzFRLfHXqRzo9itfstoUJl+Op7fON6wvrZDuPU39mx/IUYGGQDVHYSrq5gLfW+LtNDT7YHonNyDZFYxpSm3Qi7kBDMNWAOciRLvCAowhz3eVuG6Ix/EODMQw2BWM7Hem816vNdPSn9WxTr5ZnWmuvo//7kizrDN50azkNH2x1JhS7QiGIGDEcUwEY1kAQZd2IKwyRzo7OZKKdLezm++ZNfsdEbzAMASSUQG59sMAIeNbnKa4FcV0sHXf11O9bGR57qN0Ch7dYJtDqEmqgPQAwlZy52rpvxgD1oCcJ25HlycXHraHPYMbYZbu0cgkr49UkDvdeDvSmB7QrY0wTmSPNs3B584736+wbIL042Zjsrlyg/o77b3iDkXWRzWqEdHl+4GiEZMrziNWvxbSFsLPcbb1RJD/01JzgsX3NE9+VBfjrFtzGi2R2NxgXEpzfKFPKEZ79wDixQTW1Cfxb17F2TE3/L6/CeUJzmxhAjZSHEYRcEmAc5THkQcOEeYcEf/BVOEQdglTOqrTAhR7XWNu8AjJojCek3NE8fe9VuMnZ0XrE/+lvw618ieI7jOGmiNNl3NNcO1Tml54JoS60vlE5wCApKBS7GENIf6AxzM3gX+bwmy4FC2SQAI4RHsEOdQVVTDtSakq0Qu77LgVPC5d/lCV0IMOCc2jNCcfckxxo40ghXEGIB8jKQdx/jiW02nU9jhyiMLGOiDJXUWMcl7iUCk1+VGXl7UvBG7789qc0g9O3rxNak/cUvHwfVOu5878FI4NyO/Np8n2Lg4DLuTudub3Jj1ymWTIF4EW2yfdO/v63r/8Cg00VQKBIAAA=", ep.trafficAnalytics = "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", ep.vehicleProduction = "H4sIAAAAAAAEAO1caW/bSNL+vsD+B8H7ZQbKWDyabHIy7wI6Ldm6qcM2ArzoixJtHhIPXYP8921Sh3VLdjK7gyAKokjs6mZXdVXX81RT+fOf/0ilbtps5Plhj/mB5bk3v6duJEESb8GtfCvcfNqSuIssGjcLEtAANpGpqgqAqoAkXTSJgCFRATGhuNOpjhwWd+qxoUVslmr6Ho1IGN9pWyxrWyi4Ri4Kh54fCxqh5UR24JnhjkDeZyhkyTwzBf7pFxEomiqLKhQFQUgLsiD8mtntMUTuYKeHKimqquqx7F6PojuwXLZlqtUFadWeRzaJbBRPu+bRRPGKGzJ/5LMQHSjTda0wFilHLvUZDYdBw6y4ZLgSavpsYrGpwcLQcgexdWRZERQJ6sv2AgqG2EM+7XEp5m/JSQpYihjEt0bJPaKAt6WMeRAy5/MX/4u7feG24KMp/3rY0Ldc6k2D25LnO8GRfihE21c3a3Kb99zQ9+zgeGsOBezYTd8klhY613ZbsJDtDU7cYSWT95yR5zI3XIrFf13ukcEIEZZaygTxxT/jtxR/jSJsWyRFbBQEqZUz/v+bM6Z+P3ITfmX5aT3IZrStEQ/H+uXXtciOfPwKh1ZwW+HuwVW0FmyjxS+/ft4W/brWaX3hXz4bxLPczChVYIE1cJmfGjD+HodGinDPTP2Wol7K9cKU41HLnCcDhV/Cf7HYFT8+xmZWydvG203mM5cwmg0C5nBzsNhL/4wbebOQhPPKoWx72YlfF7evL31lp13aat/x0x0peXsU7q47jWCr8dGxd9qU3V1m49E7Quqe0NKxtwTgnsDad7lILPF1FcpW4hHIn2/Zpc0CL/LJtq1W1tp849/XGyzfGb31XZOGzZZ60PLA4tvcEFFTBV2gkoAxgFDABAoMUdGUoEk0Udvp05mPktvkg8nO9YqDBkmDjzKDZsMwnubaCHrjh8yT81SDxXq3pT86w9xcgZlxdT4TFq+hFhnWYz6rLhbdzrxGpKoZosim9rgwZs2e1GtF04I3LdDyqxiJamb6RAoCbMJpzh+UkfrYGL9Y1cewM6j57KVa17pKk7r951dDr8PSgFYz2ftirR846cV9Tjdm2X5LaMxA9JA27zJqPv367DpKM2fKpP+Y7Q6qgjOumS9IKxfuPMme10qOm7Vf6plu7oUZxSIcgyEsuKiUFl4HkjhARv1xvJg1OqV7L/siS20pbA964X1aAPna1GxpuGQ9B+qg4k+LOSNsLBb+SM7X6zOraQGhpS9Ghc7MewKP2sM4nX5pTsxamhjT8v3YGOp6kNPz4wFkA0nqkZri2g5Qg7n40qdW73X03Hg2M5Y3m0Xzx77bvRcZcNxAv291rOpdP7p3ugtS69fT1QkTIuN5WH3s1/Uqrj9W/L4zLei+/Nx4glk+xQej7ZeRQvQBeu2NGq/B5M5TrYxbrEXwQXK6s0pkhaW+31Ky4xq5gwVxdDfIC2mVDl7kYcdoCD3vqdvt1p+rpWZ1pnpeKSuUtdYzWVCxGYY4lDHfNkrTl07bHcvyHXeIgZtptMZ1rZqpN/QCKxZRepEPH0NRfjLrd5O+p+WrL4XWs41nlGbl5lMrmr2UXly5pqCImeqzU9QXxnyRLU9yo0WlFFq6nI+y7F5phCLEUlChbqtVrzwZ5Wfa6jVRux8FxoPh3JWaZVe+b92NWYD6Ob1fazTn7dfWLF26Kxdw87nbFvve2IBA6D3Y47RabTaa2j0cRXblhfjPRlbPpCsBzDSwq9pu2h5Ktl7rdYe518l9BfXMmt3MtNFzu5/uqU9Sg0nVtKJPMHVwtJjg1369rvQyuYEyEbN48tB8Zc2RF2iP8NUeyK9GFObc2tB8zYp+dfxSq2qkk6021NqoWRsVm6MsLmbaUt5rSZOCn6dNQs3pKNs2lUlQE1Cp2KtPhWlrMXXmLCiCGUaPtFFo5gF6njkvehp4Y3z/XIADR3moT0qGKY8HnUfhqVLxXieV2aTfwKMwb1eYZJUeHnvmnZwzjWq6kB++hNy9RqNertemxck9y9y9aqDng4o0VwiLgD/1HxcydMdjEOphVM3P1J7vdZWSc19qcZ/p6qWnXlt1zbL+gKGR44M/g5asY/o0KKtmjVRrtKYUWx1vli0y6UFWC6OaE+bv9WpVbeq0mI38oZ3WKsrrArXVVkFuiw5SnwOjbLC69oobYWUW9TPtLsqPe0LGmOXxQ0FdsF7lfu6LD09Gv1bAqNbhO0Uw6NWL0oNYXEgd137J8/VD7WlzZjqzUj1AzahWri7yubrU7PrBlKgDx5Ms2AEPXdjP94eZ4sBkOXSPK31bRHMg6eYgFLSOg5VpWlHylRYb3lm5YeWxTfDk6QFCWKoOc954lCXucNHtVu2XltcdhxWNNeFcw3eB3+9MBHf23Oo7Iwu11Ey1d9dzhjho9StzsQ0hKI2r0XjUNwwpIhN0P5PcotT1ps2h10DiI2qGwyH1srShWZ5fVMvFtNMs3Q+wrw9sxp5DcWw8Rd2Xxt0Q3Kw37K/LD1/X2SlOiMYVSaZCOfhYZbK4Twdhmy077mSDb0hGRFUkHTNANAWYWNQYYgLVEScYDBOi7/TJe3bEN77dSR5Oe2dKbeS+bg+y1MulbMZbfxP3W+JuFXel4qnuG62Otq5T5gpfGKHPEcyB1Ep/YAoQYKRqUGeAEzBsihIlVBQ4F9EVLN1sd/u6M0gClE6pnfciDlvm36D5qRE2yp8SeJf+xNR0SYSmJjITyCbWIdA0EeuawrVXiXBOf+mM/k8M+ZIg6t9ggJNDbCxwUmLPBAWPcwF2ygSM66/KKuYaS4BqEGtU5m5gMkXUmanr50wgXzaB8u0mOBxi3wSHEu8ygYQ0DHUKEIIMaEDUuBdIOiKiKRCIIThnAnDZBMK3m+BwiH0THEq8zwS6phKZihiaIhAEAauCiRniJmEqgTreNcHbl21rHEw+3nVvk633XCbAnLxcnwc4E1h3+k45QGachQAFCZoJAN8PENaRqCimqlEATQR2+jRROIzvn3CPFVP6PZM5quQW02pyurJPPt/03c1zq/LK2203ur2VXpasfr9alQiv62WiiKgEEDahiAGHP4gyYiIBENPEKqJbIXNzsQyWSOX8KBjGUoFnW/T3rZa3csfewh1kxh1VO2wWFm3mxFd2g2qtcCwh7rVt9NN0AhRZQhjrgFAVAyABbMoipydUNdFetzyn/27YZiRELkcqSUXxk/BJlAThE9gLnpuc51OW1Ps+89deY9YOTwzG/xzKdqzQZj0rsHAiaCI7YLtCsZbxEH+YnOtzAcL+78uNwQYeS3UrX25SgbWIr8jql5t//xFy4d+QbQ1cfinP4jIfv3y4cH9k3iT//UcmHvrfe5NLZnZk+1rPJ/l3f7/Y0+TMzrjx1qQWiZbudHi3jUccvV3DLXuT5VIYQ2/a8Ty7Y42OiPElIa+xWGPE3DLf+nzbOoKONi2cJoaWi1aTuqmzKUeXV+1yB7jnA04NTjg1EQgFHHxyDxYBD16efCAVVYUCBRKNadc4tSxxjwZHvLqG/IF1bAmqzIynL98KBznEGx1vaFuD4Yk+OS8MPYe3CbfCGff4YIwB7Yhm3zPMxHeFWSpOvanf4n/0nyH3V4XcAdTeDbmYFl6IuVhkHwBsxZ2sShjLkqzxjAJExoGgCCUFmUDAgk4UfFXcqcu4k75f4AkfCzz5+wceWEaeJH0o9E4w5+PceXt1CxZf1PjUaznCvm9tgTiKNaYARrBqcvCOdKYrpqxgnTIqQoqO9CzORhzBrY/UEqx6glNeHVm7k0+c7tTEdwOtzuHTCZlNlJ2UeUeAxa+vuxe+7rvREV6/syQc/eaQH1xcEYUzah5WAjAxkBSIABUUIiACTUiZcnlFSpYfhL8k67KmeXyj3f4u/HpkkCrCzL5JjkCJzzhNSFnJLn3AEVfbbnx2g8JLa8m3mXrkYOYvxQ3mTyxyfDnqbMCXYMI4VeCuEquyz/ISsTvfi0YGGyEfhcuz5U9HhzNCFC7RPyOWg+yCNbDC4FMqi3F8Urtc7YM1PtR1uZeHyDYix1ke+YR+xI4ILtvX9DHLXTQ+bPmxY+JQu7LnZ+NM7qxmnuzVF0LnSEnoI6EjcG8loixrmqADRYSckaoIIsZTFGVQxR8IHX0vdJT3hM5Bheln6PwMnTP22g+dJWbZi50zCKXMEI3dZdn7sygcwJSS54XnJS4h7XOljpXoOUiTzGHl3ysK8VlUbqGyP5Ej5ljSiXNFxXfjeHSstPd+IJ8djex5ybLj6b0Txh9YJ7Lttjc1mM2B5CpgzmhscPK1fnapZG07yw4ROCg4f4B77wGBDQdQJQ4VJU0QGaQAMQ0jhSNJU5J1jVEVXMG9Y/Qfs2+o/pjsW1L/fvwbz1Mr1P6Tfv9V9PvgjGO3Ij9E/oWwS0ROFXLNGOcIFKmmwgmcSjQIVUgxxkxQVJPuh+upuFOXcfdDsm9Z+Cb63UN2xD7AvpN+ydrV2JGU8AZYTSypSIMAKoQAHSnY1Cl/UxAlTIMiONJzF7By4PTL9cwuFkodO/OKEwnzLRasEVichTgKJK+MGiMeBCzLce0lFH+BAF9tFQawKAtEU5mpAxGZmiDrjFIdAp5TKJHebZXzoH1tlWNE9ztY5QK3udoqKhGhpIuM6boMTCZjhjnc4x7OJFMggvxuq+hXWeUYh/mAVc5EdtYfRM7hIVjSdiHQ1l2vsR9WZEUHukxECjlMkTSkyDrAqoiIoEkKeV+l63r13pvcEl3+t5j0jDbvpwdbSONvxBRqyI2Qbc+LsSCjWw50ZmkuxOra00Qh/sEFpUylGofBUBRF/k5MyTQlQAR6bl5rjz5VIthBEHfJA972bn3gzODJ/K8a+YrCwxVFh936QYwM9gWuqEicqEac0/MxO7OO7SYnnPc8Vj0f3U//vVsl2+rhne58i1b5rhuUvSPOu3PDfS55/n5JKjimW9MLrM2OEVdDrsHCyndgoPIJJKxAGcmaRCkHUQBjCZkKESUoUMxkyMwrTqGW574/LAFVpL8fAb2zPRzvwD/p519FP9WzIddOfjdUQ6PzcbcRO0VDkapSRdcVonEaKismUoEoIR3IkgoEne13OxF82g/MQhX1m1joe91zs2I/Eohc7xZ/IwjJ0d5FxBjLoNFZtIg1BUtUVBHSFQAB1FUoQEllUDMFquriQb8rWckx7Hcdwr04Y5GZfGLYZBAAyJCmYyALsmyaoipi7YBJHZvxyWewjxDQszB+tJl73/NterMfOyEq+UlgJ5/XD1QcjLIms2WGQoeHzoktFX4HFCOd2EglhbNSggRIBAIQMTUTc4qKKcWSqhONXd5Il4+b/KCPsEHtf4xhOFeZhsOfhfP/AnLRzoZZxaUWifni+VjbiJ1CLgIiVJJklWEUP2RDEIEEqkgzRUmXMNl/1vSoV2o/8LNr2oo1HCr3l+CWzXp9Bw89dkj/LYDlzEMbf0Xd5ONlkTMPaRwDBBexwGZRziICwjMX1kUg6oIGGM9YCmEUqwxQCWGCD2rT765MvxMWdHjwsbNrtZS4TjuoQgkiIgNVkAFFQJMJM02NEU2DsqgdPJH37tOIY2cRZ7Rblt/PemIiceXaaTwbQgYxVgSgYglBRUFIRjpfOAGL6nfCn5cy4enovz4dvj3XIh9schWyWo0Q+WVkm/vN69vnPf4pjp0PHEccyU2b4Y4cL7y1/R6HfPw/4fidITomug7Wm/i/xYlfR2SazHesZF2Cda7ncPfQoKnttkQQ2d94tPctile5L8VaN/ziOEJ2x7us/ndUXtSl5OdHF/S/cIj3PfS/YtW/o94Nm2egs6dYW9Bs/fHNLDuAQooxxeflr9tyNiJbkDBWNeTW2KHWRuizkAwft8RiCHK1ZPzMU1I34thEFNT14i1/N/jPf3z9DzSN0qMoSwAA", ep.websiteAnalytics = "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", F.d.StiWizardDashboardsHelper = ep
     }
     F.l.StiDashboardImages = class {};
     {
-        class ep {
+        class tp {
             clone() {
                 return this[L.System.StiObject.stimulsoft]().memberwiseClone()
             }
             meta() {
                 return [new n("Name"), new n("Expression")]
             }
             saveToJsonObject(e) {
@@ -12221,33 +12219,33 @@
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             static loadFromJson(e) {
-                let t = new ep;
+                let t = new tp;
                 return t.loadFromJsonObject(e), t
             }
             static loadFromXml(e) {
-                let t = new ep;
+                let t = new tp;
                 return t.loadFromXml(e), t
             }
             saveToString() {
                 return this.saveToJsonObject(je.Report).serialize()
             }
             getStringRepresentation() {
                 if (B.isNullOrWhiteSpace(this.name)) return b.get("FormStyleDesigner", "NotSpecified");
                 return B.isNullOrWhiteSpace(this.expression) ? this.name : this.name + ` - ` + this.expression
             }
             constructor() {
                 this.name = "", this.expression = ""
             }
         }
-        F.g.StiDashboardDrillDownParameter = ep
+        F.g.StiDashboardDrillDownParameter = tp
     }
     F.x.StiDashboardDrillDownParameterConverter = class {}, F.x.StiDashboardInteractionConverter = class {}, F.x.StiDashboardInteractionCreator = class {
         static new2(e) {
             switch (e) {
                 case "Chart":
                     return new F.g.StiChartDashboardInteraction;
                 case "Table":
@@ -12277,97 +12275,97 @@
                 case "Filter":
                     return new F.g.StiFilterDashboardInteraction;
                 default:
                     throw new ca(e)
             }
         }
     }, F.x.StiDashboardInteractionJsonConverter = class {}, F.x.StiTableDashboardInteractionConverter = class extends F.x.StiDashboardInteractionConverter {};
-    let hm = F.Z.StiWebContentElement,
-        mm = F.E.StiButtonElement,
-        cm = F.Y.StiShapeElement,
-        dm = F.S.StiComboBoxElement,
-        gm = F.P.StiListBoxElement,
-        pm = F.I.StiTreeViewBoxElement,
-        Sm = F.J.StiTreeViewElement,
-        wm = F.Q.StiDatePickerElement,
-        bm = F.W.StiTextElement,
-        fm = F.K.StiTableElement,
-        ym = F.F.StiCardsElement,
-        Cm = F.M.StiProgressElement,
-        xm = F.O.StiOnlineMapElement,
-        Mm = F.L.StiRegionMapElement,
-        Tm = F.X.StiImageElement,
-        Fm = F.T.StiGaugeElement,
-        vm = F.H.StiChartElement,
-        Am = F.R.StiNumberBoxElement,
-        Im = F.e.StiDashboard;
+    let mm = F.Z.StiWebContentElement,
+        cm = F.E.StiButtonElement,
+        dm = F.Y.StiShapeElement,
+        gm = F.S.StiComboBoxElement,
+        pm = F.P.StiListBoxElement,
+        Sm = F.I.StiTreeViewBoxElement,
+        wm = F.J.StiTreeViewElement,
+        bm = F.Q.StiDatePickerElement,
+        fm = F.W.StiTextElement,
+        ym = F.K.StiTableElement,
+        Cm = F.F.StiCardsElement,
+        xm = F.M.StiProgressElement,
+        Mm = F.O.StiOnlineMapElement,
+        Tm = F.L.StiRegionMapElement,
+        Fm = F.X.StiImageElement,
+        vm = F.T.StiGaugeElement,
+        Am = F.H.StiChartElement,
+        Im = F.R.StiNumberBoxElement,
+        Dm = F.e.StiDashboard;
     {
-        class tp {}
-        F.m.StiDashboardOptions = tp, F.m.Services = class {
+        class rp {}
+        F.m.StiDashboardOptions = rp, F.m.Services = class {
             static get elements() {
-                return null == this._elements && (this._elements = [Im, mm, ym, Fm, Tm, hm, bh, Mm, xm, St, Zh, Cm, fm, bm, cm, dm, gm, pm, Sm, wm, Am], L.Report.Chart.StiChartAssembly.isAssemblyLoaded) && this._elements.push(vm), this._elements
+                return null == this._elements && (this._elements = [Dm, cm, Cm, vm, Fm, mm, fh, Tm, Mm, St, Yh, xm, ym, fm, dm, gm, pm, Sm, wm, bm, Im], L.Report.Chart.StiChartAssembly.isAssemblyLoaded) && this._elements.push(Am), this._elements
             }
         }
     } {
-        class rp {
+        class ip {
             static fetchAll() {
                 return F.m.Services.elements
             }
             static load() {
                 L["StiOptions"].Services.components.addRange(this.fetchAll())
             }
-        }(F.m.StiDashboardElementsLoader = rp).load()
+        }(F.m.StiDashboardElementsLoader = ip).load()
     }
-    let Dm = L.Data.Engine.StiDataIndicatorValue,
-        Rm = L.Report.Chart.StiDoughnutArea,
-        Em = L.Report.Chart.IStiClusteredColumnArea,
-        Om = L.Report.Chart.IStiColumnShape3D,
-        Vm = L.Report.Chart.IStiClusteredColumnArea3D,
-        km = L.Report.Chart.IStiAxisArea3D,
-        Nm = L.Report.Chart.StiPie3dSeries,
-        Lm = L.Report.Chart.StiClusteredBarArea,
-        Bm = L.Report.Chart.StiConstantLines_StiOrientation,
-        Pm = F.H.StiLegendVisibility,
-        jm = L.Report.Chart.StiPieSeries,
-        Hm = L.Report.Chart.StiRadarArea,
-        zm = L.Report.Chart.StiMarker,
-        Gm = L.Report.Chart.IStiGanttArea,
-        Xm = F.H.StiChartLabelsStyle,
-        Wm = L.Report.Chart.IStiPieSeriesLabels,
-        Jm = L.Report.Chart.IStiOutsidePieLabels,
-        Um = L.Report.Chart.IStiCenterPieLabels,
-        Zm = L.Report.Chart.IStiYRightAxis,
-        Ym = F.H.StiXChartAxisTitle,
-        Km = L.Report.Chart.IStiClusteredBarArea,
-        Qm = L.Report.Chart.IStiAllowApplyBrushNegative,
-        qm = L.Report.Chart.IStiAllowApplyColorNegative,
-        _m = L.Report.Chart.IStiSeriesLabels,
-        $m = L.Report.Chart.IStiDoughnutSeries,
-        ec = L.Report.Chart.IStiPictorialSeries,
-        tc = L.Report.Chart.IStiParetoSeries,
-        rc = L.Report.Components.TextFormats.StiCustomFormatService,
-        ic = L.Report.Chart.IStiPieSeries,
-        sc = F.H.StiYChartAxis,
-        nc = F.H.StiXChartAxis,
-        lc = L.Report.Chart.IStiAxisArea,
-        ac = L.Report.Chart.IStiStackedBaseLineSeries,
-        oc = L.Report.Chart.IStiBaseLineSeries,
-        uc = L.Report.Chart.IStiFunnelSeries,
-        hc = L.Report.Chart.StiBoxAndWhiskerHelper,
-        mc = L.Report.Chart.StiShowSeriesLabels,
-        cc = L.Report.Chart.IStiShowZerosSeries,
-        dc = L.Report.Chart.StiShowEmptyCellsAs,
-        gc = L.Report.Chart.StiChartHelper,
-        pc = L.Report.Chart.IStiFontIconsSeries,
-        Sc = L.Report.Chart.IStiRoundValuesArea,
-        wc = L.Report.Chart.StiScatterSeries,
-        bc = L.Report.Chart.IStiScatterArea,
-        fc = L.Base.Helpers.StiValueComparer,
-        yc = L.Report.Chart.IStiShowNullsSeriesAs,
-        Cc = L.Report.Chart.IStiShowZerosSeriesAs;
+    let Rm = L.Data.Engine.StiDataIndicatorValue,
+        Em = L.Report.Chart.StiDoughnutArea,
+        Om = L.Report.Chart.IStiClusteredColumnArea,
+        Vm = L.Report.Chart.IStiColumnShape3D,
+        km = L.Report.Chart.IStiClusteredColumnArea3D,
+        Nm = L.Report.Chart.IStiAxisArea3D,
+        Lm = L.Report.Chart.StiPie3dSeries,
+        Bm = L.Report.Chart.StiClusteredBarArea,
+        Pm = L.Report.Chart.StiConstantLines_StiOrientation,
+        jm = F.H.StiLegendVisibility,
+        Hm = L.Report.Chart.StiPieSeries,
+        zm = L.Report.Chart.StiRadarArea,
+        Gm = L.Report.Chart.StiMarker,
+        Xm = L.Report.Chart.IStiGanttArea,
+        Wm = F.H.StiChartLabelsStyle,
+        Jm = L.Report.Chart.IStiPieSeriesLabels,
+        Um = L.Report.Chart.IStiOutsidePieLabels,
+        Zm = L.Report.Chart.IStiCenterPieLabels,
+        Ym = L.Report.Chart.IStiYRightAxis,
+        Km = F.H.StiXChartAxisTitle,
+        Qm = L.Report.Chart.IStiClusteredBarArea,
+        qm = L.Report.Chart.IStiAllowApplyBrushNegative,
+        _m = L.Report.Chart.IStiAllowApplyColorNegative,
+        $m = L.Report.Chart.IStiSeriesLabels,
+        ec = L.Report.Chart.IStiDoughnutSeries,
+        tc = L.Report.Chart.IStiPictorialSeries,
+        rc = L.Report.Chart.IStiParetoSeries,
+        ic = L.Report.Components.TextFormats.StiCustomFormatService,
+        sc = L.Report.Chart.IStiPieSeries,
+        nc = F.H.StiYChartAxis,
+        lc = F.H.StiXChartAxis,
+        ac = L.Report.Chart.IStiAxisArea,
+        oc = L.Report.Chart.IStiStackedBaseLineSeries,
+        uc = L.Report.Chart.IStiBaseLineSeries,
+        hc = L.Report.Chart.IStiFunnelSeries,
+        mc = L.Report.Chart.StiBoxAndWhiskerHelper,
+        cc = L.Report.Chart.StiShowSeriesLabels,
+        dc = L.Report.Chart.IStiShowZerosSeries,
+        gc = L.Report.Chart.StiShowEmptyCellsAs,
+        pc = L.Report.Chart.StiChartHelper,
+        Sc = L.Report.Chart.IStiFontIconsSeries,
+        wc = L.Report.Chart.IStiRoundValuesArea,
+        bc = L.Report.Chart.StiScatterSeries,
+        fc = L.Report.Chart.IStiScatterArea,
+        yc = L.Base.Helpers.StiValueComparer,
+        Cc = L.Report.Chart.IStiShowNullsSeriesAs,
+        xc = L.Report.Chart.IStiShowZerosSeriesAs;
     {
         class S extends F.i.StiElementBuilder {
             async render(r, i) {
                 this.storedCulture = ai.set(r.report);
                 try {
                     let e = new L.Report.Components["StiChart"];
                     if (e.horSpacing = r.area.horSpacing, e.vertSpacing = r.area.vertSpacing, e.isDashboard = !0, e.page = r.page, e.previousAnimations = r.previousAnimations, e.sortAnimation = r.sortAnimation, r.sortAnimation = !1, S.setStyle(r, e), e.series.clear(), null == i) return e;
@@ -12403,64 +12401,64 @@
                         let n = 0;
                         for (let r of c) {
                             let e = l.get(r),
                                 t = P.getValueOrFirstOrDefault(e.getArrayItem(i).firstOrDefault());
                             null != t && t[L.System.StiObject.stimulsoft]().is(w) && (s.core.isDateTimeValues = !0), s.values[n] = e.getArrayItem(i).firstOrDefaultAsNullableNumber(), n++
                         }
                         s.originalArguments = c[L.System.StiObject.stimulsoft]().toArray(), s.arguments = this.proccessSelectArguments(c, o, s, m);
-                        let r = s.as(uc);
+                        let r = s.as(hc);
                         if (null != r) {
                             let e = s.values,
                                 t = s.arguments;
                             Ln.sort3(e, t), Ln.reverse(e), Ln.reverse(t), r.values = e, r.arguments = t
-                        } else if (s.is(tc)) {
+                        } else if (s.is(rc)) {
                             let r = new P,
                                 i = new P;
                             for (let t = 0; t < s.values.length; t++) {
                                 let e = s.values[t];
                                 if (!(0 < e)) continue;
                                 r.add(e), null != s.arguments && t < s.arguments.length ? i.add(s.arguments[t]) : i.add(t + 1)
                             }
                             let e = r[L.System.StiObject.stimulsoft]().toArray(),
                                 t = i[L.System.StiObject.stimulsoft]().toArray();
                             Ln.sort3(e, t), Ln.reverse(e), Ln.reverse(t), s.valuesStart = null, s.values = e, s.arguments = t
                         }
                         t++, await S.processTopNElements(o, s), L.Report.Chart["StiHistogramHelper"].checkValuesAndArguments(s, o.argumentFormat), await this.renderSeriesInteraction(s, o, c.length, this.toString(a))
                     }
                 }
-                hc.checkArgument(u), gc.checkWaterfallTotals(u)
+                mc.checkArgument(u), pc.checkWaterfallTotals(u)
             }
             proccessSelectArguments(e, t, s, r) {
-                let i = s.as(wc);
+                let i = s.as(bc);
                 if (null != i) {
                     let i = [];
                     for (let r = 0; r < s.originalArguments.length; r++) {
                         let e = s.originalArguments[r],
                             t = null != e && 0 < e.length ? e[0] : e;
                         i.push(t)
                     }
                     return i
                 }
                 return e.select(e => this.getString(t.argumentFormat, e, r))[L.System.StiObject.stimulsoft]().toArray()
             }
             static async processTopNElements(r, s) {
-                if (r.topN.mode == ch.None) return;
+                if (r.topN.mode == dh.None) return;
                 let n = new P,
                     e = (s.values.length > s.arguments.length ? s.values : s.arguments).length;
                 for (let i = 0; i < e; i++) {
                     let e = i < s.values.length ? s.values[i] : null,
                         t = i < s.arguments.length ? s.arguments[i] : null,
                         r = i < s.originalArguments.length ? s.originalArguments[i] : null;
                     n.add({
                         key: t,
                         key1: r,
                         value: e
                     })
                 }
-                let i = (n = r.topN.mode == ch.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).take(r.topN.count);
+                let i = (n = r.topN.mode == dh.Bottom ? n.orderBy(e => e.value) : n.orderByDescending(e => e.value)).take(r.topN.count);
                 if (n.length > r.topN.count && r.topN.showOthers) {
                     let e = n.skip(r.topN.count).sum(e => V.tryToNumber(e.value)),
                         t = B.isNullOrEmpty(r.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(r.topN.othersText, r);
                     i.add({
                         key: t,
                         key1: t,
                         value: e
@@ -12474,94 +12472,94 @@
                 if (null != r) return t.style = r, void(t.customStyleName = e.customStyleName);
                 t.style = J.getChartStyle2(o.Blue)
             }
             static getDetailRows(e, r, i) {
                 if (!i.any()) return e;
                 return e.where(t => {
                     let e = i.select(e => t[e])[L.System.StiObject.stimulsoft]().toArray();
-                    return fc.equalValues(e, r)
+                    return yc.equalValues(e, r)
                 })
             }
             renderSeries(e, t, r, i) {
                 let s = t,
                     n = Pn.neww2(t.seriesType);
-                return S.renderSeriesYAxis(e, s, n), S.renderSeriesLine(s, n), S.renderSeriesShowZeros(s, n), S.renderSeriesShowNulls(s, n), n.coreTitle = this.getSeriesTitle(e, r, t), n.core.seriesColors = null != e.seriesColors && 0 < e.seriesColors.length ? e.seriesColors : null, n.isDashboard = !0, this.renderSeriesNegativeColor(e, n, i.series.count), this.renderSeriesParetoColor(e, n, i.series.count), this.renderMarker(e, n), S.renderSeriesLighting(n), S.renderSeriesIcon(e, n), S.renderSeriesPie3d(e, n), n.is(Om) && (n.columnShape = e.columnShape), i.series.add(n), n
+                return S.renderSeriesYAxis(e, s, n), S.renderSeriesLine(s, n), S.renderSeriesShowZeros(s, n), S.renderSeriesShowNulls(s, n), n.coreTitle = this.getSeriesTitle(e, r, t), n.core.seriesColors = null != e.seriesColors && 0 < e.seriesColors.length ? e.seriesColors : null, n.isDashboard = !0, this.renderSeriesNegativeColor(e, n, i.series.count), this.renderSeriesParetoColor(e, n, i.series.count), this.renderMarker(e, n), S.renderSeriesLighting(n), S.renderSeriesIcon(e, n), S.renderSeriesPie3d(e, n), n.is(Vm) && (n.columnShape = e.columnShape), i.series.add(n), n
             }
             static renderSeriesPie3d(e, t) {
                 var r;
-                t.is(Nm) && null != (r = e.options3D) && r[L.System.StiObject.stimulsoft]().is(On) && (t.options3D = e.options3D[L.System.StiObject.stimulsoft]().as(On))
+                t.is(Lm) && null != (r = e.options3D) && r[L.System.StiObject.stimulsoft]().is(On) && (t.options3D = e.options3D[L.System.StiObject.stimulsoft]().as(On))
             }
             static renderSeriesYAxis(e, t, r) {
                 t.is(Bs) && 1 < e.values.length && (r.yAxis = t.yAxis)
             }
             static renderSeriesLine(r, i) {
                 if (null != r) {
-                    let e = i.as(oc);
+                    let e = i.as(uc);
                     if (null != e) return e.lineStyle = r.lineStyle, void(e.lineWidth = r.lineWidth);
-                    let t = i.as(ac);
+                    let t = i.as(oc);
                     null != t && (t.lineStyle = r.lineStyle, t.lineWidth = r.lineWidth)
                 }
             }
             static renderSeriesShowZeros(e, t) {
-                let r = t.as(cc);
+                let r = t.as(dc);
                 if (null == r) return;
                 r.showZeros = e.showZeros == Ct.Zero;
-                let i = t.as(oc);
+                let i = t.as(uc);
                 if (null == i) return;
-                e.showZeros == Ct.Gap && (i.showZerosAs = dc.Gap), e.showZeros == Ct.ConnectPointsWithLine && (i.showZerosAs = dc.ConnectPointsWithLine)
+                e.showZeros == Ct.Gap && (i.showZerosAs = gc.Gap), e.showZeros == Ct.ConnectPointsWithLine && (i.showZerosAs = gc.ConnectPointsWithLine)
             }
             static renderSeriesShowNulls(e, t) {
                 let r = t.as(il);
                 if (null == r) return;
                 r.showNulls = e.showNulls == Ct.Zero;
-                let i = t.as(oc);
+                let i = t.as(uc);
                 if (null == i) return;
-                e.showNulls == Ct.Gap && (i.showNullsAs = dc.Gap), e.showNulls == Ct.ConnectPointsWithLine && (i.showNullsAs = dc.ConnectPointsWithLine)
+                e.showNulls == Ct.Gap && (i.showNullsAs = gc.Gap), e.showNulls == Ct.ConnectPointsWithLine && (i.showNullsAs = gc.ConnectPointsWithLine)
             }
             static renderSeriesLighting(e) {
-                e.is(ic) && (e.lighting = !1), e.is($m) && (e.lighting = !1)
+                e.is(sc) && (e.lighting = !1), e.is(ec) && (e.lighting = !1)
             }
             static renderSeriesIcon(e, t) {
-                let r = t.as(pc);
-                null != r && (t.is(ec) && null == e.icon ? r.icon = L.Report.Helpers.StiFontIcons.QuarterFull : r.icon = e.icon)
+                let r = t.as(Sc);
+                null != r && (t.is(tc) && null == e.icon ? r.icon = L.Report.Helpers.StiFontIcons.QuarterFull : r.icon = e.icon)
             }
             renderMarker(e, t) {
-                let r, i = null != t ? t.as(oc) : null,
-                    s = null != t ? t.as(ac) : null;
-                null != i ? r = null != i.marker ? i.marker.as(zm) : null : null != s && (r = null != s.marker ? s.marker.as(zm) : null), null != r && (r.size = e.marker.size, r.angle = e.marker.angle, r.type = e.marker.type, r.extendedVisible = e.marker.visible)
+                let r, i = null != t ? t.as(uc) : null,
+                    s = null != t ? t.as(oc) : null;
+                null != i ? r = null != i.marker ? i.marker.as(Gm) : null : null != s && (r = null != s.marker ? s.marker.as(Gm) : null), null != r && (r.size = e.marker.size, r.angle = e.marker.angle, r.type = e.marker.type, r.extendedVisible = e.marker.visible)
             }
             renderSeriesNegativeColor(e, t, r) {
                 if (null == e.negativeSeriesColors || e.negativeSeriesColors.length <= 0) return;
                 while (r >= e.negativeSeriesColors.length) r -= e.negativeSeriesColors.length;
-                let i = t.as(Qm),
-                    s = (null != i && (i.allowApplyBrushNegative = !0, i.brushNegative = new v(e.negativeSeriesColors[r])), t.as(qm));
+                let i = t.as(qm),
+                    s = (null != i && (i.allowApplyBrushNegative = !0, i.brushNegative = new v(e.negativeSeriesColors[r])), t.as(_m));
                 null != s && (s.allowApplyColorNegative = !0, s.lineColorNegative = e.negativeSeriesColors[r])
             }
             renderSeriesParetoColor(e, t, r) {
                 if (null == e.paretoSeriesColors || e.paretoSeriesColors.length <= 0) return;
                 while (r >= e.paretoSeriesColors.length) r -= e.paretoSeriesColors.length;
-                let i = t.as(tc);
+                let i = t.as(rc);
                 null != i && (i.allowApplyLineColor = !0, i.lineColor = e.paretoSeriesColors[r])
             }
             async renderArea(e, t) {
                 let r = jl.getBackColor(e, e.backColor);
-                N.transparent.equals(r) || (t.area.brush = 255 == r.a ? new v(r) : new rt), (e.isPieChart || e.isPie3dChart || e.isDoughnutChart || e.isFunnelChart || e.isSunburstChart || e.isPictorialStackedChart) && (t.area.allowApplyStyle = !1, t.area.borderColor = N.transparent), t.area.colorEach = S.getColorEach(e), t.area.is(Sc) && (t.area.as(Sc).roundValues = e.roundValues), await this.renderAxisAxes3d(e, t), await this.renderAxisAxes(e, t), S.renderRadarAxis(e, t), this.renderAreaIndicator(e, t)
+                N.transparent.equals(r) || (t.area.brush = 255 == r.a ? new v(r) : new rt), (e.isPieChart || e.isPie3dChart || e.isDoughnutChart || e.isFunnelChart || e.isSunburstChart || e.isPictorialStackedChart) && (t.area.allowApplyStyle = !1, t.area.borderColor = N.transparent), t.area.colorEach = S.getColorEach(e), t.area.is(wc) && (t.area.as(wc).roundValues = e.roundValues), await this.renderAxisAxes3d(e, t), await this.renderAxisAxes(e, t), S.renderRadarAxis(e, t), this.renderAreaIndicator(e, t)
             }
             static getColorEach(e) {
                 return !!(e.isPieChart || e.isPie3dChart || e.isDoughnutChart || e.isPictorialStackedChart) || null != e.area && e.area.colorEach
             }
             async renderAxisAxes3d(e, t) {
                 if (t.series.count <= 0) return;
-                let r = t.area.as(Vm),
-                    i = (null != r && (r.sideBySide = e.area.sideBySide), t.area.as(Em));
+                let r = t.area.as(km),
+                    i = (null != r && (r.sideBySide = e.area.sideBySide), t.area.as(Om));
                 null != i && (i.sideBySide = e.area.sideBySide), await this.renderXAxis3D(e, t), await this.renderYAxis3D(e, t)
             }
             async renderAxisAxes(e, t) {
                 if (t.series.count <= 0) return;
-                let r = t.area.as(lc);
+                let r = t.area.as(ac);
                 if (null == r) return;
                 r.allowApplyStyle = !1, r.borderColor = N.transparent, S.renderInterlacingHor(e, r), S.renderInterlacingVert(e, r), S.renderGridLinesHor(e, r), S.renderGridLinesVert(e, r), r.reverseHor = e.area.reverseHor, r.reverseVert = e.area.reverseVert, await this.renderXAxis(e, t, !1), await this.renderYAxis(e, t, !1), e.xTopAxis.visible && await this.renderXAxis(e, t, !0), e.yRightAxis.visible ? await this.renderYAxis(e, t, !0) : await S.renderYRightAxis(e, t)
             }
             static renderInterlacingHor(e, t) {
                 e.area.interlacingHor.visible && !N.transparent.equals(e.area.interlacingHor.color) && (t.interlacingHor.interlacedBrush = new v(e.area.interlacingHor.color)), t.interlacingHor.visible = e.area.interlacingHor.visible
             }
             static renderInterlacingVert(e, t) {
@@ -12570,61 +12568,61 @@
             static renderGridLinesHor(e, t) {
                 e.area.gridLinesHor.visible && !N.transparent.equals(e.area.gridLinesHor.color) && (t.gridLinesHor.color = e.area.gridLinesHor.color), t.gridLinesHor.visible = e.area.gridLinesHor.visible, t.gridLinesHor.style = Ri.Solid
             }
             static renderGridLinesVert(e, t) {
                 e.area.gridLinesVert.visible && !N.transparent.equals(e.area.gridLinesVert.color) && (t.gridLinesVert.color = e.area.gridLinesVert.color), t.gridLinesVert.visible = e.area.gridLinesVert.visible, t.gridLinesVert.style = Ri.Solid
             }
             async renderXAxis3D(e, t) {
-                let r = t.area.as(km);
+                let r = t.area.as(Nm);
                 if (null == r) return;
                 let i = r.xAxis,
                     s = e.xAxis;
                 await S.renderAxis3D(e, i, s), i.visible = s.visible, s.showEdgeValues == Tn.Auto && (i.showEdgeValues = !1)
             }
             async renderYAxis3D(e, t) {
-                let r = t.area.as(km);
+                let r = t.area.as(Nm);
                 if (null == r) return;
                 let i = r.yAxis,
                     s = e.yAxis;
                 await S.renderAxis3D(e, i, s), i.visible = s.visible, null != e.valueFormat && (i.labels.formatService = S.checkValueFormat(e.valueFormat, t))
             }
             async renderXAxis(e, t, r) {
-                let i = t.area.as(lc);
+                let i = t.area.as(ac);
                 if (null == i) return;
                 let s = r ? i.xTopAxis : i.xAxis,
                     n = r ? e.xTopAxis : e.xAxis,
-                    l = t.area.is(Km),
+                    l = t.area.is(Qm),
                     a = Hn.isDrillAvailable(e) && e.drillDownCurrentLevel < e.drillDownLevelCount ? e.arguments.getRange(e.drillDownCurrentLevel, 1) : e.arguments,
                     o = (l ? e.values : a).select(this.getTitle).distinct(),
-                    u = (await S.renderAxis(e, s, n), s.ticks.visible = o.any(), s.visible = n.visible, await S.renderXAxisTitleText(e, s, n, o), t.series.toList().cast().all(e => e.is(oc) || e.is(ac))),
+                    u = (await S.renderAxis(e, s, n), s.ticks.visible = o.any(), s.visible = n.visible, await S.renderXAxisTitleText(e, s, n, o), t.series.toList().cast().all(e => e.is(uc) || e.is(oc))),
                     h = (n.startFromZero == Tn.Auto && (s.startFromZero = !u), t.series.toList().cast().all(e => e.core.isDateTimeValues));
-                h && i.is(Lm) && (s.startFromZero = !1), n.showEdgeValues == Tn.Auto && (s.showEdgeValues = u), s.labels.placement == an.AutoRotation && (s.labels.textAlignment = z.Left), null != e.valueFormat && i.is(Km) && (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), null != e.argumentFormat && i.is(bc) && (s.labels.formatService = e.argumentFormat), S.renderAxisLineColor(e, s)
+                h && i.is(Bm) && (s.startFromZero = !1), n.showEdgeValues == Tn.Auto && (s.showEdgeValues = u), s.labels.placement == an.AutoRotation && (s.labels.textAlignment = z.Left), null != e.valueFormat && i.is(Qm) && (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), null != e.argumentFormat && i.is(fc) && (s.labels.formatService = e.argumentFormat), S.renderAxisLineColor(e, s)
             }
             async renderYAxis(e, t, r) {
-                let i = t.area.as(lc);
+                let i = t.area.as(ac);
                 if (null == i) return;
                 let s = r ? i.yRightAxis : i.yAxis,
                     n = r ? e.yRightAxis : e.yAxis,
-                    l = t.area.is(Gm) || t.area.is(Km),
+                    l = t.area.is(Xm) || t.area.is(Qm),
                     a = (l && e.dataMode != Vn.ManuallyEnteringData ? e.arguments : e.chartValuesList()).select(this.getTitle).distinct(),
-                    o = (await S.renderAxis(e, s, n), s.visible = a.any() && n.visible, await S.renderYAxisTitleText(e, s, n, a), null == e.valueFormat || i.is(Km) || (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), t.series.toList().cast().all(e => e.core.isDateTimeValues));
+                    o = (await S.renderAxis(e, s, n), s.visible = a.any() && n.visible, await S.renderYAxisTitleText(e, s, n, a), null == e.valueFormat || i.is(Qm) || (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), t.series.toList().cast().all(e => e.core.isDateTimeValues));
                 o && (i.yAxis.startFromZero = !1), S.renderAxisLineColor(e, s)
             }
             static renderXRadarAxis(e, t) {
-                let r = t.area.as(Hm);
+                let r = t.area.as(zm);
                 if (null == r) return;
                 this.renderXRadarAxisLabels(e.area.xAxis.labels, r.xAxis.labels), this.renderAxisRange(r.xAxis.range, e.xAxis), null != e.valueFormat && (r.yAxis.labels.formatService = S.checkValueFormat(e.valueFormat, t));
                 let i = J.getForeColor(e);
                 this.renderRadarXAxisLabelsColor(e, r.xAxis.labels, e.xAxis, i), r.xAxis.visible = e.xAxis.visible
             }
             static renderXRadarAxisLabels(e, t) {
                 t.font = e.font, t.textBefore = e.textBefore, t.textAfter = e.textAfter, t.allowApplyStyle = !1
             }
             static renderYRadarAxis(e, t) {
-                let r = t.area.as(Hm);
+                let r = t.area.as(zm);
                 if (null == r) return;
                 this.renderYRadarAxisLabels(e.area.yAxis.labels, r.yAxis.labels), this.renderAxisRange(r.yAxis.range, e.yAxis);
                 let i = J.getForeColor(e);
                 this.renderRadarYAxisLabelsColor(e, r.yAxis.labels, e.yAxis, i), r.yAxis.visible = e.yAxis.visible
             }
             static renderYRadarAxisLabels(e, t) {
                 t.font = e.font, t.textBefore = e.textBefore, t.textAfter = e.textAfter, t.step = e.step, t.angle = e.angle, t.textAlignment = e.textAlignment, t.wordWrap = e.wordWrap, t.width = e.width, t.allowApplyStyle = !1
@@ -12655,15 +12653,15 @@
                         t.useLocalSetting = !1, t.decimalDigits = e
                     }
                     return t
                 }
                 return e
             }
             static async renderYRightAxis(e, t) {
-                let r = t.area.as(lc);
+                let r = t.area.as(ac);
                 if (null == r) return;
                 await this.renderAxis(e, r.yRightAxis, e.yRightAxis), this.renderAxisLineColor(e, r.yRightAxis)
             }
             static async renderXAxisTitleText(e, t, r, i) {
                 if (!r.title.visible) return;
                 t.title.text = B.isNullOrEmpty(r.title.text) ? B.join(" / ", i) : await O.parseAsync(r.title.text, e)
             }
@@ -12673,20 +12671,20 @@
             }
             static renderAxisLineColor(e, t) {
                 if (e.style == o.Custom && !N.transparent.equals(t.lineColor)) return t.allowApplyStyle = !1, void(t.allowApplyStyle = !1);
                 J.isDarkStyle(e.dashboard) && (t.allowApplyStyle = !1, t.lineColor = J.getForeColor(e))
             }
             static renderRadarAxis(e, t) {
                 if (t.series.count <= 0) return;
-                let r = t.area.as(Hm);
+                let r = t.area.as(zm);
                 if (null == r) return;
                 this.renderXRadarAxis(e, t), this.renderYRadarAxis(e, t)
             }
             renderAreaIndicator(e, t) {
-                let r = t.area.as(Rm);
+                let r = t.area.as(Em);
                 if (null == r) return;
                 let i = null == e ? void 0 : e.report,
                     s = null == this.indicatorValueValue ? "" : this.getString(e.valueFormat, this.indicatorValueValue.toString(), i),
                     n = (r.indicator.value.value = s, r.indicator.value.color = e.area.indicator.value.color, e.area.indicator.title.text);
                 r.indicator.title.text = n, r.indicator.title.color = e.area.indicator.title.color, r.indicator.visible = !B.isNullOrEmpty(s) || !B.isNullOrEmpty(n)
             }
             static async renderAxis3D(e, t, r) {
@@ -12696,66 +12694,66 @@
             static async renderAxis(e, t, r) {
                 let i = J.getForeColor(e);
                 this.renderAxisTitle(e, t, r, i), await this.renderAxisLabels(e, t, r), this.renderAxisStartFromZero(t, r), this.renderAxisShowEdgeValues(t, r), this.renderAxisRange(t.range, r), this.renderAxisLabelsColor(e, t, r, i)
             }
             static renderAxisTitle(e, t, r, i) {
                 let s = this.getTitleAxisChart(r),
                     n = t.title;
-                n.alignment = s.alignment, n.position = s.position, n.font = s.font, this.renderAxisLabelsTitleColor(e, n, s, i), s.is(Ym) && (n.direction = s.direction), s.is(Mn) && (n.direction = s.direction)
+                n.alignment = s.alignment, n.position = s.position, n.font = s.font, this.renderAxisLabelsTitleColor(e, n, s, i), s.is(Km) && (n.direction = s.direction), s.is(Mn) && (n.direction = s.direction)
             }
             static async renderAxisLabels3D(e, t, r) {
                 t.labels.textAfter = await O.parseAsync(r.labels.textAfter, e), t.labels.textBefore = await O.parseAsync(r.labels.textBefore, e), t.labels.font = r.labels.font
             }
             static async renderAxisLabels(e, t, r) {
-                t.labels.angle = r.labels.angle, t.is(Zm) && e.isParetoChart || (t.labels.textAfter = await O.parseAsync(r.labels.textAfter, e)), t.labels.textAlignment = r.labels.textAlignment, t.labels.textBefore = await O.parseAsync(r.labels.textBefore, e), t.labels.font = r.labels.font, t.labels.placement = r.labels.placement, t.labels.step = r.labels.step, t.labels.wordWrap = r.labels.wordWrap, t.labels.width = r.labels.width
+                t.labels.angle = r.labels.angle, t.is(Ym) && e.isParetoChart || (t.labels.textAfter = await O.parseAsync(r.labels.textAfter, e)), t.labels.textAlignment = r.labels.textAlignment, t.labels.textBefore = await O.parseAsync(r.labels.textBefore, e), t.labels.font = r.labels.font, t.labels.placement = r.labels.placement, t.labels.step = r.labels.step, t.labels.wordWrap = r.labels.wordWrap, t.labels.width = r.labels.width
             }
             static renderAxisStartFromZero(t, r) {
-                if (r.is(nc)) {
+                if (r.is(lc)) {
                     let e = r;
                     null != e && e.startFromZero != Tn.Auto && (t.startFromZero = e.startFromZero != Tn.False)
                 }
-                if (r.is(sc)) {
+                if (r.is(nc)) {
                     let e = r;
                     null != e && (t.startFromZero = e.startFromZero)
                 }
             }
             static renderAxisShowEdgeValues(t, r) {
-                if (r.is(nc)) {
+                if (r.is(lc)) {
                     let e = r;
                     null != e && e.showEdgeValues != Tn.Auto && (t.showEdgeValues = e.showEdgeValues != Tn.False)
                 }
             }
             static renderAxisRange(e, t) {
-                t[L.System.StiObject.stimulsoft]().getType() != nc && t[L.System.StiObject.stimulsoft]().getType() != sc || (e.auto = t.range.auto, e.maximum = t.range.maximum, e.minimum = t.range.minimum)
+                t[L.System.StiObject.stimulsoft]().getType() != lc && t[L.System.StiObject.stimulsoft]().getType() != nc || (e.auto = t.range.auto, e.maximum = t.range.maximum, e.minimum = t.range.minimum)
             }
             static renderAxisLabelsTitleColor(e, t, r, i) {
                 if (!N.transparent.equals(r.color)) return void(t.color = r.color);
                 e.style == o.Custom && !N.transparent.equals(t.color) || (t.color = i)
             }
             static renderAxisLabelsColor3D(e, t, r, i) {
                 if (!N.transparent.equals(r.labels.color)) return void(t.labels.color = r.labels.color);
                 e.style == o.Custom && !N.transparent.equals(t.labels.color) || (t.labels.color = i)
             }
             static renderAxisLabelsColor(e, t, r, i) {
                 if (!N.transparent.equals(r.labels.color)) return void(t.labels.color = r.labels.color);
                 e.style == o.Custom && !N.transparent.equals(t.labels.color) || (t.labels.color = i)
             }
             static getTitleAxisChart(e) {
+                if (e.is(lc)) return e.title;
                 if (e.is(nc)) return e.title;
-                if (e.is(sc)) return e.title;
                 return null
             }
             async renderLegend(e, t) {
                 t.legend.horAlignment = e.legend.horAlignment, t.legend.vertAlignment = e.legend.vertAlignment, t.legend.title = await O.parseAsync(e.legend.title.text, e), t.legend.titleFont = e.legend.title.font, t.legend.allowApplyStyle = !1, t.legend.font = e.legend.labels.font, t.legend.visible = S.getChartLegendVisible(e, t), t.legend.columns = e.legend.columns, t.legend.direction = e.legend.direction;
                 let r = J.getForeColor(e);
                 S.renderLegendTitleColor(e, t, r), S.renderLegendLabelsColor(e, t, r)
             }
             static getChartLegendVisible(e, t) {
-                if (1 == t.series.count && !t.series.getByIndex(0).is(jm)) return e.legend.visibility == Pm.Always;
-                return e.legend.visibility != Pm.False
+                if (1 == t.series.count && !t.series.getByIndex(0).is(Hm)) return e.legend.visibility == jm.Always;
+                return e.legend.visibility != jm.False
             }
             static renderLegendTitleColor(e, t, r) {
                 if (!N.transparent.equals(e.legend.title.color)) return void(t.legend.titleColor = e.legend.title.color);
                 e.style == o.Custom && !N.transparent.equals(t.legend.titleColor) || (t.legend.titleColor = r)
             }
             static renderSeriesLabelsLegendValueType(e, t) {
                 let r = 0;
@@ -12837,15 +12835,15 @@
                 }
                 return e
             }
             static async renderConstantLines(i, s) {
                 for (let r of i.constantLines) {
                     let e = !B.isNullOrEmpty(r.text),
                         t = new L.Report.Chart["StiConstantLines"];
-                    t.allowApplyStyle = !1, t.text = r.text, t.axisValue = await O.parseAsync(r.axisValue, i), t.lineColor = r.lineColor, t.lineStyle = r.lineStyle, t.lineWidth = r.lineWidth, t.titleVisible = e, t.orientation = i.isBarChart ? Bm.Vertical : Bm.Horizontal, t.position = r.position, s.constantLines.add(t)
+                    t.allowApplyStyle = !1, t.text = r.text, t.axisValue = await O.parseAsync(r.axisValue, i), t.lineColor = r.lineColor, t.lineStyle = r.lineStyle, t.lineWidth = r.lineWidth, t.titleVisible = e, t.orientation = i.isBarChart ? Pm.Vertical : Pm.Horizontal, t.position = r.position, s.constantLines.add(t)
                 }
             }
             static renderTrendLines(t, e, r) {
                 var i;
                 let s = null == (i = e.trendLines) ? void 0 : i.where(e => e.keyValueMeter == r.key).toList();
                 t.trendLines.clear();
                 for (let e of s) t.trendLines.add(this.getTrendLine(e, t.chart))
@@ -12866,45 +12864,45 @@
                         let e = new L.Report.Chart["StiTrendLineLogarithmic"];
                         return e.allowApplyStyle = !1, e.lineColor = N.transparent.equals(t.lineColor) ? r.style.core.trendLineColor : t.lineColor, e.lineStyle = t.lineStyle, e.lineWidth = t.lineWidth, e.showShadow = !1, e
                     }
                 }
             }
             async renderSeriesLabels(t, r) {
                 if (!(t.isPieChart || t.isPie3dChart || t.isFunnelChart || t.isPictorialStackedChart || t.isDoughnutChart || t.isTreemapChart || t.isAxisAreaChart || t.isSunburstChart || t.isRadarChart || t.isWaterfallChart || t.isAxisAreaChart3D || t.isLineChart3D)) return void(r.seriesLabels.visible = !1);
-                if (r.allowApplyStyle = !1, t.isPieChart ? S.renderPieLabelsPosition(t, r) : t.isPie3dChart ? S.renderPie3dLabelsPosition(t, r) : t.isDoughnutChart || t.isSunburstChart ? S.renderDoughnutLabelsPosition(t, r) : t.isFunnelChart ? S.renderFunnelLabelsPosition(t, r) : t.isPictorialStackedChart ? S.renderPictorialStackedLabelsPosition(t, r) : t.isTreemapChart ? S.renderTreemapLabelsPosition(t, r) : t.isWaterfallChart ? S.renderWaterfallLabelsPosition(t, r) : t.isStackedChart ? S.renderStackedLabelsPosition(t, r) : t.isRadarChart ? S.renderRadarLabelsPosition(t, r) : t.isAxisAreaChart ? S.renderAxisLabelsPosition(t, r) : t.isAxisAreaChart3D ? S.renderClusteredColumn3DLabelsPosition(t, r) : t.isLineChart3D && this.renderLine3DLabelsPosition(t, r), r.seriesLabels.core.applyStyle(r.style), await S.applyPropertiesToSeriesLabels(t, r.seriesLabels.as(_m)), t.isStackedChart)
-                    for (let e of r.series.list) await S.applyPropertiesToSeriesLabels(t, e.seriesLabels.as(_m));
+                if (r.allowApplyStyle = !1, t.isPieChart ? S.renderPieLabelsPosition(t, r) : t.isPie3dChart ? S.renderPie3dLabelsPosition(t, r) : t.isDoughnutChart || t.isSunburstChart ? S.renderDoughnutLabelsPosition(t, r) : t.isFunnelChart ? S.renderFunnelLabelsPosition(t, r) : t.isPictorialStackedChart ? S.renderPictorialStackedLabelsPosition(t, r) : t.isTreemapChart ? S.renderTreemapLabelsPosition(t, r) : t.isWaterfallChart ? S.renderWaterfallLabelsPosition(t, r) : t.isStackedChart ? S.renderStackedLabelsPosition(t, r) : t.isRadarChart ? S.renderRadarLabelsPosition(t, r) : t.isAxisAreaChart ? S.renderAxisLabelsPosition(t, r) : t.isAxisAreaChart3D ? S.renderClusteredColumn3DLabelsPosition(t, r) : t.isLineChart3D && this.renderLine3DLabelsPosition(t, r), r.seriesLabels.core.applyStyle(r.style), await S.applyPropertiesToSeriesLabels(t, r.seriesLabels.as($m)), t.isStackedChart)
+                    for (let e of r.series.list) await S.applyPropertiesToSeriesLabels(t, e.seriesLabels.as($m));
                 t.isPieChart || t.isPie3dChart || t.isDoughnutChart || t.isSunburstChart ? (S.renderPieLabelsStyle(t, r), S.renderPieLabelsAutoRotate(t, r), S.renderSeriesLabelsLegendValueType(t, r)) : t.isFullStackedChart ? (S.renderLabelsStyle(t, r), r.seriesLabels.showInPercent = !0) : S.renderLabelsStyle(t, r), S.renderLabelsColor(t, r), S.renderLabelsTextFormat(t, r), S.renderLabelsShowZeros(r), S.renderLabelsShowZeros(r)
             }
             static renderLabelsShowZeros(i) {
                 for (let r of i.series.toList()) {
-                    let e = r.as(Cc);
-                    if (null != e) return void(i.seriesLabels.showZeros = e.showZerosAs == dc.Zero);
-                    let t = r.as(cc);
+                    let e = r.as(xc);
+                    if (null != e) return void(i.seriesLabels.showZeros = e.showZerosAs == gc.Zero);
+                    let t = r.as(dc);
                     if (null != t) return void(i.seriesLabels.showZeros = t.showZeros)
                 }
             }
             static renderLabelsShowNulls(i) {
                 for (let r of i.series.toList()) {
-                    let e = r.as(yc);
-                    if (null != e) return void(i.seriesLabels.showNulls = e.showNullsAs == dc.Zero);
+                    let e = r.as(Cc);
+                    if (null != e) return void(i.seriesLabels.showNulls = e.showNullsAs == gc.Zero);
                     let t = r.as(il);
                     if (null != t) return void(i.seriesLabels.showNulls = t.showNulls)
                 }
             }
             static async applyPropertiesToSeriesLabels(e, t) {
                 t.preventIntersection = !0, t.textAfter = await O.parseAsync(e.labels.textAfter, e), t.textBefore = await O.parseAsync(e.labels.textBefore, e), t.font = e.labels.font, t.showZeros = !1, t.width = e.labels.width, t.wordWrap = e.labels.wordWrap
             }
             static renderPieLabelsAutoRotate(e, t) {
-                let r = t.seriesLabels.as(Um);
+                let r = t.seriesLabels.as(Zm);
                 null != r && (r.autoRotate = e.labels.autoRotate)
             }
             static renderLabelsColor(e, t) {
                 var r, i;
-                let s = t.seriesLabels.as(_m),
-                    n = t.seriesLabels.as(Jm);
+                let s = t.seriesLabels.as($m),
+                    n = t.seriesLabels.as(Um);
                 N.transparent.equals(e.labels.foreColor) ? (s.labelColor = N.gray, s.labelColor = J.isDarkStyle2(e.style) ? N.fromArgb2(50, 50, 50) : null != (null == (r = null == t ? void 0 : t.style) ? void 0 : r.core) ? t.style.core.seriesLabelsColor : N.gray, null != n && (n.lineColor = null != (null == (i = null == t ? void 0 : t.style) ? void 0 : i.core) ? t.style.core.seriesLabelsLineColor : N.gray)) : (s.labelColor = e.labels.foreColor, null != n && (n.lineColor = e.labels.foreColor))
             }
             static renderLabelsTextFormat(e, t) {
                 t.seriesLabels.formatService = e.valueFormat
             }
             static renderFunnelLabelsPosition(e, t) {
                 switch (e.labels.funnelPosition) {
@@ -12993,16 +12991,16 @@
                 }
             }
             static renderStackedLabelsPosition(e, r) {
                 switch (e.labels.axisPosition) {
                     case p.Total: {
                         let t = r.series.toList().lastOrDefault();
                         r.series.toList().where(e => e != t).toList().forEach(e => {
-                            e.showSeriesLabels = mc.FromSeries, e.seriesLabels.visible = !1
-                        }), t.showSeriesLabels = mc.FromSeries, t.seriesLabels = new L.Report.Chart["StiValueAxisLabels"], t.isTotalLabel = !0, t.seriesLabels.formatService = e.valueFormat;
+                            e.showSeriesLabels = cc.FromSeries, e.seriesLabels.visible = !1
+                        }), t.showSeriesLabels = cc.FromSeries, t.seriesLabels = new L.Report.Chart["StiValueAxisLabels"], t.isTotalLabel = !0, t.seriesLabels.formatService = e.valueFormat;
                         break
                     }
                     default:
                         S.renderAxisLabelsPosition(e, r);
                         break
                 }
             }
@@ -13132,49 +13130,49 @@
                         break;
                     default:
                         t.seriesLabels.visible = !1;
                         break
                 }
             }
             static renderPieLabelsStyle(e, t) {
-                let r = t.seriesLabels.as(Wm);
+                let r = t.seriesLabels.as(Jm);
                 switch (e.labels.style) {
-                    case Xm.PercentOfTotal:
+                    case Wm.PercentOfTotal:
                         r.showInPercent = !0, r.valueType = Sn.Value;
                         break;
-                    case Xm.Category:
+                    case Wm.Category:
                         r.showInPercent = !1, r.valueType = e.arguments.any() ? Sn.Argument : Sn.SeriesTitle;
                         break;
-                    case Xm.CategoryPercentOfTotal:
+                    case Wm.CategoryPercentOfTotal:
                         r.showInPercent = !0, r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
                         break;
-                    case Xm.CategoryValue:
+                    case Wm.CategoryValue:
                         r.showInPercent = !1, r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
                         break;
-                    case Xm.Value:
+                    case Wm.Value:
                         r.showInPercent = !1, r.valueType = Sn.Value;
                         break
                 }
             }
             static renderLabelsStyle(e, t) {
                 let r = t.seriesLabels;
                 switch (e.labels.style) {
-                    case Xm.PercentOfTotal:
+                    case Wm.PercentOfTotal:
                         r.valueType = Sn.Value;
                         break;
-                    case Xm.Category:
+                    case Wm.Category:
                         r.valueType = e.arguments.any() ? Sn.Argument : Sn.SeriesTitle;
                         break;
-                    case Xm.CategoryPercentOfTotal:
+                    case Wm.CategoryPercentOfTotal:
                         r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
                         break;
-                    case Xm.CategoryValue:
+                    case Wm.CategoryValue:
                         r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
                         break;
-                    case Xm.Value:
+                    case Wm.Value:
                         r.valueType = Sn.Value;
                         break
                 }
             }
             async renderSeriesInteraction(r, i, e, s) {
                 if (r.chart.isDesigning) return;
                 let n = null == i ? void 0 : i.report,
@@ -13208,23 +13206,23 @@
                     r = L.Base.StiJsonReportObjectHelper.Serialize.jBrush(e.core.toolTipTextBrush),
                     i = L.Base.StiJsonReportObjectHelper.Serialize.jBorder2(e.core.toolTipBorder),
                     s = e.core.toolTipCornerRadius.toString();
                 return `,"StiToolTipCornerRadius":"${s}","StiToolTipBrush":"${t}","StiToolTipTextBrush":"${r}","StiToolTipBorder":"${i}"`
             }
             async getHyperlink(e, t, r, i, s) {
                 null == r && (r = ""), null == s && (s = "");
-                let n = new Co;
+                let n = new xo;
                 return n.add("Argument", r), n.add("Value", i), n.add("Series", s), O.parseAsync(t, e, !1, n)
             }
             getTitle(e) {
-                return kh.getLabel(e)
+                return Nh.getLabel(e)
             }
             getSeriesTitle(e, t, r) {
                 if (e.values.length < 2) return t;
-                let i = kh.getLabel(r),
+                let i = Nh.getLabel(r),
                     s = B.isNullOrWhiteSpace(i) ? null : i;
                 if (null == s) return t;
                 return B.isNullOrWhiteSpace(t) ? s : t + ` - ` + s
             }
             getArgumentIndex(e, t) {
                 let r = this.getArgumentMeterIndexes(e).toList();
                 if (null == r || !r.any()) return -1;
@@ -13266,28 +13264,28 @@
                     for (let e of i) t.add(this.getFormatValue(r, e, s));
                     return B.join(" - ", t)
                 }
                 return this.getFormatValue(r, i, s)
             }
             getFormatValue(e, t, r) {
                 if (null == t) return "";
-                if (t instanceof w) return e.is2(Xr) || e.is2(Gr) || e.is2(rc) ? e.format(t) : t.toShortDateString();
+                if (t instanceof w) return e.is2(Xr) || e.is2(Gr) || e.is2(ic) ? e.format(t) : t.toShortDateString();
                 let i = null == r ? void 0 : r.getParsedCulture();
                 if (li.isEligable(t, i)) return li.convert(t, i);
                 if (null != e) return e.format(t);
                 return t.toString()
             }
             async calculateIndicatorValue(r) {
                 if (null == r.indicatorValue || null != r.indicatorValue && B.isNullOrEmpty(r.indicatorValue.expression)) return;
                 let i = bl.getKey(r);
-                if (Dm.existsInCache(i)) this.indicatorValueValue = Dm.getFromCache(i);
+                if (Rm.existsInCache(i)) this.indicatorValueValue = Rm.getFromCache(i);
                 else {
                     let e = r.clone(!0),
                         t = (e.values = new P, e.arguments = new P, await bl.getOrCreate(e));
-                    null != t && (this.indicatorValueValue = t.rows.getArrayItem(0).tryCastToNullableNumber().sum(), Dm.addToCache(i, this.indicatorValueValue))
+                    null != t && (this.indicatorValueValue = t.rows.getArrayItem(0).tryCastToNullableNumber().sum(), Rm.addToCache(i, this.indicatorValueValue))
                 }
             }
             static create(e) {
                 if (e.isSunburstChart) return new F.i.StiSunburstChartElementBuilder;
                 if (e.isBubbleChart) return new F.i.StiBubbleChartElementBuilder;
                 if (e.isRange) return new F.i.StiRangeChartElementBuilder;
                 if (e.isFinancial) return new F.i.StiFinancialChartElementBuilder;
@@ -13307,30 +13305,30 @@
                 let t = e.meters.firstOrDefault(e => e.is(Ps));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getArgumentKeys(e, t) {
                 if (null == t) return null;
                 let r = this.getArgumentMeters(t),
                     i = r.select(e => t.meters.indexOf(e)).toList(),
-                    s = t.rows.groupBy2(t => i.select(e => t[e])[L.System.StiObject.stimulsoft]().toArray(), new xh);
+                    s = t.rows.groupBy2(t => i.select(e => t[e])[L.System.StiObject.stimulsoft]().toArray(), new Mh);
                 return s.select(e => e.key[L.System.StiObject.stimulsoft]().toArray())
             }
             getValueMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(Bs)).cast()
             }
             getArgumentMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(Ls)).cast()
             }
         }
         F.i.StiChartElementBuilder = S
     }
-    let xc = L.Report.Chart.IStiBubbleSeries,
-        Mc = (F.i.StiBubbleChartElementBuilder = class extends F.i.StiChartElementBuilder {
+    let Mc = L.Report.Chart.IStiBubbleSeries,
+        Tc = (F.i.StiBubbleChartElementBuilder = class extends F.i.StiChartElementBuilder {
             async renderElements(u, h, m) {
                 let c = this.getSeriesMeterIndex(m),
                     e = this.getSeriesKeys(m, c),
                     t = this.getValueMeters(m),
                     d = e.count2();
                 for (let o of e) {
                     let a = 0;
@@ -13352,15 +13350,15 @@
                 }
             }
             renderSeries(e, t, r, i) {
                 let s = new L.Report.Chart["StiBubbleSeries"];
                 return s.coreTitle = this.getSeriesTitle(e, r, t), s.isDashboard = !0, i.series.add(s), s
             }
             async renderSeriesInteraction(l, e, t, a) {
-                let o = l.as(xc);
+                let o = l.as(Mc);
                 if (null == o) return;
                 let u = e.dashboardInteraction;
                 if (u.onHover == Vr.ShowToolTip) {
                     l.toolTips = Ln.create(String, t);
                     for (let n = 0; n < t; n++) {
                         let r = "",
                             i = "",
@@ -13372,15 +13370,15 @@
                         } else l.toolTips[n] = await this.getHyperlink2(e, u.toolTip, i, r, s, a)
                     }
                 }
                 l.drillDownEnabled = !0
             }
             async getHyperlink2(e, t, r, i, s, n) {
                 null == r && (r = ""), null == n && (n = "");
-                let l = new Co;
+                let l = new xo;
                 return l.add("Argument", r), l.add("Value", i), l.add("Weight", s), l.add("Series", n), O.parseAsync(t, e, !1, l)
             }
             getWeightIndex(e, t) {
                 if (null == e) return -1;
                 let r = this.getWeightMeterIndexes(e);
                 if (null == r) return -1;
                 if (!r.any()) return -1;
@@ -13398,30 +13396,30 @@
             }
             getValueMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(_n)).cast()
             }
             getArgumentMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Ra)).cast()
+                return e.meters.where(e => e.is(Ea)).cast()
             }
         }, L.Report.Chart.IStiFinancialSeries),
-        Tc = (F.i.StiFinancialChartElementBuilder = class extends F.i.StiChartElementBuilder {
+        Fc = (F.i.StiFinancialChartElementBuilder = class extends F.i.StiChartElementBuilder {
             async renderElements(c, d, g) {
                 let p = null == d ? void 0 : d.report,
                     S = this.getSeriesMeterIndex(g),
                     e = this.getSeriesKeys(g, S),
                     t = this.getValueMeters(g),
                     w = e.count2();
                 for (let m of e) {
                     let h = 0;
                     for (let u of t) {
                         let e = this.getValueMeterIndexes(g)[h],
                             t = this.renderSeries(c, u, m, d),
-                            r = t.as(Mc);
+                            r = t.as(Tc);
                         if (null == t || null == r) continue;
                         let i = -1 != S && 1 < w ? g.rows.whereArrayItemStringEqualsTo(S, m) : g.rows,
                             s = (r.valuesOpen = i.getArrayItem(e).tryCastToNullableNumber()[L.System.StiObject.stimulsoft]().toArray(), r.valuesClose = null, this.getCloseValueIndex(g, e));
                         if (-1 != s && (r.valuesClose = i.getArrayItem(s).tryCastToNullableNumber()[L.System.StiObject.stimulsoft]().toArray()), null == r.valuesClose) {
                             r.valuesClose = [];
                             for (let e = 0; e < t.argument.length; e++) r.valuesClose[e] = 10
                         }
@@ -13444,15 +13442,15 @@
                 }
             }
             renderSeries(e, t, r, i) {
                 let s = Pn.neww2(t.as(Os).seriesType);
                 return s.coreTitle = this.getSeriesTitle(e, r, t), s.isDashboard = !0, i.series.add(s), s
             }
             async renderSeriesInteraction(o, e, t, r) {
-                let u = o.as(Mc);
+                let u = o.as(Tc);
                 if (null == u) return;
                 let i = e.dashboardInteraction;
                 if (i.onHover == Vr.ShowToolTip) {
                     o.toolTips = Ln.create(String, t);
                     for (let a = 0; a < t; a++) {
                         let e = "",
                             t = "",
@@ -13467,29 +13465,29 @@
                 o.drillDownEnabled = !0
             }
             async renderArea(e, c) {
                 await super.renderArea(e, c);
                 let d = null,
                     g = null;
                 for (let m = 0; m < c.series.count; m++) {
-                    let e = c.series.getByIndex(m).as(Mc);
+                    let e = c.series.getByIndex(m).as(Tc);
                     if (null == e) continue;
                     let t = e.valuesOpen[L.System.StiObject.stimulsoft]().toList().min(),
                         r = e.valuesClose[L.System.StiObject.stimulsoft]().toList().min(),
                         i = e.valuesLow[L.System.StiObject.stimulsoft]().toList().min(),
                         s = e.valuesHigh[L.System.StiObject.stimulsoft]().toList().min(),
                         n = e.valuesOpen[L.System.StiObject.stimulsoft]().toList().max(),
                         l = e.valuesClose[L.System.StiObject.stimulsoft]().toList().max(),
                         a = e.valuesLow[L.System.StiObject.stimulsoft]().toList().max(),
                         o = e.valuesHigh[L.System.StiObject.stimulsoft]().toList().max(),
                         u = new P([t, r, i, s]).min(),
                         h = new P([n, l, a, o]).max();
                     null == d && (d = u), null == g && (g = h), d = Math.min(d, u), g = Math.max(g, h)
                 }
-                let t = c.area.as(lc),
+                let t = c.area.as(ac),
                     r = (t.yAxis.range.auto = !1, t.yAxis.range.minimum = d, t.yAxis.range.maximum = g, t.yAxis.range.maximum - t.yAxis.range.minimum);
                 t.yAxis.labels.step = 2 < r ? Math.round(r / 10) : ae.round2(r / 10, 4)
             }
             getValueMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(Os)).cast()
             }
@@ -13539,15 +13537,15 @@
                 return this.getHighMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getHighMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(Ns)).cast()
             }
         }, L.Report.Chart.IStiRangeSeries),
-        Fc = (F.i.StiRangeChartElementBuilder = class extends F.i.StiChartElementBuilder {
+        vc = (F.i.StiRangeChartElementBuilder = class extends F.i.StiChartElementBuilder {
             async renderElements(u, h, m) {
                 let c = null == h ? void 0 : h.report,
                     d = this.getSeriesMeterIndex(m),
                     e = this.getSeriesKeys(m, d),
                     g = e.count2(),
                     r = this.getValueMeters(m),
                     p = this.getArgumentMeterIndexes(m),
@@ -13562,15 +13560,15 @@
                         let s = -1 != d && 1 < g ? m.rows.whereArrayItemStringEqualsTo(d, this.toString(o)) : m.rows,
                             n = (r.values = P.create(Number, S.length), 0);
                         for (let t of S) {
                             let e = F.i.StiChartElementBuilder.getDetailRows(s, t, p);
                             n < r.values.length && (r.values[n] = e.getArrayItem(i).firstOrDefaultAsNullableNumber()), n++
                         }
                         r.core.isDateTimeValues = P.getValueOrFirstOrDefault(s.getArrayItem(i).toList().firstOrDefault()) instanceof w;
-                        let l = r.as(Tc);
+                        let l = r.as(Fc);
                         if (null != l) {
                             l.valuesEnd = P.create(Number, S.length);
                             let r = this.getEndValueIndex(m, i);
                             if (null == l.valuesEnd && (l.valuesEnd = P.repeat(10, S.length)), -1 != r) {
                                 n = 0;
                                 for (let t of S) {
                                     let e = F.i.StiChartElementBuilder.getDetailRows(s, t, p);
@@ -13588,15 +13586,15 @@
                 let s = Pn.neww2(t.seriesType),
                     n = (s.coreTitle = this.getSeriesTitle(e, r, t), s.isDashboard = !0, t);
                 return F.i.StiChartElementBuilder.renderSeriesLine(n, s), F.i.StiChartElementBuilder.renderSeriesShowNulls(n, s), this.renderMarker(e, s), i.series.add(s), s
             }
             async renderSeriesInteraction(s, n, e, l) {
                 var a, o;
                 let u = null == n ? void 0 : n.report,
-                    h = s.as(Tc);
+                    h = s.as(Fc);
                 if (null == h) return;
                 let t = n.dashboardInteraction.as(zn);
                 if (t.onHover == Vr.ShowToolTip) {
                     s.toolTips = Ln.create(String, e);
                     for (let i = 0; i < e; i++) {
                         let e = "",
                             t = "",
@@ -13613,20 +13611,20 @@
                         t = await this.getToolTipStyle(r);
                     return "{" + B.format(e, "#ffffff", s, i, n, t) + "}"
                 }
                 return this.getHyperlink2(e, t, i, s, n, l)
             }
             async getHyperlink2(e, t, r, i, s, n) {
                 null == r && (r = ""), null == n && (n = "");
-                let l = new Co;
+                let l = new xo;
                 return l.add("Argument", r), l.add("Value", i), l.add("EndValue", s), l.add("Series", n), O.parseAsync(t, e, !1, l)
             }
             getValueMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Ea)).cast()
+                return e.meters.where(e => e.is(Oa)).cast()
             }
             getEndValueIndex(e, t) {
                 if (null == e) return -1;
                 let r = this.getEndValueMeterIndexes(e);
                 if (null == r || !r.any()) return -1;
                 if (1 == r.length) return r.toList().firstOrDefault();
                 if (r.length > t) return ae.trunc(r[t]);
@@ -13637,24 +13635,24 @@
                 return this.getEndValueMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getEndValueMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(js)).cast()
             }
         }, L.Report.Components.StiShape),
-        vc = (F.i.StiShapeElementBuilder = class {
+        Ac = (F.i.StiShapeElementBuilder = class {
             render(e) {
-                let t = new Fc;
+                let t = new vc;
                 return t.shapeType = e.shapeType, t.brush = e.fill, t.borderColor = e.stroke, t.size = e.size, t
             }
         }, L.Report.Chart.IStiStackedColumnSeries),
-        Ac = L.Report.Chart.IStiStackedBarSeries,
-        Ic = L.Report.Chart.IStiRibbonSeries;
+        Ic = L.Report.Chart.IStiStackedBarSeries,
+        Dc = L.Report.Chart.IStiRibbonSeries;
     {
-        class ip extends F.i.StiChartElementBuilder {
+        class sp extends F.i.StiChartElementBuilder {
             async renderElements(a, o, u) {
                 let h = null == o ? void 0 : o.report,
                     m = this.getSeriesMeterIndex(u),
                     e = this.getSeriesKeys(u, m),
                     c = this.getArgumentMeterIndexes(u),
                     d = this.getArgumentKeys(a, u).toList(),
                     r = this.getValueMeters(u),
@@ -13673,15 +13671,15 @@
                         for (let t of d) {
                             let e = F.i.StiChartElementBuilder.getDetailRows(s, t, c);
                             n < i.values.length && (i.values[n] = e.getArrayItem(r).firstOrDefaultAsNullableNumber()), n++
                         }
                         i.originalArguments = d[L.System.StiObject.stimulsoft]().toArray(), i.arguments = d.select(e => this.getString(a.argumentFormat, e, h))[L.System.StiObject.stimulsoft]().toArray(), t++
                     }
                 }
-                await ip.processTopNStackedChart(a, o);
+                await sp.processTopNStackedChart(a, o);
                 for (let t = 0; t < g.length; t++) {
                     if (o.series.count < t) break;
                     let e = o.series.getByIndex(t);
                     if (null == e) return;
                     await this.renderSeriesInteraction(e, a, d.length, g[t])
                 }
             }
@@ -13723,48 +13721,48 @@
                 if (r.topN.showOthers) {
                     let e = t.skip(r.topN.count).sum();
                     i.add(e)
                 }
                 return i
             }
             static async processTopNStackedChart(s, e) {
-                if (s.topN.mode == ch.None) return;
+                if (s.topN.mode == dh.None) return;
                 let n = e.series.toList();
-                if (!n.any(e => e.is(ac) || e.is(vc) || e.is(Ac) || e.is(Ic))) return;
-                let l = ip.getDataTable(n.toList());
+                if (!n.any(e => e.is(oc) || e.is(Ac) || e.is(Ic) || e.is(Dc))) return;
+                let l = sp.getDataTable(n.toList());
                 if (l.rows.count < 1) return;
                 for (let i = 0; i < l.rows.count; i++) {
                     0 < n.length && n[0].arguments.length > i ? l.rows.getByIndex(i).setValue(1, n[0].arguments[i]) : l.rows.getByIndex(i).setValue(1, null), 0 < n.length && n[0].originalArguments.length > i ? l.rows.getByIndex(i).setValue(l.columns.count - 2, n[0].originalArguments[i]) : l.rows.getByIndex(i).setValue(l.columns.count - 2, null);
                     let r = 0;
                     for (let t = 0; t < n.length; t++)
                         if (0 < n.length && n[t].values.length > i) {
                             let e = n[t].values[i];
                             l.rows.getByIndex(i).setValue(t + 2, e), r += e
                         } else l.rows.getByIndex(i).setValue(t + 2, null);
                     l.rows.getByIndex(i).setValue(l.columns.count - 1, r)
                 }
-                l.defaultView.sort = s.topN.mode == ch.Top ? "ValueSum desc" : "ValueSum asc", l = l.defaultView.toTable();
+                l.defaultView.sort = s.topN.mode == dh.Top ? "ValueSum desc" : "ValueSum asc", l = l.defaultView.toTable();
                 let a = 0;
                 for (let i of n) {
-                    let e = ip.getListByColumnName(l, "OriginalArguments"),
-                        t = (i.originalArguments = await ip.getArguments(e, s), ip.getListByColumnName(l, "Argument")),
-                        r = (i.arguments = await ip.getArguments(t, s), ip.getListByColumnName(l, "Value-" + a.toString()));
-                    i.values = ip.getValues(r, s), i.is(Ac) && (i.originalArguments = i.originalArguments.reverse(), i.arguments = i.arguments.reverse(), i.values = i.values.reverse()), a++
+                    let e = sp.getListByColumnName(l, "OriginalArguments"),
+                        t = (i.originalArguments = await sp.getArguments(e, s), sp.getListByColumnName(l, "Argument")),
+                        r = (i.arguments = await sp.getArguments(t, s), sp.getListByColumnName(l, "Value-" + a.toString()));
+                    i.values = sp.getValues(r, s), i.is(Ic) && (i.originalArguments = i.originalArguments.reverse(), i.arguments = i.arguments.reverse(), i.values = i.values.reverse()), a++
                 }
             }
             static getListByColumnName(e, r) {
                 let i = new P;
                 for (let t of e.rows.toList()) {
                     let e = t.gett(r);
                     i.add(e)
                 }
                 return i
             }
         }
-        F.i.StiStackedChartElementBuilder = ip
+        F.i.StiStackedChartElementBuilder = sp
     }
     F.i.StiSunburstChartElementBuilder = class extends F.i.StiChartElementBuilder {
         async renderElements(i, s, n) {
             let t = this.getArgumentMeters(n),
                 l = this.getValueMeters(n).firstOrDefault(),
                 a = this.getValueMeterIndexes(n)[L.System.StiObject.stimulsoft]().toList().firstOrDefault();
             for (let e = 0; e < t.length; e++) {
@@ -13778,33 +13776,33 @@
         }
         renderSeries(e, t, r, i) {
             let s = Pn.neww2(t.seriesType);
             return s.core.seriesColors = null != e.seriesColors && 0 < e.seriesColors.length ? e.seriesColors : null, s.isDashboard = !0, i.series.add(s), s
         }
     };
     {
-        class sp {
+        class np {
             static getVisualizer(e) {
                 return null
             }
         }
-        sp.typeToGdiVisualizer = new Co, sp.typeToWpfVisualizer = new Co, sp.lockObject = {}, F.n.StiVisualizer = sp
+        np.typeToGdiVisualizer = new xo, np.typeToWpfVisualizer = new xo, np.lockObject = {}, F.n.StiVisualizer = np
     }
     F.n.StiGdiVisualizer = class extends F.n.StiVisualizer {
         render(e) {}
     }, F.n.StiGdiVisualizerAttribute = class {}, F.u.StiIndicatorIconRangeValue = class {
         isBetween(e) {
             return this.start <= e && e <= this.end
         }
         constructor(e, t, r) {
             this.start = e, this.end = t, this.icon = r
         }
     };
-    let Dc = F.h.StiElementLocationHelper,
-        Rc = (F.v.StiProgressVisual = class extends F.j.StiVisual {
+    let Rc = F.h.StiElementLocationHelper,
+        Ec = (F.v.StiProgressVisual = class extends F.j.StiVisual {
             getMaxValue() {
                 return this.iterations.select(e => Math.abs(e.value)).concat(new P([0])).max()
             }
             getTargetValues() {
                 let t = this.getMaxValue(),
                     r = new P;
                 for (let e of this.iterations) r.add(null != e.target ? e.target : t);
@@ -13839,43 +13837,43 @@
                     } else l[n] = s;
                     ++r == t.length && (r = 0, a = 50)
                 }
                 return l
             }
             getContentRectangle(t) {
                 if (1 < this.iterations.length) {
-                    let e = Dc.getLocationRectangles(t, this.iterations.length, this.element);
-                    t = Dc.getSumRectangle(e)
+                    let e = Rc.getLocationRectangles(t, this.iterations.length, this.element);
+                    t = Rc.getSumRectangle(e)
                 }
                 return t
             }
             getConditionResult(i, t) {
                 let s = null;
                 switch (t.field) {
-                    case No.Value:
+                    case Lo.Value:
                         s = i.value;
                         break;
-                    case No.Series:
+                    case Lo.Series:
                         s = i.series;
                         break;
-                    case No.Target:
+                    case Lo.Target:
                         s = i.target;
                         break;
-                    case No.Percentage: {
+                    case Lo.Percentage: {
                         let e = this.getVariation(i),
                             t = new Ur,
                             r = (t.decimalDigits = 3, ts.formatAsPercentage2(this.element.report, t, e));
                         s = r.replace("%", "")[L.System.StiObject.stimulsoft]().toNumber();
                         break
                     }
                 }
                 let e = !1,
                     r = this.getConditionValue(t);
                 if (null != s) {
-                    let e = s = t.field != No.Value && t.field != No.Target && t.field != No.Percentage ? s : null == s ? 0 : s[L.System.StiObject.stimulsoft]().toNumber();
+                    let e = s = t.field != Lo.Value && t.field != Lo.Target && t.field != Lo.Percentage ? s : null == s ? 0 : s[L.System.StiObject.stimulsoft]().toNumber();
                     if (null != e && null != r) {
                         s[L.System.StiObject.stimulsoft]().getType() != r[L.System.StiObject.stimulsoft]().getType() && (s = s.toString(), r = r[L.System.StiObject.stimulsoft]().toString(), e = s);
                         try {
                             switch (t.condition) {
                                 case L.Report.Components.StiFilterCondition.EqualTo:
                                     return 0 == e[L.System.StiObject.stimulsoft]().compareTo(r);
                                 case L.Report.Components.StiFilterCondition.NotEqualTo:
@@ -13912,174 +13910,175 @@
                         } catch (e) {}
                     }
                 }
                 return e
             }
             processColor(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.Color) && this.getConditionResult(t, e)) return e.color;
+                    if (0 < (e.permissions & Bo.Color) && this.getConditionResult(t, e)) return e.color;
                 return e
             }
             getVariation(e) {
                 let t = e.value,
                     r = e.target;
                 return t / r
             }
             getConditionValue(e) {
                 if (B.isNullOrEmpty(e.value)) return null;
                 switch (e.field) {
-                    case No.Value:
-                    case No.Target:
-                    case No.Percentage:
+                    case Lo.Value:
+                    case Lo.Target:
+                    case Lo.Percentage:
                         return e.value[L.System.StiObject.stimulsoft]().toNumber();
                     default:
                         return e.value.toString()
                 }
             }
             processForeColor(t, e = null) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.TextColor) && this.getConditionResult(t, e)) return e.textColor;
+                    if (0 < (e.permissions & Bo.TextColor) && this.getConditionResult(t, e)) return e.textColor;
                 return J.getForeColor(this.element, e)
             }
             processTrackColor(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.TrackColor) && this.getConditionResult(t, e)) return e.trackColor;
+                    if (0 < (e.permissions & Bo.TrackColor) && this.getConditionResult(t, e)) return e.trackColor;
                 return e
             }
             processFontStyle(e, t) {
                 let r = this.processFontBold(e.bold, t),
                     i = this.processFontItalic(e.italic, t),
                     s = this.processFontUnderline(e.underline, t),
                     n = this.processFontStrikeout(e.strikeout, t),
                     l = hn.Regular;
                 return r && (l ^= hn.Bold), i && (l ^= hn.Italic), s && (l ^= hn.Underline), n && (l ^= hn.Strikeout), l
             }
             processFontStrikeout(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
+                    if (0 < (e.permissions & Bo.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
                 return e
             }
             processFontUnderline(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.FontStyleUnderline) && this.getConditionResult(t, e)) return e.font.underline;
+                    if (0 < (e.permissions & Bo.FontStyleUnderline) && this.getConditionResult(t, e)) return e.font.underline;
                 return e
             }
             processFontItalic(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.FontStyleItalic) && this.getConditionResult(t, e)) return e.font.italic;
+                    if (0 < (e.permissions & Bo.FontStyleItalic) && this.getConditionResult(t, e)) return e.font.italic;
                 return e
             }
             processFontBold(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.FontStyleBold) && this.getConditionResult(t, e)) return e.font.bold;
+                    if (0 < (e.permissions & Bo.FontStyleBold) && this.getConditionResult(t, e)) return e.font.bold;
                 return e
             }
             processFontName(e, t) {
                 for (let e of this.element.progressConditions)
-                    if (0 < (e.permissions & Lo.Font) && this.getConditionResult(t, e)) return e.font.name;
+                    if (0 < (e.permissions & Bo.Font) && this.getConditionResult(t, e)) return e.font.name;
                 return e
             }
             constructor(e, t) {
                 super(), this.minElementSide = 2, this.minFontSize = 3, this.element = e, this.iterations = t, this.style = J.getProgressStyle(this.element)
             }
         }, L.Base.Context.StiPieSegmentGeom),
-        Ec = (F.v.StiPieProgressVisual = class extends F.v.StiProgressVisual {
+        Oc = (F.v.StiPieProgressVisual = class extends F.v.StiProgressVisual {
             async draw(h, m) {
                 if (0 == this.iterations.length) return;
-                let c = Dc.getLocationRectangles(m, this.iterations.length, this.element);
+                let c = Rc.getLocationRectangles(m, this.iterations.length, this.element);
                 if (c.length < 1) return;
                 let d = c[0],
                     e = d.width < d.height ? d.width : d.height,
                     t = this.element.font,
                     g = this.getTitleHeight(e, t.size),
                     p = d.width,
                     S = null,
                     r = new H(t.fontFamily.name, 1, t.style, t.unit);
                 for (let t of this.iterations) {
                     if (B.isNullOrEmpty(t.series)) continue;
-                    let e = Gu.getFontSize(h, new j(0, 0, p, g), t.series, r);
+                    let e = Xu.getFontSize(h, new j(0, 0, p, g), t.series, r);
                     (null == S || S > e) && (S = e)
                 }
                 let w = (e - (g = null != S && S < t.size ? this.getTitleHeight(e, S) : g)) / 2 * .8,
                     b = (S < this.minFontSize && (S = 0, g = 0, w = e / 2 * .8), 2 * w),
                     f = this.getTargetValues(),
                     y = !1;
                 h.pushClip(m);
                 for (let u = 0; u < this.iterations.length; u++) {
                     let e = f[u],
                         t = this.iterations[u],
                         r = c[u],
-                        i = (!y && (1 < r.right - m.right || 1 < r.bottom - m.bottom) && (y = !0), r.x + r.width / 2),
+                        i = (!y && (1 < r.right - m.right || 1 < r.bottom - m.bottom) && (y = !0),
+                            r.x + r.width / 2),
                         s = r.y + g + (d.height - g) / 2,
                         n = new Yl(i, s),
                         l = new j(n.x - w, n.y - w, b, b),
                         a = new j(l.x + l.width / 2 - p / 2, l.top - g, p, g),
                         o = this.processColor(this.getColor(u), this.iterations[u]);
                     this.drawPieProgress(h, l, a, e, t, S, o)
                 }
                 if (y) {
-                    let e = Zu.factor(this.element);
+                    let e = Yu.factor(this.element);
                     this.drawArrowMore(h, m, e)
                 }
                 h.popClip()
             }
             drawPieProgress(u, e, h, t, m, c, r) {
                 let i = this.processTrackColor(this.style.trackColor, m),
                     s = (u.fillEllipse2(i, e, null), 0 != t ? 360 / t * Math.abs(m.value) : t),
-                    n = (360 < s && (s = 360), new P([new Rc(e, -90, s, null, null, null)]));
+                    n = (360 < s && (s = 360), new P([new Ec(e, -90, s, null, null, null)]));
                 if (u.fillPath(r, n, e, null), c >= this.minFontSize) {
                     let e = this.processFontName(this.element.font.fontFamily.name, m),
                         t = this.processFontStyle(this.element.font, m),
                         r = new H(e, c, t),
-                        i = new ku(r.fontFamily.name, c, r.style, r.unit),
-                        s = Nu.CenterCenter,
+                        i = new Nu(r.fontFamily.name, c, r.style, r.unit),
+                        s = Lu.CenterCenter,
                         n = new Yl,
                         l = {
-                            ref: Nu.CenterCenter
+                            ref: Lu.CenterCenter
                         },
                         a = {
                             ref: new Yl
                         },
-                        o = (Gu.measureAlignmentParameters(z.Center, h, l, a), s = l.ref, n = a.ref, this.processForeColor(m));
-                    u.drawRotatedString4(m.series, i, o, n, Gu.getStringFormatGeom(u), s, 0, !0)
+                        o = (Xu.measureAlignmentParameters(z.Center, h, l, a), s = l.ref, n = a.ref, this.processForeColor(m));
+                    u.drawRotatedString4(m.series, i, o, n, Xu.getStringFormatGeom(u), s, 0, !0)
                 }
             }
             getTitleHeight(e, t) {
                 let r = t / 13;
                 return e / 4 * (r = 4 < r ? 4 : r)
             }
             constructor(e, t) {
                 super(e, t)
             }
         }, L.Base.Context.StiArcSegmentGeom);
     F.v.StiCircleProgressVisual = class extends F.v.StiPieProgressVisual {
         async draw(g, p) {
             if (0 == this.iterations.length) return;
-            let S = Dc.getLocationRectangles(p, this.iterations.length, this.element);
+            let S = Rc.getLocationRectangles(p, this.iterations.length, this.element);
             if (S.length < 1) return;
             let w = .8,
                 b = S[0],
                 e = b.width < b.height ? b.width : b.height,
                 f = this.element.font,
                 y = this.getTitleHeight(e, f.size),
                 C = b.width,
                 x = this.getTargetValues(),
                 M = this.getTextValues(),
                 T = null,
                 r = new H(f.fontFamily.name, 1, f.style, f.unit);
             for (let t of this.iterations.where(e => !B.isNullOrEmpty(e.series))) {
-                let e = Gu.getFontSize(g, new j(0, 0, C, y), t.series, r);
+                let e = Xu.getFontSize(g, new j(0, 0, C, y), t.series, r);
                 (null == T || T > e) && (T = e)
             }
             let F = (e - (y = null != T && T < f.size ? this.getTitleHeight(e, T) : y)) / 2 * .8,
                 v = null,
                 i = new j(b.x - F * w, b.y - .79 * F, 2 * F * w, 2 * F * w),
-                s = new H(this.element.font.name, 1, hn.Bold, ph.Pixel);
+                s = new H(this.element.font.name, 1, hn.Bold, Sh.Pixel);
             for (let t = 0; t < this.iterations.length; t++) {
-                let e = Gu.getFontSize(g, i, M[t], s);
+                let e = Xu.getFontSize(g, i, M[t], s);
                 (null == v || v > e) && (v = e)
             }
             T < this.minFontSize && (y = 0, T = 0, F = e / 2 * .8);
             let A = 2 * F,
                 I = F / 5,
                 D = F - I,
                 R = 2 * D,
@@ -14089,50 +14088,50 @@
                 let e = S[d],
                     t = (!E && (1 < e.right - p.right || 1 < e.bottom - p.bottom) && (E = !0), e.x + e.width / 2),
                     r = e.y + y + (b.height - y) / 2,
                     m = new Yl(t, r),
                     c = new j(m.x - F, m.y - F, A, A),
                     i = new j(m.x - D, m.y - D, R, R),
                     s = this.processTrackColor(this.style.trackColor, this.iterations[d]),
-                    n = new Ku(s, I),
+                    n = new Qu(s, I),
                     l = (g.drawEllipse(n, c.x + I / 2, c.y + I / 2, c.width - I, c.height - I), x[d]),
                     a = 0 != l ? 360 / l * Math.abs(this.iterations[d].value) : 0,
                     o = -90,
                     u = (360 < a && (a = 360), new P),
-                    h = (u.add(new Ec(c, o, a)), u.add(new Bu(this.getPoint(m, F, o + a), this.getPoint(m, D, o + a))), u.add(new Ec(i, o + a, -a)), u.add(new Bu(this.getPoint(m, D, o), this.getPoint(m, F, o))), this.processColor(this.getColor(d), this.iterations[d]));
+                    h = (u.add(new Oc(c, o, a)), u.add(new Pu(this.getPoint(m, F, o + a), this.getPoint(m, D, o + a))), u.add(new Oc(i, o + a, -a)), u.add(new Pu(this.getPoint(m, D, o), this.getPoint(m, F, o))), this.processColor(this.getColor(d), this.iterations[d]));
                 if (g.fillPath(h, u, c, null), v >= this.minFontSize) {
                     let e = new j(m.x - F * w, m.y - .79 * F, 2 * F * w, 2 * F * w),
                         t = M[d],
-                        r = new H(this.element.font.name, v, hn.Bold, ph.Pixel),
+                        r = new H(this.element.font.name, v, hn.Bold, Sh.Pixel),
                         i = this.processFontStyle(r, this.iterations[d]),
-                        s = new ku(r.name, r.size, i, r.unit),
+                        s = new Nu(r.name, r.size, i, r.unit),
                         n = this.processForeColor(this.iterations[d]);
-                    g.drawRotatedString5(t, s, n, e, Gu.getStringFormatGeom(g), Nu.CenterCenter, 0, !0)
+                    g.drawRotatedString5(t, s, n, e, Xu.getStringFormatGeom(g), Lu.CenterCenter, 0, !0)
                 }
                 if (T >= this.minFontSize) {
                     let e = new j(m.x - C / 2, c.top - y, C, y),
                         t = new H(f.fontFamily.name, T, f.style, f.unit),
                         r = this.processFontName(t.fontFamily.name, this.iterations[d]),
                         i = this.processFontStyle(t, this.iterations[d]),
                         s = new H(r, t.size, i),
-                        n = new ku(s.fontFamily.name, T, s.style, s.unit),
-                        l = Nu.CenterCenter,
+                        n = new Nu(s.fontFamily.name, T, s.style, s.unit),
+                        l = Lu.CenterCenter,
                         a = new Yl,
                         o = {
-                            ref: Nu.CenterCenter
+                            ref: Lu.CenterCenter
                         },
                         u = {
                             ref: new Yl
                         },
-                        h = (Gu.measureAlignmentParameters(z.Center, e, o, u), l = o.ref, a = u.ref, this.processForeColor(this.iterations[d]));
-                    g.drawRotatedString4(this.iterations[d].series, n, h, a, Gu.getStringFormatGeom(g), l, 0, !0)
+                        h = (Xu.measureAlignmentParameters(z.Center, e, o, u), l = o.ref, a = u.ref, this.processForeColor(this.iterations[d]));
+                    g.drawRotatedString4(this.iterations[d].series, n, h, a, Xu.getStringFormatGeom(g), l, 0, !0)
                 }
             }
             if (E) {
-                let e = Zu.factor(this.element);
+                let e = Yu.factor(this.element);
                 this.drawArrowMore(g, p, e)
             }
             g.popClip()
         }
         getPoint(e, t, r) {
             let i = Math.PI * r / 180;
             return new Yl(e.x + Math.cos(i) * t, e.y + Math.sin(i) * t)
@@ -14152,15 +14151,15 @@
                 y = this.getTargetValues(),
                 C = this.element.font,
                 x = null,
                 n = new H(C.fontFamily.name, 1, C.style, C.unit);
             for (let i = 0; i < this.iterations.length; i++) {
                 let e = `` + this.iterations[i].series + s[i],
                     t = new j(S.x, S.y + w * i + .07 * b, f, .86 * b),
-                    r = Gu.getFontSize(p, t, e, n);
+                    r = Xu.getFontSize(p, t, e, n);
                 (null == x || x > r) && (x = r)
             }
             let M = this.element.font.size / 18 * x,
                 T = (M > x && (M = x), new H(C.fontFamily.name, M, C.style, C.unit)),
                 F = (p.pushClip(S), 1 < this.iterations.length ? .05 * w / (this.iterations.length - 1) : 0);
             for (let g = 0; g < this.iterations.length; g++) {
                 let e = this.processFontName(T.fontFamily.name, this.iterations[g]),
@@ -14170,44 +14169,44 @@
                     i = S.y + (w + F) * g,
                     l = new j(S.x, i, f, b),
                     s = this.processTrackColor(this.style.trackColor, this.iterations[g]),
                     a = (p.fillRectangle(s, l, null), 0 != r ? Math.abs(this.iterations[g].value) / r : 0),
                     o = ts.formatAsPercentage2(this.element.report, this.element.textFormat, a),
                     u = J.getForeColor(this.element);
                 if (x >= this.minFontSize) {
-                    let e = new ku(C.fontFamily.name, M, n.style, n.unit),
+                    let e = new Nu(C.fontFamily.name, M, n.style, n.unit),
                         t = p.measureString(o, e),
                         r = new j(l.right - t.width, l.top + .05 * l.height, t.width, l.height);
-                    u = this.processForeColor(this.iterations[g]), p.drawRotatedString5(o, e, u, r, Gu.getStringFormatGeom(p), Nu.CenterCenter, 0, !0)
+                    u = this.processForeColor(this.iterations[g]), p.drawRotatedString5(o, e, u, r, Xu.getStringFormatGeom(p), Lu.CenterCenter, 0, !0)
                 }
                 let h = this.iterations[g].series;
                 if (x >= this.minFontSize) {
-                    let e = new ku(C.fontFamily.name, M, n.style, n.unit),
+                    let e = new Nu(C.fontFamily.name, M, n.style, n.unit),
                         t = p.measureString(h, e),
                         r = new j(l.left, l.top + .05 * l.height, t.width, l.height);
-                    u = this.processForeColor(this.iterations[g]), p.drawRotatedString5(h, e, u, r, Gu.getStringFormatGeom(p), Nu.CenterCenter, 0, !0)
+                    u = this.processForeColor(this.iterations[g]), p.drawRotatedString5(h, e, u, r, Xu.getStringFormatGeom(p), Lu.CenterCenter, 0, !0)
                 }
                 let m = 0 != r ? f / r * this.iterations[g].value : 0,
                     c = (m > l.width && (m = l.width), new j(S.x, i, m, b)),
                     d = (p.pushClip(c), this.processColor(this.getColor(g), this.iterations[g]));
                 if (p.fillRectangle(d, c, null), x >= this.minFontSize) {
-                    let e = new ku(n.name, n.size, n.style, n.unit),
+                    let e = new Nu(n.name, n.size, n.style, n.unit),
                         t = p.measureString(o, e),
                         r = new j(l.right - t.width, l.top + .05 * l.height, t.width, l.height),
                         i = this.isColorLight(d) ? N.white : u,
                         s = this.processForeColor(this.iterations[g], i);
-                    p.drawRotatedString5(o, e, s, r, Gu.getStringFormatGeom(p), Nu.CenterCenter, 0, !0)
+                    p.drawRotatedString5(o, e, s, r, Xu.getStringFormatGeom(p), Lu.CenterCenter, 0, !0)
                 }
                 if (x >= this.minFontSize) {
-                    let e = new ku(n.name, n.size, n.style, n.unit),
+                    let e = new Nu(n.name, n.size, n.style, n.unit),
                         t = p.measureString(h, e),
                         r = new j(l.left, l.top + .05 * l.height, t.width, l.height),
                         i = this.isColorLight(d) ? N.white : u,
                         s = this.processForeColor(this.iterations[g], i);
-                    p.drawRotatedString5(h, e, s, r, Gu.getStringFormatGeom(p), Nu.CenterCenter, 0, !0)
+                    p.drawRotatedString5(h, e, s, r, Xu.getStringFormatGeom(p), Lu.CenterCenter, 0, !0)
                 }
                 p.popClip()
             }
             p.popClip()
         }
         isColorLight(e) {
             return 0 < 600 - e.r - e.g - e.b
@@ -14216,22 +14215,22 @@
             super(e, t)
         }
     };
     {
         let e;
         (q = e = F.f.StiDashboardExportFormat || (F.f.StiDashboardExportFormat = {}))[q["Pdf"] = 0] = "Pdf", q[q["Excel"] = 1] = "Excel", q[q["Data"] = 2] = "Data", q[q["Image"] = 3] = "Image", q[q["Html"] = 4] = "Html", q[q["Document"] = 5] = "Document"
     }
-    let Oc = L.Report.Components.StiPageOrientation,
-        Vc = L.System.Drawing.Printing.PaperKind,
-        kc = L.Report.Dashboard.Export.IStiDashboardExportSettings,
-        Nc = L.Report.Export.StiExportSettings;
+    let Vc = L.Report.Components.StiPageOrientation,
+        kc = L.System.Drawing.Printing.PaperKind,
+        Nc = L.Report.Dashboard.Export.IStiDashboardExportSettings,
+        Lc = L.Report.Export.StiExportSettings;
     {
-        class yd extends Nc {
+        class Cd extends Lc {
             constructor() {
-                super(...arguments), this.renderBorders = !0, this.orientation = Oc.Landscape, this.paperSize = Vc.A4, this.openAfterExport = !0
+                super(...arguments), this.renderBorders = !0, this.orientation = Vc.Landscape, this.paperSize = kc.A4, this.openAfterExport = !0
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
                 if ("function" == typeof e) return this instanceof e;
                 if (null == e) throw new Error("Type for comparison is 'undefined'");
                 return !1
             }
@@ -14239,90 +14238,90 @@
                 return this.is(e)
             }
             as(e) {
                 if (this.is(e)) return this;
                 return null
             }
             implements() {
-                return yd.ImplementsStiDashboardExportSettings || (yd.ImplementsStiDashboardExportSettings = [kc]), yd.ImplementsStiDashboardExportSettings
+                return Cd.ImplementsStiDashboardExportSettings || (Cd.ImplementsStiDashboardExportSettings = [Nc]), Cd.ImplementsStiDashboardExportSettings
             }
             get isDesignMode() {
                 return this.is(F.y.StiSvgDashboardExportSettings) && this.as(F.y.StiSvgDashboardExportSettings).designMode
             }
             getExportFormat() {
                 return F.z.StiExportFormatHelper.convert(this.format)
             }
             toParameters() {
                 let e = super.toParameters();
-                return e.Format = ve.getName(F.f.StiDashboardExportFormat, this.format), e.Orientation = ve.getName(Oc, this.orientation), e.PaperSize = ve.getName(Oc, this.paperSize), e
+                return e.Format = ve.getName(F.f.StiDashboardExportFormat, this.format), e.Orientation = ve.getName(Vc, this.orientation), e.PaperSize = ve.getName(Vc, this.paperSize), e
             }
         }
-        F.y.StiDashboardExportSettings = yd
+        F.y.StiDashboardExportSettings = Cd
     }
-    let Lc = L.Report.Export.StiImageType,
-        Bc = L.Report.Dashboard.Export.IStiImageDashboardExportSettings;
+    let Bc = L.Report.Export.StiImageType,
+        Pc = L.Report.Dashboard.Export.IStiImageDashboardExportSettings;
     {
-        class $c extends F.y.StiDashboardExportSettings {
+        class ed extends F.y.StiDashboardExportSettings {
             implements() {
-                return $c.ImplementsStiImageDashboardExportSettings || ($c.ImplementsStiImageDashboardExportSettings = super.implements().concat([F.y.IStiSizeExportSettings, Bc])), $c.ImplementsStiImageDashboardExportSettings
+                return ed.ImplementsStiImageDashboardExportSettings || (ed.ImplementsStiImageDashboardExportSettings = super.implements().concat([F.y.IStiSizeExportSettings, Pc])), ed.ImplementsStiImageDashboardExportSettings
             }
             get width() {
                 return this._width
             }
             set width(e) {
-                this._width = e, this.paperSize = Vc.Custom
+                this._width = e, this.paperSize = kc.Custom
             }
             get height() {
                 return this._height
             }
             set height(e) {
-                this._height = e, this.paperSize = Vc.Custom
+                this._height = e, this.paperSize = kc.Custom
             }
             toParameters() {
                 let e = super.toParameters();
-                return e.Format = ve.getName(F.f.StiDashboardExportFormat, this.format), e.ImageType = ve.getName(Lc, this.imageType), e.Width = 0, e.Height = 0, e
+                return e.Format = ve.getName(F.f.StiDashboardExportFormat, this.format), e.ImageType = ve.getName(Bc, this.imageType), e.Width = 0, e.Height = 0, e
             }
             constructor(e) {
-                super(), this.format = F.f.StiDashboardExportFormat.Image, this.imageType = Lc.Svg, this.scale = 100, null != e ? this.imageType = e : this.renderSinglePage = !0
+                super(), this.format = F.f.StiDashboardExportFormat.Image, this.imageType = Bc.Svg, this.scale = 100, null != e ? this.imageType = e : this.renderSinglePage = !0
             }
         }
-        F.y.StiImageDashboardExportSettings = $c
+        F.y.StiImageDashboardExportSettings = ed
     }
     F.y.StiSvgDashboardExportSettings = class extends F.y.StiImageDashboardExportSettings {
         constructor() {
-            super(...arguments), this.imageType = Lc.Svg, this.renderEmptyContent = !0
+            super(...arguments), this.imageType = Bc.Svg, this.renderEmptyContent = !0
         }
     }, F.y.StiHtmlDashboardExportSettings = class extends F.y.StiDashboardExportSettings {
         constructor() {
             super(...arguments), this.format = F.f.StiDashboardExportFormat.Html, this.imageQuality = 200, this.scale = 100, this.enableAnimation = !0
         }
     };
-    let Pc = F.y.StiHtmlDashboardExportSettings,
-        jc = F.h.StiTitleMeasureHelper,
-        Hc = F.y.StiSvgDashboardExportSettings,
-        zc = (F.z.StiTitleExportHelper = class {
+    let jc = F.y.StiHtmlDashboardExportSettings,
+        Hc = F.h.StiTitleMeasureHelper,
+        zc = F.y.StiSvgDashboardExportSettings,
+        Gc = (F.z.StiTitleExportHelper = class {
             static async render(e, t, r) {
                 var i, s;
                 let n = e.as(Oe),
                     l = F.p.StiElementControlPainter.getBorderContentRect(new j(0, 0, t.width, t.height), t.border),
                     a = null != n ? n.title : null;
                 if (null == a || !a.visible || B.isNullOrEmpty(a.text)) return l;
-                let o = jc.measureTitle3(null, l, n.title, n.title.text),
+                let o = Hc.measureTitle3(null, l, n.title, n.title.text),
                     u = 1;
                 if (a.sizeMode == Dt.Fit) {
                     let e = o.width > l.width ? l.width / o.width : 1,
                         t = o.height > l.height ? l.height / o.height : 1;
                     u = Math.min(Math.abs(e), Math.abs(t))
                 }
                 let h = N.transparent.equals(a.foreColor) ? J.getTitleForeColor(e) : a.foreColor,
-                    m = r.is(Hc) || r.is(Pc),
+                    m = r.is(zc) || r.is(jc),
                     c = a.backColor == N.transparent ? J.getBackColor(e, null, m) : a.backColor,
                     d = J.getBackColor(e, null, !0),
-                    g = (255 != d.a && c.equals(d) && (c = N.transparent), r.format == F.f.StiDashboardExportFormat.Html && e.is(el) && (l.x += 3, l.y += 3), new Iu),
-                    p = (g.name = e.name + `_Title`, g.allowHtmlTags = !0, g.clientRectangle = new j(l.x, l.y, l.width, o.height), g.text = await O.parseAsync(a.text, e), g.font = yu.changeFontSize(a.font, a.font.size * u), g.horAlignment = this.convert(a.horAlignment), g.trimming = a.sizeMode == Dt.Trimming ? Du.EllipsisCharacter : Du.None, g.wordWrap = a.sizeMode == Dt.WordWrap, g.vertAlignment = Wt.Center, g.textBrush = new v(h), g.brush = new v(c), l.height -= g.height, l.y += g.height, null == (i = a[L.System.StiObject.stimulsoft]().as(It)) ? void 0 : i.padding),
+                    g = (255 != d.a && c.equals(d) && (c = N.transparent), r.format == F.f.StiDashboardExportFormat.Html && e.is(el) && (l.x += 3, l.y += 3), new Du),
+                    p = (g.name = e.name + `_Title`, g.allowHtmlTags = !0, g.clientRectangle = new j(l.x, l.y, l.width, o.height), g.text = await O.parseAsync(a.text, e), g.font = Cu.changeFontSize(a.font, a.font.size * u), g.horAlignment = this.convert(a.horAlignment), g.trimming = a.sizeMode == Dt.Trimming ? Ru.EllipsisCharacter : Ru.None, g.wordWrap = a.sizeMode == Dt.WordWrap, g.vertAlignment = Wt.Center, g.textBrush = new v(h), g.brush = new v(c), l.height -= g.height, l.y += g.height, null == (i = a[L.System.StiObject.stimulsoft]().as(It)) ? void 0 : i.padding),
                     S = (null != p && (l.y += p.top + p.bottom, l.height -= p.top + p.bottom, g.left += p.left, g.width -= p.left + p.right, g.top += p.top), null == (s = e.as(Ze)) ? void 0 : s.cornerRadius);
                 return null != S && (0 < S.topLeft && (g.margins.left = Math.max(g.margins.left, S.topLeft / 2)), 0 < S.topRight) && (g.margins.right = Math.max(g.margins.right, S.topRight / 2)), t.components.add(g), l
             }
             static convert(e) {
                 switch (e) {
                     case z.Left:
                         return X.Left;
@@ -14362,263 +14361,263 @@
                         t = e.left > t ? e.left : t - e.left, r = e.top > r ? e.top : r - e.top, i = e.right > i ? e.right : i - e.right, s = e.bottom > s ? e.bottom : s - e.bottom
                     }
                     return new j(l.x + t, l.y + r, Math.max(1, l.width - t - i), Math.max(1, l.height - r - s))
                 }
                 return l
             }
         }, L.Report.Components.IStiBorder),
-        Gc = (F.z.StiBorderExportHelper = class {
+        Xc = (F.z.StiBorderExportHelper = class {
             static render(e, t, r) {
-                e.is(mt) && t.is(zc) && r.renderBorders && (t.border = e.border2.getBorder(), t.border.topmost = !0)
+                e.is(mt) && t.is(Gc) && r.renderBorders && (t.border = e.border2.getBorder(), t.border.topmost = !0)
             }
         }, F.z.StiBackColorExportHelper = class {
             static render(e, t) {
                 t.is(wt) && (t.backColor = J.getBackColor(e))
             }
         }, L.Report.StiExportFormat),
-        Xc = (F.z.StiExportFormatHelper = class {
+        Wc = (F.z.StiExportFormatHelper = class {
             static convert(e) {
                 switch (e) {
                     case F.f.StiDashboardExportFormat.Pdf:
-                        return Gc.Pdf;
+                        return Xc.Pdf;
                     case F.f.StiDashboardExportFormat.Excel:
-                        return Gc.Excel;
+                        return Xc.Excel;
                     case F.f.StiDashboardExportFormat.Html:
-                        return Gc.Html;
+                        return Xc.Html;
                     case F.f.StiDashboardExportFormat.Data:
-                        return Gc.Data;
+                        return Xc.Data;
                     case F.f.StiDashboardExportFormat.Image:
-                        return Gc.Image;
+                        return Xc.Image;
                     case F.f.StiDashboardExportFormat.Document:
-                        return Gc.Document;
+                        return Xc.Document;
                     default:
                         throw new ca(e)
                 }
             }
         }, L.Report.Dashboard.Export.IStiExcelDashboardExportSettings);
     {
-        class ed extends F.y.StiDashboardExportSettings {
+        class td extends F.y.StiDashboardExportSettings {
             constructor() {
                 super(...arguments), this.format = F.f.StiDashboardExportFormat.Excel, this.imageQuality = 200
             }
             implements() {
-                return ed.ImplementsStiExcelDashboardExportSettings || (ed.ImplementsStiExcelDashboardExportSettings = super.implements().concat([F.y.IStiSizeExportSettings, Xc])), ed.ImplementsStiExcelDashboardExportSettings
+                return td.ImplementsStiExcelDashboardExportSettings || (td.ImplementsStiExcelDashboardExportSettings = super.implements().concat([F.y.IStiSizeExportSettings, Wc])), td.ImplementsStiExcelDashboardExportSettings
             }
             get width() {
                 return this._width
             }
             set width(e) {
-                this._width = e, this.paperSize = Vc.Custom
+                this._width = e, this.paperSize = kc.Custom
             }
             get height() {
                 return this._height
             }
             set height(e) {
-                this._height = e, this.paperSize = Vc.Custom
+                this._height = e, this.paperSize = kc.Custom
             }
             toParameters() {
                 let e = super.toParameters();
                 return e.Width = 0, e.Height = 0, e
             }
         }
-        F.y.StiExcelDashboardExportSettings = ed
+        F.y.StiExcelDashboardExportSettings = td
     }
-    let Wc = L.Report.Dashboard.Export.IStiPdfDashboardExportSettings;
+    let Jc = L.Report.Dashboard.Export.IStiPdfDashboardExportSettings;
     {
-        class td extends F.y.StiDashboardExportSettings {
+        class rd extends F.y.StiDashboardExportSettings {
             constructor() {
                 super(...arguments), this.format = F.f.StiDashboardExportFormat.Pdf, this.imageQuality = 200
             }
             implements() {
-                return td.ImplementsStiPdfDashboardExportSettings || (td.ImplementsStiPdfDashboardExportSettings = super.implements().concat([Wc])), td.ImplementsStiPdfDashboardExportSettings
+                return rd.ImplementsStiPdfDashboardExportSettings || (rd.ImplementsStiPdfDashboardExportSettings = super.implements().concat([Jc])), rd.ImplementsStiPdfDashboardExportSettings
             }
         }
-        F.y.StiPdfDashboardExportSettings = td
+        F.y.StiPdfDashboardExportSettings = rd
     }
-    let Jc = L.Report.Export.StiDataType,
-        Uc = L.Report.Dashboard.Export.IStiDataDashboardExportSettings;
+    let Uc = L.Report.Export.StiDataType,
+        Zc = L.Report.Dashboard.Export.IStiDataDashboardExportSettings;
     {
-        class _c extends F.y.StiDashboardExportSettings {
+        class $c extends F.y.StiDashboardExportSettings {
             implements() {
-                return _c.ImplementsStiDataDashboardExportSettings || (_c.ImplementsStiDataDashboardExportSettings = super.implements().concat([Uc])), _c.ImplementsStiDataDashboardExportSettings
+                return $c.ImplementsStiDataDashboardExportSettings || ($c.ImplementsStiDataDashboardExportSettings = super.implements().concat([Zc])), $c.ImplementsStiDataDashboardExportSettings
             }
             toParameters() {
                 let e = super.toParameters();
-                return e.DataType = L.System.Enum.getName(Jc, this.dataType), e
+                return e.DataType = L.System.Enum.getName(Uc, this.dataType), e
             }
             constructor(e) {
-                super(), this.format = F.f.StiDashboardExportFormat.Data, this.dataType = Jc.Csv, null != e && (this.dataType = e)
+                super(), this.format = F.f.StiDashboardExportFormat.Data, this.dataType = Uc.Csv, null != e && (this.dataType = e)
             }
         }
-        F.y.StiDataDashboardExportSettings = _c
+        F.y.StiDataDashboardExportSettings = $c
     }
-    let Zc = L.Report.Export.StiHtmlChartType,
-        Yc = L.Report.Export.StiHtmlExportSettings,
-        Kc = L.Report.Export.StiDataExportSettings,
-        Qc = L.Report.Export.StiImageExportSettings,
-        qc = L.Report.Export.StiSvgExportSettings,
-        _c = F.y.StiDataDashboardExportSettings,
-        $c = F.y.StiImageDashboardExportSettings,
-        ed = F.y.StiExcelDashboardExportSettings,
-        td = F.y.StiPdfDashboardExportSettings,
-        rd = L.Report.Export.StiDataExportMode,
-        id = L.Report.Export.StiPdfExportSettings,
-        sd = L.Report.Export.StiExcelExportSettings;
+    let Yc = L.Report.Export.StiHtmlChartType,
+        Kc = L.Report.Export.StiHtmlExportSettings,
+        Qc = L.Report.Export.StiDataExportSettings,
+        qc = L.Report.Export.StiImageExportSettings,
+        _c = L.Report.Export.StiSvgExportSettings,
+        $c = F.y.StiDataDashboardExportSettings,
+        ed = F.y.StiImageDashboardExportSettings,
+        td = F.y.StiExcelDashboardExportSettings,
+        rd = F.y.StiPdfDashboardExportSettings,
+        id = L.Report.Export.StiDataExportMode,
+        sd = L.Report.Export.StiPdfExportSettings,
+        nd = L.Report.Export.StiExcelExportSettings;
     F.z.StiExportSettingsHelper = class {
         static getExportSettings(r) {
             switch (r.format) {
                 case F.f.StiDashboardExportFormat.Pdf: {
-                    let e = new id;
+                    let e = new sd;
                     return e.imageQuality = 1, e.imageResolution = r.imageQuality, e
                 }
                 case F.f.StiDashboardExportFormat.Excel: {
-                    let e = new sd;
+                    let e = new nd;
                     return e.imageQuality = 1, e.imageResolution = r.imageQuality, e
                 }
                 case F.f.StiDashboardExportFormat.Data: {
-                    let e = new Kc;
-                    return e.dataType = r.dataType, e.dataExportMode = rd.DataAndHeadersFooters, e.skipColumnHeaders = !0, e
+                    let e = new Qc;
+                    return e.dataType = r.dataType, e.dataExportMode = id.DataAndHeadersFooters, e.skipColumnHeaders = !0, e
                 }
                 case F.f.StiDashboardExportFormat.Image: {
                     let t = r.imageType;
                     switch (t) {
-                        case Lc.Svg:
-                            return new qc;
+                        case Bc.Svg:
+                            return new _c;
                         default: {
-                            let e = new Qc;
+                            let e = new qc;
                             return e.imageType = t, e.imageZoom = r.scale / 100, e.imageResolution = 100, e
                         }
                     }
                 }
                 case F.f.StiDashboardExportFormat.Html: {
-                    let e = new Yc;
-                    return e.imageResolution = r.imageQuality, e.useEmbeddedImages = !0, e.zoom = r.scale / 100, e.addPageBreaks = !1, e.chartType = r.enableAnimation ? Zc.AnimatedVector : Zc.Vector, e
+                    let e = new Kc;
+                    return e.imageResolution = r.imageQuality, e.useEmbeddedImages = !0, e.zoom = r.scale / 100, e.addPageBreaks = !1, e.chartType = r.enableAnimation ? Yc.AnimatedVector : Yc.Vector, e
                 }
                 case F.f.StiDashboardExportFormat.Document:
                     return null;
                 default:
                     throw new ca(r.format)
             }
         }
         static getDashboardExportSettings(e) {
             return this.getDashboardExportSettings2(e.getExportFormat())
         }
         static getDashboardExportSettings2(e) {
             switch (e) {
-                case Gc.Pdf:
+                case Xc.Pdf:
+                    return new rd;
+                case Xc.Excel:
                     return new td;
-                case Gc.Excel:
-                    return new ed;
-                case Gc.Data:
-                    return new _c;
-                case Gc.Csv:
-                    return new _c(Jc.Csv);
-                case Gc.Dbf:
-                    return new _c(Jc.Dbf);
-                case Gc.Xml:
-                    return new _c(Jc.Xml);
-                case Gc.Json:
-                    return new _c(Jc.Json);
-                case Gc.Dif:
-                    return new _c(Jc.Dif);
-                case Gc.Sylk:
-                    return new _c(Jc.Sylk);
-                case Gc.Image:
+                case Xc.Data:
                     return new $c;
-                case Gc.ImageBmp:
-                    return new $c(Lc.Bmp);
-                case Gc.ImageGif:
-                    return new $c(Lc.Gif);
-                case Gc.ImagePng:
-                    return new $c(Lc.Png);
-                case Gc.ImageTiff:
-                    return new $c(Lc.Tiff);
-                case Gc.ImageJpeg:
-                    return new $c(Lc.Jpeg);
-                case Gc.ImageEmf:
-                    return new $c(Lc.Emf);
-                case Gc.ImagePcx:
-                    return new $c(Lc.Pcx);
-                case Gc.ImageSvgz:
-                    return new $c(Lc.Svgz);
-                case Gc.ImageSvg:
-                    return new Hc;
-                case Gc.Html:
-                    return new Pc;
-                case Gc.Document:
+                case Xc.Csv:
+                    return new $c(Uc.Csv);
+                case Xc.Dbf:
+                    return new $c(Uc.Dbf);
+                case Xc.Xml:
+                    return new $c(Uc.Xml);
+                case Xc.Json:
+                    return new $c(Uc.Json);
+                case Xc.Dif:
+                    return new $c(Uc.Dif);
+                case Xc.Sylk:
+                    return new $c(Uc.Sylk);
+                case Xc.Image:
+                    return new ed;
+                case Xc.ImageBmp:
+                    return new ed(Bc.Bmp);
+                case Xc.ImageGif:
+                    return new ed(Bc.Gif);
+                case Xc.ImagePng:
+                    return new ed(Bc.Png);
+                case Xc.ImageTiff:
+                    return new ed(Bc.Tiff);
+                case Xc.ImageJpeg:
+                    return new ed(Bc.Jpeg);
+                case Xc.ImageEmf:
+                    return new ed(Bc.Emf);
+                case Xc.ImagePcx:
+                    return new ed(Bc.Pcx);
+                case Xc.ImageSvgz:
+                    return new ed(Bc.Svgz);
+                case Xc.ImageSvg:
+                    return new zc;
+                case Xc.Html:
+                    return new jc;
+                case Xc.Document:
                     return null;
                 default:
                     throw new ca(e)
             }
         }
         static isDataExport(e) {
-            return e.is(_c) || e.is(ed) && e.exportDataOnly
+            return e.is($c) || e.is(td) && e.exportDataOnly
         }
     };
     {
-        class gd {
+        class pd {
             async render(e, t, r, i) {}
             static getTool(e) {
                 let t = this.typeToTool.get(e);
                 if (null != t) return t;
                 let r = dt.attributes.get(e[L.System.StiObject.stimulsoft]().getTypeName()),
                     i = null != r ? r.exportToolTypeName : null;
                 if (null == i) return null;
                 return t = Dr.createObject2(i), this.typeToTool.set(e, t), t
             }
         }
-        gd.typeToTool = new Co, F.A.StiExportTool = gd
+        pd.typeToTool = new xo, F.A.StiExportTool = pd
     }
-    let nd = L.System.Xml.XmlTextWriter,
-        ld = L.Report.Components.StiImage;
+    let ld = L.System.Xml.XmlTextWriter,
+        ad = L.Report.Components.StiImage;
     {
-        class dd extends F.A.StiExportTool {
+        class gd extends F.A.StiExportTool {
             async render(e, t, r, i) {
                 if (this.renderEmptyDataMessage(e, t, r.clone(), i)) return;
                 await this.renderContent(e, t, r.clone())
             }
             async renderContent(e, t, r) {
-                let i = new ld(r),
+                let i = new ad(r),
                     s = (i.name = e.name + `_Content`, i.stretch = !0, i.aspectRatio = !1, await this.draw(e, r));
                 i.imageToDraw = s, t.components.add(i)
             }
             async drawElement(t, e) {
-                let r = new Na,
-                    i = new nd(ul.UTF8),
-                    s = new oh;
+                let r = new La,
+                    i = new ld(ul.UTF8),
+                    s = new uh;
                 if (s.x = 0, s.y = 0, s.width = e.width, s.height = e.height, s.component = t.as(bt), t.is(wt)) {
                     let e = J.getBackColor(t);
-                    e.a < 255 && (e = N.white), i.writeStartElement("rect"), i.writeAttributeString("x", "0"), i.writeAttributeString("y", "0"), i.writeAttributeString("height", s.height.toString()[L.System.StiObject.stimulsoft]().replaceAll(",", ".")), i.writeAttributeString("width", s.width.toString()[L.System.StiObject.stimulsoft]().replaceAll(",", ".")), i.writeAttributeString("style", rh.writeFillBrush(i, e, new Ve(0, 0, s.width, s.height))), i.writeEndElement()
+                    e.a < 255 && (e = N.white), i.writeStartElement("rect"), i.writeAttributeString("x", "0"), i.writeAttributeString("y", "0"), i.writeAttributeString("height", s.height.toString()[L.System.StiObject.stimulsoft]().replaceAll(",", ".")), i.writeAttributeString("width", s.width.toString()[L.System.StiObject.stimulsoft]().replaceAll(",", ".")), i.writeAttributeString("style", ih.writeFillBrush(i, e, new Ve(0, 0, s.width, s.height))), i.writeEndElement()
                 }
-                if (t.is(Cm)) {
+                if (t.is(xm)) {
                     let e = L.Report.Dashboards.StiDashboardHelperCreator.createProgressVisualSvgHelper();
                     null != e && await e.writeProgress(i, s)
-                } else if (t.is(bh)) {
+                } else if (t.is(fh)) {
                     let e = L.Report.Dashboards.StiDashboardHelperCreator.createIndicatorVisualSvgHelper();
                     null != e && await e.writeIndicator(i, s)
-                } else if (t.is(ym)) {
+                } else if (t.is(Cm)) {
                     let e = L.Report.Dashboards.StiDashboardHelperCreator.createCardsVisualSvgHelper();
                     null != e && await e.writeCards(i, s)
-                } else if (t.is(Fm)) {
+                } else if (t.is(vm)) {
                     let e = L.Report.Dashboards.StiDashboardHelperCreator.createGaugeVisualSvgHelper();
                     null != e && await e.writeGauge(i, s, !1)
                 }
                 let n = L.Report.Resources.StimulsoftFont.getBase64Content(),
                     l = "<style>@font-face {font-family: 'Stimulsoft';src: url(data:font/ttf;base64," + n + ") format('truetype');font-weight: normal;font-style: normal;}</style>",
                     a = B.format('<svg xmlns="http://www.w3.org/2000/svg" width="{0}" height="{1}"><defs>{3}</defs><rect x="0" y="0" width="{0}" height="{1}" style="fill: white;"/>{2}</svg>', s.width.toString(), s.height.toString(), i.textWriter.getStringBuilder().toString(), l);
                 return r.svg = a, await r.convertAsync(L.System.Drawing.Imaging.ImageFormat.Jpeg), r
             }
             async draw(t, e) {
-                if (t.is(Tm)) {
+                if (t.is(Fm)) {
                     let e = await t.imageToDraw;
                     return null != e && (e.url = t.imageHyperlink), e
                 }
                 let r = new j(0, 0, Math.trunc(e.width), Math.trunc(e.height));
-                if (t.is(bh) || t.is(Cm) || t.is(Fm) || t.is(ym)) return this.drawElement(t, r);
-                let i = new Na;
+                if (t.is(fh) || t.is(xm) || t.is(vm) || t.is(Cm)) return this.drawElement(t, r);
+                let i = new La;
                 try {
                     if (t.is(wt)) {
                         let e = J.getBackColor(t);
                         e.a < 255 && (e = N.white)
                     }
                     await this.paintContent(null, r, t)
                 } catch (e) {}
@@ -14627,41 +14626,41 @@
             async paintContent(e, t, r) {
                 try {
                     await this.paintAtom(e, t.clone(), r)
                 } catch (e) {} finally {}
             }
             async paintAtom(e, t, r) {
                 let i = null;
-                if (r.isQuerable && null == (i = await dd.getDataTable(r))) return
+                if (r.isQuerable && null == (i = await gd.getDataTable(r))) return
             }
             static async getDataTable(e) {
                 var t;
-                let r = null == (t = e.as(th)) ? void 0 : t.getManuallyEnteredDataTable();
+                let r = null == (t = e.as(rh)) ? void 0 : t.getManuallyEnteredDataTable();
                 if (null != r) return r;
                 return bl.tryToGetOrCreate(e)
             }
             renderEmptyDataMessage(t, r, i, e) {
                 var s;
-                if (!e.is(Hc) || e.renderEmptyContent) return !1;
-                if (t.is(Wo) && t.dataFrom == Xo.Manual) return !1;
-                if (t.is(ja) && (null != t.image || null != t.icon || !B.isNullOrEmpty(t.imageHyperlink))) return !1;
-                if (t.is(fu) && (!B.isNullOrEmpty(t.url) || !B.isNullOrEmpty(t.embedCode))) return !1;
-                if (0 < t.getMeters().length || (null == (s = t.as(th)) ? void 0 : s.dataMode) == Vn.ManuallyEnteringData) return !1;
+                if (!e.is(zc) || e.renderEmptyContent) return !1;
+                if (t.is(Jo) && t.dataFrom == Wo.Manual) return !1;
+                if (t.is(Ha) && (null != t.image || null != t.icon || !B.isNullOrEmpty(t.imageHyperlink))) return !1;
+                if (t.is(yu) && (!B.isNullOrEmpty(t.url) || !B.isNullOrEmpty(t.embedCode))) return !1;
+                if (0 < t.getMeters().length || (null == (s = t.as(rh)) ? void 0 : s.dataMode) == Vn.ManuallyEnteringData) return !1;
                 let n = i.size,
                     l = new H("Arial", 9),
-                    a = t.is(fu) ? b.get("FormStyleDesigner", "NotSpecified") : t.is(ja) ? b.get("Dashboard", "ImageNotSpecified") : b.get("Dashboard", "DragDropDataFromDictionary"),
-                    o = ah.measureString(a, l);
+                    a = t.is(yu) ? b.get("FormStyleDesigner", "NotSpecified") : t.is(Ha) ? b.get("Dashboard", "ImageNotSpecified") : b.get("Dashboard", "DragDropDataFromDictionary"),
+                    o = oh.measureString(a, l);
                 if (i.y += i.height / 2 - 48, i.height = Math.min(32, i.height), 48 <= n.width && 64 <= n.height) {
                     i.y += n.width > o.width + 16 ? 16 : 32;
-                    let e = new ld(new j(i.width / 2 - 16, i.y, 32, 32));
+                    let e = new ad(new j(i.width / 2 - 16, i.y, 32, 32));
                     e.name = t.name + `_EmptyImage`, e.horAlignment = z.Center, e.image = L.Base.Drawing.StiImageConverter.stringToImage(this.getEmptyDataImage(t)), r.components.add(e)
                 }
                 if (n.width > o.width + 16 && 32 <= n.height) {
                     i.y += 32;
-                    let e = new Iu(i);
+                    let e = new Du(i);
                     e.name = t.name + `_EmptyText`, e.horAlignment = X.Center, e.vertAlignment = Wt.Center, e.font = l, e.text = a, e.textBrush = new v(N.darkGray), r.components.add(e)
                 }
                 return !0
             }
             format(e, t) {
                 var r, i;
                 if (null != t && null != e) {
@@ -14680,42 +14679,42 @@
                 if (e.is(L.Report.Dashboard.IStiListBoxElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA3ZpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNi1jMTM4IDc5LjE1OTgyNCwgMjAxNi8wOS8xNC0wMTowOTowMSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDowMDEzNGViZC0wY2ZmLTczNDMtOWIwMi1jNTkzNzdiMWRiMjIiIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6NTA5MTJDN0Q4NTYwMTFFOEI3N0JBNjlFRDdGQ0IwOEIiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6NTA5MTJDN0M4NTYwMTFFOEI3N0JBNjlFRDdGQ0IwOEIiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6MDAxMzRlYmQtMGNmZi03MzQzLTliMDItYzU5Mzc3YjFkYjIyIiBzdFJlZjpkb2N1bWVudElEPSJ4bXAuZGlkOjAwMTM0ZWJkLTBjZmYtNzM0My05YjAyLWM1OTM3N2IxZGIyMiIvPiA8L3JkZjpEZXNjcmlwdGlvbj4gPC9yZGY6UkRGPiA8L3g6eG1wbWV0YT4gPD94cGFja2V0IGVuZD0iciI/PsGuI54AAACuSURBVHja7FeJCcAgDNTiEI7h/kvoGG5hm4JQQm2jGAOSgyKKyR3m0dpSipHEYYShAlxKSVbA9clmYYyxzMCIH7DRJHR4oScpQwi/e3LO9+i9pwmgOKUCyKuAlgi2EGByPGcPwRsZrOFTYAsB1c9eVTDS1qeGoNcWBO/biFp+sA1bFUC54VJc2oiA7EmI50vuAixg+V3wRayP0goLzyLpPmBFT0B/zVSAtIBTgAEAMM3EXL6e7tsAAAAASUVORK5CYII=";
                 if (e.is(L.Report.Dashboard.IStiPivotTableElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA25pVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNi1jMTM4IDc5LjE1OTgyNCwgMjAxNi8wOS8xNC0wMTowOTowMSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo4M2I5YzlhNS1lZGRmLTU0NGItODFmMi1mMzVmMDgyNTUzMTciIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6OTE1MUMzNDA5RkFDMTFFN0JERThGRDhBNTZGM0ZDN0YiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6OTE1MUMzM0Y5RkFDMTFFN0JERThGRDhBNTZGM0ZDN0YiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6OTIzODI0M0I3MzI1MTFFN0E4QTI5RjYzRTdGNDREM0MiIHN0UmVmOmRvY3VtZW50SUQ9InhtcC5kaWQ6OTIzODI0M0M3MzI1MTFFN0E4QTI5RjYzRTdGNDREM0MiLz4gPC9yZGY6RGVzY3JpcHRpb24+IDwvcmRmOlJERj4gPC94OnhtcG1ldGE+IDw/eHBhY2tldCBlbmQ9InIiPz7WOnt0AAABPUlEQVR42uxXSW6EMBBsQxASJ8R2YPkD/38FT0BCgMRygSMCZsrKJCQZlGHAQJTpk90culyuajdsHEc6MiQ6ON6mmyiKdqMjDEP2A8D7B+HFrwc96RXMoZyycy+/gPbzifAF4LwinLPj1jZd7IKXBpZEnueUZdlzV7A20jSlsiz5ehgG8n1/PwBJklBd16QoCt9XVUV49oMg2OcKUNyyLDIMg7qu42vkdtOA4zhfKMcaud0AuK77UE64C0C/LMtiXXATHCienhLKb9uWNE0T1wdgtZvgpsX7vqc4jjkDpmmKYQBNBj6H1SRJ+mg4KNo0DQcBF+i6LgbAdJwviuKT0isYVVU5K7+dfhUAUA4QYMG2bfI8b9vX8JFAUYgNIBhjs1bbdB74Hmiv91rs352I1ozdzwT79z+nhwO4CDAAvLyCJQ9KIGkAAAAASUVORK5CYII=";
                 if (e.is(L.Report.Dashboard.IStiProgressElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA4RpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNi1jMTM4IDc5LjE1OTgyNCwgMjAxNi8wOS8xNC0wMTowOTowMSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo4M2I5YzlhNS1lZGRmLTU0NGItODFmMi1mMzVmMDgyNTUzMTciIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6MTI4QjI4RjdCRjUxMTFFNzk4RThFMTk3MzM2QTVEREYiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6MTI4QjI4RjZCRjUxMTFFNzk4RThFMTk3MzM2QTVEREYiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6ZTI4MmVmYWItOTQwYy1mYjQwLTg5OTctNzNiNzU1Nzk1ZmY1IiBzdFJlZjpkb2N1bWVudElEPSJhZG9iZTpkb2NpZDpwaG90b3Nob3A6MmUxNzdhMzEtOWZlZS0xMWU3LWIxNzMtZTY1ODBhMDllOGE4Ii8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+xEa5MgAAAoxJREFUeNrEV7lOA0EMJeESFXcQLeIoiZBoEKIjKZEoIL/AFUJHR0FDRxDXJxAoEC1Ji0SBQKHjEh/ATRkQCs+SNzhmsrvZbMDS02jHM7bX4xnbgXw+X/OfVOd2YTabrccQBcaBYaAnHA63YJ7Yb8A9cAZkgGPwPt3IDTh5AApaMCSAWaBT8qCkhg3Q9ARsA0msebOTH3RQHsNwBaxo5Q7UwXuuWEZ5R4BNtRg2gZkKj7gL2IO8MYwL8MaXowdY+UEJ5TfAKjAKdANNjG6eW+U1mkjWAcu2jwEsoj+fNwhZ5jPNORxbI8fMmoG9jf3zJQ3A5mkMKbXphAzCxstyfA9Zgxi22DOSYpC1/8sAjvZrICQWnwIT2PDoJQAgkwL3CBgR0w/AgHU7ZAwklHKiWa/K+ZrS3jk1HWJdP0EISxv4nhedOQRkK33pWMay/jHWWfBARN1ziuSkjy9uUt2OTtZZZICklFO0l+mFnCG4o9KAIcXMVCHvpNX3kDSg3/Dg+E236ruv8BTDRc2K+V4FA7TM5oIBpoxGme4vKGhnnc9k9HLQ7nx8pj5TTFgGnCtmpAoGaJkX0gB9RWKc1XwhlhUzXUtpwLNg9sv32gdKqKtOOeK4YAAi/oNTp6Q1WB724e8HDbXBDussyoZJTpVFBQSnVK/Kae+Omn6UeSYo7j3l57haTHn8kP/Cy58fqlqAKC4rZVNJtmXI4VZJtm65zkYxpdklTyWZKkonDQKumUcBdAe88Hwb0MtXjcq6AcNe8saUroyNjYmPZblFu6XKctvOiJuKDUOp5pYoqBehOFVpa7bEcdHuUvEzt2brTq1ZwG13LJrTiNWcAq3MfhXNKT1qaadgLduAatG3AAMAxAf6UcvGQQYAAAAASUVORK5CYII=";
                 if (e.is(L.Report.Dashboard.IStiTreeViewElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA4RpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNi1jMTM4IDc5LjE1OTgyNCwgMjAxNi8wOS8xNC0wMTowOTowMSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDpiNGFhYjFiMC1lZTZlLTJkNDctYWZlMi1lYmQzYmI3MzJkNWQiIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6NUE2RkJGN0VBNjVFMTFFODk5OTVCRERFOTIwOEI5N0UiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6NUE2RkJGN0RBNjVFMTFFODk5OTVCRERFOTIwOEI5N0UiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6MTI3NTcwYzItM2MyZS05NDQxLTgzZjctYmYwM2ZkODU5YjRjIiBzdFJlZjpkb2N1bWVudElEPSJhZG9iZTpkb2NpZDpwaG90b3Nob3A6ZTkyYWNjNTItYTY0OS0xMWU4LWJmZGYtYWIxMTU1OWY5YTkwIi8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+WYlYxgAAAMBJREFUeNrsllEKwCAMQ9fhgbz/KbyRQ7Agm0pLbWRgQJhfi68xSDnna6dCu0kpfdzEGAlmoP6wNYQlIFGPUhVBDLxHYqUUOifcF0I+XcHsHT7WLcEMNzAJGuYWdILm1g9iAqUfeMEJCKUdG63OACmXjoBXP4QRgdaE57U8PXB6ANEDhMrA9L6bCXj1gIhAMcSm2u8VIuuz3EpGlQGPfjARGBgiKAFrP6h6wOOdgMjA9F3wrwwMRqJqvuU9YNUjwABgJX86W1bOxQAAAABJRU5ErkJggg==";
                 return null
             }
         }
-        F.A.StiElementExportTool = dd
+        F.A.StiElementExportTool = gd
     }
     let S = F.i.StiChartElementBuilder,
-        ad = (F.A.StiChartElementExportTool = class extends F.A.StiElementExportTool {
+        od = (F.A.StiChartElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, r, i, s) {
                 if (this.renderEmptyDataMessage(e, t, r.clone(), i)) return;
-                let n = e.as(vm),
+                let n = e.as(Am),
                     l = null,
                     a = (0 < n.chartValuesList().length && (l = await F.A.StiElementExportTool.getDataTable(n)), await S.create(n).render(n, l));
                 for (let e = 0; e < a.series.count; e++) {
                     if (null == s || e >= s.length) break;
                     a.series.getByIndex(e).valuesStart = s[e]
                 }
                 a.name = e.name + `_Content`, a.clientRectangle = r.clone(), t.components.add(a)
             }
         }, F.h.StiGaugeVisualSvgHelper),
-        od = (F.A.StiGaugeElementExportTool = class extends F.A.StiElementExportTool {
+        ud = (F.A.StiGaugeElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, l, t, r) {
                 if (this.renderEmptyDataMessage(e, l, t.clone(), r)) return;
-                let a = e.as(Fm),
+                let a = e.as(vm),
                     o = await F.A.StiElementExportTool.getDataTable(e),
                     u = (new Aa).render2(a, t.size, o);
-                if (1 != (await u()).count2() || r.is(ed) || r.is(td)) {
+                if (1 != (await u()).count2() || r.is(td) || r.is(rd)) {
                     if (0 < (await u()).count2())
                         if (r.isDesignMode || r.format != F.f.StiDashboardExportFormat.Html) await this.renderContent(e, l, t.clone());
                         else {
                             let i = 0,
-                                s = Dc.getLocationRectangles(t, (await u()).count2(), a),
+                                s = Rc.getLocationRectangles(t, (await u()).count2(), a),
                                 n = s[0].clone();
                             for (let r of await (u = (new Aa).render2(a, n.size, o))()) {
                                 let e = s[i].clone(),
                                     t = {
                                         ref: 0
                                     };
                                 B.isNullOrEmpty(r.series) || (await this.renderSingleGaugeTitleFromIteration(a, l, r, e, n, u, i, t), e.height -= t.ref, e.y += t.ref), this.renderSingleGaugeFromIteration(a, l, r, e, i), i++
@@ -14725,44 +14724,44 @@
             }
             renderSingleGaugeFromIteration(e, t, r, i, s = 0) {
                 let n = r.gauge;
                 n.name = e.name + `_Content` + s, n.clientRectangle = i, n.style = J.getGaugeStyle(e), n.customStyleName = e.customStyleName, n.brush = new v(J.getBackColor(e, null, !0)), t.components.add(n)
             }
             async renderSingleGaugeTitleFromIteration(l, a, e, o, t, r, u, h) {
                 let m = e.series,
-                    i = await ad.getTitleHeight(null, r, o, l, null),
-                    c = await ad.getTitleMinFontSize(null, r, l.font, t.width, t.height);
+                    i = await od.getTitleHeight(null, r, o, l, null),
+                    c = await od.getTitleMinFontSize(null, r, l.font, t.width, t.height);
                 if (h.ref = i || 0, null != i) {
                     let e = new j(o.x, o.y, o.width, h.ref),
-                        t = yu.changeFontSize(l.font, c),
-                        r = jc.measureTitle4(null, e, l.font, m),
+                        t = Cu.changeFontSize(l.font, c),
+                        r = Hc.measureTitle4(null, e, l.font, m),
                         i = (e.height = r.height, jl.getForeColor(l, l.foreColor)),
                         s = N.transparent.equals(i) ? J.getForeColor(l) : i,
-                        n = new Iu(e);
+                        n = new Du(e);
                     n.name = l.name + `_ContentTitle` + u, n.brush = new v(N.transparent), n.text = m, n.font = t, n.textBrush = new v(s), n.horAlignment = X.Center, a.components.add(n)
                 }
             }
         }, F.A.StiImageElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, r, i) {
                 if (this.renderEmptyDataMessage(e, t, r.clone(), i)) return;
                 await this.renderContent(e, t, r.clone())
             }
             async renderContent(e, t, l) {
-                let a = e.as(Tm),
+                let a = e.as(Fm),
                     o = await this.draw(a, l.clone());
                 if (a.aspectRatio && null != o) {
                     let e = l.width / o.width,
                         t = l.height / o.height,
                         r = (e = t = e < t ? e : t, o.width * (e = t)),
                         i = o.height * t,
                         s = this.calculateHorAlignmentPosition(a, l, r),
                         n = this.calculateVertAlignmentPosition(a, l, i);
                     l = new j(s, n, r, i)
                 }
-                let r = new ld(l);
+                let r = new ad(l);
                 r.name = a.name + `_Content`, r.stretch = !0, r.aspectRatio = !1, r.imageToDraw = o, t.components.add(r)
             }
             calculateHorAlignmentPosition(e, t, r) {
                 switch (e.horAlignment) {
                     case z.Left:
                         return t.x;
                     case z.Right:
@@ -14778,81 +14777,81 @@
                     case Wt.Bottom:
                         return t.bottom - r;
                     default:
                         return t.y + (t.height - r) / 2
                 }
             }
         }, F.A.StiImageElementExportTool),
-        ud = F.A.StiGaugeElementExportTool,
-        hd = F.A.StiChartElementExportTool,
-        md = F.z.StiExportSettingsHelper,
-        cd = F.z.StiExportFormatHelper,
-        dd = F.A.StiElementExportTool,
-        gd = F.A.StiExportTool,
-        pd = F.z.StiTitleExportHelper,
-        Sd = F.z.StiBackColorExportHelper,
-        wd = F.z.StiBorderExportHelper,
-        bd = F.z.StiLayoutExportHelper,
-        fd = L.Base.IStiReport,
-        yd = F.y.StiDashboardExportSettings;
+        hd = F.A.StiGaugeElementExportTool,
+        md = F.A.StiChartElementExportTool,
+        cd = F.z.StiExportSettingsHelper,
+        dd = F.z.StiExportFormatHelper,
+        gd = F.A.StiElementExportTool,
+        pd = F.A.StiExportTool,
+        Sd = F.z.StiTitleExportHelper,
+        wd = F.z.StiBackColorExportHelper,
+        bd = F.z.StiBorderExportHelper,
+        fd = F.z.StiLayoutExportHelper,
+        yd = L.Base.IStiReport,
+        Cd = F.y.StiDashboardExportSettings;
     {
-        class np {
+        class lp {
             static exportAsync(t, r, i) {
                 setTimeout(async function() {
-                    let e = await np.export(r, i);
+                    let e = await lp.export(r, i);
                     t(e)
                 })
             }
             static
             export (e, t) {
                 let r;
-                return r = t instanceof yd ? t : t instanceof Nc ? F.z.StiExportSettingsHelper.getDashboardExportSettings(t) : F.z.StiExportSettingsHelper.getDashboardExportSettings2(t), this.exportToStream(e, r)
+                return r = t instanceof Cd ? t : t instanceof Lc ? F.z.StiExportSettingsHelper.getDashboardExportSettings(t) : F.z.StiExportSettingsHelper.getDashboardExportSettings2(t), this.exportToStream(e, r)
             }
             static async exportToStream(e, r) {
                 var t;
-                let s = new qh,
-                    i = (s.isDocument = !0, s.reportUnit = Qh.HundredthsOfInch, L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !0, s.renderedPages.getByIndex(0)),
-                    n = (i.orientation = r.orientation, i.paperSize = r.paperSize, (r.is(ed) || r.is(_c) || r.is($c)) && (i.margins = new be(0)), r),
+                let s = new _h,
+                    i = (s.isDocument = !0, s.reportUnit = qh.HundredthsOfInch, L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !0, s.renderedPages.getByIndex(0)),
+                    n = (i.orientation = r.orientation, i.paperSize = r.paperSize, (r.is(td) || r.is($c) || r.is(ed)) && (i.margins = new be(0)), r),
                     l = ("width" in r && null != n && 0 < n.width && 0 < n.height && (i.width = n.width, i.height = n.height), null == (t = e.as(ue)) ? void 0 : t.dashboardWatermark);
-                if (i.tagValue = l, null == i.tagValue && (i.tagValue = "*Dashboards*"), e.is(fd)) {
+                if (i.tagValue = l, null == i.tagValue && (i.tagValue = "*Dashboards*"), e.is(yd)) {
                     let t = e.fetchPages().where(e => e.is(Ae)).cast();
                     for (let e = 0; e < t.length; e++) 0 < e && (i = i.clone(!0, !1), s.renderedPages.add(i)), await this.renderDashboardAsync(i, t[e], r)
-                } else e.is(Ae) ? (e.report && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderDashboardAsync(i, e, r)) : e.is(Fe) && (s.reportAlias = e.name, e.is(Wo) && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderSingleElementAsync(i, e, r));
+                } else e.is(Ae) ? (e.report && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderDashboardAsync(i, e, r)) : e.is(Fe) && (s.reportAlias = e.name, e.is(Jo) && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderSingleElementAsync(i, e, r));
                 for (let i of s.renderedPages.list) i.components.toList().where(e => e.is(re)).cast().forEach(e => {
                     let t = i.components.indexOf(e) + 1,
                         r = e.getComponentsList();
                     for (let e = 0; e < r.length; e++) r[e].page = i, r[e].setDirectDisplayRectangle(r[e].componentToPage(r[e].displayRectangle)), i.components.insert(t + e, r[e]);
                     e.components.clear()
                 });
-                let a, o = null == r ? Gc.Document : cd.convert(r.format);
-                if (o == Gc.Document) a = L.System.Text.Encoding.UTF8.getBytes(s.saveDocumentToJsonString());
+                let a, o = null == r ? Xc.Document : dd.convert(r.format);
+                if (o == Xc.Document) a = L.System.Text.Encoding.UTF8.getBytes(s.saveDocumentToJsonString());
                 else {
-                    let e = md.getExportSettings(r),
+                    let e = cd.getExportSettings(r),
                         t = await s.exportDocumentAsync2(o, null, e);
                     a = "string" == typeof t ? L.System.Text.Encoding.UTF8.getBytes(t) : "undefined" != typeof Buffer && Buffer.isBuffer(t) ? t.toJSON().data : t
                 }
                 return L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !1, a
             }
             static async renderDashboardAsync(e, t, r) {
                 if (null == t) return;
                 null != r && (r.renderSinglePage = !0, r.renderSingleElement = !1);
-                let i = t.as(Im),
+                let i = t.as(Dm),
                     s = await i.getElements(!1).whereAsync(async e => e.isEnabledAsync()),
                     n = e.width / i.width,
                     l = e.height / i.height;
                 r.renderSingleElement = !1, e.brush = new v(J.getDashboardBackColor(t, !1)), await this.renderElementsAsync(e, s, n, l, r)
             }
             static async renderSingleElementAsync(e, t, r) {
                 if (null == t || !await t.isEnabledAsync()) return;
                 r.renderSingleElement = !0, e.brush = new v(J.getBackColor(t));
                 let i = t.as(bt),
                     s = e.width / i.width,
                     n = e.height / i.height,
                     l = await this.renderElementAsync(e, t, s, n, r),
-                    a = md.isDataExport(r),
+                    a = cd.isDataExport(r),
                     o = t.margin;
                 l.left = a ? 0 : o.left, l.top = a ? 0 : o.top
             }
             static async renderElementsAsync(i, t, s, n, l) {
                 l.renderSingleElement = !1;
                 for (let e of t) {
                     let t = await this.renderElementAsync(i, e, s, n, l),
@@ -14864,43 +14863,43 @@
                 }
             }
             static async renderElementAsync(e, t, r, i, s, n, l = {
                 ref: new L.System.Drawing.Rectangle
             }, a = new P) {
                 var o;
                 let u = t.as(bt),
-                    h = md.isDataExport(s),
+                    h = cd.isDataExport(s),
                     m = Math.round(u.left * r),
                     c = Math.round(u.top * i),
                     d = Math.round(u.right * r),
                     g = Math.round(u.bottom * i),
                     p = new j(m, c, d - m, g - c);
-                if (h || (p = bd.excludeMargin(t, p)), u.parent.is(St)) {
+                if (h || (p = fd.excludeMargin(t, p)), u.parent.is(St)) {
                     let e = u.parent;
                     p.x -= e.margin.left, p.y -= e.margin.top
                 }
                 let S = new ct(p),
-                    w = (S.name = t.name, h || (S.brush = new v(J.getBackColor(t, null, s.is(Hc) || s.is(Pc))), S.cornerRadius = null == (o = t.as(Ze)) ? void 0 : o.cornerRadius), e.components.add(S), null != S.report && null != t.report && (S.report.styles.clear(), S.report.styles.addRange(t.report.styles)), p = await pd.render(t, S, s), h || (wd.render(t, S, s), Sd.render(t, S), p = bd.excludePadding(t, p), p = bd.excludeCornerRadius(t, p), l.ref = p), gd.getTool(Le.getType(t)));
-                return (w = null == w ? new dd : w)[L.System.StiObject.stimulsoft]().is(hd) && s.is(Pc) ? (t.previousAnimations = a, await w.render(t, S, p.clone(), s, n)) : w[L.System.StiObject.stimulsoft]().is(ud) && s.is(Pc) ? (t.previousAnimations = a, await w.render(t, S, p.clone(), s)) : !w[L.System.StiObject.stimulsoft]().is(od) && null != s && 1 == s.isDesignMode && t[L.System.StiObject.stimulsoft]().is(So) || await w.render(t, S, p.clone(), s), S
+                    w = (S.name = t.name, h || (S.brush = new v(J.getBackColor(t, null, s.is(zc) || s.is(jc))), S.cornerRadius = null == (o = t.as(Ze)) ? void 0 : o.cornerRadius), e.components.add(S), null != S.report && null != t.report && (S.report.styles.clear(), S.report.styles.addRange(t.report.styles)), p = await Sd.render(t, S, s), h || (bd.render(t, S, s), wd.render(t, S), p = fd.excludePadding(t, p), p = fd.excludeCornerRadius(t, p), l.ref = p), pd.getTool(Le.getType(t)));
+                return (w = null == w ? new gd : w)[L.System.StiObject.stimulsoft]().is(md) && s.is(jc) ? (t.previousAnimations = a, await w.render(t, S, p.clone(), s, n)) : w[L.System.StiObject.stimulsoft]().is(hd) && s.is(jc) ? (t.previousAnimations = a, await w.render(t, S, p.clone(), s)) : !w[L.System.StiObject.stimulsoft]().is(ud) && null != s && 1 == s.isDesignMode && t[L.System.StiObject.stimulsoft]().is(wo) || await w.render(t, S, p.clone(), s), S
             }
         }
-        F.f.StiDashboardExportTools = np
+        F.f.StiDashboardExportTools = lp
     }
-    let Cd = L.Report.Dashboard.Helpers.StiBorderElementHelper,
-        xd = (F.p.StiElementControlPainter = class {
+    let xd = L.Report.Dashboard.Helpers.StiBorderElementHelper,
+        Md = (F.p.StiElementControlPainter = class {
             static getBorderContentRect(e, t) {
-                return Cd.getBorderContentRect3(e.clone(), t, Io.factor, !1)
+                return xd.getBorderContentRect3(e.clone(), t, Do.factor, !1)
             }
         }, F.p.StiLocHelper = class {
             static get locAll() {
                 return `(${b.get("Report","RangeAll")[L.System.StiObject.stimulsoft]().replaceAll("& ","")})`
             }
         }, L.System.Drawing.StringFormat),
-        Md = L.System.Drawing.StringFormatFlags,
-        Td = (F.C.StiIndicatorCellPainter = class {
+        Td = L.System.Drawing.StringFormatFlags,
+        Fd = (F.C.StiIndicatorCellPainter = class {
             static draw(e, t, r, i, s, n, l, a = !0) {
                 let o = this.getCellText(r, i, n);
                 this.draw2(e, t.clone(), r, i, s, n, l, o, a)
             }
             static draw2(r, i, s, n, l, a, o, u, e = !0) {
                 let t = this.measureText(l, u, s.font),
                     h = this.calculateIndicatorRect(i.clone(), n, l, t);
@@ -14919,22 +14918,22 @@
                         r, i, s;
                     s = 0 < a ? (r = new Yl(l.left + t, l.top), i = new Yl(l.left, l.bottom), new Yl(l.right, l.bottom)) : (r = new Yl(l.left + t, l.bottom), i = new Yl(l.left, l.top), new Yl(l.right, l.top)), n.fillPolygon([r, i, s], 0 < a ? N.green : N.red)
                 }
             }
             static drawText(e, t, r, i, s, n, l) {
                 if (B.isNullOrWhiteSpace(s)) return;
                 t.width -= 2;
-                let a = new xd,
+                let a = new Md,
                     o = U.Table.Font.getGdiFont(i, null, n);
-                a.lineAlignment = mn.Center, a.alignment = this.toAlignment(r), a.trimming = Du.None, a.formatFlags |= Md.NoWrap, e.drawString(s, o, l, t.clone(), a)
+                a.lineAlignment = mn.Center, a.alignment = this.toAlignment(r), a.trimming = Ru.None, a.formatFlags |= Td.NoWrap, e.drawString(s, o, l, t.clone(), a)
             }
             static measureText(e, t, r) {
                 if (B.isNullOrWhiteSpace(t)) return 0;
                 let i = U.Table.Font.getGdiFont(e, null, r);
-                return Ou.measureString(null, t, i).width
+                return Vu.measureString(null, t, i).width
             }
             static calculateIndicatorRect(t, e, r, i) {
                 let s = 16 * r;
                 switch (this.getHorAlignment(e)) {
                     case z.Left:
                         t = new j(t.x, t.y, s, t.height);
                         break;
@@ -14989,46 +14988,46 @@
                 return mn.Center
             }
             static getHorAlignment(e) {
                 let t = e;
                 return null != t ? t.horAlignment : z.Right
             }
         }, F.C.StiIndicatorCellPainter),
-        Fd = L.Data.Engine.StiDataSortRuleHelper;
+        vd = L.Data.Engine.StiDataSortRuleHelper;
     {
-        class eg {
+        class tg {
             static getBackgroundColor(e, t) {
                 return t ? e.alternatingCellBackColor : e.cellBackColor
             }
             static measureColumn(e, t, r, i, s) {
                 let n, l = U.Table.getHeight(r.font, r.zoom);
                 if (i.is2($i)) n = this.measureSparklinesCell(r, 0, r.zoom);
                 else if (i.is2(Qi)) n = this.measureIndicatorCell(e, r, i, s, r.zoom);
                 else if (i.is2(_i)) n = this.measureDataBarsCell(e, r, i, s, r.zoom);
                 else if (i.is2(Gi)) n = this.measureBubbleCell(e, r, i, s, r.zoom);
-                else if (Lu.isImage(s)) return new W(0, U.Table.getHeight(r.font, r.zoom));
+                else if (Bu.isImage(s)) return new W(0, U.Table.getHeight(r.font, r.zoom));
                 return new W(n.width, Math.max(n.height, l))
             }
             static getArrowSize(e, t) {
                 let r = U.Table.getHeight(e.headerFont, e.zoom),
-                    i = Fd.getSortDirection(e.userSorts, t.key);
-                if (i != hh.None) return new W(1.5 * r, r);
+                    i = vd.getSortDirection(e.userSorts, t.key);
+                if (i != mh.None) return new W(1.5 * r, r);
                 return W.empty
             }
             static getRightImageRect(e, t, r) {
                 let i = r.width * e.zoom,
                     s = r.height * e.zoom;
                 return new j(t.right - 3 - i, t.y + (t.height - s) / 2, i, s)
             }
             static measureSparklinesCell(e, t, r) {
                 return new W(Math.max(t, 80 * r), 0)
             }
             static measureIndicatorCell(e, t, r, i, s) {
                 let n = r,
-                    l = Td.getCellText(t, n, V.tryToNullableNumber(i)),
+                    l = Fd.getCellText(t, n, V.tryToNullableNumber(i)),
                     a = this.measureCell2(e, l, t.font, r);
                 return a.width = (a.width + 4) * s * 1.25, a
             }
             static measureDataBarsCell(e, t, r, i, s) {
                 let n = ts.formatBasedOnColumnType(t, r, i),
                     l = this.measureCell2(e, n, t.font, r);
                 return l.width *= s, r.horAlignment != z.Center && (l.width *= 2), r.is(_i) && 0 < r.width && (l.width = s * r.width), l
@@ -15041,21 +15040,21 @@
                         t = this.measureCell2(r, e, i.font, s);
                     return t.width += l, t
                 }
             }
             static measureCommonCell(e, t, r, i, s, n) {
                 let l = ts.formatBasedOnColumnType(t, r, i),
                     a = new W(s, 0);
-                return Lu.isImage(l) || ((a = this.measureCell2(e, l, t.font, r)).width *= n, a.height *= n), a
+                return Bu.isImage(l) || ((a = this.measureCell2(e, l, t.font, r)).width *= n, a.height *= n), a
             }
             static measureHeader(e, t) {
                 return this.measureHeader2(null, e, t)
             }
             static measureHeader2(e, t, r) {
-                let i = kh.getLabel(r),
+                let i = Nh.getLabel(r),
                     s = this.measureCell2(e, i, t.headerFont, r);
                 return s.width += 36, s
             }
             static measureCell(e, t, r) {
                 return this.measureCell2(null, e, t, r)
             }
             static measureCell2(e, t, r, i) {
@@ -15065,49 +15064,49 @@
                     l = r[L.System.StiObject.stimulsoft]().getHashCode().toString() + t + n.getUniqueCode().toString();
                 if (this.captionSizeCache.contains(l)) {
                     let e = this.captionSizeCache.get(l);
                     return s.width = e.width, s.height = e.height, s
                 }
                 let a = U.Table.Font.getGdiFont(1, null, r),
                     o = 0 != n.Width ? n.Width : n.MaxWidth,
-                    u = ah.measureString(t, a, o);
+                    u = oh.measureString(t, a, o);
                 return u.width = n.getColumnWidth(u.width), u.height = n.getColumnHeight(u.height), s.width = u.width, s.height = u.height, this.captionSizeCache.set(l, u), s
             }
             static measureHeaders(t, e) {
                 let i = U.Table.Font.getGdiFont(1, null, e),
                     s = new W(8, U.Table.getHeight(i));
                 for (let e of t) {
                     let t = new W(8, 0),
-                        r = kh.getLabel(e);
+                        r = Nh.getLabel(e);
                     if (!B.isNullOrEmpty(r)) {
-                        let e = ah.measureString(r, i, 1e6);
+                        let e = oh.measureString(r, i, 1e6);
                         t.width += e.width
                     }
                     s.width += t.width
                 }
                 return s.width
             }
         }
-        eg.captionSizeCache = new Co, F.q.StiTableElementGdiPainter = eg
+        tg.captionSizeCache = new xo, F.q.StiTableElementGdiPainter = tg
     }
-    let vd = L.System.Drawing.SolidBrush,
-        Ad = (F.C.StiBubbleCellPainter = class {
+    let Ad = L.System.Drawing.SolidBrush,
+        Id = (F.C.StiBubbleCellPainter = class {
             static draw(s, e, t, n, r, l, i, a, o, u, h = !0) {
                 if (0 == l) return;
                 let m = ts.formatBasedOnColumnType(t, n, l),
                     c = (0 < i && (i = 0), a < 0 && (a = 0), n.horAlignment),
                     d = e,
                     g = (d.inflate(-2, -2), this.calculateTextRect(t, d, n)),
                     p = (d = this.calculateBubbleRect(t, d, n, Math.abs(l), i, a), J.getTableStyle(t)),
                     S = this.getForeColor(t, n, p, o, u);
                 if (h && c != z.Center && s.drawString(m, t.font, S, g, null), 0 < d.width && 0 < d.height) {
                     let e = n.as(Gi),
                         t = e.allowCustomColors ? e.positiveColor : p.cellDataBarsPositive,
                         r = e.allowCustomColors ? e.negativeColor : p.cellDataBarsNegative,
-                        i = new vd(l < 0 ? r : t);
+                        i = new Ad(l < 0 ? r : t);
                     s.fillEllipse(d, i)
                 }
             }
             static getForeColor(e, t, r, i, s) {
                 if (!N.transparent.equals(t.foreColor)) return t.foreColor;
                 if (!N.transparent.equals(e.foreColor)) return e.foreColor;
                 if (i) return r.alternatingCellForeColor;
@@ -15162,23 +15161,23 @@
                 let m = (u.a - o.a) * a + o.a,
                     c = (u.r - o.r) * a + o.r,
                     d = (u.g - o.g) * a + o.g,
                     g = (u.b - o.b) * a + o.b;
                 return m = Math.min(m, 255), c = Math.min(c, 255), d = Math.min(d, 255), g = Math.min(g, 255), m = Math.max(m, 0), c = Math.max(c, 0), d = Math.max(d, 0), g = Math.max(g, 0), N.fromArgb(Math.round(m), Math.round(c), Math.round(d), Math.round(g))
             }
         }, F.K.StiTableElementConditionHelper),
-        Id = F.K.StiDataBarsDirection,
-        Dd = F.K.StiDataBarsBrushType,
-        Rd = L.Base.Drawing.StiGradientBrush,
-        Ed = (F.C.StiDataBarsCellPainter = class {
-            static async draw(e, t, r, i, s, n, l, a, o, u, h, m, c = !0, d = Id.LeftToRight, g = Dd.Solid) {
+        Dd = F.K.StiDataBarsDirection,
+        Rd = F.K.StiDataBarsBrushType,
+        Ed = L.Base.Drawing.StiGradientBrush,
+        Od = (F.C.StiDataBarsCellPainter = class {
+            static async draw(e, t, r, i, s, n, l, a, o, u, h, m, c = !0, d = Dd.LeftToRight, g = Rd.Solid) {
                 let p = ts.formatBasedOnColumnType(r, n, a);
                 await this.draw2(e, t, a, o, u, l, p, r, i, s, n, h, m, c, d, g)
             }
-            static async draw2(s, e, n, t, r, i, l, a, o, u, h, m, c, d = !0, g = Id.LeftToRight, p = Dd.Solid) {
+            static async draw2(s, e, n, t, r, i, l, a, o, u, h, m, c, d = !0, g = Dd.LeftToRight, p = Rd.Solid) {
                 if (null == n || 0 == n) return;
                 let S = h,
                     w = (B.isNullOrWhiteSpace(S.minimum) || (t = V.tryToNumber(O.parse2(S.minimum, a.report))), B.isNullOrWhiteSpace(S.maximum) || (r = V.tryToNumber(O.parse2(S.maximum, a.report))), t = Math.min(t, 0), !1),
                     b = ((r = Math.max(r, 0)) < n && (w = !0, n = r), n < t && (w = !0, n = t), h.horAlignment),
                     f = e,
                     y = (f.inflate(-2, -2), this.calculateTextRect(f, h)),
                     C = (f = this.calculateDataBarsRect(f, h), J.getTableStyle(a)),
@@ -15188,26 +15187,26 @@
                     F = this.getFillColor(C, S),
                     v = this.getForeColor(a, h, C, m, c),
                     A = (d && s.drawString(l, a.font, v, y, null), b != z.Center && s.fillRectangle(f, F), r + Math.abs(t)),
                     I = f.width * Math.abs(t) / A,
                     D = f.width * n / A,
                     R = f.width * Math.abs(n) / A,
                     E = 0;
-                if (g == Id.LeftToRight ? f.x += n < 0 ? I - R : I : (E = 180, f.x = n < 0 ? f.right - I : f.right - I - R), f.width = R, n < 0 && (E += 180), 0 < f.width && 0 < f.height) {
-                    if (p == Dd.Gradient) {
+                if (g == Dd.LeftToRight ? f.x += n < 0 ? I - R : I : (E = 180, f.x = n < 0 ? f.right - I : f.right - I - R), f.width = R, n < 0 && (E += 180), 0 < f.width && 0 < f.height) {
+                    if (p == Rd.Gradient) {
                         let i;
-                        if (i = g == Id.LeftToRight ? 0 < n ? new Ve(e.left + I, e.top, D, e.height) : new Ve(e.left, e.top, I, e.height) : n < 0 ? new Ve(e.left + D, e.top, I, e.height) : new Ve(e.left, e.top, D, e.height), 0 < f.width && f.width < 1 && (f.width = 1), 0 < i.width && i.width < 1 && (i.width = 1), 0 < i.width && 0 < f.width) {
+                        if (i = g == Dd.LeftToRight ? 0 < n ? new Ve(e.left + I, e.top, D, e.height) : new Ve(e.left, e.top, I, e.height) : n < 0 ? new Ve(e.left + D, e.top, I, e.height) : new Ve(e.left, e.top, D, e.height), 0 < f.width && f.width < 1 && (f.width = 1), 0 < i.width && i.width < 1 && (i.width = 1), 0 < i.width && 0 < f.width) {
                             let e = n < 0 ? M : x,
-                                t = Th.light(e, 200),
-                                r = (i.x -= .1 * i.width, i.width += .2 * i.width, new Rd(e, t, E));
+                                t = Fh.light(e, 200),
+                                r = (i.x -= .1 * i.width, i.width += .2 * i.width, new Ed(e, t, E));
                             s.fillRectangle(f, r)
                         }
                     } else {
                         let e = n < 0 ? M : x;
-                        e = await Ad.processForeColor(e, h.key, a, o, u), s.fillRectangle(f, e)
+                        e = await Id.processForeColor(e, h.key, a, o, u), s.fillRectangle(f, e)
                     }
                     if (w) {
                         let e = 0 <= n ? new Ve(f.right - 6 * i, f.y, 6 * i, f.height) : new Ve(f.x, f.y, 6 * i, f.height);
                         s.fillRectangle(e, T)
                     }
                     b == z.Center && s.drawString(l, a.font, N.white, y, null)
                 }
@@ -15283,53 +15282,53 @@
                 let r = (this.Column = t).as(mi);
                 if (null == (null == r ? void 0 : r.size)) return;
                 this.IsMeasurable = !0, this.FontUniqueCode = e.getHashCode();
                 let i = r.size;
                 this.Width = i.width, this.MinWidth = i.minWidth, this.MaxWidth = i.maxWidth, this.MaxHeight = i.wordWrap ? Number.MAX_VALUE : Math.round(e.getHeight()) + 1, this.WordWrap = i.wordWrap
             }
         }, F.y.IStiSizeExportSettings = new L.System.Interface("IStiSizeExportSettings"), L.Report.Dashboard.IStiControlElement),
-        Od = F.p.StiLocHelper,
-        Vd = F.S.StiComboBoxHelper;
+        Vd = F.p.StiLocHelper,
+        kd = F.S.StiComboBoxHelper;
     {
-        class lp extends F.A.StiElementExportTool {
+        class ap extends F.A.StiElementExportTool {
             async render(i, s, n, e) {
                 var r, t, l, a;
                 if (0 == i.getMeters().length) return;
                 let o = await bl.tryToGetOrCreate(i);
                 if (null == o) return;
-                let u = e.is(Hc) && e.designMode,
-                    h = i.as(dm),
-                    m = lp.getNameMeterIndex(o),
-                    c = lp.getKeyMeterIndex(o),
+                let u = e.is(zc) && e.designMode,
+                    h = i.as(gm),
+                    m = ap.getNameMeterIndex(o),
+                    c = ap.getKeyMeterIndex(o),
                     d = u && null != h && !B.isNullOrEmpty(h.initialValue),
-                    g = new Co;
+                    g = new xo;
                 if (1 < o.meters.countItems)
                     for (let t of o.rows) {
                         let e = null == (r = t[1]) ? void 0 : r[L.System.StiObject.stimulsoft]().toString();
                         B.isNullOrWhiteSpace(e) || g.set(e, t[0])
                     }
                 let p = i,
                     S = i,
                     w = "";
                 if (p.selectionMode == gl.One)
                     if (S.userFilters.any()) w = S.userFilters[0].value, w = null != (t = g.get(w)) ? t : w;
-                    else if (p.showAllValue) w = Od.locAll;
+                    else if (p.showAllValue) w = Vd.locAll;
                 else {
                     let e = o.rows.firstOrDefault();
                     null != e && 0 < e.length && null != e[0] && (w = e[0].toString())
                 }
                 if (d)
                     if (h.initialValue[L.System.StiObject.stimulsoft]().contains(";")) w = h.initialValue;
                     else {
-                        let e = lp.getRow(h, o, c);
+                        let e = ap.getRow(h, o, c);
                         if (null == e) return;
                         let t = -1 != m ? e[m] : null,
                             r = -1 != c ? e[c] : null;
                         null == t && null == r || (w = (t || r).toString())
-                    } if (this.renderElement(s, i, n, this.format(i.as(Ed), w)), p.selectionMode == gl.Multi && !d) {
+                    } if (this.renderElement(s, i, n, this.format(i.as(Od), w)), p.selectionMode == gl.Multi && !d) {
                     let t = n;
                     if (S.userFilters.any()) {
                         let r = S.userFilters;
                         if (r.all(e => e.condition == Zi.NotEqualTo)) {
                             r = new P;
                             for (let e of o.rows) {
                                 let t = null == (l = e[1]) ? void 0 : l[L.System.StiObject.stimulsoft]().toString();
@@ -15338,38 +15337,38 @@
                             }
                         }
                         for (let e of r) {
                             if (!(t.x + t.width <= n.x + n.width)) {
                                 while (1 < s.components.count) s.components.removeAt(1);
                                 this.renderItem(s, i, n, B.format(b.get("Dashboard", "NSelected"), S.userFilters.length));
                                 break
-                            }(t = this.renderItem(s, i, t, this.format(i.as(Ed), null != (a = g.get(e.value)) ? a : e.value))).x += t.width + 4
+                            }(t = this.renderItem(s, i, t, this.format(i.as(Od), null != (a = g.get(e.value)) ? a : e.value))).x += t.width + 4
                         }
-                    } else if (p.showAllValue) this.renderItem(s, i, n, Od.locAll);
+                    } else if (p.showAllValue) this.renderItem(s, i, n, Vd.locAll);
                     else {
                         let e = this.getValuesCount(i, o);
                         this.renderItem(s, i, n, B.format(b.get("Dashboard", "NSelected"), e))
                     }
                 }
             }
             getValuesCount(e, t) {
-                let r = e.as(dm),
-                    i = Vd.fetchItems(r, t, r.showBlanks);
+                let r = e.as(gm),
+                    i = kd.fetchItems(r, t, r.showBlanks);
                 return null != i ? i.length : 0
             }
             renderElement(e, t, r, i) {
                 let s = J.getForeColor(t),
                     n = J.getBackColor(t),
-                    l = new Iu(r);
-                l.name = t.name + `_ComboBox`, l.allowHtmlTags = !0, l.vertAlignment = Wt.Center, l.horAlignment = X.Left, l.textBrush = new v(s), l.brush = new v(n), l.text = this.format(t.as(Ed), i), e.components.add(l)
+                    l = new Du(r);
+                l.name = t.name + `_ComboBox`, l.allowHtmlTags = !0, l.vertAlignment = Wt.Center, l.horAlignment = X.Left, l.textBrush = new v(s), l.brush = new v(n), l.text = this.format(t.as(Od), i), e.components.add(l)
             }
             renderItem(e, t, r, i) {
                 let s = J.getControlStyle(t),
-                    n = new Iu,
-                    l = (n.name = t.name + `_ComboBoxItem`, n.allowHtmlTags = !0, n.vertAlignment = Wt.Center, n.horAlignment = X.Center, n.textBrush = new v(s.selectedForeColor), n.brush = new v(s.selectedBackColor), n.text = this.format(t.as(Ed), i), e.components.add(n), ah.measureString(i, n.font));
+                    n = new Du,
+                    l = (n.name = t.name + `_ComboBoxItem`, n.allowHtmlTags = !0, n.vertAlignment = Wt.Center, n.horAlignment = X.Center, n.textBrush = new v(s.selectedForeColor), n.brush = new v(s.selectedBackColor), n.text = this.format(t.as(Od), i), e.components.add(n), oh.measureString(i, n.font));
                 return n.clientRectangle = new j(r.x, r.y, l.width + 4, r.height)
             }
             static getNameMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => "StiNameComboBoxMeter" == e[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName());
                 return null != t ? e.meters.indexOf(t) : -1
             }
@@ -15382,47 +15381,47 @@
                 if (B.isNullOrEmpty(r.initialValue) || -1 == i) return e.rows.firstOrDefault();
                 return e.rows.firstOrDefault(e => {
                     var t;
                     return (null == (t = e[i]) ? void 0 : t.toString()) == r.initialValue
                 })
             }
         }
-        F.A.StiComboBoxElementExportTool = lp
+        F.A.StiComboBoxElementExportTool = ap
     }
-    let kd = F.Q.StiDatePickerHelper,
-        Nd = (F.A.StiDatePickerElementExportTool = class extends F.A.StiElementExportTool {
+    let Nd = F.Q.StiDatePickerHelper,
+        Ld = (F.A.StiDatePickerElementExportTool = class extends F.A.StiElementExportTool {
             async render(t, r, i, e) {
                 var s;
                 let n = t;
                 if (null == n.getValueMeter()) return;
                 let l = await bl.tryToGetOrCreate(t),
                     a = J.getForeColor(t),
                     o = J.getBackColor(t);
                 this.storedCulture = null;
                 try {
                     let e = null == (s = t.report) ? void 0 : s.getParsedCulture();
                     B.isNullOrWhiteSpace(e) || (this.storedCulture = ni.currentCulture, ni.currentCulture = new ni(e))
                 } finally {
-                    let e = new Iu(i);
+                    let e = new Du(i);
                     e.name = t.name + `_Content`, e.allowHtmlTags = !0, e.vertAlignment = Wt.Center, e.textBrush = new v(a), e.brush = new v(o), e.text = this.getDateTimeString(n, l), e.font = n.font, r.components.add(e), null != this.storedCulture && (ni.currentCulture = this.storedCulture)
                 }
             }
             getDateTimeString(r, e) {
                 var t, i;
-                let s = kd.getDefaultValue(r);
+                let s = Nd.getDefaultValue(r);
                 if (El.isVariableSpecifiedAsExpression(r, null == (t = null == r ? void 0 : r.valueMeter) ? void 0 : t.expression)) {
-                    let e = null == (i = kd.getVariableSpecifiedAsValue(r)) ? void 0 : i.as(zs);
+                    let e = null == (i = Nd.getVariableSpecifiedAsValue(r)) ? void 0 : i.as(zs);
                     if (Al.isRangeType(null == e ? void 0 : e.type) && r.initialRangeSelectionSource == xl.Selection) {
                         let e = {
                                 ref: null
                             },
                             t = {
                                 ref: null
                             };
-                        return kd.calculateRangeFromInitial(r.initialRangeSelection, e, t), this.getRangeVariableString(r, new vl(e.ref, t.ref))
+                        return Nd.calculateRangeFromInitial(r.initialRangeSelection, e, t), this.getRangeVariableString(r, new vl(e.ref, t.ref))
                     }
                     return null != s && s[L.System.StiObject.stimulsoft]().is(vl) ? this.getRangeVariableString(r, s) : this.format(r, s)
                 }
                 if (r.userFilters.any()) {
                     let e = this.format(r, r.userFilters[0].value);
                     return r.selectionMode != Ml.AutoRange && r.selectionMode != Ml.Range || (e += ` - ` + this.format(r, r.userFilters[0].value2)), e
                 }
@@ -15445,142 +15444,142 @@
             getRangeColumnString(e) {
                 let t = {
                         ref: null
                     },
                     r = {
                         ref: null
                     };
-                return kd.calculateRangeFromInitial(e.initialRangeSelection, t, r), this.format(e, t.ref) + ` - ` + this.format(e, r.ref)
+                return Nd.calculateRangeFromInitial(e.initialRangeSelection, t, r), this.format(e, t.ref) + ` - ` + this.format(e, r.ref)
             }
         }, F.P.StiListBoxHelper),
-        Ld = L.Report.Components.StiCheckBox,
-        Bd = L.Report.Components.StiCheckStyle,
-        Pd = L.Report.Components.IStiShape;
+        Bd = L.Report.Components.StiCheckBox,
+        Pd = L.Report.Components.StiCheckStyle,
+        jd = L.Report.Components.IStiShape;
     {
-        class ap extends F.A.StiElementExportTool {
+        class op extends F.A.StiElementExportTool {
             async render(e, s, t, r) {
                 if (this.renderEmptyDataMessage(e, s, t.clone(), r)) return;
                 let n = s.report,
                     l = s.page,
-                    a = e.as(gm),
+                    a = e.as(pm),
                     o = s.clone(!0, !1),
                     u = (r.renderSinglePage || (t.height = Number.MAX_VALUE), await this.renderItems(o, t.clone(), e), 0),
                     h = s.top;
                 0 < o.components.count && (h += o.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top));
                 while (1) {
                     let e = o.getComponentsList(),
                         i = 0;
                     for (let r of e) {
                         let e = r.bottom,
                             t = r.left;
-                        r.is(Pd) && (e += U.ListBox.ItemHeight / 3), null != a ? (a.orientation == Ys.Vertical && e <= s.height || a.orientation == Ys.Horizontal && t <= s.width || 0 == i) && (o.components.remove(r), s.components.add(r)) : e <= s.height && (o.components.remove(r), s.components.add(r)), i++
+                        r.is(jd) && (e += U.ListBox.ItemHeight / 3), null != a ? (a.orientation == Ys.Vertical && e <= s.height || a.orientation == Ys.Horizontal && t <= s.width || 0 == i) && (o.components.remove(r), s.components.add(r)) : e <= s.height && (o.components.remove(r), s.components.add(r)), i++
                     }
                     if (r.renderSinglePage || 0 == o.components.count) break;
                     let t = o.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top);
                     o.getComponentsList().forEach(e => e.top = e.top - t + 1), n.renderedPages.count <= ++u && n.renderedPages.add(l.clone(!0, !1)), l = n.renderedPages.getByIndex(u), s = s.clone(!0, !1), r.renderSingleElement ? (s.top = 0, s.left = 0) : s.top = h, l.components.add(s)
                 }
                 for (let e of s.report.renderedPages.list) e.getComponentsList().forEach(e => {
                     e.report = n, e.page = l
                 })
             }
             static getCheckStyle(e, t) {
                 let r = e,
-                    i = e.is(gm) && e.as(gm).selectionMode == gl.One && e.as(gm).selectionType == io.RadioButton,
-                    s = i ? Bd.DotCircle : Bd.CheckRectangle,
-                    n = i ? Bd.NoneCircle : Bd.NoneRectangle;
+                    i = e.is(pm) && e.as(pm).selectionMode == gl.One && e.as(pm).selectionType == so.RadioButton,
+                    s = i ? Pd.DotCircle : Pd.CheckRectangle,
+                    n = i ? Pd.NoneCircle : Pd.NoneRectangle;
                 if (!r.userFilters.any()) return i ? n : s;
                 if (r.userFilters.any(e => e.condition == Zi.IsFalse)) return n;
                 if (r.userFilters.any(e => e.condition == Zi.EqualTo && e.value == (null == t ? void 0 : t.toString()))) return s;
                 return n
             }
             async renderItems(i, s, n) {
                 let e = await bl.tryToGetOrCreate(n);
                 if (null == e) return;
                 let t = n,
-                    l = Nd.fetchItems(t, e, t.showBlanks);
+                    l = Ld.fetchItems(t, e, t.showBlanks);
                 if (null != l) {
                     let e = l.select(e => null == e ? "" : null == e.label && null != e.value && e.value instanceof w ? e.value.toShortDateString() : e.toString()),
-                        t = l.select(e => ap.getCheckStyle(n, e)),
+                        t = l.select(e => op.getCheckStyle(n, e)),
                         r = l.select(e => !1);
                     this.renderItems2(i, s.clone(), n, e, t, r)
                 }
             }
             renderItems2(s, n, l, a, o, u) {
                 var e;
                 let h = l,
                     m = h.selectionMode == gl.Multi,
-                    c = h.selectionMode == gl.One && l.is(gm) && l.as(gm).selectionType == io.RadioButton,
+                    c = h.selectionMode == gl.One && l.is(pm) && l.as(pm).selectionType == so.RadioButton,
                     d = m || c,
-                    g = l.is(no) && l.orientation == Ys.Horizontal,
+                    g = l.is(lo) && l.orientation == Ys.Horizontal,
                     p = (null == (e = h[L.System.StiObject.stimulsoft]().as(ar)) ? void 0 : e.font) || new H("Arial", 8),
                     S = l,
                     w = g ? this.getHorizontalItemAutoWidth(h, p, a, n.width, d) : n.width,
                     b = g ? n.height : U.ListBox.ItemHeight,
                     f = n.x,
                     y = n.y;
                 if (h.showAllValue) {
-                    g && 0 == w && (w = this.measureItemWidth(Od.locAll, p, d));
+                    g && 0 == w && (w = this.measureItemWidth(Vd.locAll, p, d));
                     let e = new j(f, y, w, b),
-                        t = c ? Bd.DotCircle : Bd.CheckRectangle;
-                    S.userFilters.any() && (t = c ? Bd.NoneCircle : S.userFilters.any(e => e.condition == Zi.IsFalse) ? Bd.NoneRectangle : Bd.DotRectangle), this.renderItem(s, e, l, Od.locAll, t, g ? G.Right : G.Bottom, m, c, !1), g ? f += w + 1 : y += b + 1
+                        t = c ? Pd.DotCircle : Pd.CheckRectangle;
+                    S.userFilters.any() && (t = c ? Pd.NoneCircle : S.userFilters.any(e => e.condition == Zi.IsFalse) ? Pd.NoneRectangle : Pd.DotRectangle), this.renderItem(s, e, l, Vd.locAll, t, g ? G.Right : G.Bottom, m, c, !1), g ? f += w + 1 : y += b + 1
                 }
                 if (null != a) {
                     let i = 0;
                     for (let r = 0; r < a.count2(); r++) {
                         g && 0 == w && (w = this.measureItemWidth(a[r], p, d));
                         let e = new j(f + i, y, w - i, b),
                             t = o[r];
-                        if (!c || S.userFilters.any() || h.showAllValue || 0 != r || (t = Bd.DotCircle), this.renderItem(s, e, l, a[r], t, G.None, m, c, u[r]), u[r] && (i += U.ListBox.CheckBoxWidth), g ? f += w + 1 : y += b + 1, g && f >= n.right || !g && y >= n.bottom) break
+                        if (!c || S.userFilters.any() || h.showAllValue || 0 != r || (t = Pd.DotCircle), this.renderItem(s, e, l, a[r], t, G.None, m, c, u[r]), u[r] && (i += U.ListBox.CheckBoxWidth), g ? f += w + 1 : y += b + 1, g && f >= n.right || !g && y >= n.bottom) break
                     }
                 }
             }
             getHorizontalItemAutoWidth(e, t, r, i, s) {
                 let n = 0,
                     l = 0;
                 if (null != r)
                     while (n < i && l < r.length) n += this.measureItemWidth(r[l], t, s), l++;
-                return e.showAllValue && (this.measureItemWidth(Od.locAll, t, s), l++), n < i && 0 < l ? i / l : 0
+                return e.showAllValue && (this.measureItemWidth(Vd.locAll, t, s), l++), n < i && 0 < l ? i / l : 0
             }
             measureItemWidth(e, t, r) {
                 let i = U.Table.Font.getGdiFont(1, null, t),
-                    s = ah.measureString(e, i, 1e6),
+                    s = oh.measureString(e, i, 1e6),
                     n = s.width;
                 return r && (n += U.ListBox.CheckBoxWidth), n
             }
             renderItem(t, r, i, e, s, n, l, a, o) {
                 var u;
                 if (l || a) {
-                    let e = i.is(no) && i.orientation == Ys.Horizontal;
-                    ap.renderCheckControl(t, r.clone(), i, s, e ? G.None : n, a), r.x += U.ListBox.CheckBoxWidth, r.width -= U.ListBox.CheckBoxWidth
+                    let e = i.is(lo) && i.orientation == Ys.Horizontal;
+                    op.renderCheckControl(t, r.clone(), i, s, e ? G.None : n, a), r.x += U.ListBox.CheckBoxWidth, r.width -= U.ListBox.CheckBoxWidth
                 }
                 let h = J.getForeColor(i),
                     m = J.getBackColor(i, null, !0),
                     c = (null == (u = i[L.System.StiObject.stimulsoft]().as(ar)) ? void 0 : u.font) || new H("Arial", 8),
-                    d = this.format(i.as(Ed), e),
-                    g = new Iu(r),
-                    p = (g.name = i.name + `_Item`, g.allowHtmlTags = !0, g.margins = l || a ? new be(1, 0, 0, 0) : be.empty, g.border = n != G.None ? new ie(n, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), g.brush = new v(m), g.horAlignment = X.Left, g.vertAlignment = Wt.Center, g.text = d, g.textBrush = new v(h), g.wordWrap = !1, g.font = c, i.as(Ed));
+                    d = this.format(i.as(Od), e),
+                    g = new Du(r),
+                    p = (g.name = i.name + `_Item`, g.allowHtmlTags = !0, g.margins = l || a ? new be(1, 0, 0, 0) : be.empty, g.border = n != G.None ? new ie(n, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), g.brush = new v(m), g.horAlignment = X.Left, g.vertAlignment = Wt.Center, g.text = d, g.textBrush = new v(h), g.wordWrap = !1, g.font = c, i.as(Od));
                 null == p || p.textFormat.is(Jt) || (g.excelDataValue = d), t.components.add(g)
             }
             static renderCheckControl(e, t, r, i, s, n) {
                 let l = J.getForeColor(r),
-                    a = (t = new j(t.x, t.y, U.ListBox.CheckBoxWidth, t.height), new Ld(t));
-                a.name = r.name + `_ItemCheckBox`, a.border = s != G.None ? new ie(s, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), a.contourColor = N.transparent, a.textBrush = new v(l), a.checkStyleForTrue = i, a.checkStyleForFalse = n ? Bd.NoneCircle : Bd.NoneRectangle, a.checkedValue = i != Bd.NoneRectangle && i != Bd.NoneCircle, e.components.add(a)
+                    a = (t = new j(t.x, t.y, U.ListBox.CheckBoxWidth, t.height), new Bd(t));
+                a.name = r.name + `_ItemCheckBox`, a.border = s != G.None ? new ie(s, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), a.contourColor = N.transparent, a.textBrush = new v(l), a.checkStyleForTrue = i, a.checkStyleForFalse = n ? Pd.NoneCircle : Pd.NoneRectangle, a.checkedValue = i != Pd.NoneRectangle && i != Pd.NoneCircle, e.components.add(a)
             }
         }
-        F.A.StiListBoxElementExportTool = ap
+        F.A.StiListBoxElementExportTool = op
     }
-    let jd = L.Report.Components.StiVerticalLinePrimitive,
-        Hd = L.Report.Components.StiFlowchartSortShapeType;
+    let Hd = L.Report.Components.StiVerticalLinePrimitive,
+        zd = L.Report.Components.StiFlowchartSortShapeType;
     {
-        class op extends F.A.StiElementExportTool {
+        class up extends F.A.StiElementExportTool {
             async render(e, s, n, t) {
-                let l = e.as(Am);
+                let l = e.as(Im);
                 if (null == l.getValueMeter()) return;
                 let a = n.height + 2 * n.y,
-                    o = await ho.getInitialValue(l);
+                    o = await mo.getInitialValue(l);
                 if (o[L.System.StiObject.stimulsoft]().getType() == L.Report.DecimalRange) {
                     let e = new j(n.x, n.y, n.width / 2, n.height),
                         t = 1,
                         r = new j(e.right, a / 4, t, a / 2),
                         i = new j(e.right, n.y, n.width / 2, n.height);
                     this.paintItem(s, l, e, o.from), this.paintSeparator(s, l, r), this.paintItem(s, l, i, o.to)
                 } else if (L.System.Type.isNumericType(L.System.Type.getType(o))) {
@@ -15589,161 +15588,161 @@
                         r = new j(n.right - t - 3, a / 3, t, a / 3);
                     this.paintItem(s, l, n, e), this.paintNavButtons(s, l, r)
                 }
             }
             paintItem(e, t, r, i) {
                 let s = J.getForeColor(t),
                     n = J.getBackColor(t),
-                    l = new Iu(r);
-                l.name = t.name + `_NumberBox`, l.allowHtmlTags = !0, l.vertAlignment = Wt.Center, l.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), l.textBrush = new v(s), l.brush = new v(n), l.text = op.formatValue(t, i), l.font = J.getFont(t), e.components.add(l)
+                    l = new Du(r);
+                l.name = t.name + `_NumberBox`, l.allowHtmlTags = !0, l.vertAlignment = Wt.Center, l.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), l.textBrush = new v(s), l.brush = new v(n), l.text = up.formatValue(t, i), l.font = J.getFont(t), e.components.add(l)
             }
             paintSeparator(e, t, r) {
-                let i = new jd(r);
-                i.name = t.name + `_NumberBoxSep`, i.color = op.getSeparatorColor(t), e.components.add(i)
+                let i = new Hd(r);
+                i.name = t.name + `_NumberBoxSep`, i.color = up.getSeparatorColor(t), e.components.add(i)
             }
             paintNavButtons(e, t, r) {
-                let i = new Fc(r);
-                i.name = t.name + `_NumberBoxButtons`, i.shapeType = new Hd, i.borderColor = J.getForeColor(t), e.components.add(i)
+                let i = new vc(r);
+                i.name = t.name + `_NumberBoxButtons`, i.shapeType = new zd, i.borderColor = J.getForeColor(t), e.components.add(i)
             }
             static formatValue(e, t) {
                 return e.textFormat.format(t)
             }
             static getSeparatorColor(e) {
                 return J.getSeparatorColor(e)
             }
         }
-        F.A.StiNumberBoxElementExportTool = op
+        F.A.StiNumberBoxElementExportTool = up
     }
-    let zd = F.h.StiOnlineMapHelper,
-        Gd = L.Report.Maps.StiMapMode,
-        Xd = (F.A.StiOnlineMapElementExportTool = class extends F.A.StiElementExportTool {
+    let Gd = F.h.StiOnlineMapHelper,
+        Xd = L.Report.Maps.StiMapMode,
+        Wd = (F.A.StiOnlineMapElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, r, i) {
                 var s, n, l;
                 if (this.renderEmptyDataMessage(e, t, r.clone(), i)) return;
                 let a = await bl.tryToGetOrCreate(e),
-                    o = zd.calculateMapData(a, e),
+                    o = Gd.calculateMapData(a, e),
                     u = e,
-                    h = new Ho;
-                h.stretch = !0, h.page = u.page, h.dataTable = a, t.report.dictionary = u.report.dictionary, h.latitude = null == (s = u.latitude) ? void 0 : s.expression, h.longitude = null == (n = u.longitude) ? void 0 : n.expression, h.mapMode = Gd.Online, h.pushPins = JSON.stringify(null == (l = o.pushpins) ? void 0 : l.map(e => `pp=${e.lat},${e.lon};60`)), h.brush = new v(J.getBackColor(e, null, i.is(Hc) || i.is(Pc))), h.left = r.left, h.top = r.top, h.width = r.width, h.height = r.height, t.components.add(h)
+                    h = new zo;
+                h.stretch = !0, h.page = u.page, h.dataTable = a, t.report.dictionary = u.report.dictionary, h.latitude = null == (s = u.latitude) ? void 0 : s.expression, h.longitude = null == (n = u.longitude) ? void 0 : n.expression, h.mapMode = Xd.Online, h.pushPins = JSON.stringify(null == (l = o.pushpins) ? void 0 : l.map(e => `pp=${e.lat},${e.lon};60`)), h.brush = new v(J.getBackColor(e, null, i.is(zc) || i.is(jc))), h.left = r.left, h.top = r.top, h.width = r.width, h.height = r.height, t.components.add(h)
             }
         }, F.A.StiPanelElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, r, i) {
                 let s = J.getBackColor(e),
                     n = new re(r);
                 n.name = e.name + `_Content`, n.brush = new v(s), t.components.add(n)
             }
         }, L.Report.Components.StiDockStyle),
-        Wd = L.Report.Engine.StiCrossTabBuilder,
-        Jd = L.Report.CrossTab.StiCrossTabParams,
-        Ud = F.h.StiPivotTableHelper;
+        Jd = L.Report.Engine.StiCrossTabBuilder,
+        Ud = L.Report.CrossTab.StiCrossTabParams,
+        Zd = F.h.StiPivotTableHelper;
     {
-        class up extends F.A.StiElementExportTool {
+        class hp extends F.A.StiElementExportTool {
             async render(s, n, l, a) {
                 if (this.renderEmptyDataMessage(s, n, l.clone(), a)) return;
                 let o = n.report,
-                    t = s.as(Zh),
+                    t = s.as(Yh),
                     u = n.page,
-                    r = a.is(Hc) && a.designMode,
-                    e = md.isDataExport(a),
-                    h = jh.get(t);
+                    r = a.is(zc) && a.designMode,
+                    e = cd.isDataExport(a),
+                    h = Hh.get(t);
                 if (null == h) {
                     let e = await bl.tryToGetOrCreate(t);
-                    null == e && (e = new Tt), h = await Ud.convertToCrossTab(t, e), jh.put(t, h), Ph.putFalse(t)
+                    null == e && (e = new Tt), h = await Zd.convertToCrossTab(t, e), Hh.put(t, h), jh.putFalse(t)
                 }
-                Ud.applyStyle(t, h, e), r && (up.renderForWebDesigner(h, t), jh.remove(t)), up.convertSizes(t, h);
+                Zd.applyStyle(t, h, e), r && (hp.renderForWebDesigner(h, t), Hh.remove(t)), hp.convertSizes(t, h);
                 let i = h.crossTabInfo.cross,
                     m = i.widths[L.System.StiObject.stimulsoft]().toList().sum(),
                     c = i.heights[L.System.StiObject.stimulsoft]().toList().sum();
                 if (m <= l.width && c <= l.height || r || a.renderSinglePage) {
-                    wd.render(s, n, a), Sd.render(s, n);
-                    let e = await pd.render(s, n, a);
-                    e = bd.excludePadding(s, e), e = bd.excludeCornerRadius(s, e), up.renderCells(n, e, e, null, h, r)
-                } else if (a.is(ed)) {
+                    bd.render(s, n, a), wd.render(s, n);
+                    let e = await Sd.render(s, n, a);
+                    e = fd.excludePadding(s, e), e = fd.excludeCornerRadius(s, e), hp.renderCells(n, e, e, null, h, r)
+                } else if (a.is(td)) {
                     !a.renderSingleElement && 0 != o.renderedPages.getByIndex(0).components.count || o.renderedPages.removeAt(0), u = new Ie;
                     let e = new ct,
-                        t = (e.name = s.name, e.clientRectangle = new j(0, 0, m, c), u.components.add(e), o.renderedPages.add(u), wd.render(s, e, a), Sd.render(s, e), await pd.render(s, e, a)),
+                        t = (e.name = s.name, e.clientRectangle = new j(0, 0, m, c), u.components.add(e), o.renderedPages.add(u), bd.render(s, e, a), wd.render(s, e), await Sd.render(s, e, a)),
                         r = (o.renderedPages.remove(u), 2 * m - t.width + t.left + 1),
                         i = 2 * c - t.height + t.top + 1;
-                    (u = new Ie).width = r, u.height = i, (e = new ct).name = s.name, e.clientRectangle = new j(0, 0, r, i), u.components.add(e), o.renderedPages.add(u), wd.render(s, e, a), Sd.render(s, e), t = await pd.render(s, e, a), u.unlimitedHeight = !0, up.renderCells(e, t, t, null, h, !1)
+                    (u = new Ie).width = r, u.height = i, (e = new ct).name = s.name, e.clientRectangle = new j(0, 0, r, i), u.components.add(e), o.renderedPages.add(u), bd.render(s, e, a), wd.render(s, e), t = await Sd.render(s, e, a), u.unlimitedHeight = !0, hp.renderCells(e, t, t, null, h, !1)
                 } else {
                     let i = u.clone(!0, !1),
                         e = (o.renderedPages.add(i), n.clone(!0, !1)),
-                        t = (e.left = 0, e.top = 0, e.width = i.width, e.height = i.height, l = new j(0, 0, i.width, i.height), i.components.add(e), n = e, !a.renderSingleElement && 0 != o.renderedPages.getByIndex(0).components.count || o.renderedPages.removeAt(0), wd.render(s, n, a), Sd.render(s, n), await pd.render(s, n, a)),
-                        r = (t = bd.excludePadding(s, t), t = bd.excludeCornerRadius(s, t), new j(t.left, t.top, t.width + m, t.height + c));
-                    u.unlimitedHeight = !0, up.renderCells(n, r, t, null, h, !1);
+                        t = (e.left = 0, e.top = 0, e.width = i.width, e.height = i.height, l = new j(0, 0, i.width, i.height), i.components.add(e), n = e, !a.renderSingleElement && 0 != o.renderedPages.getByIndex(0).components.count || o.renderedPages.removeAt(0), bd.render(s, n, a), wd.render(s, n), await Sd.render(s, n, a)),
+                        r = (t = fd.excludePadding(s, t), t = fd.excludeCornerRadius(s, t), new j(t.left, t.top, t.width + m, t.height + c));
+                    u.unlimitedHeight = !0, hp.renderCells(n, r, t, null, h, !1);
                     for (let r = 0; r < i.segmentPerWidth; r++)
                         for (let t = 0; t < i.segmentPerHeight; t++)
                             if (0 != r || 0 != t) {
                                 let e = n.clone(!0, !1);
-                                e.left = r * u.width, e.top = t * u.height, e.width = u.width, e.height = u.height, i.components.insert(0, e), wd.render(s, e, a), Sd.render(s, e), await pd.render(s, e, a)
+                                e.left = r * u.width, e.top = t * u.height, e.width = u.width, e.height = u.height, i.components.insert(0, e), bd.render(s, e, a), wd.render(s, e), await Sd.render(s, e, a)
                             }
                 }
                 for (let e of n.report.renderedPages.list) e.getComponentsList().forEach(e => {
                     e.report = o, e.page = u
                 })
             }
             static renderForWebDesigner(e, t) {
-                let r = t.columns.where(e => Dh.getVisible(e, t.report)).toList(),
-                    i = t.rows.where(e => Dh.getVisible(e, t.report)).toList(),
-                    s = t.summaries.where(e => Dh.getVisible(e, t.report)).toList();
+                let r = t.columns.where(e => Rh.getVisible(e, t.report)).toList(),
+                    i = t.rows.where(e => Rh.getVisible(e, t.report)).toList(),
+                    s = t.summaries.where(e => Rh.getVisible(e, t.report)).toList();
                 if (!(1 < r.length || 1 < i.length)) return;
                 let n = e.crossTabInfo.cross.cells,
                     l = 0,
                     a = new P,
                     o = new P,
                     u = null,
                     h = null,
-                    m = t.summaryDirection == xo.LeftToRight ? s.length : 1,
-                    c = t.summaryDirection == xo.UpToDown ? s.length : 1,
-                    d = Ud.getHeadersBounds(n);
+                    m = t.summaryDirection == Mo.LeftToRight ? s.length : 1,
+                    c = t.summaryDirection == Mo.UpToDown ? s.length : 1,
+                    d = Zd.getHeadersBounds(n);
                 for (let r = 0; r < n.length; r++) {
                     let t = n[r][0];
-                    for (t.cellType == Rh.LeftTopLineMain && ((u = new hp).cell = t, u.x = r, u.width = t.width), t.cellType == Rh.RightTopLineMain && ((h = new hp).cell = t, h.x = r), l = 0; l < n[r].length; l++)
-                        if ((t = n[r][l]).cellType == Rh.CornerColMain || t.cellType == Rh.CornerRowMain) {
-                            let e = new hp;
+                    for (t.cellType == Eh.LeftTopLineMain && ((u = new mp).cell = t, u.x = r, u.width = t.width), t.cellType == Eh.RightTopLineMain && ((h = new mp).cell = t, h.x = r), l = 0; l < n[r].length; l++)
+                        if ((t = n[r][l]).cellType == Eh.CornerColMain || t.cellType == Eh.CornerRowMain) {
+                            let e = new mp;
                             e.cell = t, e.x = r, e.y = l, e.width = t.width, e.height = t.height, a.add(e)
                         }
                 }
                 if (-1 < d.top) {
                     let s = -1;
                     for (let i = 0; i < n.length; i++) {
                         let r = n[i][d.top];
-                        if (r.cellType == Rh.HeaderColMain || r.cellType == Rh.HeaderColTotalMain) {
+                        if (r.cellType == Eh.HeaderColMain || r.cellType == Eh.HeaderColTotalMain) {
                             s = -1 == s ? i : s;
                             let e = d.bottom - d.top + (1 < m ? 0 : 1),
-                                t = new hp;
-                            if (t.cell = r, t.x = s, t.y = d.top, t.height = e, t.width = m, a.add(t), r.text = (1 < e && r.cellType != Rh.HeaderColTotalMain ? "> " : "") + r.text, o.add(i + r.width - 1), 1 < m)
+                                t = new mp;
+                            if (t.cell = r, t.x = s, t.y = d.top, t.height = e, t.width = m, a.add(t), r.text = (1 < e && r.cellType != Eh.HeaderColTotalMain ? "> " : "") + r.text, o.add(i + r.width - 1), 1 < m)
                                 for (let t = i + r.width - m; t < i + r.width; t++) {
-                                    let e = new hp;
+                                    let e = new mp;
                                     e.cell = n[t][d.bottom], e.x = s, e.y = d.bottom, a.add(e), o.add(t), s++
                                 } else s++
                         }
                     }
                 }
                 if (-1 < d.left) {
                     let i = -1;
                     for (l = 0; l < n[0].length; l++) {
                         let r = n[0][l];
-                        if (r.cellType == Rh.HeaderRowMain || r.cellType == Rh.HeaderRowTotalMain) {
+                        if (r.cellType == Eh.HeaderRowMain || r.cellType == Eh.HeaderRowTotalMain) {
                             i = -1 == i ? l : i;
                             let e = d.right + (1 < c ? 0 : 1),
-                                t = new hp;
-                            if (t.cell = r, t.x = 0, t.y = i, t.height = c, t.width = e, t.cellRow = 1 == c ? l + r.height - 1 : -1, a.add(t), r.text = (1 < e && r.cellType != Rh.HeaderRowTotalMain ? "> " : "") + r.text, 1 < c)
+                                t = new mp;
+                            if (t.cell = r, t.x = 0, t.y = i, t.height = c, t.width = e, t.cellRow = 1 == c ? l + r.height - 1 : -1, a.add(t), r.text = (1 < e && r.cellType != Eh.HeaderRowTotalMain ? "> " : "") + r.text, 1 < c)
                                 for (let t = l + r.height - c; t < l + r.height; t++) {
-                                    let e = new hp;
+                                    let e = new mp;
                                     e.cell = n[d.right][t], e.x = d.right, e.y = i, e.cellRow = t, a.add(e), i++
                                 } else i++
                         }
                     }
                 }
                 null != u && (u.width = d.right - d.left + 1, a.add(u)), null != h && (h.width = a.max(e => e.x) - d.right, a.add(h));
                 let g = J.getPivotTableStyle(t),
                     p = a.max(e => e.y) + 1,
                     S = a.max(e => e.x) + 1,
-                    w = Ln.create2(Yh, S, p);
+                    w = Ln.create2(Kh, S, p);
                 for (let i of a)
                     if (w[i.x][i.y] = i.cell, i.cell.width = i.width, i.cell.height = i.height, 0 <= i.cellRow)
                         for (l = i.y; l < i.y + i.height; l++) {
                             let r = d.right + 1;
                             for (let e = i.width; e < n.length; e++)
                                 if (0 <= o.indexOf(e)) {
                                     w[r++][l] = n[e][i.cellRow + l - i.y], w[r - 1][l].field.border.side = e == n.length - 1 ? G.None : G.Right;
@@ -15751,90 +15750,90 @@
                                     if (null != t && null != t.field && t.field.brush.is(v)) {
                                         let e = t.field.brush.color;
                                         (e.equals(g.alternatingCellBackColor) || e.equals(g.cellBackColor)) && (t.field.brush = new v(l % 2 != 0 ? g.alternatingCellBackColor : g.cellBackColor), t.field.textBrush = new v(l % 2 != 0 ? g.alternatingCellForeColor : g.cellForeColor))
                                     }
                                     null != t && null != t.field && (t.field.brush = null != t.field.conditionBrush ? t.field.conditionBrush : t.field.brush, t.field.textBrush = null != t.field.conditionTextBrush ? t.field.conditionTextBrush : t.field.textBrush)
                                 }
                         }
-                n = Ln.create2(Yh, S, 0);
+                n = Ln.create2(Kh, S, 0);
                 for (let t = 0; t < S; t++) {
-                    n[t] = Ln.create(Yh, p);
-                    for (let e = 0; e < p; e++) n[t][e] = null != w[t][e] ? w[t][e] : new Yh, null != n[t][e].field && t == S - 1 && (n[t][e].field.border.side |= G.Top), 0 < e && (n[t][e].parentCell = n[t][e])
+                    n[t] = Ln.create(Kh, p);
+                    for (let e = 0; e < p; e++) n[t][e] = null != w[t][e] ? w[t][e] : new Kh, null != n[t][e].field && t == S - 1 && (n[t][e].field.border.side |= G.Top), 0 < e && (n[t][e].parentCell = n[t][e])
                 }
                 let b = Ln.create(Number, p),
                     f = Ln.create(Number, S);
                 Ln.copy(e.crossTabInfo.cross.heights, 0, b, p), Ln.copy(e.crossTabInfo.cross.widths, 0, f, S), e.crossTabInfo.cross.cells = n, e.crossTabInfo.cross.widths = f, e.crossTabInfo.cross.heights = b, e.crossTabInfo.cross.doAutoSize()
             }
             static renderCells(e, t, r, i, s, n) {
-                s.page.unlimitedHeight = !0, e.canBreak = !0, e.dockStyle = Xd.None;
-                let l = new Jd,
-                    a = (l.startColumn = 0, l.startRow = 0, l.destinationContainer = e, l.destinationRectangle = r, l.forceNoBreak = n, new Wd);
+                s.page.unlimitedHeight = !0, e.canBreak = !0, e.dockStyle = Wd.None;
+                let l = new Ud,
+                    a = (l.startColumn = 0, l.startRow = 0, l.destinationContainer = e, l.destinationRectangle = r, l.forceNoBreak = n, new Jd);
                 a.renderCrossTabUnlimitedBreakable(l, s, e, t.clone())
             }
             static convertSizes(e, t) {
                 let r = t.crossTabInfo.cross,
                     i = e.report.unit;
-                Ph.isConverted(e) || (this.convert(r.heights, i), this.convert(r.widths, i), this.convert(r.coordX, i), this.convert(r.coordY, i), Ph.putTrue(e))
+                jh.isConverted(e) || (this.convert(r.heights, i), this.convert(r.widths, i), this.convert(r.coordX, i), this.convert(r.coordY, i), jh.putTrue(e))
             }
             static convert(t, r) {
                 for (let e = 0; e < t.length; e++) t[e] = r.convertToHInches(t[e])
             }
         }
-        F.A.StiPivotTableElementExportTool = up;
-        class hp {
+        F.A.StiPivotTableElementExportTool = hp;
+        class mp {
             constructor() {
                 this.x = 0, this.y = 0, this.width = 1, this.height = 1, this.cellRow = -1
             }
         }
     }
     F.A.StiRegionMapElementExportTool = class extends F.A.StiElementExportTool {
         async render(e, t, r, i) {
             if (this.renderEmptyDataMessage(e, t, r.clone(), i)) return;
             let s = e,
-                n = new Ho;
-            if (n.stretch = !0, n.page = s.page, n.mapType = s.mapType, n.dataFrom = s.dataFrom, n.language = s.language, n.mapStyle = J.getMapStyleIdent(s), n.componentStyle = s.customStyleName, n.mapIdent = s.mapIdent, n.mapMode = Gd.Choropleth, n.showValue = s.showValue, n.shortValue = s.shortValue, n.showZeros = s.showZeros, n.showBubble = s.showBubble, n.colorEach = s.colorEach, n.displayNameType = s.showName, n.colorDataColumn = null == s.colorMeter ? "" : s.colorMeter.expression, n.groupDataColumn = null == s.groupMeter ? "" : s.groupMeter.expression, n.valueDataColumn = null == s.valueMeter ? "" : s.valueMeter.expression, n.nameDataColumn = null == s.nameMeter ? "" : s.nameMeter.expression, n.keyDataColumn = null == s.keyMeter ? "" : s.keyMeter.expression, n.mapData = s.mapData, n.labels = s.labels, n.brush = new v(J.getBackColor(e, null, i.is(Hc) || i.is(Pc))), n.left = r.left, n.top = r.top, n.width = r.width, n.height = r.height, s.dataFrom == Xo.DataColumns) {
+                n = new zo;
+            if (n.stretch = !0, n.page = s.page, n.mapType = s.mapType, n.dataFrom = s.dataFrom, n.language = s.language, n.mapStyle = J.getMapStyleIdent(s), n.componentStyle = s.customStyleName, n.mapIdent = s.mapIdent, n.mapMode = Xd.Choropleth, n.showValue = s.showValue, n.shortValue = s.shortValue, n.showZeros = s.showZeros, n.showBubble = s.showBubble, n.colorEach = s.colorEach, n.displayNameType = s.showName, n.colorDataColumn = null == s.colorMeter ? "" : s.colorMeter.expression, n.groupDataColumn = null == s.groupMeter ? "" : s.groupMeter.expression, n.valueDataColumn = null == s.valueMeter ? "" : s.valueMeter.expression, n.nameDataColumn = null == s.nameMeter ? "" : s.nameMeter.expression, n.keyDataColumn = null == s.keyMeter ? "" : s.keyMeter.expression, n.mapData = s.mapData, n.labels = s.labels, n.brush = new v(J.getBackColor(e, null, i.is(zc) || i.is(jc))), n.left = r.left, n.top = r.top, n.width = r.width, n.height = r.height, n.valueFormat = s.valueFormat, s.dataFrom == Wo.DataColumns) {
                 let e = await bl.tryToGetOrCreate(s);
                 n.dataTable = e, t.report.dictionary = s.report.dictionary
             }
             t.components.add(n)
         }
     }, F.A.StiShapeElementExportTool = class extends F.A.StiElementExportTool {
         async render(e, t, r, i) {
-            let s = e.as(cm),
-                n = new Fc;
+            let s = e.as(dm),
+                n = new vc;
             n.shapeType = s.shapeType, n.size = s.size, n.borderColor = s.stroke, n.brush = s.fill, n.page = s.page, n.left = r.left, n.top = r.top, n.width = r.width, n.height = r.height, t.components.add(n)
         }
     };
-    let Zd = L.Report.Dashboard.Helpers.StiTableElementPagingHelper,
-        Yd = L.Report.Dashboard.StiTableColumnVisibilityHelper,
-        Kd = F.C.StiBubbleCellPainter,
-        Qd = F.C.StiSparklinesCellPainter,
-        qd = L.Report.Components.StiSparkline,
-        _d = L.Data.Functions.StiSystemVariableObject,
-        $d = L.Report.StiNameValidator,
-        eg = F.q.StiTableElementGdiPainter,
-        tg = F.h.StiTableElementHelper,
-        rg = F.C.StiDataBarsCellPainter,
-        ig = L.Report.Export.StiSvgHelper,
-        sg = L.Report.Export.StiSvgGeomWriter,
-        ng = F.C.StiColorScaleCellPainter,
-        lg = L.Report.Components.StiTextQuality;
+    let Yd = L.Report.Dashboard.Helpers.StiTableElementPagingHelper,
+        Kd = L.Report.Dashboard.StiTableColumnVisibilityHelper,
+        Qd = F.C.StiBubbleCellPainter,
+        qd = F.C.StiSparklinesCellPainter,
+        _d = L.Report.Components.StiSparkline,
+        $d = L.Data.Functions.StiSystemVariableObject,
+        eg = L.Report.StiNameValidator,
+        tg = F.q.StiTableElementGdiPainter,
+        rg = F.h.StiTableElementHelper,
+        ig = F.C.StiDataBarsCellPainter,
+        sg = L.Report.Export.StiSvgHelper,
+        ng = L.Report.Export.StiSvgGeomWriter,
+        lg = F.C.StiColorScaleCellPainter,
+        ag = L.Report.Components.StiTextQuality;
     {
-        class mp extends F.A.StiElementExportTool {
+        class cp extends F.A.StiElementExportTool {
             async render(e, r, t, i) {
                 if (this.renderEmptyDataMessage(e, r, t.clone(), i)) return;
                 let s = r.report,
                     n = r.page,
-                    l = i.is(Hc) && i.as(Hc).designMode,
-                    a = e.as(fm),
+                    l = i.is(zc) && i.as(zc).designMode,
+                    a = e.as(ym),
                     o = null == i ? F.f.StiDashboardExportFormat.Document : i.format,
                     u = i.renderSingleElement && o == F.f.StiDashboardExportFormat.Excel,
-                    h = md.isDataExport(i),
+                    h = cd.isDataExport(i),
                     m = (delete a.cacheStyle, r.clone(!0, !1)),
-                    c = (i.renderSinglePage || (t.height = Number.MAX_VALUE), await mp.renderCells(m, t, a, 1, o, h, l), u && (t.width = m.components.toList().max(e => e.right), t.height = m.components.toList().max(e => e.bottom), r.width = r.page.width = t.width, r.height = r.page.height = t.height), 0),
+                    c = (i.renderSinglePage || (t.height = Number.MAX_VALUE), await cp.renderCells(m, t, a, 1, o, h, l), u && (t.width = m.components.toList().max(e => e.right), t.height = m.components.toList().max(e => e.bottom), r.width = r.page.width = t.width, r.height = r.page.height = t.height), 0),
                     d = r.top;
                 0 < m.components.count && (d += m.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top));
                 while (1) {
                     if (m.getComponentsList()[L.System.StiObject.stimulsoft]().toList().where(e => e.bottom <= r.height).toList().forEach(e => {
                             m.components.remove(e), (e.left < r.width || o == F.f.StiDashboardExportFormat.Data) && (r.components.add(e), e.right > r.width) && o != F.f.StiDashboardExportFormat.Data && (e.width = Math.max(0, r.width - e.left))
                         }), i.renderSinglePage || 0 == m.components.count) break;
                     let t = m.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top);
@@ -15842,15 +15841,15 @@
                 }
                 for (let e of r.report.renderedPages.list) e.getComponentsList()[L.System.StiObject.stimulsoft]().toList().forEach(e => {
                     e.report = s, e.page = n
                 })
             }
             static async renderCellsForViewer(e) {
                 var h;
-                let m = e.as(fm);
+                let m = e.as(ym);
                 if (null == m) return null;
                 let c = await bl.getOrCreate(m);
                 if (null == c) return null;
                 let d = 1,
                     g = [],
                     p = U.Table.getHeight(m.font, d),
                     S = c.meters.where(e => e.is(Cs)).cast(),
@@ -15859,60 +15858,60 @@
                 for (let u of S) {
                     u.cache = {};
                     let e = await this.getColumnVisibilityState(u, m.report);
                     if (!e) {
                         w++;
                         continue
                     }
-                    let n = mp.measureHeader(m, u, d);
-                    if (u.is($i)) n = mp.measureSparklinesCell(d, n);
+                    let n = cp.measureHeader(m, u, d);
+                    if (u.is($i)) n = cp.measureSparklinesCell(d, n);
                     else {
                         for (let r of c.rows) {
                             let e = r[w],
                                 t;
-                            t = u.is2(Qi) ? mp.measureIndicatorCell(m, u, d, e) : u.is2(_i) ? mp.measureDataBarsCell(m, u, d, e) : mp.measureCommonCell(m, u, d, e, n).width, n = Math.max(n, t)
+                            t = u.is2(Qi) ? cp.measureIndicatorCell(m, u, d, e) : u.is2(_i) ? cp.measureDataBarsCell(m, u, d, e) : cp.measureCommonCell(m, u, d, e, n).width, n = Math.max(n, t)
                         }
                         if (u.showTotalSummary) {
-                            let e = tg.calculateTotal(u, w, c),
+                            let e = rg.calculateTotal(u, w, c),
                                 t = this.measureFooter(m, u, d, e);
                             n = Math.max(n, t)
                         }
                     }
-                    let l = tg.minDataColumnValue(u, c, w),
-                        a = tg.maxDataColumnValue(u, c, w),
+                    let l = rg.minDataColumnValue(u, c, w),
+                        a = rg.maxDataColumnValue(u, c, w),
                         o = 0;
                     for (let s of c.rows) {
                         g.length < c.rows.length && g.push([]);
                         let t = this.processRowValue(o, s[w], u),
                             e = new j(0, 0, n, p),
                             r = new ct,
-                            i = (await mp.renderCell(r, e, m, s, S.select(e => e.key), u, d, t, l, a, 1 == (1 & o), F.f.StiDashboardExportFormat.Html, !1), {});
+                            i = (await cp.renderCell(r, e, m, s, S.select(e => e.key), u, d, t, l, a, 1 == (1 & o), F.f.StiDashboardExportFormat.Html, !1), {});
                         if (0 < m.tableConditions.length && 0 < r.components.length) {
                             let e = r.components.getByIndex(0);
-                            e.is(Iu) || (e.is(nr) && (i["backColor"] = Mu.toHtml(Se.toColor(e.as(nr).brush))), e.is($t) && (i["textColor"] = Mu.toHtml(Se.toColor(e.as($t).textBrush))))
+                            e.is(Du) || (e.is(nr) && (i["backColor"] = Tu.toHtml(Se.toColor(e.as(nr).brush))), e.is($t) && (i["textColor"] = Tu.toHtml(Se.toColor(e.as($t).textBrush))))
                         }
                         if ("boolean" == typeof t) i["boolValue"] = t;
                         else
                             for (let e of r.components.list)
-                                if (e.is(Iu)) {
-                                    if (i["text"] = e.text, i["textColor"] = Mu.toHtml(Se.toColor(e.textBrush)), i["backColor"] = Mu.toHtml(Se.toColor(e.brush)), i["textWidth"] = e.width, i["textHeight"] = e.height, 0 < m.tableConditions.length) {
+                                if (e.is(Du)) {
+                                    if (i["text"] = e.text, i["textColor"] = Tu.toHtml(Se.toColor(e.textBrush)), i["backColor"] = Tu.toHtml(Se.toColor(e.brush)), i["textWidth"] = e.width, i["textHeight"] = e.height, 0 < m.tableConditions.length) {
                                         let e = null == (h = m.as(ar)) ? void 0 : h.font,
-                                            t = 0 < m.tableConditions.length ? await Ad.processFontStyle(e, u.key, m, s, S.select(e => e.key)) : hn.Regular,
+                                            t = 0 < m.tableConditions.length ? await Id.processFontStyle(e, u.key, m, s, S.select(e => e.key)) : hn.Regular,
                                             r = (e = new H(e.fontFamily.name, e.size, t), {});
                                         r["bold"] = e.bold, r["italic"] = e.italic, r["underline"] = e.underline, r["strikeout"] = e.strikeout, i["textFontStyle"] = r
                                     }
                                     null != t && t.toString() != i["text"] && (i["value"] = t.toString())
-                                } else e.is(ld) ? (i["image"] = null != e.imageToDraw ? L.Base.Drawing.StiImageConverter.imageToString(e.imageToDraw) : null, i["imageWidth"] = e.width, i["imageHeight"] = e.height) : e.is(qd) && (i["sparkline"] = L.Report.Export.StiHtmlExportService.getSparklineData(null, e, e.width, e.height), i["sparklineWidth"] = e.width, i["sparklineHeight"] = e.height);
+                                } else e.is(ad) ? (i["image"] = null != e.imageToDraw ? L.Base.Drawing.StiImageConverter.imageToString(e.imageToDraw) : null, i["imageWidth"] = e.width, i["imageHeight"] = e.height) : e.is(_d) && (i["sparkline"] = L.Report.Export.StiHtmlExportService.getSparklineData(null, e, e.width, e.height), i["sparklineWidth"] = e.width, i["sparklineHeight"] = e.height);
                         null == i["boolValue"] && null == i["text"] && null == i["image"] && (i["text"] = t), g[o].push(i), o++
                     }
                     if (t) {
                         g.length < c.rows.length + 1 && g.push([]);
                         let t = {};
                         if (t["text"] = "", u.showTotalSummary) {
-                            let e = tg.calculateTotal(u, w, c);
+                            let e = rg.calculateTotal(u, w, c);
                             t["text"] = u.summaryType == Kr.Count ? ae.trunc(e).toString() : ts.formatBasedOnColumnType(m, u, e)
                         }
                         g[g.length - 1].push(t)
                     }
                     w++
                 }
                 return g
@@ -15923,15 +15922,15 @@
                 let t = U.Table.getHeight(m.headerFont, c),
                     e = U.Table.getHeight(m.font, c),
                     S = p.meters.where(e => e.is(Cs)).cast(),
                     r = null != S.firstOrDefault(e => e.showTotalSummary),
                     s = i ? 0 : m.currentPageIndex,
                     n = 0 != m.rowsPerPage && -1 != s,
                     l = 1,
-                    w = (n && (l = Zd.getNumberOfPages(p.rows.length, m.rowsPerPage)) <= 1 && (n = !1), p.rows);
+                    w = (n && (l = Yd.getNumberOfPages(p.rows.length, m.rowsPerPage)) <= 1 && (n = !1), p.rows);
                 if (n) {
                     let e = w.skip(m.rowsPerPage * s).take(m.rowsPerPage);
                     e.any() ? w = e : n = !1
                 }
                 let b = r ? U.Table.getHeight(m.footerFont, c) : 0,
                     a = n ? U.Table.getHeight(m.footerFont, c) : 0,
                     f = b + a,
@@ -15939,50 +15938,50 @@
                     C = [],
                     x = 0;
                 for (let i of S) {
                     i.cache = {};
                     let r = 0,
                         e = await this.getColumnVisibilityState(i, m.report);
                     if (e && (r = this.measureHeader(m, i, c), i.showTotalSummary)) {
-                        let e = tg.calculateTotal(i, x, p),
+                        let e = rg.calculateTotal(i, x, p),
                             t = this.measureFooter(m, i, c, e);
                         r = Math.max(r, t)
                     }
                     y.push(r), x++
                 }
                 let M = h.y + t;
                 if (M < h.bottom - f) {
                     for (let l of w) {
                         let n = e;
                         x = -1;
                         for (let s of S) {
                             x++;
-                            let e = await Yd.getVisible(s, m.report);
+                            let e = await Kd.getVisible(s, m.report);
                             if (!e) continue;
                             let i = y[x];
                             if (s.is($i)) i = this.measureSparklinesCell(c, i);
                             else {
                                 let t = l[x],
                                     r;
                                 if (s.is2(Qi)) r = this.measureIndicatorCell(m, s, c, t);
                                 else if (s.is2(_i)) r = this.measureDataBarsCell(m, s, c, t);
-                                else if (s.is2(Gi)) r = mp.measureBubbleCell(m, s, c, t);
+                                else if (s.is2(Gi)) r = cp.measureBubbleCell(m, s, c, t);
                                 else {
                                     let e = this.measureCommonCell(m, s, c, t, i);
                                     r = e.width, n = Math.max(e.height, n)
                                 }
                                 i = Math.max(i, r)
                             }
                             y[x] = i
                         }
                         if (M + n > h.bottom - f && (n = h.bottom - f - M) < 1.2 && (n = 1.2), C.push(n), (M += n) >= h.bottom - f) break
                     }
                     C.push(e)
                 }
-                if (m.sizeMode == tu.Fit) {
+                if (m.sizeMode == ru.Fit) {
                     let t = h.width / y.sum(),
                         e = ((1 < t || !i) && (y = y.select(e => e * t).toList()), -1);
                     for (let n of w) {
                         if (++e >= C.length) break;
                         x = -1;
                         let s = C[e];
                         for (let i of S) {
@@ -16007,16 +16006,16 @@
                     }
                     let a = y[x];
                     if (d == F.f.StiDashboardExportFormat.Excel && (a *= 1.1), M = h.y, d != F.f.StiDashboardExportFormat.Data) {
                         let e = new j(T, M, a, t);
                         this.renderHeader(u, e, m, o, c, d, g), M += e.height
                     }
                     if (M <= h.bottom - f) {
-                        let s = tg.minDataColumnValue(o, p, x),
-                            n = tg.maxDataColumnValue(o, p, x),
+                        let s = rg.minDataColumnValue(o, p, x),
+                            n = rg.maxDataColumnValue(o, p, x),
                             l = 0;
                         for (let i of w) {
                             let e = Math.ceil(C[l]),
                                 t = this.processRowValue(l, i[x], o),
                                 r = new j(T, M, a, e);
                             if (await this.renderCell(u, r, m, i, S.select(e => e.key), o, c, t, s, n, 1 == (1 & l), d, g), M += e, l++, M >= h.bottom - f) break
                         }
@@ -16034,201 +16033,201 @@
                     this.renderCurrentPageNumber(u, r, m, c, e)
                 }
             }
             static measureSparklinesCell(e, t) {
                 return Math.max(t, 80 * e)
             }
             static measureHeader(e, t, r) {
-                return eg.measureHeader(e, t).width * r
+                return tg.measureHeader(e, t).width * r
             }
             static measureFooter(e, t, r, i) {
                 let s = ts.formatBasedOnColumnType(e, t, i);
-                return eg.measureCell(s, e.footerFont, t).width * r
+                return tg.measureCell(s, e.footerFont, t).width * r
             }
             static measureIndicatorCell(e, t, r, i) {
                 let s = t.as(Qi),
-                    n = Td.getCellText(e, s, V.tryToNullableNumber(i)),
-                    l = eg.measureCell(n, e.font, t).width * r;
+                    n = Fd.getCellText(e, s, V.tryToNullableNumber(i)),
+                    l = tg.measureCell(n, e.font, t).width * r;
                 return l *= 1.25
             }
             static measureDataBarsCell(e, t, r, i) {
                 let s = ts.formatBasedOnColumnType(e, t, i),
-                    n = eg.measureCell(s, e.font, t).width * r;
+                    n = tg.measureCell(s, e.font, t).width * r;
                 return t.horAlignment != z.Center && (n *= 2), n = t.is(_i) && 0 < t.width ? r * t.width : n
             }
             static measureBubbleCell(e, t, r, i) {
                 let s = ts.formatBasedOnColumnType(e, t, i),
-                    n = eg.measureCell(s, e.font, t).width * r,
+                    n = tg.measureCell(s, e.font, t).width * r,
                     l = U.Table.getHeight(e.font, r);
                 if (t.horAlignment == z.Center) return l;
                 return n += l
             }
             static measureCommonCell(e, t, r, i, s) {
-                if (Lu.isImage(i)) return new W(s, 0);
+                if (Bu.isImage(i)) return new W(s, 0);
                 let n = ts.formatBasedOnColumnType(e, t, i),
-                    l = eg.measureCell(n, e.font, t);
+                    l = tg.measureCell(n, e.font, t);
                 return l.width *= r, l.height *= r, l
             }
             static renderHeader(e, t, r, i, s, n, l) {
-                let a = null != i ? kh.getLabel(i) : "",
-                    o = B.isNullOrWhiteSpace(a) ? r.name + `_Column` : $d.correctName(a),
+                let a = null != i ? Nh.getLabel(i) : "",
+                    o = B.isNullOrWhiteSpace(a) ? r.name + `_Column` : eg.correctName(a),
                     u = J.getTableStyle(r),
                     h = 0 != r.columns.indexOf(i) && t.left < e.width && !l,
                     m = r.columns.indexOf(i) != r.columns.length - 1 && t.right <= e.width && !l,
                     c = (h ? G.Left : G.None) | (m ? G.Right : G.None),
                     d = l ? N.black : this.getHeaderForeColor(r),
                     g = l ? N.transparent : u.headerBackColor,
                     p = l ? new H("Arial", 10, hn.Bold) : r.headerFont,
-                    S = new Iu(t);
+                    S = new Du(t);
                 S.name = o, S.allowHtmlTags = !0, S.autoWidth = !1, S.horAlignment = this.getHeaderAlignment(i), S.vertAlignment = Wt.Center, S.wordWrap = !1, S.border = new ie(c, u.lineColor, 1, Ri.Solid), S.brush = new v(g), S.font = U.Table.Font.getGdiFont(s, null, p), S.text = a, S.textFormat = null != i.textFormat ? i.textFormat.clone() : null, S.textBrush = new v(d), S.componentPlacement = `h.` + r.name, e.components.add(S)
             }
             static getHeaderAlignment(e) {
                 if (e.headerAlignment == z.Left) return X.Left;
                 if (e.headerAlignment == z.Right) return X.Right;
                 return X.Center
             }
             static renderFooter(e, t, r, i, s, n, l) {
                 let a = J.getTableStyle(r),
                     o = this.getFooterForeColor(r),
                     u = a.footerColor,
                     h = r.footerFont,
                     m = "",
                     c = 0,
-                    d = (i.showTotalSummary && (c = tg.calculateTotal(i, s, l), m = i.summaryType == Kr.Count ? ae.trunc(c).toString() : ts.formatBasedOnColumnType(r, i, c)), X.Right),
-                    g = (i.summaryAlignment == z.Left ? d = X.Left : i.summaryAlignment == z.Center && (d = X.Center), new Iu(t)),
+                    d = (i.showTotalSummary && (c = rg.calculateTotal(i, s, l), m = i.summaryType == Kr.Count ? ae.trunc(c).toString() : ts.formatBasedOnColumnType(r, i, c)), X.Right),
+                    g = (i.summaryAlignment == z.Left ? d = X.Left : i.summaryAlignment == z.Center && (d = X.Center), new Du(t)),
                     p = (g.name = r.name + `_FooterCell`, null != i.textFormat && i.textFormat.is(Jt) ? null : m);
                 null != i.textFormat && (i.textFormat.is(Jr) || i.textFormat.is(Wr) || i.textFormat.is(Ur)) && (p = c.toString()), g.border = this.getBorderSides(e, t, r, i, G.All), g.brush = new v(u), g.excelDataValue = p, g.font = U.Table.Font.getGdiFont(n, null, h), g.horAlignment = d, g.vertAlignment = Wt.Center, g.text = m, g.textBrush = new v(o), g.textFormat = null != i.textFormat ? i.textFormat.clone() : null, g.wordWrap = !1, g.componentPlacement = `f.` + r.name, e.components.add(g)
             }
             static renderCurrentPageNumber(e, t, r, i, s) {
                 let n = J.getTableStyle(r),
                     l = this.getFooterForeColor(r),
                     a = n.footerColor,
                     o = r.footerFont,
-                    u = new Iu(t);
-                u.name = r.name + `_CurrentPage`, u.brush = new v(a), u.font = U.Table.Font.getGdiFont(i, null, o), u.horAlignment = X.Center, u.vertAlignment = Wt.Center, u.margins = new be(0, 0, 1, 0), u.textQuality = lg.Typographic, u.text = s, u.textBrush = new v(l), u.wordWrap = !1, u.componentPlacement = `f.` + r.name, e.components.add(u)
+                    u = new Du(t);
+                u.name = r.name + `_CurrentPage`, u.brush = new v(a), u.font = U.Table.Font.getGdiFont(i, null, o), u.horAlignment = X.Center, u.vertAlignment = Wt.Center, u.margins = new be(0, 0, 1, 0), u.textQuality = ag.Typographic, u.text = s, u.textBrush = new v(l), u.wordWrap = !1, u.componentPlacement = `f.` + r.name, e.components.add(u)
             }
             static async renderCell(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 let d = J.getTableStyle(r),
                     g = this.getForeColor(r, n, d, h),
-                    p = eg.getBackgroundColor(d, null != h && h);
-                p = 0 < r.tableConditions.length ? await Ad.processBackColor(p, n.key, r, i, s) : p, c ? await this.renderTextCell(e, t, r, i, s, n, l, a, G.None, N.black, N.transparent, m, !0) : n.is2(_i) || n.is2($i) || n.is2(Qi) || n.is2(Gi) ? await this.renderGraphicCell(e, t, r, i, s, n, l, a, o, u, p, d, null != h && h, m) : n.is2(qi) ? await this.drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, d, m) : Lu.isImage(a) ? this.renderImageCell(e, t, r, n, a, p, m) : "boolean" == typeof a ? await this.renderBoolCell2(e, t, r, i, s, n, l, a, g, p, m) : await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, g, p, m, !1)
+                    p = tg.getBackgroundColor(d, null != h && h);
+                p = 0 < r.tableConditions.length ? await Id.processBackColor(p, n.key, r, i, s) : p, c ? await this.renderTextCell(e, t, r, i, s, n, l, a, G.None, N.black, N.transparent, m, !0) : n.is2(_i) || n.is2($i) || n.is2(Qi) || n.is2(Gi) ? await this.renderGraphicCell(e, t, r, i, s, n, l, a, o, u, p, d, null != h && h, m) : n.is2(qi) ? await this.drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, d, m) : Bu.isImage(a) ? this.renderImageCell(e, t, r, n, a, p, m) : "boolean" == typeof a ? await this.renderBoolCell2(e, t, r, i, s, n, l, a, g, p, m) : await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, g, p, m, !1)
             }
             static processRowValue(e, t, r) {
                 var i;
                 let s = r.textFormat,
-                    n = (null != t && t[L.System.StiObject.stimulsoft]().is(_d) && (t = t == _d.Line && null != s ? s.format(e + 1) : es.getSystemVariable(null == t ? void 0 : t[L.System.StiObject.stimulsoft]().as(_d), e + 1)), r.ident == Wu.SparklinesColumn);
-                return t = Xu.isList(t) ? n ? Xu.toList(t) : null == (i = Xu.toList(t)) ? void 0 : i.firstOrDefault() : t
+                    n = (null != t && t[L.System.StiObject.stimulsoft]().is($d) && (t = t == $d.Line && null != s ? s.format(e + 1) : es.getSystemVariable(null == t ? void 0 : t[L.System.StiObject.stimulsoft]().as($d), e + 1)), r.ident == Ju.SparklinesColumn);
+                return t = Wu.isList(t) ? n ? Wu.toList(t) : null == (i = Wu.toList(t)) ? void 0 : i.firstOrDefault() : t
             }
             static async renderGraphicCell(s, n, l, t, r, a, i, o, u, h, m, c, d, g) {
                 let p = "",
                     S = n,
                     w = this.getForeColor(l, a, c, d),
-                    b = new nd(ul.UTF8);
-                if (b.indentation = -1, b.writeStartElement("svg"), b.writeAttributeString("version", "1.1"), b.writeAttributeString("baseProfile", "full"), b.writeAttributeString("xmlns", "http://www.w3.org/2000/svg"), b.writeAttributeString("xmlns:xlink", "http://www.w3.org/1999/xlink"), b.writeAttributeString("xmlns:ev", "http://www.w3.org/2001/xml-events"), b.writeAttributeString("height", ig.toUnits(n.height)), b.writeAttributeString("width", ig.toUnits(n.width)), b.writeStartElement("rect"), b.writeAttributeString("x", "0"), b.writeAttributeString("y", "0"), b.writeAttributeString("width", ig.toUnits(n.width)), b.writeAttributeString("height", ig.toUnits(n.height)), b.writeAttributeString("style", ig.writeFillBrush(b, m, n)), b.writeEndElement(), a.is2($i)) {
-                    let e = Qd.castToArray(o),
+                    b = new ld(ul.UTF8);
+                if (b.indentation = -1, b.writeStartElement("svg"), b.writeAttributeString("version", "1.1"), b.writeAttributeString("baseProfile", "full"), b.writeAttributeString("xmlns", "http://www.w3.org/2000/svg"), b.writeAttributeString("xmlns:xlink", "http://www.w3.org/1999/xlink"), b.writeAttributeString("xmlns:ev", "http://www.w3.org/2001/xml-events"), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeStartElement("rect"), b.writeAttributeString("x", "0"), b.writeAttributeString("y", "0"), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("style", sg.writeFillBrush(b, m, n)), b.writeEndElement(), a.is2($i)) {
+                    let e = qd.castToArray(o),
                         t = null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toList().select(e => null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toNumber()),
                         r = a.as($i),
-                        i = new qd(n);
+                        i = new _d(n);
                     return i.values = t, i.positiveColor = r.allowCustomColors ? r.positiveColor : c.cellSparkline, i.negativeColor = r.allowCustomColors ? r.negativeColor : c.cellWinLossNegative, i.showFirstLastPoints = r.showFirstLastPoints, i.showHighLowPoints = r.showHighLowPoints, i.type = r.type, i.brush = new v(m), i.componentPlacement = `d.` + l.name, void s.components.add(i)
                 }
-                let f = new sg(b),
+                let f = new ng(b),
                     y = G.None,
                     C = "GraphicCell",
                     x = new j(0, 0, n.width, n.height),
                     M = a.horAlignment;
                 if (a.is2(_i)) {
-                    await rg.draw(f, x, l, t, r, a, i, V.tryToNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = rg.calculateTextRect(n.clone(), a)).inflate(2, 2), p = ts.formatBasedOnColumnType(l, a, o), w = rg.getForeColor(l, a, c, d, !1);
+                    await ig.draw(f, x, l, t, r, a, i, V.tryToNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = ig.calculateTextRect(n.clone(), a)).inflate(2, 2), p = ts.formatBasedOnColumnType(l, a, o), w = ig.getForeColor(l, a, c, d, !1);
                     let e = V.tryToNumber(o);
-                    e < 0 && gh.isNegativeInRed(a.textFormat) && (w = Z.Engine.negativeColor), w = 0 < l.tableConditions.length ? await Ad.processForeColor(w, a.key, l, t, r) : w, y = G.Right, C = "DataBarsCell"
-                } else if (a.is2(Qi)) Td.draw(f, x, l, a, i, V.tryToNullableNumber(o), c, !1), S = Td.calculateTextRect(n.clone(), a), p = Td.getCellText(l, a, V.tryToNullableNumber(o)), w = Td.getColor(a, V.tryToNullableNumber(o), c), w = 0 < l.tableConditions.length ? await Ad.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "IndicatorCell";
+                    e < 0 && ph.isNegativeInRed(a.textFormat) && (w = Z.Engine.negativeColor), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.Right, C = "DataBarsCell"
+                } else if (a.is2(Qi)) Fd.draw(f, x, l, a, i, V.tryToNullableNumber(o), c, !1), S = Fd.calculateTextRect(n.clone(), a), p = Fd.getCellText(l, a, V.tryToNullableNumber(o)), w = Fd.getColor(a, V.tryToNullableNumber(o), c), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "IndicatorCell";
                 else if (a.is2(Gi)) {
-                    Kd.draw(f, x, l, a, i, V.tryToNullableNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = Kd.calculateTextRect(l, n.clone(), a)).inflate(2, 2), p = Kd.getCellText(l, a, V.tryToNullableNumber(o)), w = rg.getForeColor(l, a, c, d, !1), w = 0 < l.tableConditions.length ? await Ad.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "BubbleCell";
+                    Qd.draw(f, x, l, a, i, V.tryToNullableNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = Qd.calculateTextRect(l, n.clone(), a)).inflate(2, 2), p = Qd.getCellText(l, a, V.tryToNullableNumber(o)), w = ig.getForeColor(l, a, c, d, !1), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "BubbleCell";
                     let e = a[L.System.StiObject.stimulsoft]().as(Cr);
                     null != e && (e.horAlignment == z.Center && g != F.f.StiDashboardExportFormat.Data && (p = null), e.horAlignment == z.Left && (M = z.Right), e.horAlignment == z.Right) && (M = z.Left)
                 }
                 if (b.writeFullEndElement(), b.flush(), g != F.f.StiDashboardExportFormat.Data && !a.is2($i)) {
-                    let e = new ld(n),
+                    let e = new ad(n),
                         t = (e.name = l.name + `_` + C, e.border = this.getBorderSides(s, n, l, a, G.All), e.stretch = !0, e.aspectRatio = a.is2(Qi) || a.is2(Gi), b.textWriter.getStringBuilder().toString());
-                    e.image = Ba.stringToImage(L.System.Convert.toBase64String(t)), e.brush = new v(m), e.horAlignment = M, s.components.add(e)
+                    e.image = Pa.stringToImage(L.System.Convert.toBase64String(t)), e.brush = new v(m), e.horAlignment = M, s.components.add(e)
                 }
                 g != F.f.StiDashboardExportFormat.Data && B.isNullOrEmpty(p) || await this.renderTextCell(s, S, l, t, r, a, i, o, y, w, m, g, !1, !1)
             }
             static async drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, h, m) {
                 let c = n.as(qi),
                     d = this.getForeColor(r, n, h, !1),
-                    g = ng.getScaleColor(V.tryToNumber(a), o, u, h, c.minimumColor, c.maximumColor),
-                    p = r.tableConditions.length ? await Ad.processForeAndBackColor(d, g, n.key, r, i, s) : {
+                    g = lg.getScaleColor(V.tryToNumber(a), o, u, h, c.minimumColor, c.maximumColor),
+                    p = r.tableConditions.length ? await Id.processForeAndBackColor(d, g, n.key, r, i, s) : {
                         foreColor: d,
                         backColor: g
                     };
                 await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, p.foreColor, p.backColor, m, !1)
             }
             static async renderBoolCell2(i, s, n, l, a, o, e, u, h, m, t) {
                 if (t == F.f.StiDashboardExportFormat.Data) await this.renderTextCell(i, s, n, l, a, o, e, u, G.None, h, m, t, !1);
                 else {
-                    let e = 0 < n.tableConditions.length ? await Ad.processForeAndBackColor(h, m, o.key, n, l, a) : {
+                    let e = 0 < n.tableConditions.length ? await Id.processForeAndBackColor(h, m, o.key, n, l, a) : {
                             foreColor: h,
                             backColor: m
                         },
-                        t = u ? Bd.CheckRectangle : Bd.NoneRectangle,
-                        r = new Ld(s);
-                    r.name = n.name + `_Cell`, r.border = this.getBorderSides(i, s, n, o, G.All), r.contourColor = N.transparent, r.textBrush = new v(e.foreColor), r.brush = new v(e.backColor), r.checkStyleForTrue = t, r.checkStyleForFalse = Bd.NoneRectangle, r.checkedValue = t != Bd.NoneRectangle, r.excelDataValue = u.toString(), r.componentPlacement = `d.` + n.name, i.components.add(r)
+                        t = u ? Pd.CheckRectangle : Pd.NoneRectangle,
+                        r = new Bd(s);
+                    r.name = n.name + `_Cell`, r.border = this.getBorderSides(i, s, n, o, G.All), r.contourColor = N.transparent, r.textBrush = new v(e.foreColor), r.brush = new v(e.backColor), r.checkStyleForTrue = t, r.checkStyleForFalse = Pd.NoneRectangle, r.checkedValue = t != Pd.NoneRectangle, r.excelDataValue = u.toString(), r.componentPlacement = `d.` + n.name, i.components.add(r)
                 }
             }
             static async renderTextCell(e, t, s, n, l, r, i, a, o, u, h, m, c, d = null) {
                 var g;
                 let p = ts.formatBasedOnColumnType(s, r, a),
                     S = c ? new H("Arial", 10) : s.font,
-                    w = (r.is(rs) && r.showHyperlink && (S = new H(S.fontFamily.name, S.size, S.style | hn.Underline)), 0 < s.tableConditions.length ? await Ad.processFontStyle(S, r.key, s, n, l) : hn.Regular),
+                    w = (r.is(rs) && r.showHyperlink && (S = new H(S.fontFamily.name, S.size, S.style | hn.Underline)), 0 < s.tableConditions.length ? await Id.processFontStyle(S, r.key, s, n, l) : hn.Regular),
                     b = (S = new H(S.fontFamily.name, S.size, w), V.tryToNumber(a));
-                if (b < 0 && gh.isNegativeInRed(r.textFormat) && (u = Z.Engine.negativeColor), r.is($i)) {
-                    let e = Qd.castToArray(a),
+                if (b < 0 && ph.isNegativeInRed(r.textFormat) && (u = Z.Engine.negativeColor), r.is($i)) {
+                    let e = qd.castToArray(a),
                         t = null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toList().select(e => e.toString());
                     p = B.join(" ", t)
                 }
-                let f = 0 < s.tableConditions.length ? await Ad.processForeAndBackColor(u, h, r.key, s, n, l) : {
+                let f = 0 < s.tableConditions.length ? await Id.processForeAndBackColor(u, h, r.key, s, n, l) : {
                         foreColor: u,
                         backColor: h
                     },
-                    y = pd.convert(r.horAlignment),
+                    y = Sd.convert(r.horAlignment),
                     C = (r.is(Gi) && (y = X.Right), r.as(mi)),
                     x = (null != C && null == d && (d = C.size.wordWrap), null);
                 if (r.is(rs) && r.showHyperlink && !B.isNullOrWhiteSpace(r.hyperlinkPattern)) {
                     let i = new L.System.Collections.Hashtable;
                     i.add("Value", a);
                     for (let r = 0; r < l.length; r++) {
                         let e = s.columns.firstOrDefault(e => e.key == l[r]),
-                            t = "Row." + $d.correctName(e.label, !0);
+                            t = "Row." + eg.correctName(e.label, !0);
                         i.add(t, null == (g = n[r]) ? void 0 : g.toString())
                     }
                     x = await L.Report.Dashboard.StiReportParser.parseAsync(r.hyperlinkPattern, s, !1, i)
                 }
                 let M = null != r.textFormat && r.textFormat.is(Jt) ? null : p,
-                    T = (null != a && null != r.textFormat && (r.textFormat.is(Jr) || r.textFormat.is(Wr) || r.textFormat.is(Ur)) && (M = a.toString()), new Iu(t));
-                T.name = s.name + `_Cell`, T.border = this.getBorderSides(e, t, s, r, o), T.brush = new v(f.backColor), T.excelDataValue = M, T.font = U.Table.Font.getGdiFont(i, null, S), T.horAlignment = y, T.vertAlignment = Wt.Center, T.text = p, T.textBrush = new v(f.foreColor), T.textFormat = null != r.textFormat ? r.textFormat.clone() : null, T.wordWrap = 0 != d, T.componentPlacement = `d.` + s.name, T.trimming = Du.EllipsisCharacter, T.hyperlinkValue = x, e.components.add(T)
+                    T = (null != a && null != r.textFormat && (r.textFormat.is(Jr) || r.textFormat.is(Wr) || r.textFormat.is(Ur)) && (M = a.toString()), new Du(t));
+                T.name = s.name + `_Cell`, T.border = this.getBorderSides(e, t, s, r, o), T.brush = new v(f.backColor), T.excelDataValue = M, T.font = U.Table.Font.getGdiFont(i, null, S), T.horAlignment = y, T.vertAlignment = Wt.Center, T.text = p, T.textBrush = new v(f.foreColor), T.textFormat = null != r.textFormat ? r.textFormat.clone() : null, T.wordWrap = 0 != d, T.componentPlacement = `d.` + s.name, T.trimming = Ru.EllipsisCharacter, T.hyperlinkValue = x, e.components.add(T)
             }
             static renderImageCell(e, t, r, i, s, n, l) {
                 if (l == F.f.StiDashboardExportFormat.Data) return;
-                let a = Lu.getImageFromObject(s);
+                let a = Bu.getImageFromObject(s);
                 if (null == a) return;
-                let o = new ld(t);
+                let o = new ad(t);
                 o.name = r.name + `_Cell`, o.border = this.getBorderSides(e, t, r, i, G.All), o.brush = new v(n), o.stretch = !0, o.aspectRatio = !0, o.imageToDraw = a, o.horAlignment = i.horAlignment, e.components.add(o)
             }
             static async renderBoolCell(e, t, r, i, s, n, l, a, o, u, h) {
                 if (h == F.f.StiDashboardExportFormat.Data) return void await this.renderTextCell(e, t, r, i, s, n, l, a, o, null, u, h, !1);
                 let m = 0 != r.columns.indexOf(n),
                     c = r.columns.indexOf(n) != r.columns.length - 1,
                     d = (m ? G.Left : G.None) | (c ? G.Right : G.None),
                     g = J.getTableStyle(r),
-                    p = new ld(t);
+                    p = new ad(t);
                 p.name = r.name + `_Cell`, p.border = o ? new ie(d, g.lineColor, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), p.brush = new v(u), p.horAlignment = z.Center, p.vertAlignment = Wt.Center, e.components.add(p)
             }
             static async getColumnVisibilityState(e, t) {
                 if (e.visibility == Hr.TrueAndHidden) return !1;
-                return Yd.getVisible(e, t)
+                return Kd.getVisible(e, t)
             }
             static getForeColor(e, t, r, i) {
                 if (!N.transparent.equals(t.foreColor)) return t.foreColor;
                 if (t.is(rs) && t.showHyperlink) return vr.get("165dc8");
                 let s = jl.getForeColor(e, e.foreColor);
                 if (!N.transparent.equals(s)) return s;
                 return null != r ? i ? r.alternatingCellForeColor : r.cellForeColor : U.Table.Font.Color
@@ -16249,142 +16248,142 @@
                     a = 0 != (s & G.Right) && r.columns.indexOf(i) != r.columns.length - 1 && t.right <= e.width,
                     o = (l ? G.Left : G.None) | (a ? G.Right : G.None),
                     u = o != G.None ? 1 : 0,
                     h = o != G.None ? n.lineColor : N.transparent;
                 return new ie(o, h, u, Ri.Solid)
             }
         }
-        F.A.StiTableElementExportTool = mp
+        F.A.StiTableElementExportTool = cp
     }
-    let ag = F.h.StiAutoSizeHtmlTextHelper,
-        og = (F.A.StiTextElementExportTool = class extends F.A.StiElementExportTool {
+    let og = F.h.StiAutoSizeHtmlTextHelper,
+        ug = (F.A.StiTextElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, s, r) {
                 if (this.renderEmptyDataMessage(e, t, s.clone(), r)) return;
-                let n = e.as(bm),
+                let n = e.as(fm),
                     l = "";
-                if (Z.Engine.dashboardTextElementExpressionParser == lu.ReportParser || Rs.isTimeExpression(n.text)) l = await O.parseAsync(n.text, n, !1);
+                if (Z.Engine.dashboardTextElementExpressionParser == au.ReportParser || Rs.isTimeExpression(n.text)) l = await O.parseAsync(n.text, n, !1);
                 else if (n.isQuerable) {
                     let e = await bl.tryToGetOrCreate(n),
                         t = new P(null == e ? void 0 : e.rows.firstOrDefault()).select(e => V.tryToString(e)).toList();
                     null != t && (l = Rs.replaceExpressionBlocksByValues(n.text, t))
                 } else l = n.text;
                 if (!B.isNullOrEmpty(l) && l.toLowerCase()[L.System.StiObject.stimulsoft]().replaceAll(" ", "")[L.System.StiObject.stimulsoft]().contains("javascript:") && (l = l.toLowerCase()[L.System.StiObject.stimulsoft]().replaceAll("javascript", "")), n.sizeMode == Dt.Fit) {
                     let i, e = 3;
                     do {
-                        let e = ag.measure(null, s.clone(), l, n),
+                        let e = og.measure(null, s.clone(), l, n),
                             t = e.width > s.width ? s.width / e.width : 1,
                             r = e.height > s.height ? s.height / e.height : 1;
                         (i = Math.min(Math.abs(t), Math.abs(r))) < 1 && (l = this.changeFontSize(l, .99 * i))
                     } while (i < 1 && 0 < e--)
                 }
-                let i = new Iu(s);
-                i.name = e.name + `_Content`, i.allowHtmlTags = !0, i.vertAlignment = n.vertAlignment, i.horAlignment = n.horAlignment, i.text = l, i.textBrush = new v(J.getForeColor(n)), i.trimming = n.sizeMode == Dt.Trimming ? Du.EllipsisCharacter : Du.None, i.wordWrap = n.sizeMode == Dt.WordWrap, t.components.add(i)
+                let i = new Du(s);
+                i.name = e.name + `_Content`, i.allowHtmlTags = !0, i.vertAlignment = n.vertAlignment, i.horAlignment = n.horAlignment, i.text = l, i.textBrush = new v(J.getForeColor(n)), i.trimming = n.sizeMode == Dt.Trimming ? Ru.EllipsisCharacter : Ru.None, i.wordWrap = n.sizeMode == Dt.WordWrap, t.components.add(i)
             }
             changeFontSize(e, t) {
                 if (null == e || !e[L.System.StiObject.stimulsoft]().startsWith("<font ") || e.indexOf(' size="') < 0) return e;
                 let r = e.indexOf(' size="') + 7,
                     i = e.substring(r),
                     s = (i = i.substring(0, i.indexOf('"')))[L.System.StiObject.stimulsoft]().toNumber();
                 return null == s && (s = 12), s = Math.ceil(s * t * 10) / 10, e.substring(0, r) + s.toString().replace(",", ".") + e.substring(r + i.length)
             }
         }, F.A.StiTreeViewBoxElementExportTool = class extends F.A.StiComboBoxElementExportTool {
             async render(e, t, r, i) {
                 return super.render(e, t, r, i)
             }
             getValuesCount(e, t) {
-                let r = e.as(wu),
-                    i = Su.fetchItems(t, r.showBlanks);
+                let r = e.as(bu),
+                    i = wu.fetchItems(t, r.showBlanks);
                 return null != i ? i.length : 0
             }
         }, L.Report.Components.StiShapeDirection),
-        ug = L.Report.Components.StiTriangleShapeType;
+        hg = L.Report.Components.StiTriangleShapeType;
     {
-        class cp extends F.A.StiListBoxElementExportTool {
+        class dp extends F.A.StiListBoxElementExportTool {
             async render(e, t, r, i) {
                 return super.render(e, t, r, i)
             }
             getCheckStyle(t, r) {
                 let e = t;
-                if (!e.userFilters.any()) return Bd.CheckRectangle;
-                if (e.userFilters.any(e => e.condition == Zi.IsFalse)) return Bd.NoneRectangle;
+                if (!e.userFilters.any()) return Pd.CheckRectangle;
+                if (e.userFilters.any(e => e.condition == Zi.IsFalse)) return Pd.NoneRectangle;
                 if (null != r.items) {
                     let e = r.items.select(e => this.getCheckStyle(t, e));
-                    if (e.all(e => e == Bd.CheckRectangle)) return Bd.CheckRectangle;
-                    if (e.all(e => e == Bd.NoneRectangle)) return Bd.NoneRectangle;
-                    return Bd.DotRectangle
+                    if (e.all(e => e == Pd.CheckRectangle)) return Pd.CheckRectangle;
+                    if (e.all(e => e == Pd.NoneRectangle)) return Pd.NoneRectangle;
+                    return Pd.DotRectangle
                 }
-                if (e.userFilters.any(e => e.condition == Zi.EqualTo && e.value == r.toString())) return Bd.CheckRectangle;
-                return Bd.NoneRectangle
+                if (e.userFilters.any(e => e.condition == Zi.EqualTo && e.value == r.toString())) return Pd.CheckRectangle;
+                return Pd.NoneRectangle
             }
             async renderItems(e, t, r) {
                 var i;
                 let s = await bl.tryToGetOrCreate(r);
                 if (null == s) return;
                 let n = !1,
-                    l = r.as(du),
-                    a = Su.fetchItems(s, l.showBlanks),
+                    l = r.as(gu),
+                    a = wu.fetchItems(s, l.showBlanks),
                     o = (1 == (null === a || void 0 === a ? void 0 : a.length) && 0 < (null == (i = a[0].items) ? void 0 : i.length) && (a = a.concat(a[0].items), n = !0), null === a || void 0 === a ? void 0 : a.select(e => null == e ? "" : null != e.key && e.key instanceof w ? e.key.toShortDateString() : e.toString())),
                     u = null === a || void 0 === a ? void 0 : a.select(e => this.getCheckStyle(r, e)),
                     h = null === a || void 0 === a ? void 0 : a.select(e => n && e == a.first());
                 this.renderItems2(e, t.clone(), r, o, u, h)
             }
             renderItem(e, t, r, i, s, n, l, a, o) {
-                i != Od.locAll && (cp.renderExpander(e, t.clone(), r, o), t.x += U.ListBox.CheckBoxWidth / 2, t.width -= U.ListBox.CheckBoxWidth / 2), super.renderItem(e, t.clone(), r, i, s, n, l, a, o)
+                i != Vd.locAll && (dp.renderExpander(e, t.clone(), r, o), t.x += U.ListBox.CheckBoxWidth / 2, t.width -= U.ListBox.CheckBoxWidth / 2), super.renderItem(e, t.clone(), r, i, s, n, l, a, o)
             }
             static renderExpander(e, t, r, i) {
                 t = new j(t.x, t.y + t.height / 2 - t.height / 8, U.ListBox.CheckBoxWidth / 3, t.height / 4);
-                let s = new Fc(t);
-                s.name = r.name + `_ItemExpander`, s.shapeType = new ug(i ? og.Down : og.Right), s.brush = new v(N.dimGray), s.style = Ri.None, e.components.add(s)
+                let s = new vc(t);
+                s.name = r.name + `_ItemExpander`, s.shapeType = new hg(i ? ug.Down : ug.Right), s.brush = new v(N.dimGray), s.style = Ri.None, e.components.add(s)
             }
         }
-        F.A.StiTreeViewElementExportTool = cp
+        F.A.StiTreeViewElementExportTool = dp
     }
-    let hg = L.Report.Components.StiHorizontalLinePrimitive;
+    let mg = L.Report.Components.StiHorizontalLinePrimitive;
     F.A.StiWebContentElementExportTool = class extends F.A.StiElementExportTool {
         async render(e, i, s, t) {
             if (this.renderEmptyDataMessage(e, i, s.clone(), t)) return;
-            let n = e.as(hm),
+            let n = e.as(mm),
                 l = B.isNullOrEmpty(n.url) ? "EmbedCode" : "URL",
                 a = B.isNullOrEmpty(n.url) ? n.embedCode : n.url;
-            if (null != t && t.is(Hc) && t.designMode) {
+            if (null != t && t.is(zc) && t.designMode) {
                 let e = 30,
                     t = 1,
                     r = 20;
                 this.paintHeader(i, n, new j(s.x, s.top, s.width, e), l), this.paintSeparator(i, n, new j(s.x + r, s.top + e, s.width - 2 * r, t)), this.paintWebContent(i, n, new j(s.x, s.top + e + t, s.width, e), a, !0)
             } else this.paintWebContent(i, n, new j(s.x, s.top, s.width, s.height), a)
         }
         paintHeader(e, t, r, i) {
             let s = J.getForeColor(t),
-                n = new Iu(r);
+                n = new Du(r);
             n.name = t.name + `__WebContentHeader`, n.vertAlignment = Wt.Center, n.horAlignment = X.Left, n.textBrush = new v(s), n.brush = new v(N.transparent), n.margins = new be(20, 0, 0, 0), n.text = i, n.font = new H("Arial", 8, hn.Bold), e.components.add(n)
         }
         paintSeparator(e, t, r) {
             let i = J.getForeColor(t),
-                s = new hg(r);
+                s = new mg(r);
             s.name = t.name + `_WebContentSep`, s.color = i, e.components.add(s)
         }
         paintWebContent(e, t, r, i, s = !1) {
             let n = J.getForeColor(t),
-                l = new Iu(r);
+                l = new Du(r);
             l.name = t.name + `__WebContentContent`, l.vertAlignment = s ? Wt.Center : Wt.Top, l.horAlignment = X.Left, l.textBrush = new v(n), l.brush = new v(N.transparent), l.margins = new be(s ? 20 : 0, 0, 0, 0), l.text = i, l.font = new H("Arial", 8, hn.Bold), l.allowHtmlTags = !s, e.components.add(l)
         }
     };
     {
-        class dp {
+        class gp {
             static run(i, s) {
-                if (void 0 === i) return void dp.run(L, "Stimulsoft");
+                if (void 0 === i) return void gp.run(L, "Stimulsoft");
                 if ("Stimulsoft.ExternalLibrary" == s || "Stimulsoft.Blockly" == s) return;
                 s = s.replace("Stimulsoft.System", "System");
                 for (let r in i) {
                     let e = i[r],
                         t = typeof e;
-                    "function" == t ? (e.ssTypeName = r, e.ssNamespace = s) : "object" == t && dp.run(e, s + `.` + r)
+                    "function" == t ? (e.ssTypeName = r, e.ssNamespace = s) : "object" == t && gp.run(e, s + `.` + r)
                 }
             }
         }
-        F.c.StiTypesHelper = dp
+        F.c.StiTypesHelper = gp
     }
     return F.c.StiTypesHelper.run(), {
         Stimulsoft: L,
         StiOptions: Z
     }
 });
```

### Comparing `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/PKG-INFO` & `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft-dashboards
-Version: 2024.2.4
+Version: 2024.2.5
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/SOURCES.txt` & `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

