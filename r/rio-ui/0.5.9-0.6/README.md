# Comparing `tmp/rio_ui-0.5.9.tar.gz` & `tmp/rio_ui-0.6.tar.gz`

## Comparing `rio_ui-0.5.9.tar` & `rio_ui-0.6.tar`

### file list

```diff
@@ -1,343 +1,361 @@
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.prettierrc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.python-version
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.sassrc
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 rio_ui-0.5.9/README-DEV.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.5.9/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 rio_ui-0.5.9/package.json
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 rio_ui-0.5.9/requirements-dev.lock
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rio_ui-0.5.9/requirements.lock
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.5.9/vite.config.js
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/index.html
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/layouting.ts
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/utils.ts
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/button.ts
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/card.ts
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13816 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/debuggerConnector.ts
--rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11000 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/html.ts
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    27578 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    20315 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/website.ts
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/fonts.scss
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    63395 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/style.scss
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/icon_search.py
--rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/pack.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/webgl.html
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/__main__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/index.html
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/script.ts
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/styles.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/benchmark.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/check_docs.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/code_coverage.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/publish_new_release.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/__main__.py
--rw-r--r--   0        0        0    18767 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/app.py
--rw-r--r--   0        0        0    32239 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/app_server.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/byte_serving.py
--rw-r--r--   0        0        0    19606 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/color.py
--rw-r--r--   0        0        0     9924 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/common.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cursor_style.py
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/dataclass.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/errors.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/event.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/global_state.py
--rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/icon_registry.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/inspection.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/py.typed
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/self_serializing.py
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/serialization.py
--rw-r--r--   0        0        0    76883 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/session.py
--rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/state_properties.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/text_style.py
--rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/theme.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/world_units.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/README.md
--rw-r--r--   0        0        0   557380 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
--rw-r--r--   0        0        0   401608 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
--rw-r--r--   0        0        0   403724 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
--rw-r--r--   0        0        0   556216 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/OFL.txt
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/__init__.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/project.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22196 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/app_root.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/auto_form.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/banner.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/build_failed.py
--rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/button.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/card.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/class_container.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/color_picker.py
--rw-r--r--   0        0        0    26038 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/component.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/component_tree.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/devel_component.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/drawer.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/dropdown.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/flow_container.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/grid.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/html.py
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/icon.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/image.py
--rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/labeled_column.py
--rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/linear_containers.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/link.py
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/list_items.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/list_view.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/markdown.py
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/media_player.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/node_input.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/node_output.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/number_input.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/overlay.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/page_view.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/plot.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/popup.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/progress_circle.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/rectangle.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/revealer.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/root_components.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/separator.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/slider.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/slideshow.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/spacer.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/stack.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switch.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switcher.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/table.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/text.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/text_input.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/tooltip.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/__init__.py
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/validator.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/__init__.py
--rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/component_details.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/debugger.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/deploy_page.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/docs_page.py
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/icons_page.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/project_page.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/sample_icons_grid.py
--rw-r--r--   0        0        0    16597 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/tree_page.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/docs/__init__.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/docs/custom.py
--rw-r--r--   0        0        0   942785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/generated/index.html
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/README.md
--rw-r--r--   0        0        0    12479 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_app_build.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_custom_components.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_project_templates.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_reconciliation.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_refresh.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_session.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_state_bindings.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_user_settings.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/utils.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rio_ui-0.5.9/LICENSE.txt
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 rio_ui-0.5.9/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 rio_ui-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 rio_ui-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.6/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.6/.sassrc
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 rio_ui-0.6/README-DEV.md
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 rio_ui-0.6/devel.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.6/package.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.6/vite.config.js
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/index.html
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20600 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0    13885 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    20143 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/code/components/website.ts
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/css/fonts.scss
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    50530 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.6/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/commits.py
+-rw-r--r--   0        0        0    14388 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/db_wrap.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/icon_search.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/pack.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/webgl.html
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/node_editor/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/node_editor/index.html
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/node_editor/script.ts
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 rio_ui-0.6/prototyping/node_editor/styles.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.6/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/__main__.py
+-rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/app.py
+-rw-r--r--   0        0        0    32393 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/app_server.py
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/byte_serving.py
+-rw-r--r--   0        0        0    19392 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/color.py
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/common.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cursor_style.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/dataclass.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/errors.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/event.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/global_state.py
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/py.typed
+-rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/self_serializing.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/serialization.py
+-rw-r--r--   0        0        0    79493 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/session.py
+-rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/state_properties.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/text_style.py
+-rw-r--r--   0        0        0    25816 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/theme.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/world_units.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0   557380 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
+-rw-r--r--   0        0        0   401608 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   403724 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
+-rw-r--r--   0        0        0   556216 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/OFL.txt
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/project.py
+-rw-r--r--   0        0        0    12858 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/app_root.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/banner.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/build_failed.py
+-rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/button.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/card.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/class_container.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26338 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/component.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/drawer.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/grid.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/html.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/icon.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/image.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/link.py
+-rw-r--r--   0        0        0    10119 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/list_items.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/list_view.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/markdown.py
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/media_player.py
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/node_output.py
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/number_input.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/overlay.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/page_view.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/plot.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/popup.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/revealer.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/root_components.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/separator.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/slider.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/spacer.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/stack.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/switch.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/switcher.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/table.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/text.py
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/text_input.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/tooltip.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/validator.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/__init__.py
+-rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/component_details.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/debugger.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/deploy_page.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/sample_icons_grid.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/debug/client_side_debugger/tree_page.py
+-rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/docs/__init__.py
+-rw-r--r--   0        0        0   418612 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/generated/index.html
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/README.md
+-rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/benchmark.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/check_docs.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 rio_ui-0.6/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_app_build.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_project_templates.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_refresh.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_session.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_user_settings.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.6/tests/utils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.6/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.6/LICENSE.txt
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 rio_ui-0.6/README.md
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 rio_ui-0.6/pyproject.toml
+-rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 rio_ui-0.6/PKG-INFO
```

### Comparing `rio_ui-0.5.9/frontend/index.html` & `rio_ui-0.6/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/app.ts` & `rio_ui-0.6/frontend/code/app.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import { getComponentByElement } from './componentManagement';
 import { updateLayout } from './layouting';
 import { callRemoteMethodDiscardResponse, initWebsocket } from './rpc';
+import { scrollToUrlFragment } from './utils';
 
 // Most of these don't have to be available in the global scope, however, since
 // these are injected by Python after the build process, there have been issues
 // with some build tool inlining their placeholders, which in turn lead to
 // incorrect code.
 //
 // Assigning them to `globalThis` convinces the build tool to leave them alone.
@@ -50,14 +51,21 @@
 
 const SCROLL_BAR_SIZE_IN_PIXELS = getScrollBarWidthInPixels();
 
 export let pixelsPerRem = 16;
 export let scrollBarSize = SCROLL_BAR_SIZE_IN_PIXELS / pixelsPerRem;
 
 function main(): void {
+    if (typeof globalThis.PING_PONG_INTERVAL_SECONDS !== 'number') {
+        console.error(
+            `Received erroneous HTML from the server: The ping pong interval is ${globalThis.PING_PONG_INTERVAL_SECONDS} instead of a number`
+        );
+        return;
+    }
+
     // Display a warning if running in debug mode
     if (globalThis.RIO_DEBUG_MODE) {
         console.warn(
             'Rio is running in DEBUG mode.\nDebug mode includes helpful tools' +
                 ' for development, but is slower and disables some safety checks.' +
                 ' Never use it in production!'
         );
@@ -109,12 +117,15 @@
                 rootElement as HTMLElement
             );
             rootInstance.makeLayoutDirty();
             updateLayout();
         }
     });
 
+    // If the URL fragment changes, scroll to the corresponding element
+    window.addEventListener('hashchange', scrollToUrlFragment);
+
     // Connect to the websocket
     initWebsocket();
 }
 
 main();
```

### Comparing `rio_ui-0.5.9/frontend/code/colorConversion.ts` & `rio_ui-0.6/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/componentManagement.ts` & `rio_ui-0.6/frontend/code/componentManagement.ts`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import { ButtonComponent } from './components/button';
 import { CardComponent } from './components/card';
 import { ClassContainerComponent } from './components/classContainer';
 import { CodeExplorerComponent } from './components/codeExplorer';
 import { ColorPickerComponent } from './components/colorPicker';
 import { ColumnComponent, RowComponent } from './components/linearContainers';
 import { ComponentBase, ComponentState } from './components/componentBase';
-import { ComponentId } from './models';
+import { ComponentId } from './dataModels';
 import { ComponentTreeComponent } from './components/componentTree';
 import { CustomListItemComponent } from './components/customListItem';
 import { DebuggerConnectorComponent } from './components/debuggerConnector';
 import { DrawerComponent } from './components/drawer';
 import { DropdownComponent } from './components/dropdown';
 import { FlowComponent as FlowContainerComponent } from './components/flowContainer';
 import { FundamentalRootComponent } from './components/fundamentalRootComponent';
@@ -33,15 +33,15 @@
 import { OverlayComponent } from './components/overlay';
 import { PlaceholderComponent } from './components/placeholder';
 import { PlotComponent } from './components/plot';
 import { PopupComponent } from './components/popup';
 import { ProgressBarComponent } from './components/progressBar';
 import { ProgressCircleComponent } from './components/progressCircle';
 import { RectangleComponent } from './components/rectangle';
-import { reprElement } from './utils';
+import { reprElement, scrollToUrlFragment } from './utils';
 import { RevealerComponent } from './components/revealer';
 import { ScrollContainerComponent } from './components/scrollContainer';
 import { ScrollTargetComponent } from './components/scrollTarget';
 import { SeparatorComponent } from './components/separator';
 import { SeparatorListItemComponent } from './components/separatorListItem';
 import { SliderComponent } from './components/slider';
 import { SlideshowComponent } from './components/slideshow';
@@ -236,15 +236,15 @@
         let marginId = (componentId * -10) as ComponentId;
         message[marginId] = {
             _type_: 'Margin-builtin',
             _python_type_: 'Margin (injected)',
             _key_: null,
             _margin_: [0, 0, 0, 0],
             _size_: [0, 0],
-            _grow_: entireState['_grow_'],
+            _grow_: entireState._grow_,
             _rio_internal_: true,
             // @ts-ignore
             content: resultId,
             margin_left: margin[0],
             margin_top: margin[1],
             margin_right: margin[2],
             margin_bottom: margin[3],
@@ -260,16 +260,16 @@
     if (align[0] !== null || align[1] !== null) {
         let alignId = (componentId * -10 - 1) as ComponentId;
         message[alignId] = {
             _type_: 'Align-builtin',
             _python_type_: 'Align (injected)',
             _key_: null,
             _margin_: [0, 0, 0, 0],
-            _size_: entireState['_size_'],
-            _grow_: entireState['_grow_'],
+            _size_: [0, 0],
+            _grow_: entireState._grow_,
             _rio_internal_: true,
             // @ts-ignore
             content: resultId,
             align_x: align[0],
             align_y: align[1],
         };
         resultId = alignId;
@@ -507,14 +507,20 @@
             delete componentsById[comp.id];
             componentsByElement.delete(comp.element);
         }
     }
 
     // Update the layout
     updateLayout();
+
+    // If this is the first time, check if there's an #url-fragment and scroll
+    // to it
+    if (rootComponentId !== null) {
+        scrollToUrlFragment();
+    }
 }
 
 function canHaveKeyboardFocus(instance: ComponentBase): boolean {
     // @ts-expect-error
     return typeof instance.grabKeyboardFocus === 'function';
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/cssUtils.ts` & `rio_ui-0.6/frontend/code/cssUtils.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { Color, Fill, TextStyle } from './models';
+import { Color, Fill, TextStyle } from './dataModels';
 
 export function colorToCssString(color: Color): string {
     const [r, g, b, a] = color;
     return `rgba(${r * 255}, ${g * 255}, ${b * 255}, ${a})`;
 }
 
 function gradientToCssString(
@@ -76,96 +76,113 @@
     'text-style': string;
     'text-decoration': string;
     'text-transform': string;
     color: string;
     background: string;
     '-webkit-background-clip': string;
     '-webkit-text-fill-color': string;
+    opacity: string;
 } {
-    let result = {
-        background: 'none',
-        color: 'unset', // FIXME
-    };
+    let fontFamily: string;
+    let fontSize: string;
+    let fontWeight: string;
+    let textStyle: string;
+    let textDecoration: string;
+    let textTransform: string;
+    let color: string;
+    let background: string;
+    let backgroundClip: string;
+    let textFillColor: string;
+    let opacity: string;
 
     // `Dim` is the same as `text`, just with some opacity
     if (style === 'dim') {
         style = 'text';
-        result['opacity'] = '0.4';
+        opacity = '0.4';
     } else {
-        result['opacity'] = '1';
+        opacity = '1';
     }
 
     // Predefined style from theme
     if (typeof style === 'string') {
         let globalPrefix = `var(--rio-global-${style}-`;
         let localPrefix = `var(--rio-local-${style}-`;
 
         // Text fill
-        result['color'] = localPrefix + 'color)';
-        result['background'] = localPrefix + 'background)';
-        result['-webkit-background-clip'] = localPrefix + 'background-clip)';
-        result['-webkit-text-fill-color'] = localPrefix + 'fill-color)';
-
-        // Font weight. This is local, so that buttons can make their label text
-        // be bold.
-        result['font-weight'] = localPrefix + 'font-weight)';
+        color = localPrefix + 'color)';
+        background = localPrefix + 'background)';
+        backgroundClip = localPrefix + 'background-clip)';
+        textFillColor = localPrefix + 'fill-color)';
+
+        // Font weight. This is local so that buttons can make their label text
+        // bold.
+        fontWeight = localPrefix + 'font-weight)';
 
         // Others
-        result['font-family'] = globalPrefix + 'font-name)';
-        result['font-size'] = globalPrefix + 'font-size)';
-        result['text-style'] = globalPrefix + 'font-italic)';
-        result['text-decoration'] = globalPrefix + 'underlined)';
-        result['text-transform'] = globalPrefix + 'all-caps)';
+        fontFamily = globalPrefix + 'font-name)';
+        fontSize = globalPrefix + 'font-size)';
+        textStyle = globalPrefix + 'font-italic)';
+        textDecoration = globalPrefix + 'underlined)';
+        textTransform = globalPrefix + 'all-caps)';
     }
 
     // Explicitly defined style
     else {
-        result['font-size'] = style.fontSize + 'em';
-        result['font-style'] = style.italic ? 'italic' : 'normal';
-        result['font-weight'] = style.fontWeight;
-        result['text-decoration'] = style.underlined ? 'underline' : 'none';
-        result['text-transform'] = style.allCaps ? 'uppercase' : 'none';
+        fontSize = style.fontSize + 'em';
+        textStyle = style.italic ? 'italic' : 'normal';
+        fontWeight = style.fontWeight;
+        textDecoration = style.underlined ? 'underline' : 'none';
+        textTransform = style.allCaps ? 'uppercase' : 'none';
 
         // If no font family is provided, stick to the theme's.
         if (style.fontName === null) {
-            result['font-family'] = 'inherit';
+            fontFamily = 'inherit';
         } else {
-            result['font-family'] = style.fontName;
+            fontFamily = style.fontName;
         }
 
         // If no fill is provided, stick to the local text color. This allows
         // the user to have their text automatically adapt to different
         // themes/contexts.
         if (style.fill === null) {
-            result['color'] = 'var(--rio-local-text-color)';
-            result['background'] = 'var(--rio-local-text-background)';
-            result['-webkit-background-clip'] =
-                'var(--rio-local-text-background-clip)';
-            result['-webkit-text-fill-color'] =
-                'var(--rio-local-text-fill-color)';
+            color = 'var(--rio-local-text-color)';
+            background = 'var(--rio-local-text-background)';
+            backgroundClip = 'var(--rio-local-text-background-clip)';
+            textFillColor = 'var(--rio-local-text-fill-color)';
         }
         // Color?
         else if (Array.isArray(style.fill)) {
-            result['color'] = colorToCssString(style.fill);
-            result['background'] = 'none';
-            result['-webkit-background-clip'] = 'unset';
-            result['-webkit-text-fill-color'] = 'unset';
+            color = colorToCssString(style.fill);
+            background = 'none';
+            backgroundClip = 'unset';
+            textFillColor = 'unset';
         }
         // Solid fill, i.e. also a color
         else if (style.fill.type === 'solid') {
-            result['color'] = colorToCssString(style.fill.color);
-            result['background'] = 'none';
-            result['-webkit-background-clip'] = 'unset';
-            result['-webkit-text-fill-color'] = 'unset';
+            color = colorToCssString(style.fill.color);
+            background = 'none';
+            backgroundClip = 'unset';
+            textFillColor = 'unset';
         }
         // Anything else
         else {
-            result['color'] = 'unset';
-            result['background'] = fillToCssString(style.fill);
-            result['-webkit-background-clip'] = 'text';
-            result['-webkit-text-fill-color'] = 'transparent';
+            color = 'unset';
+            background = fillToCssString(style.fill);
+            backgroundClip = 'text';
+            textFillColor = 'transparent';
         }
     }
 
-    // @ts-ignore
-    return result;
+    return {
+        'font-family': fontFamily,
+        'font-size': fontSize,
+        'font-weight': fontWeight,
+        'text-style': textStyle,
+        'text-decoration': textDecoration,
+        'text-transform': textTransform,
+        color: color,
+        background: background,
+        '-webkit-background-clip': backgroundClip,
+        '-webkit-text-fill-color': textFillColor,
+        opacity: opacity,
+    };
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/dataModels.ts` & `rio_ui-0.6/frontend/code/dataModels.ts`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,20 @@
     | 'background'
     | 'neutral'
     | 'hud'
     | 'disabled'
     | 'success'
     | 'warning'
     | 'danger'
-    | 'accent-to-plain'
     | 'keep'
     | {
-          plainBg: Color;
-          plainBgVariant: Color;
-          plainBgActive: Color;
-          plainFg: Color;
-          accentBg: Color;
-          accentFg: Color;
+          localBg: Color;
+          localBgVariant: Color;
+          localBgActive: Color;
+          localFg: Color;
       };
 
 export type Fill =
     | {
           type: 'solid';
           color: Color;
       }
```

### Comparing `rio_ui-0.5.9/frontend/code/designApplication.ts` & `rio_ui-0.6/frontend/code/designApplication.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-import { Color, ColorSet, Fill } from './models';
+import { Color, ColorSet, Fill } from './dataModels';
 import { colorToCssString } from './cssUtils';
 
 const ICON_PROMISE_CACHE: { [key: string]: Promise<string> } = {};
 
-export function applyColorSet(element: HTMLElement, colorSet: ColorSet): void {
-    // Remove all switcheroos
+/// Removes any switcheroos from the given element
+function removeSwitcheroos(element: HTMLElement): void {
     element.classList.remove(
-        'rio-switcheroo-primary',
-        'rio-switcheroo-secondary',
         'rio-switcheroo-background',
         'rio-switcheroo-neutral',
         'rio-switcheroo-hud',
-        'rio-switcheroo-disabled',
+        'rio-switcheroo-primary',
+        'rio-switcheroo-secondary',
         'rio-switcheroo-success',
         'rio-switcheroo-warning',
         'rio-switcheroo-danger',
+        'rio-switcheroo-disabled',
         'rio-switcheroo-custom',
-        'rio-switcheroo-accent-to-plain'
+        'rio-switcheroo-bump'
     );
+}
+
+export function applySwitcheroo(
+    element: HTMLElement,
+    colorSet: ColorSet | 'bump'
+): void {
+    // Remove any preexisting switcheroos
+    element.classList.remove('rio-switcheroo-bump-outer');
 
-    // If no colorset is desired don't apply any new one
+    // If no color set is desired don't apply any new one
     if (colorSet === 'keep') {
         return;
     }
 
-    // Otherwise find and apply the correct switcheroo
-    let switcheroo: string;
-
-    // Is this a color instance?
-    if (typeof colorSet !== 'string') {
-        // Expose the color as CSS variables
-        element.style.setProperty(
-            '--rio-local-custom-plain-bg',
-            colorToCssString(colorSet.plainBg)
-        );
-        element.style.setProperty(
-            '--rio-local-custom-plain-bg-variant',
-            colorToCssString(colorSet.plainBgVariant)
-        );
-        element.style.setProperty(
-            '--rio-local-custom-plain-bg-active',
-            colorToCssString(colorSet.plainBgActive)
-        );
-        element.style.setProperty(
-            '--rio-local-custom-plain-fg',
-            colorToCssString(colorSet.plainFg)
-        );
-
-        element.style.setProperty(
-            '--rio-local-custom-accent-bg',
-            colorToCssString(colorSet.accentBg)
-        );
-        element.style.setProperty(
-            '--rio-local-custom-accent-fg',
-            colorToCssString(colorSet.accentFg)
-        );
-
-        // Select the custom switcheroo
-        switcheroo = 'custom';
-    } else {
-        switcheroo = colorSet;
+    // Is this a well-known switcheroo?
+    if (typeof colorSet === 'string') {
+        element.classList.add(`rio-switcheroo-${colorSet}`);
+        return;
     }
 
-    // Add the new switcheroo
-    element.classList.add(`rio-switcheroo-${switcheroo}`);
+    // Custom color sets need additional variables to be defined
+    element.style.setProperty(
+        '--rio-custom-local-bg',
+        colorToCssString(colorSet.localBg)
+    );
+    element.style.setProperty(
+        '--rio-custom-local-bg-variant',
+        colorToCssString(colorSet.localBgVariant)
+    );
+    element.style.setProperty(
+        '--rio-custom-local-bg-active',
+        colorToCssString(colorSet.localBgActive)
+    );
+    element.style.setProperty(
+        '--rio-custom-local-fg',
+        colorToCssString(colorSet.localFg)
+    );
+
+    // Apply the switcheroo
+    element.classList.add('rio-switcheroo-custom');
 }
 
 export function applyFillToSVG(svgRoot: SVGSVGElement, fill: Fill): void {
     switch (fill.type) {
         case 'solid':
             applySolidFill(svgRoot, fill.color);
             break;
```

### Comparing `rio_ui-0.5.9/frontend/code/easeFunctions.ts` & `rio_ui-0.6/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/eventHandling.ts` & `rio_ui-0.6/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/inputBoxTools.ts` & `rio_ui-0.6/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/layoutHelpers.ts` & `rio_ui-0.6/frontend/code/layoutHelpers.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { pixelsPerRem } from './app';
 import { textStyleToCss } from './cssUtils';
-import { TextStyle } from './models';
+import { TextStyle } from './dataModels';
 
 const _textDimensionsCache = new Map<string, [number, number]>();
 
 let cacheHits: number = 0;
 let cacheMisses: number = 0;
 
 /// Returns the width and height of the given text in pixels. Does not cache
@@ -127,19 +127,77 @@
 
     return result;
 }
 
 globalThis.getElementDimensions = getElementDimensions; // For debugging
 
 export function getElementWidth(element: HTMLElement): number {
-    // TODO: Don't request both height and width - that's the whole point of
-    // this function
-    let dimensions = getElementDimensions(element);
-    return dimensions[0];
+    // Remember everything necessary to restore the original state
+    let isInDom = element.isConnected;
+    let originalDisplay = element.style.display;
+
+    let parentElement: HTMLElement | null = null;
+    let nextSibling: Node | null = null;
+    if (!isInDom) {
+        parentElement = element.parentElement;
+        nextSibling = element.nextSibling;
+    }
+
+    // Ensure the element is in the DOM
+    if (!isInDom) {
+        document.body.appendChild(element);
+    } else {
+        element.style.display = 'fixed';
+    }
+
+    // Get its dimensions
+    let result = element.scrollWidth / pixelsPerRem;
+
+    // Restore the original state
+    if (isInDom) {
+        element.style.display = originalDisplay;
+    } else if (parentElement === null) {
+        element.remove();
+    } else if (nextSibling === null) {
+        parentElement.appendChild(element);
+    } else {
+        parentElement.insertBefore(element, nextSibling);
+    }
+
+    return result;
 }
 
 export function getElementHeight(element: HTMLElement): number {
-    // TODO: Don't request both height and width - that's the whole point of
-    // this function
-    let dimensions = getElementDimensions(element);
-    return dimensions[1];
+    // Remember everything necessary to restore the original state
+    let isInDom = element.isConnected;
+    let originalDisplay = element.style.display;
+
+    let parentElement: HTMLElement | null = null;
+    let nextSibling: Node | null = null;
+    if (!isInDom) {
+        parentElement = element.parentElement;
+        nextSibling = element.nextSibling;
+    }
+
+    // Ensure the element is in the DOM
+    if (!isInDom) {
+        document.body.appendChild(element);
+    } else {
+        element.style.display = 'fixed';
+    }
+
+    // Get its dimensions
+    let result = element.scrollHeight / pixelsPerRem;
+
+    // Restore the original state
+    if (isInDom) {
+        element.style.display = originalDisplay;
+    } else if (parentElement === null) {
+        element.remove();
+    } else if (nextSibling === null) {
+        parentElement.appendChild(element);
+    } else {
+        parentElement.insertBefore(element, nextSibling);
+    }
+
+    return result;
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/layouting.ts` & `rio_ui-0.6/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/rpc.ts` & `rio_ui-0.6/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/rpcFunctions.ts` & `rio_ui-0.6/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/utils.ts` & `rio_ui-0.6/frontend/code/utils.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import { componentsByElement } from './componentManagement';
+
 export class AsyncQueue<T> {
     private waitingForValue: ((value: T) => void)[] = [];
     private values: T[] = [];
 
     push(value: T): void {
         // If someone is waiting for a value, give it to them
         let notifyFirstWaiter = this.waitingForValue.shift();
@@ -90,7 +92,34 @@
         if (arg !== undefined) {
             return arg;
         }
     }
 
     return undefined;
 }
+
+/// Copies the given text to the clipboard
+export function copyToClipboard(text: string): void {
+    const textArea = document.createElement('textarea');
+    textArea.value = text;
+
+    document.body.appendChild(textArea);
+    textArea.select();
+    document.execCommand('copy');
+    document.body.removeChild(textArea);
+}
+
+/// Checks if there's an #url-fragment, and if so, scrolls the corresponding
+/// ScrollTarget into view
+export function scrollToUrlFragment(): void {
+    let fragment = window.location.hash.substring(1);
+    if (!fragment) {
+        return;
+    }
+
+    let element = document.getElementById(fragment);
+    if (element === null) {
+        return;
+    }
+
+    element.scrollIntoView();
+}
```

### Comparing `rio_ui-0.5.9/frontend/code/components/align.ts` & `rio_ui-0.6/frontend/code/components/align.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type AlignState = ComponentState & {
     _type_: 'Align-builtin';
     content?: ComponentId;
     align_x?: number | null;
     align_y?: number | null;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/buildFailed.ts` & `rio_ui-0.6/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/button.ts` & `rio_ui-0.6/frontend/code/components/button.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import { applyColorSet } from '../designApplication';
-import { ColorSet, ComponentId } from '../models';
+import { applySwitcheroo } from '../designApplication';
+import { ColorSet, ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
-import { MDCRipple } from '@material/ripple';
-import { LayoutContext } from '../layouting';
+import { RippleEffect } from '../rippleEffect';
 import { SingleContainer } from './singleContainer';
 import { firstDefined } from '../utils';
 
 export type ButtonState = ComponentState & {
     _type_: 'Button-builtin';
     shape?: 'pill' | 'rounded' | 'rectangle';
     style?: 'major' | 'minor' | 'plain';
@@ -14,32 +13,32 @@
     content?: ComponentId;
     is_sensitive?: boolean;
     initially_disabled_for?: number;
 };
 
 export class ButtonComponent extends SingleContainer {
     state: Required<ButtonState>;
-    private mdcRipple: MDCRipple;
+    private rippleInstance: RippleEffect;
 
     private innerElement: HTMLElement;
 
     // In order to prevent a newly created button from being clicked on
     // accident, it starts out disabled and enables itself after a short delay.
     private isStillInitiallyDisabled: boolean = true;
 
     createElement(): HTMLElement {
         // Create the element
         let element = document.createElement('div');
-        element.classList.add('rio-button', 'mdc-ripple-surface');
+        element.classList.add('rio-button');
 
         this.innerElement = document.createElement('div');
         element.appendChild(this.innerElement);
 
         // Add a material ripple effect
-        this.mdcRipple = new MDCRipple(this.innerElement);
+        this.rippleInstance = new RippleEffect(this.innerElement);
 
         // Detect button presses
         this.innerElement.onclick = (event) => {
             event.stopPropagation();
 
             // Do nothing if the button isn't sensitive
             if (!this.state['is_sensitive'] || this.isStillInitiallyDisabled) {
@@ -108,30 +107,17 @@
                 this.state['is_sensitive']
             );
 
             let colorSet = is_sensitive
                 ? firstDefined(deltaState.color, this.state['color'])
                 : 'disabled';
 
-            // If no new colorset is specified, turn the accent color into the
-            // plain color. This allows all styles to just assume that the color
-            // they should use is the plain color.
-            //
-            // The exception to this is the plain style, which obviously isn't
-            // trying to stand out.
-            if (colorSet === 'keep') {
-                colorSet = 'accent-to-plain';
-            }
-
-            applyColorSet(this.innerElement, colorSet);
+            // If no new colorset is specified, bump to the next palette. This
+            // allows all styles to just assume that the palette they should use
+            // is the current one.
+            applySwitcheroo(
+                this.innerElement,
+                colorSet === 'keep' ? 'bump' : colorSet
+            );
         }
     }
-
-    updateAllocatedHeight(ctx: LayoutContext): void {
-        super.updateAllocatedHeight(ctx);
-
-        // The ripple stores the coordinates of its rectangle. Since Rio likes
-        // to resize and move around components, the rectangle must be updated
-        // appropriately.
-        this.mdcRipple.layout();
-    }
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/card.ts` & `rio_ui-0.6/frontend/code/components/card.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-import { applyColorSet } from '../designApplication';
-import { ColorSet, ComponentId } from '../models';
+import { applySwitcheroo } from '../designApplication';
+import { ColorSet, ComponentId } from '../dataModels';
+import { RippleEffect } from '../rippleEffect';
 import { ComponentBase, ComponentState } from './componentBase';
 import { SingleContainer } from './singleContainer';
 
 export type CardState = ComponentState & {
     _type_: 'Card-builtin';
     content?: ComponentId;
     corner_radius?: number | [number, number, number, number];
     reportPress?: boolean;
+    ripple?: boolean;
     elevate_on_hover?: boolean;
     colorize_on_hover?: boolean;
     color?: ColorSet;
 };
 
 export class CardComponent extends SingleContainer {
     state: Required<CardState>;
 
+    // If this card has a ripple effect, this is the ripple instance. `null`
+    // otherwise.
+    private rippleInstance: RippleEffect | null = null;
+
     createElement(): HTMLElement {
         // Create the element
         let element = document.createElement('div');
         element.classList.add('rio-card');
 
         // Detect presses
         element.onclick = (event) => {
@@ -54,15 +60,31 @@
             }
         }
 
         // Report presses?
         if (deltaState.reportPress === true) {
             this.element.style.cursor = 'pointer';
         } else if (deltaState.reportPress === false) {
-            this.element.style.cursor = 'default';
+            this.element.style.removeProperty('cursor');
+        }
+
+        // Ripple
+        if (deltaState.ripple === true) {
+            if (this.rippleInstance === null) {
+                this.rippleInstance = new RippleEffect(this.element);
+
+                this.element.classList.add('rio-card-ripple');
+            }
+        } else if (deltaState.ripple === false) {
+            if (this.rippleInstance !== null) {
+                this.rippleInstance.destroy();
+                this.rippleInstance = null;
+
+                this.element.classList.remove('rio-card-ripple');
+            }
         }
 
         // Elevate on hover
         if (deltaState.elevate_on_hover === true) {
             this.element.classList.add('rio-card-elevate-on-hover');
         } else if (deltaState.elevate_on_hover === false) {
             this.element.classList.remove('rio-card-elevate-on-hover');
@@ -73,11 +95,11 @@
             this.element.classList.add('rio-card-colorize-on-hover');
         } else if (deltaState.colorize_on_hover === false) {
             this.element.classList.remove('rio-card-colorize-on-hover');
         }
 
         // Colorize
         if (deltaState.color !== undefined) {
-            applyColorSet(this.element, deltaState.color);
+            applySwitcheroo(this.element, deltaState.color);
         }
     }
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/classContainer.ts` & `rio_ui-0.6/frontend/code/components/classContainer.ts`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { SingleContainer } from './singleContainer';
 import { ComponentBase, ComponentState } from './componentBase';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 export type ClassContainerState = ComponentState & {
     _type_: 'ClassContainer-builtin';
     content?: ComponentId | null;
     classes?: string[];
 };
```

### Comparing `rio_ui-0.5.9/frontend/code/components/codeExplorer.ts` & `rio_ui-0.6/frontend/code/components/codeExplorer.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import hljs from 'highlight.js/lib/common';
 import { componentsByElement, componentsById } from '../componentManagement';
-import { getElementDimensions, getElementHeight } from '../layoutHelpers';
+import { getElementDimensions } from '../layoutHelpers';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { applyIcon } from '../designApplication';
-import { commitCss, disableTransitions, enableTransitions } from '../utils';
-import { pixelsPerRem } from '../app';
 
 // Layouting variables needed by both JS and CSS
 const MAIN_GAP = 1;
 const BOX_PADDING = 1;
 const ARROW_SIZE = 3;
 const ADDITIONAL_SPACE = (BOX_PADDING * 2 + MAIN_GAP) * 2 + ARROW_SIZE;
 
 export type CodeExplorerState = ComponentState & {
     _type_: 'CodeExplorer-builtin';
     source_code?: string;
     build_result?: ComponentId;
-    line_indices_to_component_keys: (string | null)[];
+    line_indices_to_component_keys?: (string | null)[];
+    style?: 'horizontal' | 'vertical';
 };
 
 export class CodeExplorerComponent extends ComponentBase {
     state: Required<CodeExplorerState>;
 
     private sourceCodeElement: HTMLElement;
     private arrowElement: HTMLElement;
@@ -62,20 +61,14 @@
         this.sourceCodeElement.style.padding = `${BOX_PADDING}rem`;
 
         element.style.gap = `${MAIN_GAP}rem`;
 
         this.arrowElement.style.width = `${ARROW_SIZE}rem`;
         this.arrowElement.style.height = `${ARROW_SIZE}rem`;
 
-        applyIcon(
-            this.arrowElement,
-            'material/arrow-right-alt:fill',
-            'var(--rio-global-secondary-bg)'
-        );
-
         // this.arrowElement.style.opacity = '0.3';
 
         // Listen for mouse events
         this.buildResultElement.addEventListener(
             'mousemove',
             this.onResultMouseMove.bind(this),
             { capture: true }
@@ -129,14 +122,32 @@
             let buildResultElement = componentsById[deltaState.build_result]!;
             buildResultElement.element.style.removeProperty('left');
             buildResultElement.element.style.removeProperty('top');
 
             // (Re-)Add the highlighter
             this.buildResultElement.appendChild(this.resultHighlighterElement);
         }
+
+        if (deltaState.style !== undefined) {
+            if (deltaState.style === 'horizontal') {
+                this.element.style.flexDirection = 'row';
+                applyIcon(
+                    this.arrowElement,
+                    'material/arrow-right-alt:fill',
+                    'var(--rio-global-secondary-bg)'
+                );
+            } else {
+                this.element.style.flexDirection = 'column';
+                applyIcon(
+                    this.arrowElement,
+                    'material/arrow-downward:fill',
+                    'var(--rio-global-secondary-bg)'
+                );
+            }
+        }
     }
 
     private _connectHighlightEventListeners(): void {
         // The text is a mix of spans and raw text. Some of them may extend over
         // multiple lines. Split them up, and use this opportunity to wrap all
         // text in spans as well.
         let lineIndex = 0;
@@ -378,31 +389,49 @@
 
         // Exhausted all children
         return null;
     }
 
     updateNaturalWidth(ctx: LayoutContext): void {
         let buildResultElement = componentsById[this.state.build_result]!;
-        this.naturalWidth =
-            this.sourceCodeDimensions[0] +
-            ADDITIONAL_SPACE +
-            buildResultElement.requestedWidth;
+
+        if (this.state.style === 'horizontal') {
+            this.naturalWidth =
+                this.sourceCodeDimensions[0] +
+                ADDITIONAL_SPACE +
+                buildResultElement.requestedWidth;
+        } else {
+            this.naturalWidth = Math.max(
+                this.sourceCodeDimensions[0],
+                ADDITIONAL_SPACE,
+                buildResultElement.requestedWidth
+            );
+        }
     }
 
     updateAllocatedWidth(ctx: LayoutContext): void {
         let buildResultElement = componentsById[this.state.build_result]!;
         buildResultElement.allocatedWidth = buildResultElement.requestedWidth;
     }
 
     updateNaturalHeight(ctx: LayoutContext): void {
         let buildResultElement = componentsById[this.state.build_result]!;
-        this.naturalHeight = Math.max(
-            this.sourceCodeDimensions[1],
-            buildResultElement.requestedHeight
-        );
+
+        if (this.state.style === 'horizontal') {
+            this.naturalHeight = Math.max(
+                this.sourceCodeDimensions[1],
+                ADDITIONAL_SPACE,
+                buildResultElement.requestedHeight
+            );
+        } else {
+            this.naturalHeight =
+                this.sourceCodeDimensions[1] +
+                ADDITIONAL_SPACE +
+                buildResultElement.requestedHeight;
+        }
     }
 
     updateAllocatedHeight(ctx: LayoutContext): void {
         let buildResultElement = componentsById[this.state.build_result]!;
         buildResultElement.allocatedHeight = buildResultElement.requestedHeight;
 
         // Positioning the child is already done in `updateElement`
```

### Comparing `rio_ui-0.5.9/frontend/code/components/colorPicker.ts` & `rio_ui-0.6/frontend/code/components/colorPicker.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { Color } from '../models';
+import { Color } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { hsvToRgb, rgbToHsv, rgbToHex, rgbaToHex } from '../colorConversion';
 import { LayoutContext } from '../layouting';
 import { getElementDimensions } from '../layoutHelpers';
 
 export type ColorPickerState = ComponentState & {
     _type_: 'ColorPicker-builtin';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/componentBase.ts` & `rio_ui-0.6/frontend/code/components/componentBase.ts`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     EventHandler,
     DragHandler,
     DragHandlerArguments,
     ClickHandlerArguments,
     ClickHandler,
 } from '../eventHandling';
 import { DebuggerConnectorComponent } from './debuggerConnector';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 /// Base for all component states. Updates received from the backend are
 /// partial, hence most properties may be undefined.
 export type ComponentState = {
     // The component type's unique id. Crucial so the client knows what kind of
     // component to spawn.
     _type_?: string;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/componentTree.ts` & `rio_ui-0.6/frontend/code/components/componentTree.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { componentsById, getRootScroller } from '../componentManagement';
 import { applyIcon } from '../designApplication';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { DebuggerConnectorComponent } from './debuggerConnector';
 
 export type ComponentTreeState = ComponentState & {
     _type_: 'ComponentTree-builtin';
 };
```

### Comparing `rio_ui-0.5.9/frontend/code/components/debuggerConnector.ts` & `rio_ui-0.6/frontend/code/components/debuggerConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/drawer.ts` & `rio_ui-0.6/frontend/code/components/drawer.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { pixelsPerRem } from '../app';
 import { commitCss } from '../utils';
 import { componentsById } from '../componentManagement';
 import { ComponentBase, ComponentState } from './componentBase';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 export type DrawerState = ComponentState & {
     _type_: 'Drawer-builtin';
     anchor?: ComponentId;
     content?: ComponentId;
     side?: 'left' | 'right' | 'top' | 'bottom';
     is_modal?: boolean;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/dropdown.ts` & `rio_ui-0.6/frontend/code/components/dropdown.ts`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,15 @@
     private highlightedOptionElement: HTMLElement | null = null;
 
     private longestOptionWidth: number = 0;
 
     createElement(): HTMLElement {
         // Create the elements
         let element = document.createElement('div');
-        element.classList.add(
-            'rio-dropdown',
-            'mdc-ripple-surface',
-            'rio-input-box'
-        );
+        element.classList.add('rio-dropdown', 'rio-input-box');
 
         element.innerHTML = `
             <input type="text" placeholder="">
             <div class="rio-input-box-label"></div>
             <div class="rio-dropdown-arrow"></div>
             <div class="rio-input-box-plain-bar"></div>
             <div class="rio-input-box-color-bar"></div>
```

### Comparing `rio_ui-0.5.9/frontend/code/components/flowContainer.ts` & `rio_ui-0.6/frontend/code/components/flowContainer.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type FlowState = ComponentState & {
     _type_: 'FlowContainer-builtin';
     children?: ComponentId[];
     row_spacing?: number;
     column_spacing?: number;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.6/frontend/code/components/fundamentalRootComponent.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { pixelsPerRem } from '../app';
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { setConnectionLostPopupVisibleUnlessGoingAway } from '../rpc';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type FundamentalRootComponentState = ComponentState & {
     _type_: 'FundamentalRootComponent-builtin';
     content: ComponentId;
     debugger: ComponentId | null;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/grid.ts` & `rio_ui-0.6/frontend/code/components/grid.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { range } from '../utils';
 import { ComponentBase, ComponentState } from './componentBase';
 
 type GridChildPosition = {
     row: number;
     column: number;
     width: number;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/headingListItem.ts` & `rio_ui-0.6/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/html.ts` & `rio_ui-0.6/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/icon.ts` & `rio_ui-0.6/frontend/code/components/icon.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { ColorSet, Fill } from '../models';
+import { ColorSet, Fill } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { applyFillToSVG } from '../designApplication';
 import { pixelsPerRem } from '../app';
 
 export type IconState = ComponentState & {
     _type_: 'Icon-builtin';
     svgSource: string;
@@ -23,15 +23,15 @@
         svgRoot.style.fill = 'var(--rio-local-text-color)';
         return;
     }
 
     // "dim" is a special case, which is represented by using the "neutral"
     // style, but with a reduced opacity.
     if (fill === 'dim') {
-        svgRoot.style.fill = `var(--rio-global-neutral-fg)`;
+        svgRoot.style.fill = `var(--rio-local-text-color)`;
         svgRoot.style.opacity = '0.4';
         return;
     }
 
     // If the fill is a string apply the appropriate theme color. Note that this
     // uses the background rather than foreground color. The foreground is
     // intended to be used if the background was already set to background
```

### Comparing `rio_ui-0.5.9/frontend/code/components/image.ts` & `rio_ui-0.6/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/keyEventListener.ts` & `rio_ui-0.6/frontend/code/components/keyEventListener.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { SingleContainer } from './singleContainer';
 import { ComponentBase, ComponentState } from './componentBase';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { firstDefined } from '../utils';
 
 // https://developer.mozilla.org/en-US/docs/Web/API/UI_Events/Keyboard_event_code_values
 const HARDWARE_KEY_MAP = {
     Unidentified: 'unknown',
     '': 'unknown',
```

### Comparing `rio_ui-0.5.9/frontend/code/components/linearContainers.ts` & `rio_ui-0.6/frontend/code/components/linearContainers.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { pixelsPerRem } from '../app';
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type LinearContainerState = ComponentState & {
     _type_: 'Row-builtin' | 'Column-builtin' | 'ListView-builtin';
     children?: ComponentId[];
     spacing?: number;
     proportions?: 'homogeneous' | number[] | null;
@@ -360,15 +360,15 @@
                 this.state.proportions === 'homogeneous'
                     ? Array(this.children.size).fill(1)
                     : this.state.proportions;
 
             let spacing =
                 Math.max(this.children.size - 1, 0) * this.state.spacing;
             let proportionSize =
-                (this.allocatedWidth - spacing) / this.totalProportions;
+                (this.allocatedHeight - spacing) / this.totalProportions;
 
             for (let i = 0; i < proportions.length; i++) {
                 let child = componentsById[this.state.children[i]]!;
                 child.allocatedHeight = proportionSize * proportions[i];
             }
         }
     }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/link.ts` & `rio_ui-0.6/frontend/code/components/link.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { componentsById } from '../componentManagement';
 import { getTextDimensions } from '../layoutHelpers';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type LinkState = ComponentState & {
     _type_: 'Link-builtin';
     child_text?: string | null;
     child_component?: ComponentId | null;
     open_in_new_tab?: boolean;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/listView.ts` & `rio_ui-0.6/frontend/code/components/listView.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { componentsByElement } from '../componentManagement';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase } from './componentBase';
 import { CustomListItemComponent } from './customListItem';
 import { HeadingListItemComponent } from './headingListItem';
 import { ColumnComponent, LinearContainerState } from './linearContainers';
 import { SeparatorListItemComponent } from './separatorListItem';
 
 export class ListViewComponent extends ColumnComponent {
```

### Comparing `rio_ui-0.5.9/frontend/code/components/margin.ts` & `rio_ui-0.6/frontend/code/components/margin.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { ComponentBase, ComponentState } from './componentBase';
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 export type MarginState = ComponentState & {
     _type_: 'Margin-builtin';
     content?: ComponentId;
     margin_left?: number;
     margin_top?: number;
     margin_right?: number;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/markdown.ts` & `rio_ui-0.6/frontend/code/components/markdown.ts`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 //
 // https://github.com/highlightjs/highlight.js#importing-the-library
 import hljs from 'highlight.js/lib/common';
 import { Language } from 'highlight.js';
 
 import { LayoutContext } from '../layouting';
 import { getElementHeight, getElementWidth } from '../layoutHelpers';
-import { firstDefined } from '../utils';
+import { copyToClipboard, firstDefined } from '../utils';
 import { applyIcon } from '../designApplication';
 
 export type MarkdownState = ComponentState & {
     _type_: 'Markdown-builtin';
     text?: string;
     default_language?: null | string;
 };
@@ -112,21 +112,16 @@
             'material/content-copy',
             'var(--rio-local-text-color)'
         );
 
         copyButton.addEventListener('click', (event) => {
             const codeToCopy =
                 (codeBlockInner as HTMLElement).textContent ?? '';
-            const textArea = document.createElement('textarea');
-            textArea.value = codeToCopy;
 
-            document.body.appendChild(textArea);
-            textArea.select();
-            document.execCommand('copy');
-            document.body.removeChild(textArea);
+            copyToClipboard(codeToCopy);
 
             copyButton.title = 'Copied!';
             applyIcon(
                 copyButton,
                 'material/done',
                 'var(--rio-local-text-color)'
             );
```

### Comparing `rio_ui-0.5.9/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.6/frontend/code/components/mediaPlayer.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { fillToCss } from '../cssUtils';
 import { applyIcon } from '../designApplication';
 import { LayoutContext } from '../layouting';
-import { Fill } from '../models';
+import { Fill } from '../dataModels';
 import { sleep } from '../utils';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type MediaPlayerState = ComponentState & {
     _type_: 'MediaPlayer-builtin';
     loop?: boolean;
     autoplay?: boolean;
@@ -108,15 +108,15 @@
         if (visibilityBefore == this._overlayVisible) {
             return;
         }
 
         // Apply the visibility
         if (this._overlayVisible) {
             this.controls.style.opacity = '1';
-            this.mediaPlayer.style.cursor = 'default';
+            this.mediaPlayer.style.removeProperty('cursor');
         } else {
             this.controls.style.opacity = '0';
             this.mediaPlayer.style.cursor = 'none';
         }
     }
 
     interactWorker(): void {
@@ -205,15 +205,19 @@
         }
     }
 
     private _onFullscreenChange(): void {
         this._isFullScreen = document.fullscreenElement === this.element;
 
         if (this._isFullScreen) {
-            applyIcon(this.fullscreenButton, 'material/fullscreen-exit', 'white');
+            applyIcon(
+                this.fullscreenButton,
+                'material/fullscreen-exit',
+                'white'
+            );
         } else {
             applyIcon(this.fullscreenButton, 'material/fullscreen', 'white');
         }
     }
 
     /// Pretty-string a duration (in seconds. FU JS)
     _durationToString(duration: number): string {
@@ -640,15 +644,19 @@
             let color = this._hasAudio ? 'white' : 'gray';
             applyIcon(this.muteButton, 'material/volume-off:fill', color);
             this.volumeKnob.style.background = color;
         } else {
             this.volumeCurrent.style.width = `${humanVolume * 100}%`;
 
             if (humanVolume < 0.5) {
-                applyIcon(this.muteButton, 'material/volume-down:fill', 'white');
+                applyIcon(
+                    this.muteButton,
+                    'material/volume-down:fill',
+                    'white'
+                );
             } else {
                 applyIcon(this.muteButton, 'material/volume-up:fill', 'white');
             }
         }
     }
 
     private _onVolumeWheelEvent(event: WheelEvent): void {
@@ -827,14 +835,22 @@
 
     private _onPlaybackEnd(event: Event): void {
         this.sendMessageToBackend({
             type: 'onPlaybackEnd',
         });
     }
 
+    onDestruction(): void {
+        // Explicitly unload the video, just in case someone is still holding a
+        // reference to this component or element
+        this.mediaPlayer.pause();
+        this.mediaPlayer.src = '';
+        this.mediaPlayer.load();
+    }
+
     updateNaturalWidth(ctx: LayoutContext): void {
         this.naturalWidth = 16;
     }
 
     updateNaturalHeight(ctx: LayoutContext): void {
         this.naturalHeight = 5;
     }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.6/frontend/code/components/mouseEventListener.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { pixelsPerRem } from '../app';
 import { SingleContainer } from './singleContainer';
 import { ComponentBase, ComponentState } from './componentBase';
 import { DragHandler } from '../eventHandling';
 import { tryGetComponentByElement } from '../componentManagement';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 function eventMouseButtonToString(event: MouseEvent): object {
     return {
         button: ['left', 'middle', 'right'][event.button],
     };
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.6/frontend/code/components/multiLineTextInput.ts`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,15 @@
 
     private labelElement: HTMLElement;
     private inputElement: HTMLTextAreaElement;
 
     createElement(): HTMLElement {
         // Create the element
         let element = document.createElement('div');
-        element.classList.add(
-            'rio-text-input',
-            'rio-input-box',
-            'mdc-ripple-surface'
-        );
+        element.classList.add('rio-text-input', 'rio-input-box');
 
         element.innerHTML = `
             <textarea placeholder=""></textarea>
             <div class="rio-input-box-label"></div>
             <div class="rio-input-box-plain-bar"></div>
             <div class="rio-input-box-color-bar"></div>
         `;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/nodeInput.ts` & `rio_ui-0.6/frontend/code/components/nodeInput.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { ComponentBase, ComponentState } from './componentBase';
 import { LayoutContext } from '../layouting';
-import { Color } from '../models';
+import { Color } from '../dataModels';
 import { getTextDimensions } from '../layoutHelpers';
 import { colorToCssString } from '../cssUtils';
 
 export type NodeInputState = ComponentState & {
     _type_: 'NodeInput-builtin';
     name: string;
     color: Color;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/nodeOutput.ts` & `rio_ui-0.6/frontend/code/components/nodeOutput.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { ComponentBase, ComponentState } from './componentBase';
 import { LayoutContext } from '../layouting';
-import { Color } from '../models';
+import { Color } from '../dataModels';
 import { getTextDimensions } from '../layoutHelpers';
 import { colorToCssString } from '../cssUtils';
 
 export type NodeOutputState = ComponentState & {
     _type_: 'NodeOutput-builtin';
     name: string;
     color: Color;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/overlay.ts` & `rio_ui-0.6/frontend/code/components/overlay.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { componentsById, getRootComponent } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type OverlayState = ComponentState & {
     _type_: 'Overlay-builtin';
     content?: ComponentId;
 };
```

### Comparing `rio_ui-0.5.9/frontend/code/components/placeholder.ts` & `rio_ui-0.6/frontend/code/components/placeholder.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { SingleContainer } from './singleContainer';
 import { ComponentBase, ComponentState } from './componentBase';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 export type PlaceholderState = ComponentState & {
     _type_: 'Placeholder'; // Not 'Placeholder-builtin'!
     _child_?: ComponentId;
 };
 
 export class PlaceholderComponent extends SingleContainer {
```

### Comparing `rio_ui-0.5.9/frontend/code/components/plot.ts` & `rio_ui-0.6/frontend/code/components/plot.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { pixelsPerRem } from '../app';
 import { fillToCss } from '../cssUtils';
 import { LayoutContext } from '../layouting';
-import { Fill } from '../models';
+import { Fill } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 type PlotlyPlot = {
     type: 'plotly';
     json: string;
 };
 
@@ -90,15 +90,15 @@
 
                 svgElement.style.width = '100%';
                 svgElement.style.height = '100%';
             }
         }
 
         if (deltaState.background === null) {
-            this.element.style.background = 'var(--rio-local-plain-bg-variant)';
+            this.element.style.background = 'var(--rio-local-bg-variant)';
         } else if (deltaState.background !== undefined) {
             Object.assign(this.element.style, fillToCss(deltaState.background));
         }
 
         if (deltaState.corner_radius !== undefined) {
             let [topLeft, topRight, bottomRight, bottomLeft] =
                 deltaState.corner_radius;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/popup.ts` & `rio_ui-0.6/frontend/code/components/popup.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import { pixelsPerRem } from '../app';
 import { componentsById } from '../componentManagement';
-import { applyColorSet } from '../designApplication';
+import { applySwitcheroo } from '../designApplication';
 import { LayoutContext } from '../layouting';
-import { ColorSet, ComponentId } from '../models';
+import { ColorSet, ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type PopupState = ComponentState & {
     _type_: 'Popup-builtin';
     anchor?: ComponentId;
     content?: ComponentId;
     color?: ColorSet;
@@ -58,15 +58,15 @@
             this.open();
         } else {
             this.element.classList.remove('rio-popup-open');
         }
 
         // Colorize
         if (deltaState.color !== undefined) {
-            applyColorSet(this.element, deltaState.color);
+            applySwitcheroo(this.element, deltaState.color);
         }
     }
 
     open() {
         // Add the open class. This will trigger the CSS animation
         let element = this.element;
         element.classList.add('rio-popup-open');
```

### Comparing `rio_ui-0.5.9/frontend/code/components/progressCircle.ts` & `rio_ui-0.6/frontend/code/components/progressCircle.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import { applyColorSet } from '../designApplication';
-import { ColorSet } from '../models';
+import { applySwitcheroo } from '../designApplication';
+import { ColorSet } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type ProgressCircleState = ComponentState & {
     _type_: 'ProgressCircle-builtin';
     color: ColorSet;
     progress?: number | null;
 };
@@ -41,17 +41,13 @@
                         (1 - deltaState.progress) * fullCircle
                     }`
                 );
             }
         }
 
         // Apply the color
-        if (deltaState.color !== undefined) {
-            applyColorSet(
-                this.element,
-                deltaState.color === 'keep'
-                    ? 'accent-to-plain'
-                    : deltaState.color
-            );
-        }
+        applySwitcheroo(
+            this.element,
+            deltaState.color === 'keep' ? 'bump' : deltaState.color
+        );
     }
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/rectangle.ts` & `rio_ui-0.6/frontend/code/components/rectangle.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import { Color, ComponentId, Fill } from '../models';
+import { Color, ComponentId, Fill } from '../dataModels';
 import { colorToCssString, fillToCssString } from '../cssUtils';
 import { ComponentBase, ComponentState } from './componentBase';
-import { MDCRipple } from '@material/ripple';
+import { RippleEffect } from '../rippleEffect';
 import { SingleContainer } from './singleContainer';
 import { LayoutContext } from '../layouting';
 
 export type RectangleState = ComponentState & {
     _type_: 'Rectangle-builtin';
     content?: ComponentId | null;
     transition_time?: number;
@@ -48,95 +48,76 @@
 };
 
 export class RectangleComponent extends SingleContainer {
     state: Required<RectangleState>;
 
     // If this rectangle has a ripple effect, this is the ripple instance.
     // `null` otherwise.
-    private mdcRipple: MDCRipple | null = null;
+    private rippleInstance: RippleEffect | null = null;
 
     createElement(): HTMLElement {
         let element = document.createElement('div');
         element.classList.add('rio-rectangle');
         return element;
     }
 
     updateElement(
         deltaState: RectangleState,
         latentComponents: Set<ComponentBase>
     ): void {
-        let element = this.element;
-
         this.replaceOnlyChild(latentComponents, deltaState.content);
 
         if (deltaState.transition_time !== undefined) {
-            element.style.transitionDuration = `${deltaState.transition_time}s`;
+            this.element.style.transitionDuration = `${deltaState.transition_time}s`;
         }
 
         if (deltaState.cursor !== undefined) {
             if (deltaState.cursor === 'default') {
-                element.style.removeProperty('cursor');
+                this.element.style.removeProperty('cursor');
             } else {
-                element.style.cursor = deltaState.cursor;
+                this.element.style.cursor = deltaState.cursor;
             }
         }
 
         if (deltaState.ripple === true) {
-            if (this.mdcRipple === null) {
-                this.mdcRipple = new MDCRipple(element);
+            if (this.rippleInstance === null) {
+                this.rippleInstance = new RippleEffect(this.element);
 
-                element.classList.add('mdc-ripple-surface');
-                element.classList.add('rio-rectangle-ripple');
+                this.element.classList.add('rio-rectangle-ripple');
             }
         } else if (deltaState.ripple === false) {
-            if (this.mdcRipple !== null) {
-                this.mdcRipple.destroy();
-                this.mdcRipple = null;
+            if (this.rippleInstance !== null) {
+                this.rippleInstance.destroy();
+                this.rippleInstance = null;
 
-                element.classList.remove('mdc-ripple-surface');
-                element.classList.remove('rio-rectangle-ripple');
+                this.element.classList.remove('rio-rectangle-ripple');
             }
         }
 
         // Apply all the styling properties
         for (let [attrName, js_to_css] of Object.entries(JS_TO_CSS_VALUE)) {
             let value = deltaState[attrName];
             if (value !== undefined) {
-                element.style.setProperty(
+                this.element.style.setProperty(
                     `--rio-rectangle-${attrName}`,
                     js_to_css(value)
                 );
             }
 
             let hoverValue = deltaState['hover_' + attrName];
             if (hoverValue !== undefined) {
                 if (hoverValue === null) {
                     // No hover value? Use the corresponding non-hover value
-                    element.style.setProperty(
+                    this.element.style.setProperty(
                         `--rio-rectangle-hover-${attrName}`,
                         `var(--rio-rectangle-${attrName})`
                     );
                 } else {
-                    element.style.setProperty(
+                    this.element.style.setProperty(
                         `--rio-rectangle-hover-${attrName}`,
                         js_to_css(hoverValue)
                     );
                 }
             }
         }
     }
-
-    updateAllocatedHeight(ctx: LayoutContext): void {
-        super.updateAllocatedHeight(ctx);
-
-        // The ripple effect stores the coordinates of its rectangle. Since
-        // rio likes to resize and move around components, the rectangle must be
-        // updated appropriately.
-        if (this.mdcRipple !== null) {
-            requestAnimationFrame(() => {
-                if (this.mdcRipple !== null) {
-                    this.mdcRipple.layout();
-                }
-            });
-        }
-    }
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/revealer.ts` & `rio_ui-0.6/frontend/code/components/revealer.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import { componentsById } from '../componentManagement';
 import { textStyleToCss } from '../cssUtils';
 import { applyIcon } from '../designApplication';
 import { easeInOut } from '../easeFunctions';
 import { getTextDimensions } from '../layoutHelpers';
 import { LayoutContext, updateLayout } from '../layouting';
-import { ComponentId, TextStyle } from '../models';
+import { ComponentId, TextStyle } from '../dataModels';
 import { firstDefined } from '../utils';
 import { ComponentBase, ComponentState } from './componentBase';
+import { RippleEffect } from '../rippleEffect';
 
 let HEADER_PADDING: number = 0.6;
 
 export type RevealerState = ComponentState & {
     _type_: 'Revealer-builtin';
     header?: string | null;
     content?: ComponentId;
@@ -33,14 +34,16 @@
     private contentInnerElement: HTMLElement;
     private contentOuterElement: HTMLElement;
 
     private headerScale: number;
     private labelWidth: number;
     private labelHeight: number;
 
+    private rippleInstance: RippleEffect;
+
     createElement(): HTMLElement {
         // Create the HTML
         let element = document.createElement('div');
         element.classList.add('rio-revealer');
 
         element.innerHTML = `
             <div class="rio-revealer-header">
@@ -72,16 +75,23 @@
         this.contentOuterElement = element.querySelector(
             '.rio-revealer-content-outer'
         ) as HTMLElement;
 
         // Initialize them
         applyIcon(this.arrowElement, 'material/expand-more', 'currentColor');
 
+        this.rippleInstance = new RippleEffect(element, {
+            triggerOnPress: false,
+        });
+
         // Listen for presses
-        this.headerElement.onclick = (e) => {
+        this.headerElement.onclick = (event) => {
+            // Trigger the ripple effect
+            this.rippleInstance.trigger(event);
+
             // Toggle the open state
             this.state.is_open = !this.state.is_open;
 
             // Notify the backend
             this.setStateAndNotifyBackend({
                 is_open: this.state.is_open,
             });
@@ -95,15 +105,15 @@
 
             // Update the UI
             this.startAnimationIfNotRunning();
         };
 
         // Color change on hover/leave
         this.headerElement.onmouseenter = () => {
-            this.element.style.background = 'var(--rio-local-plain-bg-variant)';
+            this.element.style.background = 'var(--rio-local-bg-variant)';
         };
 
         this.headerElement.onmouseleave = () => {
             this.element.style.removeProperty('background');
         };
 
         return element;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/scrollContainer.ts` & `rio_ui-0.6/frontend/code/components/scrollContainer.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { pixelsPerRem, scrollBarSize } from '../app';
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 
 export type ScrollContainerState = ComponentState & {
     _type_: 'ScrollContainer-builtin';
     content?: ComponentId;
     scroll_x?: 'never' | 'auto' | 'always';
     scroll_y?: 'never' | 'auto' | 'always';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/separator.ts` & `rio_ui-0.6/frontend/code/components/separator.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { Color } from '../models';
+import { Color } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { pixelsPerRem } from '../app';
 import { LayoutContext } from '../layouting';
 import { colorToCssString } from '../cssUtils';
 
 export type SeparatorState = ComponentState & {
     _type_: 'Separator-builtin';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/separatorListItem.ts` & `rio_ui-0.6/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/singleContainer.ts` & `rio_ui-0.6/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/slideshow.ts` & `rio_ui-0.6/frontend/code/components/slideshow.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { ComponentBase, ComponentState } from './componentBase';
 import { easeIn, easeInOut, easeOut } from '../easeFunctions';
 import { SingleContainer } from './singleContainer';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 
 const switchDuration = 0.8;
 const progressBarFadeDuration = 0.2;
 
 export type SlideshowState = ComponentState & {
     _type_: 'Slideshow-builtin';
     children?: ComponentId[];
```

### Comparing `rio_ui-0.5.9/frontend/code/components/stack.ts` & `rio_ui-0.6/frontend/code/components/stack.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { SingleContainer } from './singleContainer';
 
 export type StackState = ComponentState & {
     _type_: 'Stack-builtin';
     children?: ComponentId[];
 };
```

### Comparing `rio_ui-0.5.9/frontend/code/components/switch.ts` & `rio_ui-0.6/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/switcher.ts` & `rio_ui-0.6/frontend/code/components/switcher.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { componentsById } from '../componentManagement';
 import { LayoutContext, updateLayout } from '../layouting';
 import { easeInOut } from '../easeFunctions';
 
 const TRANSITION_TIME: number = 0.35;
```

### Comparing `rio_ui-0.5.9/frontend/code/components/switcherBar.ts` & `rio_ui-0.6/frontend/code/components/switcherBar.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import { ComponentBase, ComponentState } from './componentBase';
-import { MDCRipple } from '@material/ripple';
-import { ColorSet, TextStyle } from '../models';
-import { applyColorSet } from '../designApplication';
+import { ColorSet, TextStyle } from '../dataModels';
+import { applySwitcheroo } from '../designApplication';
 import { getTextDimensions } from '../layoutHelpers';
 import { LayoutContext } from '../layouting';
 import { textStyleToCss } from '../cssUtils';
 import { easeInOut } from '../easeFunctions';
 import { firstDefined } from '../utils';
 
 const ACCELERATION: number = 350; // rem/s^2
@@ -386,17 +385,14 @@
             }
 
             // Text
             let textElement = document.createElement('div');
             optionElement.appendChild(textElement);
             textElement.textContent = name;
 
-            // Add a ripple effect
-            MDCRipple.attachTo(optionElement);
-
             // Detect clicks
             optionElement.addEventListener('click', (event) => {
                 // If this item was already selected, the new value may be `None`
                 if (this.state.selectedName === name) {
                     if (this.state.allow_none) {
                         this.state.selectedName = null;
                     } else {
@@ -498,19 +494,17 @@
             // Request updates
             markerPositionNeedsUpdate = true;
             needsReLayout = true;
         }
 
         // Color
         if (deltaState.color !== undefined) {
-            applyColorSet(
+            applySwitcheroo(
                 this.markerElement,
-                deltaState.color === 'keep'
-                    ? 'accent-to-plain'
-                    : deltaState.color
+                deltaState.color === 'keep' ? 'bump' : deltaState.color
             );
         }
 
         // Orientation
         if (deltaState.orientation !== undefined) {
             let flexDirection =
                 deltaState.orientation == 'vertical' ? 'column' : 'row';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/table.ts` & `rio_ui-0.6/frontend/code/components/table.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/code/components/text.ts` & `rio_ui-0.6/frontend/code/components/text.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { TextStyle } from '../models';
+import { TextStyle } from '../dataModels';
 import { textStyleToCss } from '../cssUtils';
 import { ComponentBase, ComponentState } from './componentBase';
 import { LayoutContext } from '../layouting';
 import { getTextDimensions } from '../layoutHelpers';
 
 export type TextState = ComponentState & {
     _type_: 'Text-builtin';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/textInput.ts` & `rio_ui-0.6/frontend/code/components/textInput.ts`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 
     private prefixTextWidth: number = 0;
     private suffixTextWidth: number = 0;
 
     createElement(): HTMLElement {
         // Create the element
         let element = document.createElement('div');
-        element.classList.add(
-            'rio-text-input',
-            'rio-input-box',
-            'mdc-ripple-surface'
-        );
+        element.classList.add('rio-text-input', 'rio-input-box');
 
         element.innerHTML = `
             <input type="text" style="order: 2" placeholder="">
             <div class="rio-text-input-hint-text rio-text-input-prefix-text" style="order: 1"></div>
             <div class="rio-text-input-hint-text rio-text-input-suffix-text" style="order: 3"></div>
             <div class="rio-input-box-label"></div>
             <div class="rio-input-box-plain-bar"></div>
```

### Comparing `rio_ui-0.5.9/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.6/frontend/code/components/themeContextSwitcher.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import { applyColorSet } from '../designApplication';
-import { ColorSet, ComponentId } from '../models';
+import { applySwitcheroo } from '../designApplication';
+import { ColorSet, ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
 import { SingleContainer } from './singleContainer';
 
 export type ThemeContextSwitcherState = ComponentState & {
     _type_: 'ThemeContextSwitcher-builtin';
     content?: ComponentId;
     color?: ColorSet;
@@ -22,11 +22,11 @@
         latentComponents: Set<ComponentBase>
     ): void {
         // Update the child
         this.replaceOnlyChild(latentComponents, deltaState.content);
 
         // Colorize
         if (deltaState.color !== undefined) {
-            applyColorSet(this.element, deltaState.color);
+            applySwitcheroo(this.element, deltaState.color);
         }
     }
 }
```

### Comparing `rio_ui-0.5.9/frontend/code/components/tooltip.ts` & `rio_ui-0.6/frontend/code/components/tooltip.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../models';
+import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
-import { SingleContainer } from './singleContainer';
 
 export type TooltipState = ComponentState & {
     _type_: 'Tooltip-builtin';
     anchor?: ComponentId;
-    tip_component?: ComponentId | null;
+    _tip_component?: ComponentId | null;
     position?: 'left' | 'top' | 'right' | 'bottom';
 };
 
 export class TooltipComponent extends ComponentBase {
     state: Required<TooltipState>;
 
     private anchorContainer: HTMLElement;
@@ -57,18 +56,18 @@
                 latentComponents,
                 deltaState.anchor,
                 this.anchorContainer
             );
         }
 
         // Update tip
-        if (deltaState.tip_component !== undefined) {
+        if (deltaState._tip_component !== undefined) {
             this.replaceOnlyChild(
                 latentComponents,
-                deltaState.tip_component,
+                deltaState._tip_component,
                 this.labelElement
             );
         }
 
         // Position
         if (deltaState.position !== undefined) {
             let left, top, right, bottom, transform;
@@ -111,28 +110,28 @@
 
     updateNaturalWidth(ctx: LayoutContext): void {
         this.naturalWidth = componentsById[this.state.anchor!]!.requestedWidth;
     }
 
     updateAllocatedWidth(ctx: LayoutContext): void {
         let anchor = componentsById[this.state.anchor!]!;
-        let tip = componentsById[this.state.tip_component!]!;
+        let tip = componentsById[this.state._tip_component!]!;
 
         anchor.allocatedWidth = this.allocatedWidth;
         tip.allocatedWidth = tip.naturalWidth;
     }
 
     updateNaturalHeight(ctx: LayoutContext): void {
         this.naturalHeight =
             componentsById[this.state.anchor!]!.requestedHeight;
     }
 
     updateAllocatedHeight(ctx: LayoutContext): void {
         let anchor = componentsById[this.state.anchor!]!;
-        let tip = componentsById[this.state.tip_component!]!;
+        let tip = componentsById[this.state._tip_component!]!;
 
         anchor.allocatedHeight = this.allocatedHeight;
         tip.allocatedHeight = tip.naturalHeight;
 
         // Position the children
         anchor.element.style.left = '0';
         anchor.element.style.top = '0';
```

### Comparing `rio_ui-0.5.9/frontend/code/components/website.ts` & `rio_ui-0.6/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/css/fonts.scss` & `rio_ui-0.6/frontend/css/fonts.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.6/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/frontend/css/highlightjs-default-light.css` & `rio_ui-0.6/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/prototyping/icon_search.py` & `rio_ui-0.6/prototyping/icon_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,23 @@
     # "multi-qa-MiniLM-L6-cos-v1",
 )
 
 
 query = "alarm"
 query_embedding = model.encode("How big is London")
 
-hay = scan_for_icons(Path("/home/jakob/.cache/rio/extracted-icon-sets/material"))
+hay = scan_for_icons(
+    Path("/home/jakob/.cache/rio/extracted-icon-sets/material")
+)
 hay_embeddings = model.encode(hay)
 
 # Find the 5 most similar entries
-similarities = sentence_transformers.util.dot_score(query_embedding, hay_embeddings)
+similarities = sentence_transformers.util.dot_score(
+    query_embedding, hay_embeddings
+)
 similarities = similarities.ravel()
 
 topk = np.argsort(similarities)
 topk = topk[-5:]
 
 
 for ii in topk:
```

### Comparing `rio_ui-0.5.9/prototyping/pack.py` & `rio_ui-0.6/prototyping/pack.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import revel
 from revel import input, print, print_chapter, warning
 
 import rio.cli
 from rio.cli.rio_api import RioApi
 
 
-def should_directory_likely_be_excluded(dir_path: Path) -> tuple[str, str] | None:
+def should_directory_likely_be_excluded(
+    dir_path: Path,
+) -> tuple[str, str] | None:
     """
     Some directories should very likely not be part of the user's project. This
     function looks at a directory, and if the directory should likely be
     excluded it returns a name and explanation of why. Returns `None` otherwise.
     """
     assert dir_path.is_dir(), dir_path
 
@@ -81,18 +83,23 @@
         # If this is a file, yield it
         if path.is_file():
             yield path
             continue
 
         # Is this a directory that the user likely doesn't want to include?
         exclude_reason = should_directory_likely_be_excluded(path)
-        if exclude_reason is not None and not proj.ignores.is_explicitly_included(path):
+        if (
+            exclude_reason is not None
+            and not proj.ignores.is_explicitly_included(path)
+        ):
             appears_to, explanation = exclude_reason
             rel_path = path.relative_to(proj.project_directory)
-            warning(f'Excluding "{rel_path}". This directory appears to {appears_to}.')
+            warning(
+                f'Excluding "{rel_path}". This directory appears to {appears_to}.'
+            )
             warning(explanation)
             warning(
                 f'If you do want to include it after all, add the following to your ".rioignore" file:'
             )
             warning(f"!{rel_path}")
             print()
 
@@ -194,16 +201,20 @@
     print_chapter("Packaging project")
     with tempfile.TemporaryDirectory() as tmp_dir:
         assert Path(tmp_dir).exists(), tmp_dir
         archive_path = Path(tmp_dir) / "packed-project.tar.xz"
         uncompressed_size_in_bytes = pack_up_project(proj, archive_path)
         compressed_size_in_bytes = archive_path.stat().st_size
 
-        print(f"Compressed size: {compressed_size_in_bytes / 1024 / 1024:.2f} MiB")
-        print(f"Uncompressed size: {uncompressed_size_in_bytes / 1024 / 1024:.2f} MiB")
+        print(
+            f"Compressed size: {compressed_size_in_bytes / 1024 / 1024:.2f} MiB"
+        )
+        print(
+            f"Uncompressed size: {uncompressed_size_in_bytes / 1024 / 1024:.2f} MiB"
+        )
         print(
             f"Compression ratio: {uncompressed_size_in_bytes / compressed_size_in_bytes:.2f}x"
         )
 
     # Make sure the user has the ability to create this app
     # TODO:
     # - # of apps
```

### Comparing `rio_ui-0.5.9/prototyping/webgl.html` & `rio_ui-0.6/prototyping/webgl.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/prototyping/node_editor/__main__.py` & `rio_ui-0.6/prototyping/node_editor/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,13 +16,13 @@
                 rio.Text("Child 1"),
                 rio.NodeOutput("output 1", rio.Color.RED, key="output1"),
             ),
             rio.NodeInput("input 2", rio.Color.RED, key="input2"),
             rio.NodeOutput("output 2", rio.Color.RED, key="output2"),
         ],
     ),
-    theme=rio.Theme.from_color(light=False),
+    theme=rio.Theme.from_colors(light=False),
 )
 
 app.run_as_web_server(
     port=8001,
 )
```

### Comparing `rio_ui-0.5.9/prototyping/node_editor/index.html` & `rio_ui-0.6/prototyping/node_editor/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/prototyping/node_editor/script.ts` & `rio_ui-0.6/prototyping/node_editor/script.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/prototyping/node_editor/styles.scss` & `rio_ui-0.6/prototyping/node_editor/styles.scss`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     gap: 0.5rem;
 
     padding: $node-padding;
 
     border-radius: 0 0 var(--rio-global-corner-radius-small)
         var(--rio-global-corner-radius-small);
 
-    background-color: var(--rio-local-plain-bg);
+    background-color: var(--rio-local-bg);
 
     // By default, the margin is negative rather than just zero. This is to
     // prevent the odd pixel peeping through when the node isn't hovered. These
     // can be really obvious and distracting, since the body is neutrally
     // colored, while the header is bright and colorful.
     //
     // This in turn makes animations awkward, as any amount of time causes a
```

### Comparing `rio_ui-0.5.9/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.6/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.6/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.6/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.6/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/logo.svg` & `rio_ui-0.6/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.6/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.6/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/color/logo.svg` & `rio_ui-0.6/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.6/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.6/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/rio/fill/logo.svg` & `rio_ui-0.6/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.6/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.6/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.6/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.6/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/scripts/benchmark.py` & `rio_ui-0.6/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/scripts/build_material_icon_set.py` & `rio_ui-0.6/scripts/build_material_icon_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,17 @@
                 parsed = name_from_icon_path(file_path.relative_to(INPUT_DIR))
 
                 if parsed is None:
                     print(f"{file_path.name} -> [bold]skipped[/bold]")
                     continue
 
                 icon_name, icon_variant = parsed
-                variant_suffix = "" if icon_variant is None else f"/{icon_variant}"
+                variant_suffix = (
+                    "" if icon_variant is None else f"/{icon_variant}"
+                )
 
                 print(f"{file_path.name} -> {icon_name}{variant_suffix}")
 
                 # Parse the SVG
                 svg_str = file_path.read_text()
                 tree = ET.fromstring(svg_str)
```

### Comparing `rio_ui-0.5.9/scripts/check_docs.py` & `rio_ui-0.6/scripts/check_docs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Helper script for running checks on documentation, such as looking for missing
 docstrings.
 """
 
-import inspect
 import sys
 from pathlib import Path
 from typing import *  # type: ignore
 
 import imy.docstrings
 
 # Some rio modules optionally depend on libraries and evaling their type
@@ -23,43 +22,50 @@
 
 
 def check_function(
     docs: imy.docstrings.FunctionDocs,
     owning_cls: type | None,
 ) -> None:
     qualname = (
-        f"{owning_cls.__name__}.{docs.name}" if owning_cls is not None else docs.name
+        f"{owning_cls.__name__}.{docs.name}"
+        if owning_cls is not None
+        else docs.name
     )
 
     # __init__ methods for components need no documentation, since the
     # class' documentation already fills that role
     if (
         docs.name == "__init__"
         and owning_cls is not None
         and issubclass(owning_cls, rio.Component)
     ):  # type: ignore
         return
 
     # Run checks
-    if docs.summary is None and docs.name != "__init__":
-        warning(f"Docstring for `{qualname}` is missing a short description")
+    if docs.name != "__init__":
+        if docs.summary is None:
+            warning(
+                f"Docstring for `{qualname}` is missing a short description"
+            )
 
-    if docs.details is None and docs.name != "__init__":
-        warning(f"Docstring for `{qualname}` is missing a long description")
+        if docs.details is None:
+            warning(f"Docstring for `{qualname}` is missing a long description")
 
-    if docs.return_type is None:
-        warning(f"`{qualname}` is missing a return type hint")
+        if docs.return_type is imy.docstrings.Unset:
+            warning(f"`{qualname}` is missing a return type hint")
 
     # Chain to parameters
     for param in docs.parameters:
         if param.name == "self":
             continue
 
         if param.type is None:
-            warning(f"`{qualname}` is missing a type hint for parameter `{param.name}`")
+            warning(
+                f"`{qualname}` is missing a type hint for parameter `{param.name}`"
+            )
 
         if param.description is None:
             warning(
                 f"Docstring for `{qualname}` is missing a description for parameter `{param.name}`"
             )
 
 
@@ -69,15 +75,17 @@
         warning(f"Docstring for `{docs.name}` is missing a short description")
 
     if docs.details is None:
         warning(f"Docstring for `{docs.name}` is missing a long description")
 
     for attr in docs.attributes:
         if attr.description is None:
-            warning(f"Docstring for `{docs.name}.{attr.name}` is missing a description")
+            warning(
+                f"Docstring for `{docs.name}.{attr.name}` is missing a description"
+            )
 
     for func_docs in docs.functions:
         check_function(func_docs, cls)
 
 
 def main() -> None:
     print_chapter("Saving you hours of debugging")
@@ -91,63 +99,38 @@
         "An easy way to find out is to run this script in a debugger and "
         "have it stop on exceptions. Go up one scope in the stack and "
         "display the value of `globalns`."
     )
 
     # Find all items that should be documented
     print_chapter("Looking for objects in the Rio module")
-    candidate_objects: list[type | Callable[..., Any]] = list(
-        rio.docs.custom.find_objects_possibly_needing_documentation()
-    )
+    public_objects = {
+        obj: docs
+        for obj, docs in rio.docs.find_documented_objects(postprocess=True)
+        if docs.metadata.public
+    }
 
-    print(f"Found {len(candidate_objects)} items")
+    print(f"Found {len(public_objects)} items")
 
     # Make sure they're all properly documented
     print_chapter("Making you depressed")
-    for item in candidate_objects:
+    for item, docs in public_objects.items():
         # Classes / Components
-        if inspect.isclass(item):
-            # Fetch the docs
-            docs = imy.docstrings.ClassDocs.from_class(item)
-
-            # Drop internals
-            if not docs.metadata.public:
-                continue
-
-            # Post-process them as needed
-            if isinstance(item, rio.Component):
-                rio.docs.custom.postprocess_component_docs(docs)
-            else:
-                rio.docs.custom.postprocess_class_docs(docs)
-
+        if isinstance(docs, imy.docstrings.ClassDocs):
+            item = cast(type, item)
             check_class(item, docs)
-
         else:
-            assert inspect.isfunction(item), item
-
-            # Fetch the docs
-            docs = imy.docstrings.FunctionDocs.from_function(item)
-
-            # Drop internals
-            if not docs.metadata.public:
-                continue
-
             check_function(docs, None)
 
     # Make sure all items are displayed Rio's documentation
-    visited_item_names: set[str] = set()
-
-    for entry in rio_website.structure.DOCUMENTATION_STRUCTURE_LINEAR:
-        section_name, section_url, builder = entry
-
-        if not isinstance(builder, rio_website.article_models.ArticleBuilder):
-            continue
+    visited_objects: set[object] = set()
 
-        visited_item_names.add(builder.component_class.__name__)
+    for _, _, _, objects in rio_website.structure.API_DOCS_SECTIONS:
+        visited_objects.update(objects)
 
-    for item in candidate_objects:
-        if item.__name__ not in visited_item_names:
-            warning(f"Item `{item.__name__}` is not displayed in the documentation")
+    unvisited_objects = public_objects.keys() - visited_objects
+    for obj in unvisited_objects:
+        warning(f"Item `{obj.__name__}` is not displayed in the documentation")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rio_ui-0.5.9/scripts/code_coverage.py` & `rio_ui-0.6/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/scripts/publish_new_release.py` & `rio_ui-0.6/scripts/publish_new_release.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,75 @@
 import subprocess
-from pathlib import Path
+import sys
 
 import requests
 import revel
 
-PROJECT_DIR = Path(__file__).absolute().parent.parent
+import rio
 
 
 def main() -> None:
+    revel.print("Running sanity checks...")
+
     # Make sure we're on the correct branch
     process = subprocess.run(
-        ["git", "branch"], check=True, capture_output=True, text=True
+        ["git", "branch", "--show-current"],
+        check=True,
+        capture_output=True,
+        text=True,
     )
     if process.stdout.strip("\n") != "dev":
         revel.fatal("You must checkout the 'dev' branch")
 
+    # Make sure there are no uncommitted changes
+    process = subprocess.run(
+        ["git", "status", "--porcelain"],
+        check=True,
+        capture_output=True,
+        text=True,
+    )
+    if process.stdout.strip():
+        revel.fatal("There are uncommitted changes")
+
     # Make sure the version number got bumped
-    version = get_current_version()
-    if version == get_latest_published_version():
+    if rio.__version__ == get_latest_published_version():
         revel.fatal("You forgot to increment the version number")
 
     # Build the TS code
-    subprocess.run(["rye", "run", "build"], check=True)
+    #
+    # Note: `shell=True` is required on Windows because `npm` is a `.cmd` file
+    # and not a `.exe`
+    subprocess.run(["npm", "run", "build"], shell=True, check=True)
 
     # Run the test suite
-    if not tests_pass():
-        revel.fatal("The test don't pass")
+    if tests_pass():
+        revel.print("Everything is in order. Publishing...")
+    else:
+        # revel.fatal("The test don't pass")
+        if not revel.select_yes_no(
+            "The test suite does not pass. Do you want to publish anyway?"
+        ):
+            sys.exit(1)
+
+        revel.print("Publishing...")
 
     # Merge dev into main and push
     subprocess.run(["git", "fetch", ".", "dev:main"], check=True)
     subprocess.run(["git", "push", "-u", "origin", "main"], check=True)
 
     # Publish
-    subprocess.run(["rye", "publish", "--skip-existing"], check=True)
+    subprocess.run(["rye", "build", "--clean"], check=True)
+    subprocess.run(["rye", "publish"], check=True)
 
 
 def get_latest_published_version() -> str:
     response = requests.get(f"https://pypi.org/pypi/rio-ui/json")
     return response.json()["info"]["version"]
 
 
-def get_current_version() -> str:
-    process = subprocess.run(
-        ["rye", "version"], capture_output=True, text=True, check=True
-    )
-    return process.stdout.strip()
-
-
 def tests_pass() -> bool:
-    return subprocess.run(["rye", "test"], check=True) == 0
+    process = subprocess.run(["rye", "test", "--", "-x", "--disable-warnings"])
+    return process.returncode == 0
 
 
-main()
+if __name__ == "__main__":
+    main()
```

### Comparing `rio_ui-0.5.9/src/rio/__init__.py` & `rio_ui-0.6/rio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-__version__ = "0.5.9"
+__version__ = "0.6"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
 from dataclasses import field as field
 
 # URLs are used as an important datatype within rio. Re-export them for easy
 # use.
 from yarl import URL as URL
 
-# Fix issues in 3rd-party code (like asyncio)
 from . import event as event
 from . import patches_for_3rd_party_stuff
 from .app import *
 from .color import *
 from .common import *
 from .components import *
 from .cursor_style import *
```

### Comparing `rio_ui-0.5.9/src/rio/app.py` & `rio_ui-0.6/rio/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 import uvicorn
 
 import rio
 
 from . import app_server, assets, common, debug, maybes
 from .common import ImageLike
 
-# Only available with the `window` extra
-try:
-    import webview  # type: ignore
-except ImportError:
-    webview = None
-
 
 __all__ = [
     "App",
 ]
 
 
 def make_default_connection_lost_component() -> rio.Component:
@@ -103,27 +97,29 @@
     Or create a server, without running it. This allows you to start the script
     externally with tools such as uvicorn:
 
     ```py
     fastapi_app = app.as_fastapi()
     ```
 
+
     ## Attributes
-        name: The name to display for this app. This can show up in window
-            titles, error messages and wherever else the app needs to be
-            referenced in a nice, human-readable way.
 
-        pages: The pages that make up this app. You can navigate between these
-            using `Session.navigate_to` or using `Link` components. If running
-            as website the user can also access these pages directly via their
-            URL.
-
-        assets_dir: The directory where the app's assets are stored. This allows
-            you to conveniently access any images or other files that are needed
-            by your app.
+    `name`: The name to display for this app. This can show up in window
+        titles, error messages and wherever else the app needs to be
+        referenced in a nice, human-readable way.
+
+    `pages`: The pages that make up this app. You can navigate between these
+        using `Session.navigate_to` or using `Link` components. If running
+        as website the user can also access these pages directly via their
+        URL.
+
+    `assets_dir`: The directory where the app's assets are stored. This allows
+        you to conveniently access any images or other files that are needed
+        by your app.
     """
 
     # Type hints so the documentation generator knows which fields exist
     name: str
     pages: tuple[rio.Page, ...]
     assets_dir: Path
 
@@ -143,90 +139,102 @@
         assets_dir: str | os.PathLike = "assets",
         theme: rio.Theme | tuple[rio.Theme, rio.Theme] | None = None,
         build_connection_lost_message: Callable[
             [], rio.Component
         ] = make_default_connection_lost_component,
     ):
         """
-        Args:
-            build: A function that returns the root component of the app. This
-                function will be called whenever a new session is created. Note
-                that since classes are callable in Python, you can pass a class
-                here instead of a function, so long as the class doesn't require
-                any arguments.
-
-                If no build method is passed, the app will create a `PageView`
-                as the root component.
-
-            name: The name to display for this app. This can show up in window
-                titles, error messages and wherever else the app needs to be
-                referenced in a nice, human-readable way. If not specified,
-                `Rio` name will try to guess a name based on the name of the
-                main Python file.
-
-            icon: The icon to display for this app. This can show up in window
-                the title bars of windows, browser tabs, or similar.
-
-            pages: The pages that make up this app. You can navigate between
-                these using `Session.navigate_to` or using `Link` components. If
-                running as website the user can also access these pages directly
-                via their URL.
-
-            on_app_start: A function that will be called when the app is first
-                started. You can use this to perform any initialization tasks
-                that need to happen before the app is ready to use.
-
-                The app start will be delayed until this function returns. This
-                makes sure initialization is complete before the app is
-                displayed to the user. If you would prefer to perform
-                initialization in the background try using `asyncio.create_task`
-                to run your code in a separate task.
-
-            on_session_start: A function that will be called each time a new
-                session is created. In the context of a website that would be
-                each time a new user visits the site. In the context of a window
-                there is only one session, so this will only be called once.
-
-                This function does not block the creation of the session. This
-                is to make sure initialization code doesn't accidentally make
-                the user wait.
-
-            on_session_close: A function that will be called each time a session
-                ends. In the context of a website that would be each time a user
-                closes their browser tab. In the context of a window this will
-                only be called once, when the window is closed.
-
-            default_attachments: A list of attachments that will be attached to
-                every new session.
-
-            ping_pong_interval: Rio periodically sends ping-pong messages
-                between the client and server to prevent overzealous proxies
-                from closing the connection. The default value should be fine
-                for most deployments, but feel free to change it if your hosting
-                provider deploys a particularly obnoxious proxy.
-
-            assets_dir: The directory where the app's assets are stored. This
-                allows you to conveniently access any images or other files that
-                are needed by your app. If not specified, Rio will assume the
-                assets are stored in a directory called "assets" in the same
-                directory as the main Python file.
+        ## Parameters
+
+        `build`: A function that returns the root component of the app. This
+            function will be called whenever a new session is created. Note
+            that since classes are callable in Python, you can pass a class
+            here instead of a function, so long as the class doesn't require
+            any arguments.
+
+            If no build method is passed, the app will create a `PageView`
+            as the root component.
+
+        `name`: The name to display for this app. This can show up in window
+            titles, error messages and wherever else the app needs to be
+            referenced in a nice, human-readable way. If not specified,
+            `Rio` name will try to guess a name based on the name of the
+            main Python file.
+
+        `icon`: The icon to display for this app. This can show up in window
+            the title bars of windows, browser tabs, or similar.
+
+        `theme`: The `Theme` for the app. You can also pass in a tuple of two
+            themes, which will be used as the light mode theme and the dark mode
+            theme.
+
+        `pages`: The pages that make up this app. You can navigate between
+            these using `Session.navigate_to` or using `Link` components. If
+            running as website the user can also access these pages directly
+            via their URL.
+
+        `on_app_start`: A function that will be called when the app is first
+            started. You can use this to perform any initialization tasks
+            that need to happen before the app is ready to use.
+
+            The app start will be delayed until this function returns. This
+            makes sure initialization is complete before the app is
+            displayed to the user. If you would prefer to perform
+            initialization in the background try using `asyncio.create_task`
+            to run your code in a separate task.
+
+        `on_app_close`: A function that will be called right before the app
+            shuts down. You can use this to clean up open resources like for
+            example a database connection.
+
+        `on_session_start`: A function that will be called each time a new
+            session is created. In the context of a website that would be
+            each time a new user visits the site. In the context of a window
+            there is only one session, so this will only be called once.
+
+            This function does not block the creation of the session. This
+            is to make sure initialization code doesn't accidentally make
+            the user wait.
+
+        `on_session_close`: A function that will be called each time a session
+            ends. In the context of a website that would be each time a user
+            closes their browser tab. In the context of a window this will
+            only be called once, when the window is closed.
+
+        `default_attachments`: A list of attachments that will be attached to
+            every new session.
+
+        `ping_pong_interval`: Rio periodically sends ping-pong messages
+            between the client and server to prevent overzealous proxies
+            from closing the connection. The default value should be fine
+            for most deployments, but feel free to change it if your hosting
+            provider deploys a particularly obnoxious proxy.
+
+        `assets_dir`: The directory where the app's assets are stored. This
+            allows you to conveniently access any images or other files that
+            are needed by your app. If not specified, Rio will assume the
+            assets are stored in a directory called "assets" in the same
+            directory as the main Python file.
+
+        `build_connection_lost_message`: A function that creates a "Connection
+            lost" error popup, in case you want to override the default one.
         """
         main_file = _get_main_file()
 
         if name is None:
             name = _get_default_app_name(main_file)
 
         if icon is None:
             icon = common.HOSTED_ASSETS_DIR / "rio-logos/rio-logo-square.png"
 
         if build is None:
             build = rio.PageView
 
         if theme is None:
-            theme = rio.Theme.from_color()
+            theme = rio.Theme.from_colors()
 
         # The `main_file` isn't detected correctly if the app is launched via
         # `rio run`. We'll store the user input so that `rio run` can fix the
         # assets dir.
         self._assets_dir = assets_dir
         self.assets_dir = main_file.parent / assets_dir
 
@@ -234,15 +242,17 @@
         self._build = build
         self._icon = assets.Asset.from_image(icon)
         self.pages = tuple(pages)
         self._on_app_start = on_app_start
         self._on_app_close = on_app_close
         self._on_session_start = on_session_start
         self._on_session_close = on_session_close
-        self.default_attachments: MutableSequence[Any] = list(default_attachments)
+        self.default_attachments: MutableSequence[Any] = list(
+            default_attachments
+        )
         self._theme = theme
         self._build_connection_lost_message = build_connection_lost_message
 
         if isinstance(ping_pong_interval, timedelta):
             self._ping_pong_interval = ping_pong_interval
         else:
             self._ping_pong_interval = timedelta(seconds=ping_pong_interval)
@@ -304,17 +314,19 @@
     def _run_as_web_server(
         self,
         *,
         host: str,
         port: int,
         quiet: bool,
         running_in_window: bool,
-        validator_factory: Callable[[rio.Session], debug.Validator] | None = None,
+        validator_factory: Callable[[rio.Session], debug.Validator]
+        | None = None,
         internal_on_app_start: Callable[[], None] | None = None,
-        internal_on_server_created: Callable[[uvicorn.Server], None] | None = None,
+        internal_on_server_created: Callable[[uvicorn.Server], None]
+        | None = None,
     ) -> None:
         """
         Internal equivalent of `run_as_web_server` that takes additional
         arguments.
         """
         port = common.ensure_valid_port(host, port)
 
@@ -375,23 +387,24 @@
         )
 
         app.run_as_web_server()
         ```
 
         The will synchronously block until the server is shut down.
 
-        Args:
-            host: Which IP address to serve the webserver on. `localhost` will
-                make the service only available on your local machine. This is
-                the recommended setting if running behind a proxy like nginx.
+        ## Parameters
+
+        host: Which IP address to serve the webserver on. `localhost` will
+            make the service only available on your local machine. This is
+            the recommended setting if running behind a proxy like nginx.
 
-            port: Which port the webserver should listen to.
+        port: Which port the webserver should listen to.
 
-            quiet: If `True` Rio won't send any routine messages to `stdout`.
-                Error messages will be printed regardless of this setting.
+        quiet: If `True` Rio won't send any routine messages to `stdout`.
+            Error messages will be printed regardless of this setting.
         """
         self._run_as_web_server(
             host=host,
             port=port,
             quiet=quiet,
             running_in_window=False,
         )
@@ -403,36 +416,36 @@
         port: int | None = None,
         quiet: bool = False,
     ) -> None:
         """
         Runs an internal webserver and opens the app in the default browser.
 
         This method creates and immediately runs a webserver that serves this
-        app, and then opens the app in the default browser. This is a quick and easy
-        way to access your app.
+        app, and then opens the app in the default browser. This is a quick and
+        easy way to access your app.
 
         ```py
         app = rio.App(
             name="My App",
             build=MyAppRoot,
         )
 
         app.run_in_browser()
         ```
 
-        Args:
-            host: Which IP address to serve the webserver on. `localhost` will
-                make the service only available on your local machine. This is
-                the recommended setting if running behind a proxy like nginx.
+        ## Parameters
+        host: Which IP address to serve the webserver on. `localhost` will
+            make the service only available on your local machine. This is the
+            recommended setting if running behind a proxy like nginx.
 
-            port: Which port the webserver should listen to. If not specified,
-                Rio will choose a random free port.
+        port: Which port the webserver should listen to. If not specified,
+            Rio will choose a random free port.
 
-            quiet: If `True` Rio won't send any routine messages to `stdout`.
-                Error messages will be printed regardless of this setting.
+        quiet: If `True` Rio won't send any routine messages to `stdout`.
+            Error messages will be printed regardless of this setting.
         """
         port = common.ensure_valid_port(host, port)
 
         def on_startup() -> None:
             webbrowser.open(f"http://{host}:{port}")
 
         self._run_as_web_server(
@@ -468,24 +481,27 @@
 
         ```sh
         pip install rio-ui[window]
         ```
 
         This method will synchronously block until the window is closed.
 
-        Args:
-            quiet: If `True` Rio won't send any routine messages to `stdout`.
-                Error messages will be printed regardless of this setting.
-        """
 
-        if webview is None:
+        ## Parameters
+
+        `quiet`: If `True` Rio won't send any routine messages to `stdout`.
+            Error messages will be printed regardless of this setting.
+        """
+        try:
+            import webview  # type: ignore
+        except ImportError:
             raise Exception(
                 "The `window` extra is required to use `App.run_in_window`."
                 " Run `pip install rio-ui[window]` to install it."
-            )
+            ) from None
 
         # Unfortunately, WebView must run in the main thread, which makes this
         # tricky. We'll have to banish uvicorn to a background thread, and shut
         # it down when the window is closed.
 
         host = "localhost"
         port = common.ensure_valid_port(host, None)
@@ -515,19 +531,16 @@
         server_thread.start()
 
         # Wait for the server to start
         app_ready_event.wait()
 
         # Start the webview
         try:
-            webview.create_window(
-                self.name,
-                url,
-            )
-            webview.start()
+            webview.create_window(self.name, url)
+            webview.start(debug=os.environ.get("RIO_WEBVIEW_DEBUG") == "1")
 
         finally:
             assert isinstance(server, uvicorn.Server)
 
             server.should_exit = True
             server_thread.join()
```

### Comparing `rio_ui-0.5.9/src/rio/app_server.py` & `rio_ui-0.6/rio/app_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,23 +185,27 @@
         ] = timer_dict.TimerDict(default_duration=timedelta(minutes=15))
 
         # FastAPI
         self.add_api_route("/robots.txt", self._serve_robots, methods=["GET"])
         self.add_api_route("/rio/sitemap", self._serve_sitemap, methods=["GET"])
         # self.add_api_route("/app.js.map", self._serve_js_map, methods=["GET"])
         # self.add_api_route("/style.css.map", self._serve_css_map, methods=["GET"])
-        self.add_api_route("/rio/favicon.png", self._serve_favicon, methods=["GET"])
+        self.add_api_route(
+            "/rio/favicon.png", self._serve_favicon, methods=["GET"]
+        )
         self.add_api_route(
             "/rio/asset/{asset_id:path}", self._serve_asset, methods=["GET"]
         )
         self.add_api_route(
             "/rio/icon/{icon_name:path}", self._serve_icon, methods=["GET"]
         )
         self.add_api_route(
-            "/rio/upload/{upload_token}", self._serve_file_upload, methods=["PUT"]
+            "/rio/upload/{upload_token}",
+            self._serve_file_upload,
+            methods=["PUT"],
         )
         self.add_api_websocket_route("/rio/ws", self._serve_websocket)
 
         # Because this is a single page application, all other routes should
         # serve the index page. The session will determine which components
         # should be shown.
         self.add_api_route(
@@ -268,15 +272,18 @@
             # Close all sessions
             rio._logger.debug(
                 f"App server shutting down; closing"
                 f" {len(self._active_session_tokens)} active session(s)"
             )
 
             results = await asyncio.gather(
-                *(sess._close(True) for sess in self._active_session_tokens.values()),
+                *(
+                    sess._close(True)
+                    for sess in self._active_session_tokens.values()
+                ),
                 return_exceptions=True,
             )
             for result in results:
                 if isinstance(result, BaseException):
                     traceback.print_exception(
                         type(result), result, result.__traceback__
                     )
@@ -290,15 +297,17 @@
         Python objects are alive.
 
         If another asset with the same id is already hosted, it will be
         replaced.
         """
         self._assets[asset.secret_id] = asset
 
-    def host_asset_with_timeout(self, asset: assets.HostedAsset, timeout: float) -> URL:
+    def host_asset_with_timeout(
+        self, asset: assets.HostedAsset, timeout: float
+    ) -> URL:
         """
         Hosts an asset for a limited time. Returns the asset's url.
         """
         self.weakly_host_asset(asset)
 
         async def keep_alive():
             await asyncio.sleep(timeout)
@@ -367,27 +376,27 @@
         html = html.replace(
             '"{child_attribute_names}"',
             json.dumps(
                 inspection.get_child_component_containing_attribute_names_for_builtin_components()
             ),
         )
 
-        # TODO: uvicorn has ping-pong built in, configurable via `ws_ping_interval`
         html = html.replace(
             '"{ping_pong_interval}"',
             str(self.app._ping_pong_interval.total_seconds()),
         )
 
         html = html.replace(
             '"{debug_mode}"',
             json.dumps(self.debug_mode),
         )
 
         html = html.replace(
-            '"{running_in_window}"', "true" if self.running_in_window else "false"
+            '"{running_in_window}"',
+            "true" if self.running_in_window else "false",
         )
 
         html = html.replace("{title}", self.app.name)
 
         # Respond
         return fastapi.responses.HTMLResponse(html)
 
@@ -627,15 +636,17 @@
                     media_type=file_types[ii],
                     _contents=await file_streams[ii].read(),
                 )
                 for ii in range(n_names)
             ]
         )
 
-        return fastapi.responses.Response(status_code=fastapi.status.HTTP_200_OK)
+        return fastapi.responses.Response(
+            status_code=fastapi.status.HTTP_200_OK
+        )
 
     async def _serve_websocket(
         self,
         websocket: fastapi.WebSocket,
         sessionToken: str,
     ):
         """
@@ -669,15 +680,17 @@
                 3000,  # Custom error code
                 "Invalid session token.",
             )
             return
 
         # Optionally create a validator
         validator_instance = (
-            None if self.validator_factory is None else self.validator_factory(sess)
+            None
+            if self.validator_factory is None
+            else self.validator_factory(sess)
         )
 
         # Create a function for sending messages to the frontend. This function
         # will also pipe the message to the validator if one is present.
         if self.validator_factory is None:
 
             async def send_message(msg: uniserde.Jsonable) -> None:
@@ -852,15 +865,17 @@
 
         global_state.currently_building_session = None
 
         # Trigger the `on_session_start` event.
         #
         # Since this event is often used for important initialization tasks like
         # adding attachments, actually wait for it to finish before continuing.
-        await sess._call_event_handler(self.app._on_session_start, sess, refresh=False)
+        await sess._call_event_handler(
+            self.app._on_session_start, sess, refresh=False
+        )
 
         # Run any page guards for the initial page
         #
         # Guards have access to the session. Thus, it should be fully
         # initialized, or at least pretend to be. Fill in any not yet final
         # values with placeholders.
         sess._base_url = (
@@ -875,21 +890,23 @@
         # Then, run the guards
         try:
             (
                 active_page_instances,
                 active_page_url_absolute,
             ) = routing.check_page_guards(
                 sess,
-                sess._base_url.join(rio.URL(initial_message.website_url.lower())),
+                sess._base_url.join(
+                    rio.URL(initial_message.website_url.lower())
+                ),
             )
         except routing.NavigationFailed:
             # TODO: Notify the client? Show an error?
             raise fastapi.HTTPException(
                 status_code=fastapi.status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=f'Navigation to initial page "{sess._active_page_url}" has failed.',
+                detail=f"Navigation to initial page `{sess._active_page_url}` has failed.",
             ) from None
 
         # Is this a page, or a full URL to another site?
         try:
             common.make_url_relative(
                 sess._base_url,
                 active_page_url_absolute,
```

### Comparing `rio_ui-0.5.9/src/rio/assets.py` & `rio_ui-0.6/rio/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import abc
 import hashlib
 import io
 import os
 import secrets
 from pathlib import Path
 from typing import *  # type: ignore
+from typing_extensions import Self
 
 import httpx
 from PIL.Image import Image
 from yarl import URL
 
 import rio
 
@@ -21,17 +22,17 @@
 # difficult to guess
 _HASH_SALT = secrets.token_bytes(32)
 
 
 def _securely_hash_bytes_changes_between_runs(data: bytes) -> bytes:
     """
     Returns an undefined, cryptographically secure hash of the given bytes. A
-    random value is added to the hash to make it difficult to guess the
-    original value. This random value is the same for all hashes generated by
-    this function during the same run of the program, but changes between runs.
+    random value is added to the hash to make it difficult to guess the original
+    value. This random value is the same for all hashes generated by this
+    function during the same run of the program, but changes between runs.
     """
 
     hasher = hashlib.sha256()
     hasher.update(_HASH_SALT)
     hasher.update(data)
     return hasher.digest()
 
@@ -43,16 +44,18 @@
     """
     Base class for assets - i.e. files that the client needs to be able to
     access. Assets can be hosted locally or remotely.
 
     Assets are "singletons", i.e. if you create two assets with the same input,
     they will be the same object:
 
-        >>> Asset.new(Path("foo.png")) is Asset.new(Path("foo.png"))
-        True
+    ```python
+    >>> Asset.new(Path("foo.png")) is Asset.new(Path("foo.png"))
+    True
+    ```
 
     To use an asset in a component, simply store it in the component's state. The
     asset will automatically register itself with the AppServer (if necessary)
     and serialize itself as a URL.
     """
 
     def __init__(
@@ -144,15 +147,15 @@
 
         if type(self) != type(other):
             return False
 
         return self._eq(other)
 
     @abc.abstractmethod
-    def _eq(self, other: Asset) -> bool:
+    def _eq(self, other: Self) -> bool:
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def url(self) -> URL:
         """
         Returns the URL at which the asset can be accessed. The URL may or may
```

### Comparing `rio_ui-0.5.9/src/rio/byte_serving.py` & `rio_ui-0.6/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/color.py` & `rio_ui-0.6/rio/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import colorsys
+import math
 from typing import *  # type: ignore
 
 from typing_extensions import TypeAlias
 from uniserde import Jsonable
 
 import rio
 
@@ -22,14 +23,15 @@
     A color, optionally with an opacity.
 
     The `Color` class does exactly what it says on the tin: It represents a
     single color. They're used throughout Rio to specify the color of text,
     fills, and more.
 
     `Color` supports a variety of color spaces:
+
     ```python
     # Color from RGB(A)
     Color.from_rgb(1.0, 0.0, 0.0, 1.0)
 
     # Color from hex
     Color.from_hex("#ff0000")
 
@@ -43,29 +45,44 @@
     # Color(1.0, 0.0, 0.0, 1.0)  # Raises a `RuntimeError`
     ```
 
     Regardless of how the color was created, all of the color's components will
     be accessible as attributes. For example, you can access `color.red`, even
     if the color was created from HSV values.
 
+
     ## Attributes
-        BLACK: A pure black color.
-        GREY: A medium grey color.
-        WHITE: A pure white color.
-        RED: A pure red color.
-        GREEN: A pure green color.
-        BLUE: A pure blue color.
-        CYAN: A pure cyan color.
-        MAGENTA: A pure magenta color.
-        YELLOW: A pure yellow color.
-        PINK: A pure pink color.
-        PURPLE: A pure purple color.
-        ORANGE: A pure orange color.
-        BROWN: A pure brown color.
-        TRANSPARENT: A fully transparent color.
+
+    `BLACK`: A pure black color.
+
+    `GREY`: A medium grey color.
+
+    `WHITE`: A pure white color.
+
+    `RED`: A pure red color.
+
+    `GREEN`: A pure green color.
+
+    `BLUE`: A pure blue color.
+
+    `CYAN`: A pure cyan color.
+
+    `MAGENTA`: A pure magenta color.
+
+    `YELLOW`: A pure yellow color.
+
+    `PINK`: A pure pink color.
+
+    `PURPLE`: A pure purple color.
+
+    `ORANGE`: A pure orange color.
+
+    `BROWN`: A pure brown color.
+
+    `TRANSPARENT`: A fully transparent color.
     """
 
     _red: float
     _green: float
     _blue: float
     _opacity: float
 
@@ -86,43 +103,49 @@
         Creates a color from RGB(A) values.
 
         Creates a color from RGB(A) values. All values must be between `0.0` and
         `1.0`, inclusive.
 
         If no `opacity` is given, the color will be fully opaque.
 
-        Args:
-            red: The red component of the color. `0.0` is no red, `1.0` is full
-                red.
-
-            green: The green component of the color. `0.0` is no green, `1.0`
-                is full green.
-
-            blue: The blue component of the color. `0.0` is no blue, `1.0` is
-                full blue.
-
-            opacity: The opacity of the color. `0.0` is fully transparent,
-                `1.0` is fully opaque.
-
-        Raises:
-            ValueError: If any of the values are outside of the range `0.0` to
-                `1.0`.
+        ## Parameters
+
+        red: The red component of the color. `0.0` is no red, `1.0` is full
+            red.
+
+        green: The green component of the color. `0.0` is no green, `1.0`
+            is full green.
+
+        blue: The blue component of the color. `0.0` is no blue, `1.0` is
+            full blue.
+
+        opacity: The opacity of the color. `0.0` is fully transparent,
+            `1.0` is fully opaque.
+
+        ## Raises
+
+        ValueError: If any of the values are outside of the range `0.0` to
+            `1.0`.
         """
 
         if red < 0.0 or red > 1.0:
             raise ValueError(f"`red` must be between 0.0 and 1.0, not {red}")
 
         if green < 0.0 or green > 1.0:
-            raise ValueError(f"`green` must be between 0.0 and 1.0, not {green}")
+            raise ValueError(
+                f"`green` must be between 0.0 and 1.0, not {green}"
+            )
 
         if blue < 0.0 or blue > 1.0:
             raise ValueError(f"`blue` must be between 0.0 and 1.0, not {blue}")
 
         if opacity < 0.0 or opacity > 1.0:
-            raise ValueError(f"`opacity` must be between 0.0 and 1.0, not {opacity}")
+            raise ValueError(
+                f"`opacity` must be between 0.0 and 1.0, not {opacity}"
+            )
 
         self = object.__new__(cls)
 
         self._red = red
         self._green = green
         self._blue = blue
         self._opacity = opacity
@@ -139,23 +162,26 @@
         - `rgb`
         - `rgba`
         - `rrggbb`
         - `rrggbbaa`
 
         All values may optionally be prefixed with a `#`.
 
-        Raises:
-            ValueError: If the string is not a valid hex color.
+        ## Raises
+
+        ValueError: If the string is not a valid hex color.
         """
         # Drop any leading `#` if present
         hex_color = hex_color.removeprefix("#")
 
         # Make sure the string is the correct length
         if len(hex_color) not in (3, 4, 6, 8):
-            raise ValueError("The hex string must be 3, 4, 6 or 8 characters long")
+            raise ValueError(
+                "The hex string must be 3, 4, 6 or 8 characters long"
+            )
 
         # Split the string into the individual components
         if len(hex_color) == 3:
             rh, gh, bh = hex_color
             ah = "f"
             max = 15
         elif len(hex_color) == 4:
@@ -194,30 +220,32 @@
         Create a color from HSV(A) values.
 
         Creates a color from HSV(A) values. All values must be between `0.0` and
         `1.0`, inclusive.
 
         If no `opacity` is given, the color will be fully opaque.
 
-        Args:
-            hue: The hue of the color. `0.0` is red, `0.33` is green, `0.66` is
-                blue, and `1.0` is red again.
-
-            saturation: The saturation of the color. `0.0` is no saturation,
-                `1.0` is full saturation.
-
-            value: The value of the color. `0.0` is black, `1.0` is full
-                brightness.
-
-            opacity: The opacity of the color. `0.0` is fully transparent,
-                `1.0` is fully opaque.
-
-        Raises:
-            ValueError: If any of the values are outside of the range `0.0` to
-                `1.0`.
+        ## Parameters
+
+        hue: The hue of the color. `0.0` is red, `0.33` is green, `0.66` is
+            blue, and `1.0` is red again.
+
+        saturation: The saturation of the color. `0.0` is no saturation,
+            `1.0` is full saturation.
+
+        value: The value of the color. `0.0` is black, `1.0` is full
+            brightness.
+
+        opacity: The opacity of the color. `0.0` is fully transparent,
+            `1.0` is fully opaque.
+
+        ## Raises
+
+        ValueError: If any of the values are outside of the range `0.0` to
+            `1.0`.
         """
         if hue < 0.0 or hue > 1.0:
             raise ValueError("`hue` must be between 0.0 and 1.0")
 
         if saturation < 0.0 or saturation > 1.0:
             raise ValueError("`saturation` must be between 0.0 and 1.0")
 
@@ -237,23 +265,25 @@
         Creates a greyscale color.
 
         Creates a grey color with the given intensity. A `grey` value of 0.0
         corresponds to black, and 1.0 to white.
 
         If no `opacity` is given, the color will be fully opaque.
 
-        Args:
-            grey: The intensity of the grey color. `0.0` is black, `1.0` is
-                white.
+        ## Parameters
 
-            opacity: The opacity of the color. `0.0` is fully transparent,
-                `1.0` is fully opaque.
+        grey: The intensity of the grey color. `0.0` is black, `1.0` is
+            white.
 
-        Raises:
-            ValueError: If `grey` is outside of the range `0.0` to `1.0`.
+        opacity: The opacity of the color. `0.0` is fully transparent,
+            `1.0` is fully opaque.
+
+        ## Raises
+
+        ValueError: If `grey` is outside of the range `0.0` to `1.0`.
         """
         if grey < 0.0 or grey > 1.0:
             raise ValueError("`grey` must be between 0.0 and 1.0")
 
         # Opacity will be checked by `from_rgb`
 
         return cls.from_rgb(grey, grey, grey, opacity)
@@ -355,16 +385,16 @@
         return colorsys.rgb_to_hsv(self._red, self._green, self._blue)
 
     @property
     def hue(self) -> float:
         """
         The hue of the color.
 
-        The hue of the color. `0.0` is red, `0.33` is green, `0.66` is blue,
-        and `1.0` is red again.
+        The hue of the color. `0.0` is red, `0.33` is green, `0.66` is blue, and
+        `1.0` is red again.
         """
         return self.hsv[0]
 
     @property
     def saturation(self) -> float:
         """
         The saturation of the color.
@@ -388,23 +418,17 @@
         """
         How bright the color appears to humans.
 
         Approximates how bright the color appears to humans. `0.0` is black,
         `1.0` is full brightness.
         """
 
-        # Account for the nonlinearity of human vision / gamma / sRGB
-        red_linear = self.red**2.2
-        green_linear = self.green**2.2
-        blue_linear = self.blue**2.2
-
-        # Calculate the perceived brightness
-        brightness = 0.299 * red_linear + 0.587 * green_linear + 0.114 * blue_linear
-
-        return brightness
+        return math.sqrt(
+            0.299 * self.red**2 + 0.587 * self.green**2 + 0.114 * self.blue**2
+        )
 
     @property
     def hex(self) -> str:
         """
         The color as a hex string.
 
         The color, formatted as 8 hex digits. The first two digits are the red
@@ -424,38 +448,39 @@
         green: float | None = None,
         blue: float | None = None,
         opacity: float | None = None,
     ) -> "Color":
         """
         Return a new `Color` instance with the given values replaced.
 
-        Return a new `Color` instance with the given values replaced. Any
-        values that are not given will be copied from this color.
+        Return a new `Color` instance with the given values replaced. Any values
+        that are not given will be copied from this color.
 
-        Args:
-            red: The red component of the new color.
+        ## Parameters
 
-            green: The green component of the new color.
+        red: The red component of the new color.
 
-            blue: The blue component of the new color.
+        green: The green component of the new color.
 
-            opacity: The opacity of the new color.
+        blue: The blue component of the new color.
+
+        opacity: The opacity of the new color.
         """
 
         return Color.from_rgb(
             red=self.red if red is None else red,
             green=self.green if green is None else green,
             blue=self.blue if blue is None else blue,
             opacity=self.opacity if opacity is None else opacity,
         )
 
     def _map_rgb(self, func: Callable[[float], float]) -> "Color":
         """
-        Apply a function to each of the RGB values of this color, and return
-        a new `Color` instance with the result. The opacity value is copied
+        Apply a function to each of the RGB values of this color, and return a
+        new `Color` instance with the result. The opacity value is copied
         unchanged.
         """
         return Color.from_rgb(
             func(self.red),
             func(self.green),
             func(self.blue),
             self.opacity,
@@ -467,18 +492,19 @@
 
         Return a new `Color` instance that is brighter than this one by the
         given amount. `0` means no change, `1` will turn the color into white.
         Values less than `0` will darken the color instead.
 
         How exactly the lightening/darkening happens isn't defined.
 
-        Args:
-            amount: How much to lighten the color. `0` means no change, `1`
-                will turn the color into white. Values less than `0` will
-                darken the color instead.
+        ## Parameters
+
+        amount: How much to lighten the color. `0` means no change, `1`
+            will turn the color into white. Values less than `0` will
+            darken the color instead.
         """
         # The amount may be negative. If that is the case, delegate to `darker`
         if amount <= 0:
             return self.darker(-amount)
 
         # HSV has an explicit value for brightness, so convert to HSV and bump
         # the value.
@@ -502,24 +528,25 @@
 
         return Color.from_hsv(hue, saturation, value_clip)
 
     def darker(self, amount: float) -> "Color":
         """
         Return a darker version of this color.
 
-        Return a new `Color` instance that is darker than this one by the
-        given amount. `0` means no change, `1` will turn the color into black.
-        Values less than `0` will brighten the color instead.
+        Return a new `Color` instance that is darker than this one by the given
+        amount. `0` means no change, `1` will turn the color into black. Values
+        less than `0` will brighten the color instead.
 
         How exactly the lightening/darkening happens isn't defined.
 
-        Args:
-            amount: How much to darken the color. `0` means no change, `1`
-                will turn the color into black. Values less than `0` will
-                brighten the color instead.
+        ## Parameters
+
+        amount: How much to darken the color. `0` means no change, `1`
+            will turn the color into black. Values less than `0` will brighten
+            the color instead.
         """
         # The value may be negative. If that is the case, delegate to `brighter`
         if amount <= 0:
             return self.brighter(-amount)
 
         return Color._map_rgb(self, lambda x: max(x - amount, 0))
 
@@ -527,17 +554,18 @@
         """
         Returns a desaturated version of this color.
 
         Return a copy of this color with the saturation reduced by the given
         amount. `0` means no change, `1` will turn the color into a shade of
         grey.
 
-        Args:
-            amount: How much to desaturate the color. `0` means no change, `1`
-                will turn the color into a shade of grey.
+        ## Parameters
+
+        amount: How much to desaturate the color. `0` means no change, `1`
+            will turn the color into a shade of grey.
         """
 
         if amount < 0.0 or amount > 1.0:
             raise ValueError("`amount` must be between 0.0 and 1.0")
 
         hue, saturation, brightness = self.hsv
         saturation = saturation * (1 - amount)
@@ -552,19 +580,20 @@
         given `other` color. `factor` controls how much of the other color is
         used. A value of `0` will return this color, a value of `1` will return
         the other color.
 
         Values outside of the range `0` to `1` are allowed and will lead to the
         color being extrapolated.
 
-        Args:
-            other: The other color to blend with.
+        ## Parameters
+
+        other: The other color to blend with.
 
-            factor: How much of the other color to use. `0` will return this
-                color, `1` will return the other color.
+        factor: How much of the other color to use. `0` will return this
+            color, `1` will return the other color.
         """
         one_minus_factor = 1 - factor
 
         return Color.from_rgb(
             red=self.red * one_minus_factor + other.red * factor,
             green=self.green * one_minus_factor + other.green * factor,
             blue=self.blue * one_minus_factor + other.blue * factor,
```

### Comparing `rio_ui-0.5.9/src/rio/common.py` & `rio_ui-0.6/rio/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import socket
 from dataclasses import dataclass
 from io import BytesIO, StringIO
 from pathlib import Path
 from typing import *  # type: ignore
 
 import imy.assets
-import imy.package_metadata
 from PIL.Image import Image
 from typing_extensions import Annotated
 from yarl import URL
 
 import rio
 
 __all__ = [
@@ -57,15 +56,15 @@
 
 ImageLike = Path | Image | URL | bytes
 
 
 ASSET_MANGER: imy.assets.AssetManager = imy.assets.AssetManager(
     xz_dir=RIO_ASSETS_DIR,
     cache_dir=USER_CACHE_DIR / "rio",
-    version=imy.package_metadata.get_package_version("rio-ui"),
+    version=rio.__version__,
 )
 
 
 # Precompiled regexes
 MARKDOWN_ESCAPE = re.compile(r"([\\`\*_\{\}\[\]\(\)#\+\-.!])")
 MARKDOWN_CODE_ESCAPE = re.compile(r"([\\`])")
 
@@ -98,21 +97,23 @@
     When asking the user to select a file, this class is used to represent the
     file. It contains metadata about the file, and can also be used to access
     the file's contents.
 
     Be careful when running your app as a webserver, since files will need to be
     uploaded by the user, which is a potentially very slow operation.
 
+
     ## Attributes
-        name: The name of the file, including the extension.
 
-        size_in_bytes: The size of the file, in bytes.
+    `name`: The name of the file, including the extension.
+
+    `size_in_bytes`: The size of the file, in bytes.
 
-        media_type: The MIMe type of the file, for example `text/plain` or
-            `image/png`.
+    `media_type`: The MIME type of the file, for example `text/plain` or
+        `image/png`.
     """
 
     name: str
     size_in_bytes: int
     media_type: str
     _contents: bytes
 
@@ -129,20 +130,22 @@
         """
         Asynchronously reads the entire file as text.
 
         Reads and returns the entire file as a `str` object. The file is decoded
         using the given `encoding`. If you don't know that the file is valid
         text, use `read_bytes` instead.
 
-        Args:
-            encoding: The encoding to use when decoding the file.
+        ## Parameters
+
+        encoding: The encoding to use when decoding the file.
+
+        ## Raises
 
-        Raises:
-            UnicodeDecodeError: The file could not be decoded using the given
-                `encoding`.
+        UnicodeDecodeError: The file could not be decoded using the given
+            `encoding`.
         """
         return self._contents.decode(encoding)
 
     @overload
     async def open(self, type: Literal["r"]) -> StringIO: ...
 
     @overload
@@ -153,19 +156,19 @@
         Asynchronously opens the file, as though it were a regular file on this
         device.
 
         Opens and returns the file as a file-like object. If 'r' is specified,
         the file is opened as text. If 'rb' is specified, the file is opened as
         bytes.
 
-        Args:
-            type: The mode to open the file in. 'r' for text, 'rb' for bytes.
+        Returns a file-like object containing the file's contents.
 
-        Returns:
-            A file-like object containing the file's contents.
+        ## Parameters
+
+        type: The mode to open the file in. 'r' for text, 'rb' for bytes.
         """
         # Bytes
         if type == "rb":
             return BytesIO(await self.read_bytes())
 
         # UTF
         if type == "r":
@@ -192,15 +195,17 @@
     # Verify the URLs have the same scheme and host
     if base.scheme != other.scheme:
         raise ValueError(
             f'URLs have different schemes: "{base.scheme}" and "{other.scheme}"'
         )
 
     if base.host != other.host:
-        raise ValueError(f'URLs have different hosts: "{base.host}" and "{other.host}"')
+        raise ValueError(
+            f'URLs have different hosts: "{base.host}" and "{other.host}"'
+        )
 
     # Get the path segments of the URLs
     base_parts = base.parts
     other_parts = other.parts
 
     # Strip empty segments
     if base_parts and base_parts[-1] == "":
@@ -233,16 +238,16 @@
     return re.sub(MARKDOWN_ESCAPE, r"\\\1", text)
 
 
 def escape_markdown_code(text: str) -> str:
     """
     Escape text such that it appears as-is inside a markdown code block.
 
-    Given any text, this function returns a string which, when rendered inside
-    a markdown code block, will look identical to the original text.
+    Given any text, this function returns a string which, when rendered inside a
+    markdown code block, will look identical to the original text.
     """
     # TODO: Find a proper function for this. The current one is a total hack.
     return MARKDOWN_CODE_ESCAPE.sub(r"\\\1", text)
 
 
 def choose_free_port(host: str) -> int:
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
@@ -284,15 +289,15 @@
 def _repr_build_function(build_function: Callable[[], rio.Component]) -> str:
     """
     Return a recognizable name for the provided function such as
     `Component.build`.
     """
 
     try:
-        self = build_function.__self__
+        self = build_function.__self__  # type: ignore
     except AttributeError:
         return build_function.__qualname__
 
     return f"{type(self).__name__}.{build_function.__name__}"
 
 
 def safe_build(build_function: Callable[[], rio.Component]) -> rio.Component:
@@ -307,30 +312,34 @@
     try:
         build_result = build_function()
 
     # The function has crashed. Return a placeholder instead
     except Exception as err:
         build_function_repr = _repr_build_function(build_function)
 
-        rio._logger.exception(f"An exception occurred in `{build_function_repr}`")
+        rio._logger.exception(
+            f"An exception occurred in `{build_function_repr}`"
+        )
 
-        from rio.components.build_failed import BuildFailed  # Screw circular imports
+        # Screw circular imports
+        from rio.components.build_failed import BuildFailed
 
         return BuildFailed(f"`{build_function_repr}` has crashed", repr(err))
 
     # Make sure the result meets expectations
     if not isinstance(build_result, rio.Component):  # type: ignore[unnecessary-isinstance]
         build_function_repr = _repr_build_function(build_function)
 
         rio._logger.error(
             f"The output of `build` methods must be instances of"
             f" `rio.Component`, but `{build_function_repr}` returned `{build_result!r}`"
         )
 
-        from rio.components.build_failed import BuildFailed  # Screw circular imports
+        # Screw circular imports
+        from rio.components.build_failed import BuildFailed
 
         return BuildFailed(
             f"`{build_function_repr}` has returned an invalid result",
             f"Build functions must return instances of `rio.Component`, but the result was {build_result!r}",
         )
 
     # All is well
```

### Comparing `rio_ui-0.5.9/src/rio/dataclass.py` & `rio_ui-0.6/rio/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     TypeVar,
     dataclass_transform,
     get_origin,
 )
 
 from . import inspection
 
-__all__ = ["RioDataclassMeta", "RioField", "internal_field", "class_local_fields"]
+__all__ = [
+    "RioDataclassMeta",
+    "RioField",
+    "internal_field",
+    "class_local_fields",
+]
 
 
 T = TypeVar("T")
 
 
 _FIELDS_BY_CLASS: dict[type, dict[str, RioField]] = {}
```

### Comparing `rio_ui-0.5.9/src/rio/errors.py` & `rio_ui-0.6/rio/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     """
     Raised when an error occurs related to assets.
 
     Signifies that some operation related to assets has failed. E.g. trying to
     access a nonexistent asset.
 
     ## Attributes
-        message: A human-readable error message.
+
+    `message`: A human-readable error message.
     """
 
     def __init__(self, message: str):
         super().__init__(message)
 
     @property
     def message(self) -> str:
@@ -22,16 +23,16 @@
 
 
 class NavigationFailed(Exception):
     """
     Raised when navigation to a page fails.
 
     This exception is raised when attempting to navigate to a page, but the
-    navigation fails for some reason. This could happen, for example, because
-    a page guard throws an exception.
+    navigation fails for some reason. This could happen, for example, because a
+    page guard throws an exception.
 
     Note that navigating to a nonexistent pages is not an error, as `PageViews`
     will simply display their fallback in that case. Thus this exception will
     not be raised in that case.
     """
 
     pass
```

### Comparing `rio_ui-0.5.9/src/rio/event.py` & `rio_ui-0.6/rio/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,40 +21,55 @@
 
 MethodWithNoParametersVar = TypeVar(
     "MethodWithNoParametersVar", bound=Callable[[Any], Any]
 )
 
 
 class EventTag(enum.Enum):
+    """
+    Event tags are internal markers used to keep track of which function needs
+    to be called when.
+
+    ## Metadata
+
+    public: False
+    """
+
     ON_POPULATE = enum.auto()
     ON_PAGE_CHANGE = enum.auto()
     ON_MOUNT = enum.auto()
     ON_UNMOUNT = enum.auto()
     PERIODIC = enum.auto()
 
 
-def _register_as_event_handler(function: Callable, tag: EventTag, args: Any) -> None:
+def _register_as_event_handler(
+    function: Callable, tag: EventTag, args: Any
+) -> None:
     all_events: dict[EventTag, list[Any]] = vars(function).setdefault(
         "_rio_events_", {}
     )
     events_like_this = all_events.setdefault(tag, [])
     events_like_this.append(args)
 
 
-def on_populate(handler: MethodWithNoParametersVar) -> MethodWithNoParametersVar:
+def on_populate(
+    handler: MethodWithNoParametersVar,
+) -> MethodWithNoParametersVar:
     """
     Triggered after the component has been created or has been reconciled. This
     allows you to asynchronously fetch any data which depends on the component's
     state.
     """
     _register_as_event_handler(handler, EventTag.ON_POPULATE, None)
     return handler
 
 
-def on_page_change(handler: MethodWithNoParametersVar) -> MethodWithNoParametersVar:
+def on_page_change(
+    handler: MethodWithNoParametersVar,
+) -> MethodWithNoParametersVar:
     """
     Triggered whenever the session changes pages.
     """
     _register_as_event_handler(handler, EventTag.ON_PAGE_CHANGE, None)
     return handler
 
 
@@ -80,29 +95,36 @@
     return handler
 
 
 def periodic(
     interval: float | timedelta,
 ) -> Decorator[MethodWithNoParametersVar]:
     """
-    TODO / unfinished / do not use
-
     This event is triggered repeatedly at a fixed time interval for as long as
     the component exists. The component does not have to be mounted for this
     event to trigger.
 
     The interval only starts counting after the previous handler has finished
     executing, so the handler will never run twice simultaneously, even if it
     takes longer than the interval to execute.
 
-    Args:
-        period: The number of seconds, or timedelta, between each trigger.
+
+    ## Parameters
+
+    `period`: The number of seconds, or timedelta, between each trigger.
+
+
+    ## Metadata
+
+    `experimental`: True
     """
     # Convert timedelta to float
     if isinstance(interval, timedelta):
         interval = interval.total_seconds()
 
-    def decorator(handler: MethodWithNoParametersVar) -> MethodWithNoParametersVar:
+    def decorator(
+        handler: MethodWithNoParametersVar,
+    ) -> MethodWithNoParametersVar:
         _register_as_event_handler(handler, EventTag.PERIODIC, interval)
         return handler
 
     return decorator
```

### Comparing `rio_ui-0.5.9/src/rio/fills.py` & `rio_ui-0.6/rio/fills.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 class Fill(SelfSerializing, ABC):
     """
     Base class for how shapes are filled.
 
     This is a base class for all fills. Fills determine how the inside of a
     shape is colored.
 
-    This class is abstract and cannot be instantiated directly. Instead, use
-    one of its subclasses.
+    This class is abstract and cannot be instantiated directly. Instead, use one
+    of its subclasses.
     """
 
     @staticmethod
     def _try_from(value: FillLike) -> "Fill":
         """
         Creates a fill instance from a `FillLike` value.
 
-        Raises:
-            TypeError: If the value is not a valid fill.
+        ## Raises
+
+        TypeError: If the value is not a valid fill.
         """
         if isinstance(value, Fill):
             return value
 
         if isinstance(value, Color):
             return SolidFill(value)
 
@@ -56,15 +57,16 @@
     """
     Fills a shape with a single color.
 
     `SolidFill` is the simplest of all fills. It fills the entire shape with a
     single, solid color.
 
     ## Attributes
-        color: The color to fill the shape with.
+
+    `color`: The color to fill the shape with.
     """
 
     color: Color
 
     def _serialize(self, sess: rio.Session) -> Jsonable:
         return {
             "type": "solid",
@@ -79,29 +81,31 @@
 
     `LinearGradientFill` fills the shape with a linear gradient. The gradient
     can have any number of stops, each with a color and a position. The gradient
     will smoothly transition between the colors at the given positions. The
     positions are given as are given as fractions, where 0 is the start of the
     gradient and 1 is the end.
 
+
     ## Attributes
-        stops: The different colors that comprise the gradient, along with where
-            they are positioned.
 
-            The stops are given as tuples. Each tuple contains a color and a
-            position. The position is a fraction, where 0 is the start of the
-            gradient and 1 is the end.
+    `stops`: The different colors that comprise the gradient, along with where
+        they are positioned.
+
+        The stops are given as tuples. Each tuple contains a color and a
+        position. The position is a fraction, where 0 is the start of the
+        gradient and 1 is the end.
 
-            The order of the stops has no effect.
+        The order of the stops has no effect.
 
-            There must be at least one stop.
+        There must be at least one stop.
 
-        angle_degrees: The angle of the gradient, in degrees. 0 degrees points
-            straight to the right, and the angle increases counterclockwise.
-            (This lines up with how angles are typically used mathematically.)
+    `angle_degrees`: The angle of the gradient, in degrees. 0 degrees points
+        straight to the right, and the angle increases counterclockwise.
+        (This lines up with how angles are typically used mathematically.)
     """
 
     stops: tuple[tuple[Color, float], ...]
     angle_degrees: float = 0.0
 
     def __init__(
         self,
@@ -127,17 +131,15 @@
         stop_strings = []
 
         for stop in self.stops:
             color = stop[0]
             position = stop[1]
             stop_strings.append(f"#{color.hex} {position * 100}%")
 
-        return (
-            f"linear-gradient({90 - self.angle_degrees}deg, {', '.join(stop_strings)})"
-        )
+        return f"linear-gradient({90 - self.angle_degrees}deg, {', '.join(stop_strings)})"
 
     def _serialize(self, sess: rio.Session) -> Jsonable:
         return {
             "type": "linearGradient",
             "stops": [(color.rgba, position) for color, position in self.stops],
             "angleDegrees": self.angle_degrees,
         }
@@ -162,23 +164,24 @@
     def __init__(
         self,
         image: ImageLike,
         *,
         fill_mode: Literal["fit", "stretch", "zoom"] = "fit",
     ):
         """
-        Args:
-            image: The image to fill the shape with. fill_mode: How the image should
-                be scaled to fit the shape.
-
-            fill_mode: How the image should be scaled to fit the shape. If `fit`,
-                the image is scaled to fit entirely inside the shape. If `stretch`,
-                the image is stretched to fill the shape exactly, possibly
-                distorting it in the process. If `zoom`, the image is scaled to fill
-                the shape entirely, possibly overflowing.
+        ## Parameters
+
+        `image`: The image to fill the shape with. fill_mode: How the image
+            should be scaled to fit the shape.
+
+        `fill_mode`: How the image should be scaled to fit the shape. If `fit`,
+            the image is scaled to fit entirely inside the shape. If `stretch`,
+            the image is stretched to fill the shape exactly, possibly
+            distorting it in the process. If `zoom`, the image is scaled to fill
+            the shape entirely, possibly overflowing.
         """
         self._image_asset = assets.Asset.from_image(image)
         self._fill_mode = fill_mode
 
     def _serialize(self, sess: rio.Session) -> Jsonable:
         return {
             "type": "image",
@@ -210,11 +213,13 @@
             return f"{css_url} top left / 100% 100%"
         elif self._fill_mode == "tile":
             return f"{css_url} left top repeat"
         elif self._fill_mode == "zoom":
             return f"{css_url} center/cover no-repeat"
         else:
             # Invalid fill mode
-            raise Exception(f"Invalid fill mode for image fill: {self._fill_mode}")
+            raise Exception(
+                f"Invalid fill mode for image fill: {self._fill_mode}"
+            )
 
 
 FillLike: TypeAlias = Fill | Color
```

### Comparing `rio_ui-0.5.9/src/rio/global_state.py` & `rio_ui-0.6/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/icon_registry.py` & `rio_ui-0.6/rio/icon_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,17 @@
         else:
             svg_path = icon_set_dir / variant / f"{icon_name}.svg"
 
         # Extract the icon set if necessary
         try:
             self._ensure_icon_set_is_extracted(icon_set)
         except KeyError:
-            raise AssetError(f"No icon set with the name {icon_set!r} is registered")
+            raise AssetError(
+                f"No icon set with the name {icon_set!r} is registered"
+            )
 
         if not svg_path.exists():
             raise AssetError(f"There is no icon named {icon_name!r}")
 
         return svg_path
 
     def get_icon_svg(self, icon_name: str) -> str:
@@ -191,15 +193,17 @@
 
         # Read the SVG file
         try:
             svg_string = svg_path.read_text()
         except FileNotFoundError:
             # Figure out which part of the name is the problem to show a
             # descriptive error message
-            icon_set, icon_name, variant = IconRegistry.parse_icon_name(icon_name)
+            icon_set, icon_name, variant = IconRegistry.parse_icon_name(
+                icon_name
+            )
 
             icon_set_dir = self._icon_set_extraction_dir(icon_set)
 
             if not icon_set_dir.exists():
                 raise AssetError(
                     f"Unknown icon set `{icon_set}`. Known icon sets are: `{'`, `'.join(self.icon_set_archives.keys())}`"
                 ) from None
@@ -261,16 +265,17 @@
         variant: str | None = None,
     ) -> Iterable[tuple[str, str | None]]:
         """
         Given the name of an icon set, list all icon names and variants in that
         set. If `variant` is given, only return icons with that variant.
         Otherwise, icons of all variants are returned.
 
-        Raises a `KeyError` if there is not icon set or variant with the given
-        name.
+        ## Raises
+
+        `KeyError`: if there is not icon set or variant with the given name.
         """
         # Find all available variants. This will also extract the icon set if
         # necessary.
         variants = dict(self._get_variant_directories(icon_set))
 
         # Apply the variant filter. Any `KeyError` is propagated.
         if variant is not None:
```

### Comparing `rio_ui-0.5.9/src/rio/inspection.py` & `rio_ui-0.6/rio/inspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,17 @@
 def get_child_component_containing_attribute_names(
     cls: type[rio.Component],
 ) -> Collection[str]:
     from . import serialization
 
     attr_names: list[str] = []
 
-    for attr_name, serializer in serialization.get_attribute_serializers(cls).items():
+    for attr_name, serializer in serialization.get_attribute_serializers(
+        cls
+    ).items():
         # : Component
         if serializer is serialization._serialize_child_component:
             attr_names.append(attr_name)
         elif isinstance(serializer, functools.partial):
             # : Component | None
             if (
                 serializer.func is serialization._serialize_optional
```

### Comparing `rio_ui-0.5.9/src/rio/maybes.py` & `rio_ui-0.6/rio/maybes.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     FLOAT_TYPES = (float, int)
     INT_TYPES = (int,)
     BOOL_TYPES = (bool,)
     STR_TYPES = (str,)
 
     # Is numpy available and loaded?
     if "numpy" in sys.modules:
-        import numpy
+        import numpy  # type: ignore
 
         NUMPY_ARRAY_TYPES = (numpy.ndarray,)
 
         numpy_floats = tuple(introspection.iter_subclasses(numpy.floating))
         numpy_ints = tuple(introspection.iter_subclasses(numpy.integer))
         numpy_bools = tuple(introspection.iter_subclasses(numpy.bool_))
         numpy_strings = tuple(introspection.iter_subclasses(numpy.str_))
@@ -101,15 +101,17 @@
         PLOTLY_GRAPH_TYPES = (plotly.graph_objects.Figure,)
 
     if "matplotlib" in sys.modules:
         import matplotlib.axes  # type: ignore
         import matplotlib.figure  # type: ignore
 
         MATPLOTLIB_AXES_TYPES = (matplotlib.axes.Axes,)
-        MATPLOTLIB_GRAPH_TYPES = (matplotlib.figure.Figure,) + MATPLOTLIB_AXES_TYPES
+        MATPLOTLIB_GRAPH_TYPES = (
+            matplotlib.figure.Figure,
+        ) + MATPLOTLIB_AXES_TYPES
 
     # Populate our mapping of type normalizers
     for canonical_type, weird_types in (
         (str, STR_TYPES),
         (bool, BOOL_TYPES),
         (int, INT_TYPES),
         (float, FLOAT_TYPES),
```

### Comparing `rio_ui-0.5.9/src/rio/routing.py` & `rio_ui-0.6/rio/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,80 +19,95 @@
     """
     A routable page in a Rio app.
 
     Rio apps can consist of many pages. You might have a welcome page, a
     settings page, a login, and so on. `Page` components contain all information
     needed to display those pages, as well as to navigate between them.
 
-    A minimal example:
+    This is not just specific to websites. Apps might, for example, have
+    a settings page, a profile page, a help page, and so on.
+
+    Pages are passed directly to the app during construction, like so:
 
     ```python
     import rio
 
     app = rio.App(
         build=lambda: rio.Column(
-            rio.Text("Welcome to my page!"), rio.PageView(
-                width="grow", height="grow",
-            ),
+            rio.Text("Welcome to my app!"),
+            rio.PageView(height="grow"),
         ),
         pages=[
             rio.Page(
-                "Home", "", build=lambda: rio.Text("This is the home page"),
+                name="Home",
+                page_url="",
+                build=lambda: rio.Text("This is the home page"),
             ),
             rio.Page(
-                "Subpage", "subpage", build=lambda: rio.Text("This is a subpage"),
+                name="Subpage",
+                page_url="subpage",
+                build=lambda: rio.Text("This is a subpage"),
             ),
         ],
     )
 
     app.run_in_browser()
     ```
 
     This will display "This is the home page" when navigating to the root URL,
     but "This is a subpage" when navigating to "/subpage". Note that on both
     pages the text "Welcome to my page!" is displayed above the page content.
     That's because it's not part of the `PageView`.
 
-    # TODO: Link to the routing/multipage how-to page
+    TODO: Link to the routing/multipage how-to page
 
     ## Attributes
-        page_url: The URL segment at which this page should be displayed. For
-            example, if this is "subpage", then the page will be displayed at
-            "https://yourapp.com/subpage". If this is "", then the page will be
-            displayed at the root URL.
-
-        build: A callback that is called when this page is displayed. It should
-            return a Rio component.
-
-        children: A list of child pages. These pages will be displayed when
-            navigating to a sub-URL of this page. For example, if this page's
-            `page_url` is "page1", and it has a child page with `page_url`
-            "page2", then the child page will be displayed at
-            "https://yourapp.com/page1/page2".
-
-        guard: A callback that is called before this page is displayed. It
-            can prevent users from accessing pages which they are not allowed to
-            see. For example, you may want to redirect users to your login page
-            if they are trying to access their profile page without being
-            logged in.
-
-            The callback should return `None` if the user is allowed to access
-            the page, or a string or `rio.URL` if the user should be redirected
-            to a different page.
+
+    `name`: A human-readable name for the page. While the page itself doesn't
+        use this value directly, it serves as important information for
+        debugging, as well as other components such as navigation bars.
+
+    `page_url`: The URL segment at which this page should be displayed. For
+        example, if this is "subpage", then the page will be displayed at
+        "https://yourapp.com/subpage". If this is "", then the page will be
+        displayed at the root URL.
+
+    `build`: A callback that is called when this page is displayed. It should
+        return a Rio component.
+
+    `icon`: The name of an icon to associate with the page. While the page
+        itself doesn't use this value directly, it serves as additional
+        information for other components such as navigation bars.
+
+    `children`: A list of child pages. These pages will be displayed when
+        navigating to a sub-URL of this page. For example, if this page's
+        `page_url` is "page1", and it has a child page with `page_url` "page2",
+        then the child page will be displayed at
+        "https://yourapp.com/page1/page2".
+
+    `guard`: A callback that is called before this page is displayed. It
+        can prevent users from accessing pages which they are not allowed to
+        see. For example, you may want to redirect users to your login page
+        if they are trying to access their profile page without being
+        logged in.
+
+        The callback should return `None` if the user is allowed to access
+        the page, or a string or `rio.URL` if the user should be redirected
+        to a different page.
     """
 
     name: str
     page_url: str
     build: Callable[[], rio.Component]
     _: KW_ONLY
     icon: str = "rio/logo:color"
-    show_in_navigation = True
     children: list[Page] = field(default_factory=list)
     guard: (
-        Callable[[rio.Session, tuple[rio.Page, ...]], None | rio.URL | str] | None
+        Callable[[rio.Session, tuple[rio.Page, ...]], None | rio.URL | str]
+        | None
     ) = None
 
     def __post_init__(self) -> None:
         # URLs are case insensitive. An easy way to enforce this, and also
         # prevent casing issues in the user code is to make sure the page's URL
         # fragment is lowercase.
         if self.page_url != self.page_url.lower():
@@ -163,15 +178,17 @@
         #   to a completely different site
         target_url_relative = common.make_url_relative(
             sess._base_url, target_url_absolute
         )
 
         # Find all pages which would by activated by this navigation
         active_page_instances = tuple(
-            _get_active_page_instances(sess.app.pages, target_url_relative.parts)
+            _get_active_page_instances(
+                sess.app.pages, target_url_relative.parts
+            )
         )
 
         # Check the guards for each activated page
         redirect = None
         for page in active_page_instances:
             if page.guard is None:
                 continue
@@ -196,15 +213,17 @@
 
         redirect = sess._active_page_url.join(redirect)
 
         assert redirect.is_absolute(), redirect
 
         # Detect infinite loops and break them
         if redirect in visited_redirects:
-            page_strings = [str(page_url) for page_url in past_redirects + [redirect]]
+            page_strings = [
+                str(page_url) for page_url in past_redirects + [redirect]
+            ]
             page_strings_list = "\n -> ".join(page_strings)
 
             message = f"Rejecting navigation to `{initial_target_url}` because page guards have created an infinite loop:\n\n    {page_strings_list}"
             logging.warning(message)
             raise NavigationFailed(message)
 
         # Remember that this page has been visited before
```

### Comparing `rio_ui-0.5.9/src/rio/serialization.py` & `rio_ui-0.6/rio/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,17 @@
 
     # If it's a fundamental component, serialize its state because JS needs it.
     # For non-fundamental components, there's no reason to send the state to
     # the frontend.
     if isinstance(component, fundamental_component.FundamentalComponent):
         sess = component.session
 
-        for name, serializer in get_attribute_serializers(type(component)).items():
+        for name, serializer in get_attribute_serializers(
+            type(component)
+        ).items():
             result[name] = serializer(sess, getattr(component, name))
 
         # Encode any internal additional state. Doing it this late allows the custom
         # serialization to overwrite automatically generated values.
         result["_type_"] = component._unique_id
         result.update(component._custom_serialize())
 
@@ -164,15 +166,17 @@
             continue
 
         serializers[attr_name] = serializer
 
     return serializers
 
 
-def _serialize_basic_json_value(sess: session.Session, value: Jsonable) -> Jsonable:
+def _serialize_basic_json_value(
+    sess: session.Session, value: Jsonable
+) -> Jsonable:
     return value
 
 
 def _serialize_self_serializing(
     sess: session.Session, obj: SelfSerializing
 ) -> Jsonable:
     return obj._serialize(sess)
@@ -192,15 +196,17 @@
 
 def _serialize_enum(
     sess: session.Session, value: object, as_type: Type[enum.Enum]
 ) -> Jsonable:
     return uniserde.as_json(value, as_type=as_type)
 
 
-def _serialize_colorset(sess: session.Session, colorset: color.ColorSet) -> Jsonable:
+def _serialize_colorset(
+    sess: session.Session, colorset: color.ColorSet
+) -> Jsonable:
     return sess.theme._serialize_colorset(colorset)
 
 
 def _serialize_optional(
     sess: session.Session, value: T | None, serializer: Serializer[T]
 ) -> Jsonable:
     if value is None:
@@ -209,17 +215,17 @@
     return serializer(sess, value)
 
 
 def _get_serializer_for_annotation(
     annotation: introspection.types.TypeAnnotation,
 ) -> Serializer | None:
     """
-    Which values are serialized for state depends on the annotated
-    datatypes. There is no point in sending fancy values over to the client
-    which it can't interpret.
+    Which values are serialized for state depends on the annotated datatypes.
+    There is no point in sending fancy values over to the client which it can't
+    interpret.
 
     This function looks at the annotation and returns a suitable serialization
     function, or `None` if this attribute shouldn't be serialized.
     """
     # Basic JSON values
     if annotation in (int, float, str, bool, None):
         return _serialize_basic_json_value
@@ -243,15 +249,17 @@
             return functools.partial(_serialize_enum, as_type=annotation)
 
     # Sequences of serializable values
     if origin is list:
         item_serializer = _get_serializer_for_annotation(args[0])
         if item_serializer is None:
             return None
-        return functools.partial(_serialize_list, item_serializer=item_serializer)
+        return functools.partial(
+            _serialize_list, item_serializer=item_serializer
+        )
 
     # Literal
     if origin is Literal:
         return _serialize_basic_json_value
 
     if origin in (Union, types.UnionType):
         # ColorSet
```

### Comparing `rio_ui-0.5.9/src/rio/session.py` & `rio_ui-0.6/rio/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     routing,
     serialization,
     text_style,
     theme,
     user_settings_module,
 )
 from .components import fundamental_component, root_components
-from .state_properties import StateBinding
+from .state_properties import AttributeBinding
 
 __all__ = ["Session"]
 
 
 T = typing.TypeVar("T")
 
 
@@ -242,30 +242,32 @@
         # These are split in two to avoid the dictionaries keeping the
         # components alive. Notice how both dictionaries are weak on the actual
         # component.
         #
         # Never access these directly. Instead, use helper functions
         # - `lookup_component`
         # - `lookup_component_data`
-        self._weak_components_by_id: weakref.WeakValueDictionary[int, rio.Component] = (
-            weakref.WeakValueDictionary()
-        )
+        self._weak_components_by_id: weakref.WeakValueDictionary[
+            int, rio.Component
+        ] = weakref.WeakValueDictionary()
 
         self._weak_component_data_by_component: weakref.WeakKeyDictionary[
             rio.Component, ComponentData
         ] = weakref.WeakKeyDictionary()
 
         # Keep track of all dirty components, once again, weakly.
         #
         # Components are dirty if any of their properties have changed since the
         # last time they were built. Newly created components are also considered
         # dirty.
         #
         # Use `register_dirty_component` to add a component to this set.
-        self._dirty_components: weakref.WeakSet[rio.Component] = weakref.WeakSet()
+        self._dirty_components: weakref.WeakSet[rio.Component] = (
+            weakref.WeakSet()
+        )
 
         # HTML components have source code which must be evaluated by the client
         # exactly once. Keep track of which components have already sent their
         # source code.
         self._initialized_html_components: set[str] = set(
             inspection.get_child_component_containing_attribute_names_for_builtin_components()
         )
@@ -284,98 +286,114 @@
         # This allows easy access to the app's assets. Users can simply write
         # `component.session.assets / "my_asset.png"`.
         self.assets = self._app_server.app.assets_dir
 
     @property
     def app(self) -> rio.App:
         """
-        Returns the app which this session belongs to.
+        The app which this session belongs to.
         """
         return self._app_server.app
 
     @property
     def running_in_window(self) -> bool:
         """
-        Returns `True` if the app is running in a local window, and `False` if
-        it is hosted as a website.
+        `True` if the app is running in a local window, and `False` if it is
+        hosted as a website.
         """
         return self._app_server.running_in_window
 
     @property
     def running_as_website(self) -> bool:
         """
-        Returns `True` if the app is running as a website, and `False` if it is
-        running in a local window.
+        `True` if the app is running as a website, and `False` if it is running
+        in a local window.
         """
         return self._app_server.running_in_window
 
     @property
     def base_url(self) -> rio.URL:
         """
         Returns the base URL of the app.
 
         Only available when running as a website.
         """
+        # TODO: Example
+
         if self._app_server.running_in_window:
             raise RuntimeError(
                 "Cannot get the base URL of an app that is running in a window"
             )
 
         return self._base_url
 
     @property
     def active_page_url(self) -> rio.URL:
         """
         Returns the current page as a tuple of strings.
 
-        This property is read-only. To change the page, use `Session.navigate_to`.
+        This property is read-only. To change the page, use
+        `Session.navigate_to`.
         """
         return self._active_page_url
 
     @property
     def active_page_instances(self) -> tuple[rio.Page, ...]:
         """
         Returns the current page as a tuple of `Page` instances.
 
-        This property is read-only. To change the page, use `Session.navigate_to`.
+        This property is read-only. To change the page, use
+        `Session.navigate_to`.
         """
         return self._active_page_instances
 
     @property
     def _is_active(self) -> bool:
         """
         Returns whether there is an active websocket connection to a client
         """
         return self._websocket is not None
 
     def attach(self, value: Any) -> None:
         """
         Attaches the given value to the `Session`. It can be retrieved later
         using `session[...]`.
+
+        ## Parameters
+
+        `value`: The value to attach.
         """
         self._attachments.add(value)
 
-    def __getitem__(self, typ: type[T]) -> T:
+    def __getitem__(self, typ: type[T], /) -> T:
         """
         Retrieves an attachment from this session. To attach values to the
         session, use `Session.attach`.
+
+        ## Parameters
+
+        `typ`: The class of the value you want to retrieve.
+
+        ## Raises
+
+        `KeyError`: If no attachment of this type is attached to the session.
         """
         return self._attachments[typ]
 
-    def __delete__(self, typ: type) -> None:
+    def __delete__(self, typ: type, /) -> None:
         """
         Removes an attachment from this session.
 
         ## Raises
 
         `KeyError`: If no attachment of this type is attached to the session.
         """
         self._attachments.remove(typ)
 
-    def detach(self, typ: type) -> None:
+    def detach(self, typ: type, /) -> None:
         """
         Removes an attachment from this session.
 
         ## Raises
 
         `KeyError`: If no attachment of this type is attached to the session.
         """
@@ -446,19 +464,27 @@
     @overload
     async def _call_event_handler(
         self, handler: common.EventHandler[[]], *, refresh: bool
     ) -> None: ...
 
     @overload
     async def _call_event_handler(
-        self, handler: common.EventHandler[[T]], event_data: T, /, *, refresh: bool
+        self,
+        handler: common.EventHandler[[T]],
+        event_data: T,
+        /,
+        *,
+        refresh: bool,
     ) -> None: ...
 
     async def _call_event_handler(
-        self, handler: common.EventHandler[...], *event_data: object, refresh: bool
+        self,
+        handler: common.EventHandler[...],
+        *event_data: object,
+        refresh: bool,
     ) -> None:
         """
         Calls an event handler function. If it's async, it's awaited.
 
         Does *not* refresh the session. It's the caller's responsibility to do
         that.
         """
@@ -548,19 +574,20 @@
         """
         Creates an `asyncio.Task` that is cancelled when the session is closed.
 
         This is identical to `asyncio.create_task`, except that any tasks are
         automatically cancelled when the session is closed. This makes sure that
         old tasks don't keep piling up long after they are no longer needed.
 
-        Args:
-            coro: The coroutine to run.
+        ## Parameters
 
-            name: An optional name for the task. Assigning descriptive names can
-                be helpful when debugging.
+        `coro`: The coroutine to run.
+
+        `name`: An optional name for the task. Assigning descriptive names can
+            be helpful when debugging.
         """
         task = asyncio.create_task(coro, name=name)
 
         self._running_tasks.add(task)
         task.add_done_callback(self._running_tasks.remove)
 
         return task
@@ -576,22 +603,22 @@
 
         Switches the app to display the given page URL. If `replace` is `True`,
         the browser's most recent history entry is replaced with the new page.
         This means that the user can't go back to the previous page using the
         browser's back button. If `False`, a new history entry is created,
         allowing the user to go back to the previous page.
 
-        Args:
-            target_url: The URL of the page to navigate to.
+        ## Parameters
 
-            replace: If `True`, the browser's most recent history entry is
-                replaced with the new page. If `False`, a new history entry is
-                created, allowing the user to go back to the previous page.
-        """
+        `target_url`: The URL of the page to navigate to.
 
+        `replace`: If `True`, the browser's most recent history entry is
+            replaced with the new page. If `False`, a new history entry is
+            created, allowing the user to go back to the previous page.
+        """
         # Normalize the target URL. Having it always be lowercase helps the user
         # avoid navigation problems because of casing issues.
         if isinstance(target_url, rio.URL):
             target_url = str(target_url)
 
         target_url = rio.URL(target_url.lower())
 
@@ -603,15 +630,17 @@
             common.make_url_relative(
                 self._base_url,
                 target_url_absolute,
             )
 
         # This is an external URL. Navigate to it
         except ValueError:
-            logging.debug(f"Navigating to external site `{target_url_absolute}`")
+            logging.debug(
+                f"Navigating to external site `{target_url_absolute}`"
+            )
 
             async def history_worker() -> None:
                 await self._evaluate_javascript(
                     f"""
 window.location.href = {json.dumps(str(target_url))};
 """,
                 )
@@ -640,50 +669,55 @@
         self.create_task(self._refresh())
 
         # Update the browser's history
         async def history_worker() -> None:
             method = "replaceState" if replace else "pushState"
             await self._evaluate_javascript(
                 f"""
-window.history.{method}(null, "", {json.dumps(str(active_page_url))})
+// Scroll to the top. This has to happen before we change the URL, because if
+// the URL has a #fragment then we will scroll to the corresponding ScrollTarget
 getRootScroller().element.scrollTo({{ top: 0, behavior: "smooth" }});
+
+window.history.{method}(null, "", {json.dumps(str(active_page_url))})
 """,
             )
 
         self.create_task(
             history_worker(),
             name="Update browser history due to call to `navigate_to`",
         )
 
         # Trigger the `on_page_change` event
         async def event_worker() -> None:
             for component, callbacks in self._page_change_callbacks.items():
                 for callback in callbacks:
                     self.create_task(
-                        self._call_event_handler(callback, component, refresh=True),
+                        self._call_event_handler(
+                            callback, component, refresh=True
+                        ),
                         name="`on_page_change` event handler",
                     )
 
         self.create_task(event_worker())
 
     def _register_dirty_component(
         self,
         component: rio.Component,
         *,
         include_children_recursively: bool,
     ) -> None:
         """
-        Add the component to the set of dirty components. The component is only held
-        weakly by the session.
+        Add the component to the set of dirty components. The component is only
+        held weakly by the session.
 
         If `include_children_recursively` is true, all children of the component
         are also added.
 
-        The children of non-fundamental components are not added, since they will
-        be added after the parent is built anyway.
+        The children of non-fundamental components are not added, since they
+        will be added after the parent is built anyway.
         """
         self._dirty_components.add(component)
 
         if not include_children_recursively or not isinstance(
             component, fundamental_component.FundamentalComponent
         ):
             return
@@ -709,15 +743,17 @@
         The session keeps track of components which are no longer referenced in
         its component tree. Those components are NOT included in the function's
         result.
         """
 
         # Keep track of all components which are visited. Only they will be sent to
         # the client.
-        visited_components: collections.Counter[rio.Component] = collections.Counter()
+        visited_components: collections.Counter[rio.Component] = (
+            collections.Counter()
+        )
 
         # Keep track of of previous child components
         old_children_in_build_boundary_for_visited_children = {}
 
         # Build all dirty components
         while self._dirty_components:
             component = self._dirty_components.pop()
@@ -732,15 +768,17 @@
                     f"The component `{component}` has been rebuilt"
                     f" {build_count} times during a single refresh. This is"
                     f" likely because one of your components' `build` methods"
                     f" is modifying the component's state"
                 )
 
             # Fundamental components require no further treatment
-            if isinstance(component, fundamental_component.FundamentalComponent):
+            if isinstance(
+                component, fundamental_component.FundamentalComponent
+            ):
                 continue
 
             # Trigger the `on_populate` event, if it hasn't already. Since the
             # whole point of this event is to fetch data and modify the
             # component's state, wait for it to finish if it is synchronous.
             if not component._on_populate_triggered_:
                 component._on_populate_triggered_ = True
@@ -767,25 +805,29 @@
                     f"The `build()` method of the component `{component}`"
                     f" changed the component's state. Assignments to properties"
                     f" of the component aren't allowed in the `build()` method."
                 )
 
             # Has this component been built before?
             try:
-                component_data = self._weak_component_data_by_component[component]
+                component_data = self._weak_component_data_by_component[
+                    component
+                ]
 
             # No, this is the first time
             except KeyError:
                 # Create the component data and cache it
                 component_data = ComponentData(
                     build_result,
                     set(),  # Set of all children - filled in below
                     0,
                 )
-                self._weak_component_data_by_component[component] = component_data
+                self._weak_component_data_by_component[component] = (
+                    component_data
+                )
 
             # Yes, rescue state. This will:
             #
             # - Look for components in the build output which correspond to
             #   components in the previous build output, and transfers state
             #   from the new to the old component ("reconciliation")
             #
@@ -840,15 +882,17 @@
         }
 
         all_children_old = set()
         all_children_new = set()
 
         for component in visited_and_live_components:
             # Fundamental components aren't tracked, since they are never built
-            if isinstance(component, fundamental_component.FundamentalComponent):
+            if isinstance(
+                component, fundamental_component.FundamentalComponent
+            ):
                 continue
 
             all_children_old.update(
                 old_children_in_build_boundary_for_visited_children[component]
             )
             all_children_new.update(
                 self._weak_component_data_by_component[
@@ -898,19 +942,23 @@
 
                 # Avoid sending empty messages
                 if not visited_components:
                     return
 
                 # Serialize all components which have been visited
                 delta_states: dict[int, JsonDoc] = {
-                    component._id: serialization.serialize_and_host_component(component)
+                    component._id: serialization.serialize_and_host_component(
+                        component
+                    )
                     for component in visited_components
                 }
 
-                await self._update_component_states(visited_components, delta_states)
+                await self._update_component_states(
+                    visited_components, delta_states
+                )
 
                 # Trigger the `on_unmount` event
                 #
                 # Notes:
                 # - All events are triggered only after the client has been
                 #   notified of the changes. This way, if the event handlers
                 #   trigger another client message themselves, any referenced
@@ -938,44 +986,53 @@
                         self._call_event_handler_sync(handler, component)
 
                 # If there were any synchronous `on_mount` or `on_unmount`
                 # handlers, we must immediately refresh again. So we'll simply
                 # loop until there are no more dirty components.
 
     async def _update_component_states(
-        self, visited_components: set[rio.Component], delta_states: dict[int, JsonDoc]
+        self,
+        visited_components: set[rio.Component],
+        delta_states: dict[int, JsonDoc],
     ) -> None:
         # Initialize all new FundamentalComponents
         for component in visited_components:
             if (
-                not isinstance(component, fundamental_component.FundamentalComponent)
+                not isinstance(
+                    component, fundamental_component.FundamentalComponent
+                )
                 or component._unique_id in self._initialized_html_components
             ):
                 continue
 
             await component._initialize_on_client(self)
             self._initialized_html_components.add(type(component)._unique_id)
 
         # Check whether the root component needs replacing. Take care to never
         # send the high level root component. JS only cares about the
         # fundamental one.
         if self._root_component in visited_components:
             del delta_states[self._root_component._id]
 
-            root_build = self._weak_component_data_by_component[self._root_component]
+            root_build = self._weak_component_data_by_component[
+                self._root_component
+            ]
             fundamental_root_component = root_build.build_result
             assert isinstance(
-                fundamental_root_component, fundamental_component.FundamentalComponent
+                fundamental_root_component,
+                fundamental_component.FundamentalComponent,
             ), fundamental_root_component
             root_component_id = fundamental_root_component._id
         else:
             root_component_id = None
 
         # Send the new state to the client
-        await self._remote_update_component_states(delta_states, root_component_id)
+        await self._remote_update_component_states(
+            delta_states, root_component_id
+        )
 
     async def _send_all_components_on_reconnect(self) -> None:
         self._initialized_html_components.clear()
 
         # For why this lock is here see its creation in `__init__`
         async with self._refresh_lock:
             visited_components: set[rio.Component] = set()
@@ -983,15 +1040,17 @@
 
             for component in self._root_component._iter_component_tree():
                 visited_components.add(component)
                 delta_states[component._id] = (
                     serialization.serialize_and_host_component(component)
                 )
 
-            await self._update_component_states(visited_components, delta_states)
+            await self._update_component_states(
+                visited_components, delta_states
+            )
 
     def _reconcile_tree(
         self,
         old_build_data: ComponentData,
         new_build: rio.Component,
     ) -> None:
         # Find all pairs of components which should be reconciled
@@ -1007,15 +1066,18 @@
         # -> Collect them into a set first.
         reconciled_components_new_to_old: dict[rio.Component, rio.Component] = {
             new_component: old_component
             for old_component, new_component in matched_pairs
         }
 
         # Reconcile all matched pairs
-        for new_component, old_component in reconciled_components_new_to_old.items():
+        for (
+            new_component,
+            old_component,
+        ) in reconciled_components_new_to_old.items():
             assert (
                 new_component is not old_component
             ), f"Attempted to reconcile {new_component!r} with itself!?"
 
             self._reconcile_component(
                 old_component,
                 new_component,
@@ -1027,44 +1089,52 @@
             # the component tree. It is thus safe to remove from the set of dirty
             # components to prevent a pointless rebuild.
             self._dirty_components.discard(new_component)
 
         # Update the component data. If the root component was not reconciled,
         # the new component is the new build result.
         try:
-            reconciled_build_result = reconciled_components_new_to_old[new_build]
+            reconciled_build_result = reconciled_components_new_to_old[
+                new_build
+            ]
         except KeyError:
             reconciled_build_result = new_build
             old_build_data.build_result = new_build
 
         # Replace any references to new reconciled components to old ones instead
         def remap_components(parent: rio.Component) -> None:
             parent_vars = vars(parent)
 
-            for attr_name in inspection.get_child_component_containing_attribute_names(
+            for (
+                attr_name
+            ) in inspection.get_child_component_containing_attribute_names(
                 type(parent)
             ):
                 attr_value = parent_vars[attr_name]
 
                 # Just a component
                 if isinstance(attr_value, rio.Component):
                     try:
-                        attr_value = reconciled_components_new_to_old[attr_value]
+                        attr_value = reconciled_components_new_to_old[
+                            attr_value
+                        ]
                     except KeyError:
                         # Make sure that any components which are now in the
                         # tree have their builder properly set.
                         #
                         # TODO: Why is this needed exactly? IT IS - I have
                         # encountered apps which only work with this code - but,
                         # a comment why this is the case would've been nice.
                         if isinstance(
                             parent, fundamental_component.FundamentalComponent
                         ):
                             attr_value._weak_builder_ = parent._weak_builder_
-                            attr_value._build_generation_ = parent._build_generation_
+                            attr_value._build_generation_ = (
+                                parent._build_generation_
+                            )
                     else:
                         parent_vars[attr_name] = attr_value
 
                     remap_components(attr_value)
 
                 # List / Collection
                 elif isinstance(attr_value, list):
@@ -1079,18 +1149,21 @@
                                 # the tree have their builder properly set.
                                 #
                                 # TODO: Why is this needed exactly? IT IS - I
                                 # have encountered apps which only work with
                                 # this code - but, a comment why this is the
                                 # case would've been nice.
                                 if isinstance(
-                                    parent, fundamental_component.FundamentalComponent
+                                    parent,
+                                    fundamental_component.FundamentalComponent,
                                 ):
                                     item._weak_builder_ = parent._weak_builder_
-                                    item._build_generation_ = parent._build_generation_
+                                    item._build_generation_ = (
+                                        parent._build_generation_
+                                    )
                             else:
                                 attr_value[ii] = item
 
                             remap_components(item)
 
         remap_components(reconciled_build_result)
 
@@ -1128,19 +1201,19 @@
 
         overridden_property_names = (
             old_component._properties_set_by_creator_
             - old_component._properties_assigned_after_creation_
         ) | new_component._properties_set_by_creator_
 
         for prop_name in overridden_property_names:
-            # Take care to keep state bindings up to date
+            # Take care to keep attribute bindings up to date
             old_value = old_component_dict[prop_name]
             new_value = new_component_dict[prop_name]
-            old_is_binding = isinstance(old_value, StateBinding)
-            new_is_binding = isinstance(new_value, StateBinding)
+            old_is_binding = isinstance(old_value, AttributeBinding)
+            new_is_binding = isinstance(new_value, AttributeBinding)
 
             # If the old value was a binding, and the new one isn't, split the
             # tree of bindings. All children are now roots.
             if old_is_binding and not new_is_binding:
                 binding_value = old_value.get_value()
                 old_value.owning_component_weak = lambda: None
 
@@ -1148,15 +1221,17 @@
                     child_binding.is_root = True
                     child_binding.parent = None
                     child_binding.value = binding_value
 
             # If both values are bindings transfer the children to the new
             # binding
             elif old_is_binding and new_is_binding:
-                new_value.owning_component_weak = old_value.owning_component_weak
+                new_value.owning_component_weak = (
+                    old_value.owning_component_weak
+                )
                 new_value.children = old_value.children
 
                 for child in old_value.children:
                     child.parent = new_value
 
                 # Save the binding's value in case this is the root binding
                 new_value.value = old_value.value
@@ -1172,15 +1247,17 @@
             # Components are a special case. Component attributes are dirty iff the
             # component isn't reconciled, i.e. it is a new component
             if isinstance(new, rio.Component):
                 if old is new:
                     return True
 
                 try:
-                    new_before_reconciliation = reconciled_components_new_to_old[new]
+                    new_before_reconciliation = (
+                        reconciled_components_new_to_old[new]
+                    )
                 except KeyError:
                     return False
                 else:
                     return old is new_before_reconciliation
 
             if isinstance(new, list):
                 if not isinstance(old, list):
@@ -1270,61 +1347,71 @@
             components_by_key[component.key] = component
 
         def key_scan(
             components_by_key: dict[str, rio.Component],
             component: rio.Component,
             include_self: bool = True,
         ) -> None:
-            for (
-                child
-            ) in component._iter_direct_and_indirect_child_containing_attributes(
-                include_self=include_self,
-                recurse_into_high_level_components=True,
+            for child in (
+                component._iter_direct_and_indirect_child_containing_attributes(
+                    include_self=include_self,
+                    recurse_into_high_level_components=True,
+                )
             ):
                 register_component_by_key(components_by_key, child)
 
         def chain_to_children(
             old_component: rio.Component,
             new_component: rio.Component,
         ) -> None:
             def _extract_components(attr: object) -> list[rio.Component]:
                 if isinstance(attr, rio.Component):
                     return [attr]
 
                 if isinstance(attr, list):
                     attr = cast(list[object], attr)
 
-                    return [item for item in attr if isinstance(item, rio.Component)]
+                    return [
+                        item for item in attr if isinstance(item, rio.Component)
+                    ]
 
                 return []
 
             # Iterate over the children, but make sure to preserve the topology.
             # Can't just use `iter_direct_children` here, since that would
             # discard topological information.
-            for attr_name in inspection.get_child_component_containing_attribute_names(
+            for (
+                attr_name
+            ) in inspection.get_child_component_containing_attribute_names(
                 type(new_component)
             ):
                 old_value = getattr(old_component, attr_name, None)
                 new_value = getattr(new_component, attr_name, None)
 
                 old_components = _extract_components(old_value)
                 new_components = _extract_components(new_value)
 
                 # Chain to the children
                 common = min(len(old_components), len(new_components))
                 for old_child, new_child in zip(old_components, new_components):
                     worker(old_child, new_child)
 
                 for old_child in old_components[common:]:
-                    key_scan(old_components_by_key, old_child, include_self=True)
+                    key_scan(
+                        old_components_by_key, old_child, include_self=True
+                    )
 
                 for new_child in new_components[common:]:
-                    key_scan(new_components_by_key, new_child, include_self=True)
+                    key_scan(
+                        new_components_by_key, new_child, include_self=True
+                    )
 
-        def worker(old_component: rio.Component, new_component: rio.Component) -> None:
+        def worker(
+            old_component: rio.Component, new_component: rio.Component
+        ) -> None:
             # If a component was passed to a container, it is possible that the
             # container returns the same instance of that component in multiple
             # builds. This would reconcile a component with itself, which ends
             # in disaster.
             if old_component is new_component:
                 return
 
@@ -1334,31 +1421,37 @@
 
             # If the components' types or keys don't match, stop looking for
             # topological matches. Just keep track of the children's keys.
             if (
                 type(old_component) is not type(new_component)
                 or old_component.key != new_component.key
             ):
-                key_scan(old_components_by_key, old_component, include_self=False)
-                key_scan(new_components_by_key, new_component, include_self=False)
+                key_scan(
+                    old_components_by_key, old_component, include_self=False
+                )
+                key_scan(
+                    new_components_by_key, new_component, include_self=False
+                )
                 return
 
             # Key matches are handled elsewhere, so if the key is not `None`, do
             # nothing. We'd just end up doing the same work twice.
             if old_component.key is not None:
                 return
 
             matches_by_topology.append((old_component, new_component))
             chain_to_children(old_component, new_component)
 
         worker(old_build, new_build)
 
         # Find matches by key and reconcile their children. This can produce new
         # key matches, so we do it in a loop.
-        new_key_matches = old_components_by_key.keys() & new_components_by_key.keys()
+        new_key_matches = (
+            old_components_by_key.keys() & new_components_by_key.keys()
+        )
         all_key_matches = new_key_matches
 
         while new_key_matches:
             for key in new_key_matches:
                 old_component = old_components_by_key[key]
                 new_component = new_components_by_key[key]
 
@@ -1446,15 +1539,17 @@
         # Keys in this dict can be attributes of the "root" section or names of
         # sections. To prevent name clashes, section names are prefixed with
         # "section:".
         settings_json: dict[str, object]
 
         if self.running_in_window:
             try:
-                async with aiofiles.open(self._get_settings_file_path()) as file:
+                async with aiofiles.open(
+                    self._get_settings_file_path()
+                ) as file:
                     settings_text = await file.read()
 
                 settings_json = json.loads(settings_text)
             except (IOError, json.JSONDecodeError):
                 settings_json = {}
                 settings_text = "{}"
 
@@ -1466,22 +1561,26 @@
             settings_json = {}
 
             for key, value in settings_sent_by_client.items():
                 # Find the section name
                 section_name, _, key = key.rpartition(":")
 
                 if section_name:
-                    section = settings_json.setdefault("section:" + section_name, {})
+                    section = settings_json.setdefault(
+                        "section:" + section_name, {}
+                    )
                     section[key] = value  # type: ignore
                 else:
                     settings_json[key] = value
 
         # Instantiate and attach the settings
         for default_settings in self._app_server.app.default_attachments:
-            if not isinstance(default_settings, user_settings_module.UserSettings):
+            if not isinstance(
+                default_settings, user_settings_module.UserSettings
+            ):
                 continue
 
             settings = type(default_settings)._from_json(
                 settings_json,
                 default_settings,
             )
 
@@ -1530,15 +1629,17 @@
                     self._settings_json.setdefault(
                         "section:" + settings.section_name, {}
                     ),
                 )
             else:
                 section = self._settings_json
 
-            annotations = inspection.get_resolved_type_annotations(type(settings))
+            annotations = inspection.get_resolved_type_annotations(
+                type(settings)
+            )
 
             for attr_name in dirty_attributes:
                 section[attr_name] = uniserde.as_json(
                     getattr(settings, attr_name),
                     as_type=annotations[attr_name],
                 )
 
@@ -1559,31 +1660,37 @@
         settings_to_save: Iterable[
             tuple[user_settings_module.UserSettings, Iterable[str]]
         ],
     ) -> None:
         delta_settings: dict[str, Any] = {}
 
         for settings, dirty_attributes in settings_to_save:
-            prefix = f"{settings.section_name}:" if settings.section_name else ""
+            prefix = (
+                f"{settings.section_name}:" if settings.section_name else ""
+            )
 
-            annotations = inspection.get_resolved_type_annotations(type(settings))
+            annotations = inspection.get_resolved_type_annotations(
+                type(settings)
+            )
 
             # Get the dirty attributes
             for attr_name in dirty_attributes:
                 delta_settings[f"{prefix}{attr_name}"] = uniserde.as_json(
                     getattr(settings, attr_name),
                     as_type=annotations[attr_name],
                 )
 
         # Sync them with the client
         await self._set_user_settings(delta_settings)
 
     def _save_settings_soon(self) -> None:
         if self._settings_save_task is None:
-            self._settings_save_task = self.create_task(self.__wait_and_save_settings())
+            self._settings_save_task = self.create_task(
+                self.__wait_and_save_settings()
+            )
 
     async def __wait_and_save_settings(self) -> None:
         # Wait some time to see if more attributes are marked as dirty
         await asyncio.sleep(0.5)
 
         # If we've recently saved, wait a bit longer. Some apps change
         # the settings very often, and we don't need to save immediately every
@@ -1597,17 +1704,32 @@
             await self._save_settings_now()
 
         # Housekeeping
         finally:
             self._settings_save_task = None
 
     async def set_title(self, title: str) -> None:
+        """
+        Changes the window title of this session.
+
+        ## Parameters
+
+        `title`: The new window title.
+        """
         if self.running_in_window:
+            import webview.util
+
             window = await self._get_webview_window()
-            window.set_title(title)
+
+            while True:
+                try:
+                    window.set_title(title)
+                    break
+                except webview.util.WebViewException:
+                    await asyncio.sleep(0.2)
         else:
             await self._remote_set_title(title)
 
     @overload
     async def file_chooser(
         self,
         *,
@@ -1634,34 +1756,37 @@
 
         This function opens a file chooser dialog, allowing the user to select a
         file. The selected file is returned, allowing you to access its
         contents.
 
         See also `save_file`, if you want to save a file instead of opening one.
 
-        Args:
-            file_extensions: A list of file extensions which the user is allowed
-                to select. Defaults to `None`, which means that the user may
-                select any file.
+        ## Parameters
+
+        file_extensions: A list of file extensions which the user is allowed
+            to select. Defaults to `None`, which means that the user may
+            select any file.
 
-            multiple: Whether the user should pick a single file, or multiple.
+        multiple: Whether the user should pick a single file, or multiple.
+
+        ## Raises
 
-        Raises:
-            NoFileSelectedError: If the user did not select a file.
+        NoFileSelectedError: If the user did not select a file.
         """
         # Create a secret id and register the file upload with the app server
         upload_id = secrets.token_urlsafe()
         future = asyncio.Future[list[common.FileInfo]]()
 
         self._app_server._pending_file_uploads[upload_id] = future
 
         # Allow the user to specify both `jpg` and `.jpg`
         if file_extensions is not None:
             file_extensions = [
-                ext if ext.startswith(".") else f".{ext}" for ext in file_extensions
+                ext if ext.startswith(".") else f".{ext}"
+                for ext in file_extensions
             ]
 
         # Tell the frontend to upload a file
         await self._request_file_upload(
             upload_url=f"/rio/upload/{upload_id}",
             file_extensions=file_extensions,
             multiple=multiple,
@@ -1700,26 +1825,27 @@
 
         This function allows you to save a file to the user's device. The user
         will be prompted to select a location to save the file to.
 
         See also `file_chooser` if you want to open a file instead of saving
         one.
 
-        Args:
-            file_contents: The contents of the file to save. This can be a
-                string, bytes, or a path to a file on the server.
+        ## Parameters
 
-            file_name: The default file name that will be displayed in the file
-                dialog. The user can freely change it.
+        `file_contents`: The contents of the file to save. This can be a
+            string, bytes, or a path to a file on the server.
 
-            media_type: The media type of the file. Defaults to `None`, which
-                means that the media type will be guessed from the file name.
+        `file_name`: The default file name that will be displayed in the file
+            dialog. The user can freely change it.
 
-            directory: The directory where the file dialog should open. This has
-                no effect if the user is visiting the app in a browser.
+        `media_type`: The media type of the file. Defaults to `None`, which
+            means that the media type will be guessed from the file name.
+
+        `directory`: The directory where the file dialog should open. This has
+            no effect if the user is visiting the app in a browser.
         """
         if self.running_in_window:
             # FIXME: Find (1) a better way to get the active window and (2) a
             # way to open a file dialog without blocking the event loop.
             import webview  # type: ignore
 
             window = await self._get_webview_window()
@@ -1733,15 +1859,17 @@
 
             destination = destinations[0]
 
             if isinstance(file_contents, pathlib.Path):
                 await asyncio.to_thread(shutil.copy, file_contents, destination)
 
             elif isinstance(file_contents, str):
-                async with aiofiles.open(destination, "w", encoding="utf8") as file:
+                async with aiofiles.open(
+                    destination, "w", encoding="utf8"
+                ) as file:
                     await file.write(file_contents)
 
             elif isinstance(file_contents, bytes):  # type: ignore[unnecessary-isinstance]
                 async with aiofiles.open(destination, "wb") as file:
                     await file.write(file_contents)
 
             else:
@@ -1760,15 +1888,17 @@
                 file_contents.encode("utf-8"),
                 "text/plain" if media_type is None else media_type,
             )
 
         elif isinstance(file_contents, bytes):  # type: ignore[unnecessary-isinstance]
             as_asset = assets.BytesAsset(
                 file_contents,
-                "application/octet-stream" if media_type is None else media_type,
+                "application/octet-stream"
+                if media_type is None
+                else media_type,
             )
 
         else:
             raise ValueError(
                 f"The file contents must be a Path, str or bytes, not {file_contents!r}"
             )
 
@@ -1785,15 +1915,17 @@
 a.target = "_blank";
 document.body.appendChild(a);
 a.click();
 a.remove();
 """
         )
 
-    def _host_and_get_fill_as_css_variables(self, fill: rio.FillLike) -> dict[str, str]:
+    def _host_and_get_fill_as_css_variables(
+        self, fill: rio.FillLike
+    ) -> dict[str, str]:
         # Convert the fill
         fill = rio.Fill._try_from(fill)
 
         if isinstance(fill, rio.SolidFill):
             return {
                 "color": f"#{fill.color.hex}",
                 "background": "none",
@@ -1841,22 +1973,26 @@
             "danger",
         )
 
         for palette_name in palette_names:
             palette = getattr(thm, f"{palette_name}_palette")
             assert isinstance(palette, theme.Palette), palette
 
-            variables[f"--rio-global-{palette_name}-bg"] = f"#{palette.background.hex}"
+            variables[f"--rio-global-{palette_name}-bg"] = (
+                f"#{palette.background.hex}"
+            )
             variables[f"--rio-global-{palette_name}-bg-variant"] = (
                 f"#{palette.background_variant.hex}"
             )
             variables[f"--rio-global-{palette_name}-bg-active"] = (
                 f"#{palette.background_active.hex}"
             )
-            variables[f"--rio-global-{palette_name}-fg"] = f"#{palette.foreground.hex}"
+            variables[f"--rio-global-{palette_name}-fg"] = (
+                f"#{palette.foreground.hex}"
+            )
 
         # Text styles
         style_names = (
             "heading1",
             "heading2",
             "heading3",
             "text",
@@ -1867,26 +2003,32 @@
             assert isinstance(style, rio.TextStyle), style
 
             css_prefix = f"--rio-global-{style_name}"
             variables[f"{css_prefix}-font-name"] = (
                 "inherit" if style.font is None else style.font._serialize(self)
             )
             variables[f"{css_prefix}-font-size"] = f"{style.font_size}rem"
-            variables[f"{css_prefix}-italic"] = "italic" if style.italic else "normal"
+            variables[f"{css_prefix}-italic"] = (
+                "italic" if style.italic else "normal"
+            )
             variables[f"{css_prefix}-font-weight"] = style.font_weight
             variables[f"{css_prefix}-underlined"] = (
                 "underline" if style.underlined else "unset"
             )
             variables[f"{css_prefix}-all-caps"] = (
                 "uppercase" if style.all_caps else "unset"
             )
 
             # CSS variables for the fill
-            assert style.fill is not None, "Text fills must be defined in the theme."
-            fill_variables = self._host_and_get_fill_as_css_variables(style.fill)
+            assert (
+                style.fill is not None
+            ), "Text fills must be defined the theme's text styles."
+            fill_variables = self._host_and_get_fill_as_css_variables(
+                style.fill
+            )
 
             for var, value in fill_variables.items():
                 variables[f"{css_prefix}-{var}"] = value
 
         # Update the variables client-side
         await self._remote_apply_theme(
             variables,
@@ -1948,19 +2090,21 @@
         parameter_format="dict",
         await_response=True,
     )
     async def _evaluate_javascript(self, java_script_source: str) -> Any:
         """
         Evaluate the given JavaScript code in the client.
 
-        - The code is run as the body of a function, i.e.
-          - `return` statements are allowed and must be used to receive a result
-            other than `None`
-          - Variables are neatly contained in a scope and don't pollute the
-            global scope
+        The code is run as the body of a function, i.e.
+
+        - `return` statements are allowed and must be used to receive a result
+          other than `None`
+
+        - Variables are neatly contained in a scope and don't pollute the global
+          scope
         """
         raise NotImplementedError  # pragma: no cover
 
     @unicall.remote(
         name="requestFileUpload",
         parameter_format="dict",
         await_response=False,
@@ -1984,25 +2128,29 @@
 
         Any keys not present here are still preserved. Thus the function
         effectively behaves like `dict.update`.
         """
         raise NotImplementedError  # pragma: no cover
 
     @unicall.remote(name="registerFont", await_response=False)
-    async def _remote_register_font(self, name: str, urls: list[str | None]) -> None:
+    async def _remote_register_font(
+        self, name: str, urls: list[str | None]
+    ) -> None:
         raise NotImplementedError  # pragma: no cover
 
     @unicall.remote(
         name="closeSession",
         await_response=False,
     )
     async def _remote_close_session(self) -> None:
         raise NotImplementedError  # pragma: no cover
 
-    def _try_get_component_for_message(self, component_id: int) -> rio.Component | None:
+    def _try_get_component_for_message(
+        self, component_id: int
+    ) -> rio.Component | None:
         """
         Attempts to get the component referenced by `component_id`. Returns
         `None` if there is no such component. This can happen during normal
         opration, e.g. because a component has been deleted while the message
         was in flight.
         """
 
@@ -2032,15 +2180,15 @@
 
         # Update the component's state
         component._validate_delta_state_from_frontend(delta_state)
         component._apply_delta_state_from_frontend(delta_state)
         await component._call_event_handlers_for_delta_state(delta_state)
 
         # Trigger a refresh. The component itself doesn't need to rebuild, but
-        # other components with a state binding to the changed values might.
+        # other components with a attribute binding to the changed values might.
         await self._refresh()
 
     @unicall.local(name="componentMessage")
     async def _component_message(
         self,
         component_id: int,
         payload: Any,
@@ -2069,15 +2217,17 @@
             replace=True,
         )
 
         # Refresh the session
         await self._refresh()
 
     @unicall.local(name="onWindowResize")
-    async def _on_window_resize(self, new_width: float, new_height: float) -> None:
+    async def _on_window_resize(
+        self, new_width: float, new_height: float
+    ) -> None:
         """
         Called by the client when the window is resized.
         """
         # Update the stored window size
         self._window_width = new_width
         self._window_height = new_height
```

### Comparing `rio_ui-0.5.9/src/rio/state_properties.py` & `rio_ui-0.6/rio/state_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 if TYPE_CHECKING:
     from .components import Component
 
 
 __all__ = [
     "StateProperty",
-    "StateBinding",
-    "StateBindingMaker",
-    "PleaseTurnThisIntoAStateBinding",
+    "AttributeBinding",
+    "AttributeBindingMaker",
+    "PleaseTurnThisIntoAnAttributeBinding",
 ]
 
 
 class StateProperty:
     """
     StateProperties act like regular properties, with additional considerations:
 
@@ -30,15 +30,15 @@
       dirty in the session
 
     - State properties have the ability to share their value with other state
       property instances. If state property `A` is assigned to state property
       `B`, then `B` creates a `StateBinding` and any future access to `B` will
       be routed to `A` instead:
 
-    ```
+    ```python
     class Foo(Component):
         foo_text = "Hello"
 
         def build(self) -> Component:
             return Bar(bar_text=Foo.foo_text)  # Note `Foo` instead of `self`
     ```
     """
@@ -77,90 +77,90 @@
         # instance
         try:
             value = vars(instance)[self.name]
         except KeyError:
             raise AttributeError(self.name) from None
 
         # If the value is a binding return the binding's value
-        if isinstance(value, StateBinding):
+        if isinstance(value, AttributeBinding):
             return value.get_value()
 
         # Otherwise return the value
         return value
 
     def __set__(self, instance: Component, value: object) -> None:
         if self.readonly:
             cls_name = type(instance).__name__
             raise AttributeError(
                 f"Cannot assign to readonly property {cls_name}.{self.name}"
             )
 
         assert not isinstance(
             value, StateProperty
-        ), f"You're still using the old state binding syntax for {instance} {self.name}"
+        ), f"You're still using the old attribute binding syntax for {instance} {self.name}"
 
         instance._properties_assigned_after_creation_.add(self.name)
 
         # Look up the stored value
         instance_vars = vars(instance)
         try:
             local_value = instance_vars[self.name]
         except KeyError:
             # If no value is currently stored, that means this component is
             # currently being instantiated. We may have to create a state
             # binding.
-            if isinstance(value, PleaseTurnThisIntoAStateBinding):
-                value = self._create_state_binding(instance, value)
+            if isinstance(value, PleaseTurnThisIntoAnAttributeBinding):
+                value = self._create_attribute_binding(instance, value)
         else:
             # If a value is already stored, that means this is a re-assignment.
             # Which further means it's an assignment outside of `__init__`.
-            # Which is not a valid place to create a state binding.
-            if isinstance(value, PleaseTurnThisIntoAStateBinding):
+            # Which is not a valid place to create a attribute binding.
+            if isinstance(value, PleaseTurnThisIntoAnAttributeBinding):
                 raise RuntimeError(
-                    "State bindings can only be created when calling the component constructor"
+                    "Attribute bindings can only be created when calling the component constructor"
                 )
 
             # Delegate to the binding if it exists
-            if isinstance(local_value, StateBinding):
+            if isinstance(local_value, AttributeBinding):
                 local_value.set_value(value)
                 return
 
         # Otherwise set the value directly and mark the component as dirty
         instance_vars[self.name] = value
 
         instance._session_._register_dirty_component(
             instance,
             include_children_recursively=False,
         )
 
-    def _create_state_binding(
+    def _create_attribute_binding(
         self,
         component: Component,
-        request: PleaseTurnThisIntoAStateBinding,
-    ) -> StateBinding:
+        request: PleaseTurnThisIntoAnAttributeBinding,
+    ) -> AttributeBinding:
         # In order to create a `StateBinding`, the creator's attribute must
         # also be a binding
         creator = global_state.currently_building_component
         creator_vars = vars(creator)
 
         parent_binding = creator_vars[request.state_property.name]
 
-        if not isinstance(parent_binding, StateBinding):
-            parent_binding = StateBinding(
+        if not isinstance(parent_binding, AttributeBinding):
+            parent_binding = AttributeBinding(
                 owning_component_weak=weakref.ref(creator),
                 owning_property=self,
                 is_root=True,
                 parent=None,
                 value=parent_binding,
                 children=weakref.WeakSet(),
             )
             creator_vars[request.state_property.name] = parent_binding
 
         # Create the child binding
-        child_binding = StateBinding(
+        child_binding = AttributeBinding(
             owning_component_weak=weakref.ref(component),
             owning_property=self,
             is_root=False,
             parent=parent_binding,
             value=None,
             children=weakref.WeakSet(),
         )
@@ -169,29 +169,29 @@
         return child_binding
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} {self.name}>"
 
 
 @dataclasses.dataclass(eq=False)
-class StateBinding:
+class AttributeBinding:
     # Weak reference to the component containing this binding
     owning_component_weak: Callable[[], Component | None]
 
     # The state property whose value this binding is
     owning_property: StateProperty
 
     # Each binding is either the root-most binding, or a child of another
     # binding. This value is True if this binding is the root.
     is_root: bool
 
-    parent: StateBinding | None
+    parent: AttributeBinding | None
     value: object | None
 
-    children: weakref.WeakSet[StateBinding] = dataclasses.field(
+    children: weakref.WeakSet[AttributeBinding] = dataclasses.field(
         default_factory=weakref.WeakSet
     )
 
     def get_value(self) -> object:
         if self.is_root:
             return self.value
 
@@ -207,44 +207,44 @@
         # Otherwise this is the root-most binding. Set the value
         self.value = value
 
         # Then recursively mark all children as dirty
         self.recursively_mark_children_as_dirty()
 
     def recursively_mark_children_as_dirty(self) -> None:
-        to_do: list[StateBinding] = [self]
+        to_do: list[AttributeBinding] = [self]
 
         while to_do:
             cur = to_do.pop()
             owning_component = cur.owning_component_weak()
 
             if owning_component is not None:
                 owning_component._session_._register_dirty_component(
                     owning_component,
                     include_children_recursively=False,
                 )
 
             to_do.extend(cur.children)
 
 
-class StateBindingMaker:
+class AttributeBindingMaker:
     """
-    Helper class returned by `Component.bind()`. Used to create state bindings.
+    Helper class returned by `Component.bind()`. Used to create attribute bindings.
     """
 
     def __init__(self, component: Component):
         self.component = component
 
     def __getattribute__(self, name: str) -> object:
         component = super().__getattribute__("__dict__")["component"]
         component_cls = type(component)
 
         if name not in component_cls._state_properties_:
             raise AttributeError
 
         state_property = getattr(component_cls, name)
-        return PleaseTurnThisIntoAStateBinding(state_property)
+        return PleaseTurnThisIntoAnAttributeBinding(state_property)
 
 
-class PleaseTurnThisIntoAStateBinding:
+class PleaseTurnThisIntoAnAttributeBinding:
     def __init__(self, state_property: StateProperty):
         self.state_property = state_property
```

### Comparing `rio_ui-0.5.9/src/rio/text_style.py` & `rio_ui-0.6/rio/text_style.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 
 __all__ = [
     "Font",
     "TextStyle",
 ]
 
 
+class UnsetType:
+    pass
+
+
+UNSET = UnsetType()
+
+
 @dataclass(frozen=True)
 class Font(SelfSerializing):
     name: str
     regular: pathlib.Path | bytes
     bold: pathlib.Path | bytes | None = None
     italic: pathlib.Path | bytes | None = None
     bold_italic: pathlib.Path | bytes | None = None
@@ -41,15 +48,16 @@
     bold=common.HOSTED_ASSETS_DIR / "fonts/Roboto/Roboto-Bold.ttf",
     italic=common.HOSTED_ASSETS_DIR / "fonts/Roboto/Roboto-Italic.ttf",
     bold_italic=common.HOSTED_ASSETS_DIR / "fonts/Roboto/Roboto-BoldItalic.ttf",
 )
 
 Font.ROBOTO_MONO = Font(
     "Roboto Mono",
-    regular=common.HOSTED_ASSETS_DIR / "fonts/Roboto Mono/RobotoMono-Regular.ttf",
+    regular=common.HOSTED_ASSETS_DIR
+    / "fonts/Roboto Mono/RobotoMono-Regular.ttf",
     bold=common.HOSTED_ASSETS_DIR / "fonts/Roboto Mono/RobotoMono-Bold.ttf",
     italic=common.HOSTED_ASSETS_DIR / "fonts/Roboto Mono/RobotoMono-Italic.ttf",
     bold_italic=common.HOSTED_ASSETS_DIR
     / "fonts/Roboto Mono/RobotoMono-BoldItalic.ttf",
 )
 
 
@@ -64,34 +72,38 @@
     underlined: bool = False
     all_caps: bool = False
 
     def replace(
         self,
         *,
         font: Font | None = None,
-        fill: FillLike | None = None,
+        fill: FillLike | None | UnsetType = UNSET,
         font_size: float | None = None,
         italic: bool | None = None,
         font_weight: Literal["normal", "bold"] | None = None,
         underlined: bool | None = None,
         all_caps: bool | None = None,
     ) -> TextStyle:
         return type(self)(
             font=self.font if font is None else font,
-            fill=self.fill if fill is None else fill,
+            fill=self.fill if isinstance(fill, UnsetType) else fill,
             font_size=self.font_size if font_size is None else font_size,
             italic=self.italic if italic is None else italic,
-            font_weight=self.font_weight if font_weight is None else font_weight,
+            font_weight=self.font_weight
+            if font_weight is None
+            else font_weight,
             underlined=self.underlined if underlined is None else underlined,
             all_caps=self.all_caps if all_caps is None else all_caps,
         )
 
     def _serialize(self, sess: rio.Session) -> JsonDoc:
         return {
-            "fontName": None if self.font is None else self.font._serialize(sess),
+            "fontName": None
+            if self.font is None
+            else self.font._serialize(sess),
             "fill": None if self.fill is None else self.fill._serialize(sess),
             "fontSize": self.font_size,
             "italic": self.italic,
             "fontWeight": self.font_weight,
             "underlined": self.underlined,
             "allCaps": self.all_caps,
         }
```

### Comparing `rio_ui-0.5.9/src/rio/theme.py` & `rio_ui-0.6/rio/theme.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,87 +17,123 @@
     "Theme",
 ]
 
 
 T = TypeVar("T")
 
 
-def map_range(value: float, in1: float, in2: float, out1: float, out2: float) -> float:
-    """
-    Maps a value from one range to another.
-    """
-    frac = (value - in1) / (in2 - in1)
-    frac = min(max(frac, 0), 1)
-    return out1 + frac * (out2 - out1)
+def _derive_color(
+    color: rio.Color,
+    offset: float,
+    *,
+    bias_to_bright: float = 0,
+    target_color: rio.Color | None = None,
+) -> rio.Color:
+    # If a target color was provided, move towards that color
+    #
+    # The more different the two colors are, the less the new color will be
+    # used. This helps e.g. with dark themes, which look bonkers if the target
+    # color is very light.
+    if target_color is not None:
+        difference = (
+            abs(target_color.red - color.red)
+            + abs(target_color.green - color.green)
+            + abs(target_color.blue - color.blue)
+        )
 
+        if difference < 0.01:
+            offset_scale = 1
+        else:
+            offset_scale = min(1.0 / difference, 1)
 
-def color_with_brightness(color: rio.Color, target_brightness: float) -> rio.Color:
-    """
-    Returns the same shade of color, but with a different brightness. Brightness
-    0 corresponds to pure black. 1 is pure white. 0.5 is the original color.
-    """
-    hue, saturation, value = color.hsv
+        result = color.blend(target_color, offset * offset_scale)
 
-    # Keep neutral colors neutral
-    if saturation == 0 or value == 0:
-        return rio.Color.from_grey(
-            target_brightness,
-            opacity=color.opacity,
-        )
+    # Otherwise change the color's brightness
+    else:
+        threshold = 0.5 + 0.5 * bias_to_bright
+        perceived_brightness = color.perceived_brightness
+        brighten = perceived_brightness <= threshold
+
+        # Calculate the new color
+        if brighten:
+            result = color.brighter(offset)
+        else:
+            result = color.darker(offset)
+
+    # Desaturate the color slightly
+    hue, saturation, value = result.hsv
+    saturation = max(saturation - offset * 0.6, 0)
 
-    # Otherwise keep the color and adjust the brightness
     return rio.Color.from_hsv(
         hue=hue,
-        saturation=map_range(saturation, 0.5, 1, 1, 0),
-        value=min(target_brightness * 2, 1),
-        opacity=color.opacity,
+        saturation=saturation,
+        value=value,
+        opacity=result.opacity,
+    )
+
+
+def _make_semantic_palette(color: rio.Color) -> Palette:
+    return Palette(
+        background=color,
+        background_variant=_derive_color(
+            color,
+            0.08,
+            bias_to_bright=-0.4,
+        ),
+        background_active=_derive_color(
+            color,
+            0.15,
+            bias_to_bright=0.8,
+        ),
+        foreground=_derive_color(
+            color,
+            0.4,
+        ),
     )
 
 
 @final
 @dataclass(frozen=True)
 class Palette:
     background: rio.Color
     background_variant: rio.Color
     background_active: rio.Color
 
     foreground: rio.Color
 
-    @classmethod
-    def _from_color(
-        cls,
+    @staticmethod
+    def from_color(
         color: rio.Color,
         *,
-        colorful: bool,
-    ) -> Self:
-        # For the foreground color, keep the same shade but adjust the
-        # brightness to make it readable.
-        current_brightness = color.perceived_brightness
-
-        if colorful:
-            brightness_offset = 0.5
-            brightness_cutoff = 0.2
-        else:
-            brightness_offset = 0.8
-            brightness_cutoff = 0.08
-
-        target_brightness = (
-            current_brightness - brightness_offset
-            if current_brightness > 0.55  # Bias towards bright labels
-            else current_brightness + brightness_offset
-        )
-        target_brightness = max(
-            min(target_brightness, 1 - brightness_cutoff), brightness_cutoff
-        )
+        offset: float = 1,
+        target_color: rio.Color | None = None,
+    ) -> Palette:
+        """
+        ## Metadata
 
-        return cls(
+        experimental: True
+        """
+        return Palette(
             background=color,
-            background_variant=color.brighter(0.05),
-            background_active=color.brighter(0.15),
-            foreground=color_with_brightness(color, target_brightness),
+            background_variant=_derive_color(
+                color,
+                offset=0.1 * offset,
+                bias_to_bright=-0.3,
+                target_color=target_color,
+            ),
+            background_active=_derive_color(
+                color,
+                offset=0.2 * offset,
+                bias_to_bright=-0.3,
+                target_color=target_color,
+            ),
+            foreground=_derive_color(
+                color,
+                offset=0.8,
+            ),
         )
 
     def replace(
         self,
         background: rio.Color | None = None,
         background_variant: rio.Color | None = None,
         background_active: rio.Color | None = None,
@@ -120,18 +156,14 @@
 class Theme:
     """
     Defines the visual style of the application.
 
     The `Theme` contains all colors, text styles, and other visual properties
     that are used throughout the application. If you wish to change the
     appearance of your app, this is the place to do it.
-
-    TODO: Finalize theming and document it
-
-    TODO: Give an example for how to create a theme and use it in an app.
     """
 
     _: KW_ONLY
 
     primary_palette: Palette
     secondary_palette: Palette
 
@@ -157,187 +189,299 @@
     # Text styles
     heading1_style: rio.TextStyle
     heading2_style: rio.TextStyle
     heading3_style: rio.TextStyle
     text_style: rio.TextStyle
 
     @classmethod
-    def from_color(
+    def from_colors(
         cls,
         primary_color: rio.Color | None = None,
         secondary_color: rio.Color | None = None,
         background_color: rio.Color | None = None,
         neutral_color: rio.Color | None = None,
         hud_color: rio.Color | None = None,
         disabled_color: rio.Color | None = None,
         success_color: rio.Color | None = None,
         warning_color: rio.Color | None = None,
         danger_color: rio.Color | None = None,
         corner_radius_small: float = 0.5,
-        corner_radius_medium: float = 1.4,
-        corner_radius_large: float = 2.4,
-        color_headings: bool | Literal["auto"] = "auto",
+        corner_radius_medium: float = 1.0,
+        corner_radius_large: float = 2.0,
+        heading_fill: Literal["primary", "plain", "auto"]
+        | rio.FillLike = "auto",
         font: text_style_module.Font = text_style_module.Font.ROBOTO,
         monospace_font: text_style_module.Font = text_style_module.Font.ROBOTO_MONO,
         light: bool = True,
     ) -> Self:
-        # Impute defaults
-        if primary_color is None:
-            primary_color = rio.Color.from_hex("01dffd")
+        """
+        Creates a new theme based on the provided colors.
 
-        if secondary_color is None:
-            secondary_color = rio.Color.from_hex("0083ff")
+        Themes store a large number of colors and text styles that are used
+        throughout the app. This function provides a convenient way to only
+        specify the most important colors of your theme, and have Rio handle the
+        rest. It is the recommended way to create a new theme.
 
-        if success_color is None:
-            success_color = rio.Color.from_hex("1E8E3E")
+        To use a custom theme in your app first create a theme, and then pass it
+        to your app instance
 
-        if warning_color is None:
-            warning_color = rio.Color.from_hex("F9A825")
+        ```python
+        # Create a new theme
+        theme = rio.Theme.from_colors(
+            # Configure your theme here
+        )
 
-        if danger_color is None:
-            danger_color = rio.Color.from_hex("B3261E")
+        # And apply it to your app
+        app = rio.App(
+            theme=theme,
+            # ...
+        )
+        ```
 
-        # Extract palettes from the material theme
-        primary_palette = Palette._from_color(primary_color, colorful=False)
-        secondary_palette = Palette._from_color(secondary_color, colorful=False)
-
-        if light:
-            if background_color is None:
-                background_palette = Palette(
-                    background=rio.Color.WHITE,
-                    background_variant=rio.Color.from_grey(0.96).blend(
-                        primary_color, 0.04
-                    ),
-                    background_active=rio.Color.from_grey(0.96).blend(
-                        primary_color, 0.1
-                    ),
-                    foreground=rio.Color.from_grey(0.15),
-                )
-            else:
-                background_palette = Palette._from_color(
-                    background_color, colorful=False
-                )
+        Alternatively, there is also `pair_from_colors`, which creates both a
+        light and a dark theme at the same time. This is useful if you want Rio
+        to automatically switch between the two based on the user's system
+        preferences.
 
-            if neutral_color is None:
-                neutral_palette = Palette(
-                    background=rio.Color.from_grey(0.97).blend(primary_color, 0.04),
-                    background_variant=rio.Color.from_grey(0.93).blend(
-                        primary_color, 0.07
-                    ),
-                    background_active=rio.Color.from_grey(0.93).blend(
-                        primary_color, 0.15
-                    ),
-                    foreground=rio.Color.from_grey(0.1),
-                )
-            else:
-                neutral_palette = Palette._from_color(neutral_color, colorful=False)
+        ## Parameters
 
-            if hud_color is None:
-                hud_palette = Palette._from_color(
-                    rio.Color.from_grey(
-                        0.06,
-                        opacity=0.9,
-                    ),
-                    colorful=False,
-                )
-            else:
-                hud_palette = Palette._from_color(hud_color, colorful=False)
+        `primary_color`: The main color of your app. This color will be used to
+            tint the background and by some large components to fill entire
+            areas with color.
 
-            if disabled_color is None:
-                disabled_palette = Palette(
-                    rio.Color.from_grey(0.7),
-                    rio.Color.from_grey(0.75),
-                    rio.Color.from_grey(0.80),
-                    rio.Color.from_grey(0.4),
-                )
-            else:
-                disabled_palette = Palette._from_color(disabled_color, colorful=False)
+        `secondary_color`: A color that nicely complements the primary color. It
+            is often used by small components such as buttons and switches.
 
-            shadow_color = rio.Color.from_rgb(0.1, 0.1, 0.4, 0.3)
+        `background_color`: The app's background color. This should be a neutral
+            color that doesn't distract from the content.
 
-        else:
-            if background_color is None:
-                background_palette = Palette(
-                    background=rio.Color.from_grey(0.08).blend(primary_color, 0.02),
-                    background_variant=rio.Color.from_grey(0.14).blend(
-                        primary_color, 0.04
-                    ),
-                    background_active=rio.Color.from_grey(0.14).blend(
-                        primary_color, 0.10
-                    ),
-                    foreground=rio.Color.from_grey(0.9),
-                )
-            else:
-                background_palette = Palette._from_color(
-                    background_color, colorful=False
-                )
+        `neutral_color`: Similar to the background color, it is also used for
+            neutral areas. It should however be slightly different, allowing you
+            to create a visual hierarchy. This is the default color of large
+            elements such as cards.
 
-            if neutral_color is None:
-                neutral_palette = Palette(
-                    background=rio.Color.from_grey(0.16).blend(primary_color, 0.03),
-                    background_variant=rio.Color.from_grey(0.2).blend(
-                        primary_color, 0.04
-                    ),
-                    background_active=rio.Color.from_grey(0.2).blend(
-                        primary_color, 0.10
-                    ),
-                    foreground=rio.Color.from_grey(0.5),
-                )
-            else:
-                neutral_palette = Palette._from_color(neutral_color, colorful=False)
+        `hud_color`: Used for elements that pop over the content, such as
+            tooltips.
 
-            if hud_color is None:
-                hud_palette = Palette._from_color(
-                    rio.Color.from_grey(
-                        0.2,
-                        opacity=0.8,
-                    ),
-                    colorful=False,
-                )
-            else:
-                hud_palette = Palette._from_color(hud_color, colorful=False)
+        `disabled_color`: Used by insensitive components to indicate that they
+            are not interactive. Typically a shade of grey.
+
+        `success_color`: A color to give positive feedback the user. Typically
+            a shade of green.
+
+        `warning_color`: A color to indicate that something might be wrong, but
+            isn't critical. Typically orange.
+
+        `danger_color`: A color to indicate that something is wrong and needs
+            immediate attention. Typically a shade of red.
+
+        `corner_radius_small`: The corner radius of small components such as
+            text inputs
 
-            if disabled_color is None:
-                disabled_palette = Palette(
-                    rio.Color.from_grey(0.2),
-                    rio.Color.from_grey(0.15),
-                    rio.Color.from_grey(0.10),
-                    rio.Color.from_grey(0.6),
+        `corner_radius_medium`: The corner radius of medium-sized components,
+            such as small cards.
+
+        `corner_radius_large`: The corner radius of large components, such as
+            large cards and dialogs.
+
+        `heading_fill`: The fill to use for headings. This allows you to specify
+            a more interesting color, or even a gradient. If set to `"auto"`,
+            Rio will automatically switch between the primary color and a plain
+            text color based on legibility.
+
+            This only affects headings in background and neutral contexts.
+
+        `font`: The default font to use when no other is specified.
+
+        `monospace_font`: The font to use for monospace text, such as code.
+
+        `light`: Whether to create a light or dark theme. This affects the
+            default values for some colors, such as the background.
+        """
+        # Primary palette
+        if primary_color is None:
+            primary_color = rio.Color.from_hex("01dffd")
+
+        primary_palette = Palette(
+            background=primary_color,
+            background_variant=_derive_color(
+                primary_color,
+                0.08,
+                bias_to_bright=-0.5,
+            ),
+            background_active=_derive_color(
+                primary_color,
+                0.15,
+                bias_to_bright=0.6,
+            ),
+            foreground=(
+                rio.Color.from_grey(0.1)
+                if primary_color.perceived_brightness > 0.5
+                else rio.Color.from_grey(0.9)
+            ),
+        )
+
+        # Secondary palette
+        if secondary_color is None:
+            secondary_color = rio.Color.from_hex("0083ff")
+
+        secondary_palette = Palette(
+            background=secondary_color,
+            background_variant=_derive_color(
+                secondary_color,
+                0.08,
+                bias_to_bright=-0.3,
+            ),
+            background_active=_derive_color(
+                secondary_color,
+                0.15,
+                bias_to_bright=0.6,
+            ),
+            foreground=(
+                rio.Color.from_grey(0.1)
+                if secondary_color.perceived_brightness > 0.75
+                else rio.Color.from_grey(0.9)
+            ),
+        )
+
+        # Background palette
+        if background_color is None:
+            if light:
+                background_color = rio.Color.from_grey(1.00).blend(
+                    primary_color, 0.05
                 )
             else:
-                disabled_palette = Palette._from_color(disabled_color, colorful=False)
+                background_color = rio.Color.from_grey(0.08).blend(
+                    primary_color, 0.05
+                )
+
+        neutral_text_color = (
+            rio.Color.from_grey(0.1)
+            if background_color.perceived_brightness > 0.5
+            else rio.Color.from_grey(0.9)
+        )
+
+        background_palette = Palette(
+            background=background_color,
+            background_variant=_derive_color(
+                background_color,
+                0.25,
+                bias_to_bright=-0.15,
+                target_color=primary_color,
+            ),
+            background_active=_derive_color(
+                background_color,
+                0.4,
+                bias_to_bright=0.15,
+                target_color=primary_color,
+            ),
+            foreground=neutral_text_color,
+        )
+
+        # Neutral palette
+        #
+        # This one is similar to the background palette, but with a slightly
+        # different shade.
+        if neutral_color is None:
+            neutral_color = background_palette.background_variant
+
+        neutral_palette = Palette(
+            background=neutral_color,
+            background_variant=_derive_color(
+                neutral_color,
+                0.35,
+                bias_to_bright=-0.15,
+                target_color=primary_color,
+            ),
+            background_active=_derive_color(
+                neutral_color,
+                0.5,
+                bias_to_bright=0.15,
+                target_color=primary_color,
+            ),
+            foreground=neutral_text_color,
+        )
+
+        # HUD palette
+        if hud_color is None:
+            hud_color = rio.Color.from_grey(0.2)
+
+        hud_palette = Palette(
+            background=hud_color,
+            background_variant=_derive_color(
+                hud_color,
+                0.08,
+            ),
+            background_active=_derive_color(
+                hud_color,
+                0.15,
+            ),
+            foreground=(
+                rio.Color.from_grey(0.1)
+                if hud_color.perceived_brightness > 0.5
+                else rio.Color.from_grey(0.9)
+            ),
+        )
+
+        # Keep the disabled palette subdued. It's not meant to be perfectly
+        # readable
+        if disabled_color is None:
+            disabled_color = rio.Color.from_grey(0.7)
+
+        disabled_palette = Palette(
+            background=disabled_color,
+            background_variant=_derive_color(disabled_color, 0.08),
+            background_active=_derive_color(disabled_color, 0.15),
+            foreground=_derive_color(disabled_color, 0.3),
+        )
 
-            shadow_color = rio.Color.from_rgb(0.0, 0.0, 0.1, 0.35)
+        shadow_color = rio.Color.from_rgb(0.1, 0.1, 0.4, 0.3)
 
         # Semantic colors
-        success_palette = Palette._from_color(success_color, colorful=True)
-        warning_palette = Palette._from_color(warning_color, colorful=True)
-        danger_palette = Palette._from_color(danger_color, colorful=True)
+        if success_color is None:
+            success_color = rio.Color.from_hex("1e8e3e")
+
+        if warning_color is None:
+            warning_color = rio.Color.from_hex("f9a825")
+
+        if danger_color is None:
+            danger_color = rio.Color.from_hex("b3261e")
+
+        success_palette = _make_semantic_palette(success_color)
+        warning_palette = _make_semantic_palette(warning_color)
+        danger_palette = _make_semantic_palette(danger_color)
 
         # Colorful headings can be a problem when the primary color is similar
         # to the background/neutral color. If the `color_headings` argument is
         # set to `auto`, disable coloring if the colors are close.
-        if color_headings == "auto":
+        if heading_fill == "auto":
             brightness1 = primary_palette.background.perceived_brightness
             brightness2 = background_palette.background.perceived_brightness
 
-            color_headings = abs(brightness1 - brightness2) > 0.3
+            heading_fill = (
+                "primary" if abs(brightness1 - brightness2) > 0.3 else "plain"
+            )
+
+        if heading_fill == "primary":
+            heading_fill = primary_color
+        elif heading_fill == "plain":
+            heading_fill = neutral_text_color
+        else:
+            heading_fill = heading_fill
 
         # Text styles
-        text_color = rio.Color.from_grey(0.1 if light else 0.9)
-
         heading1_style = rio.TextStyle(
             font_size=3.0,
-            fill=primary_color if color_headings else text_color,
+            fill=heading_fill,
         )
         heading2_style = heading1_style.replace(font_size=1.8)
         heading3_style = heading1_style.replace(font_size=1.2)
         text_style = heading1_style.replace(
             font_size=1,
-            fill=text_color,
+            fill=neutral_text_color,
         )
 
         return cls(
             primary_palette=primary_palette,
             secondary_palette=secondary_palette,
             background_palette=background_palette,
             neutral_palette=neutral_palette,
@@ -355,15 +499,15 @@
             heading1_style=heading1_style,
             heading2_style=heading2_style,
             heading3_style=heading3_style,
             text_style=text_style,
         )
 
     @classmethod
-    def pair_from_color(
+    def pair_from_colors(
         cls,
         *,
         primary_color: rio.Color | None = None,
         secondary_color: rio.Color | None = None,
         background_color: rio.Color | None = None,
         neutral_color: rio.Color | None = None,
         hud_color: rio.Color | None = None,
@@ -372,75 +516,138 @@
         warning_color: rio.Color | None = None,
         danger_color: rio.Color | None = None,
         corner_radius_small: float = 0.6,
         corner_radius_medium: float = 1.6,
         corner_radius_large: float = 2.6,
         font: text_style_module.Font = text_style_module.Font.ROBOTO,
         monospace_font: text_style_module.Font = text_style_module.Font.ROBOTO_MONO,
-        color_headings: bool | Literal["auto"] = "auto",
+        heading_fill: Literal["primary", "plain", "auto"]
+        | rio.FillLike = "auto",
     ) -> tuple[Self, Self]:
+        """
+        This function is very similar to `from_colors`, but it returns two
+        themes: A light and a dark one. When applying two themes to your app,
+        Rio will automatically switch between them based on the user's system
+        preferences.
+
+        ```python
+        # Create a theme pair
+        themes = rio.Theme.pair_from_colors(
+            # Configure your theme here
+        )
+
+        # And apply them to your app
+        app = rio.App(
+            theme=themes,
+            # ...
+        )
+        ```
+
+        ## Parameters
+
+        `primary_color`: The main color of your app. This color will be used to
+            tint the background and by some large components to fill entire
+            areas with color.
+
+        `secondary_color`: A color that nicely complements the primary color. It
+            is often used by small components such as buttons and switches.
+
+        `background_color`: The app's background color. This should be a neutral
+            color that doesn't distract from the content.
+
+        `neutral_color`: Similar to the background color, it is also used for
+            neutral areas. It should however be slightly different, allowing you
+            to create a visual hierarchy. This is the default color of large
+            elements such as cards.
+
+        `hud_color`: Used for elements that pop over the content, such as
+            tooltips.
+
+        `disabled_color`: Used by insensitive components to indicate that they
+            are not interactive. Typically a shade of grey.
+
+        `success_color`: A color to give positive feedback the user. Typically
+            a shade of green.
+
+        `warning_color`: A color to indicate that something might be wrong, but
+            isn't critical. Typically orange.
+
+        `danger_color`: A color to indicate that something is wrong and needs
+            immediate attention. Typically a shade of red.
+
+        `corner_radius_small`: The corner radius of small components such as
+            text inputs
+
+        `corner_radius_medium`: The corner radius of medium-sized components,
+            such as small cards.
+
+        `corner_radius_large`: The corner radius of large components, such as
+            large cards and dialogs.
+
+        `heading_fill`: The fill to use for headings. This allows you to specify
+            a more interesting color, or even a gradient. If set to `"auto"`,
+            Rio will automatically switch between the primary color and a plain
+            text color based on legibility.
+
+            This only affects headings in background and neutral contexts.
+
+        `font`: The default font to use when no other is specified.
+
+        `monospace_font`: The font to use for monospace text, such as code.
+        """
         func = functools.partial(
-            cls.from_color,
+            cls.from_colors,
             primary_color=primary_color,
             secondary_color=secondary_color,
             background_color=background_color,
             neutral_color=neutral_color,
             hud_color=hud_color,
             disabled_color=disabled_color,
             success_color=success_color,
             warning_color=warning_color,
             danger_color=danger_color,
             corner_radius_small=corner_radius_small,
             corner_radius_medium=corner_radius_medium,
             corner_radius_large=corner_radius_large,
             font=font,
             monospace_font=monospace_font,
-            color_headings=color_headings,
+            heading_fill=heading_fill,
         )
         return (
             func(light=True),
             func(light=False),
         )
 
     def text_color_for(self, color: rio.Color) -> rio.Color:
         """
-        Given the color of a background, return which color should be used for
-        text on top of it.
+        Given the color of a background, return a legible text color to use on
+        top of it.
         """
-        if color.perceived_brightness > 0.6:
-            return rio.Color.from_grey(0.1)
-        else:
-            return rio.Color.from_grey(0.9)
+        return _derive_color(color, offset=0.8)
 
     def _serialize_colorset(self, color: color.ColorSet) -> Jsonable:
         # A colorset more-or-less translates to a switcheroo. Thus, this
         # function needs to provide all information needed to create one.
 
         # If the color is a string, just pass it through. In this case there is
         # an actual switcheroo which can be used.
         if isinstance(color, str):
             return color
 
         # TODO: If the color is identical/very similar to a theme color use the
         #       corresponding switcheroo.
 
         # Otherwise create all the necessary variables to emulate a switcheroo.
-        plain_bg = color
-        foreground = self.text_color_for(color)
-
-        plain_bg_variant = plain_bg.blend(foreground, 0.15)
-        plain_bg_active = plain_bg.blend(foreground, 0.3)
+        palette = Palette.from_color(color)
 
         return {
-            "plainBg": color.rgba,
-            "plainBgVariant": plain_bg_variant.rgba,
-            "plainBgActive": plain_bg_active.rgba,
-            "plainFg": foreground.rgba,
-            "accentBg": self.secondary_palette.background.rgba,
-            "accentFg": self.secondary_palette.foreground.rgba,
+            "localBg": palette.background.rgba,
+            "localBgVariant": palette.background_variant.rgba,
+            "localBgActive": palette.background_active.rgba,
+            "localFg": palette.foreground.rgba,
         }
 
     def replace(
         self,
         primary_palette: Palette | None = None,
         secondary_palette: Palette | None = None,
         background_palette: Palette | None = None,
@@ -480,36 +687,46 @@
             ),
             success_palette=common.first_non_null(
                 success_palette, self.success_palette
             ),
             warning_palette=common.first_non_null(
                 warning_palette, self.warning_palette
             ),
-            danger_palette=common.first_non_null(danger_palette, self.danger_palette),
+            danger_palette=common.first_non_null(
+                danger_palette, self.danger_palette
+            ),
             corner_radius_small=common.first_non_null(
                 corner_radius_small, self.corner_radius_small
             ),
             corner_radius_medium=common.first_non_null(
                 corner_radius_medium, self.corner_radius_medium
             ),
             corner_radius_large=common.first_non_null(
                 corner_radius_large, self.corner_radius_large
             ),
             shadow_color=common.first_non_null(shadow_color, self.shadow_color),
             font=common.first_non_null(font_family, self.font),
-            monospace_font=common.first_non_null(monospace_font, self.monospace_font),
-            heading1_style=common.first_non_null(heading1_style, self.heading1_style),
-            heading2_style=common.first_non_null(heading2_style, self.heading2_style),
-            heading3_style=common.first_non_null(heading3_style, self.heading3_style),
+            monospace_font=common.first_non_null(
+                monospace_font, self.monospace_font
+            ),
+            heading1_style=common.first_non_null(
+                heading1_style, self.heading1_style
+            ),
+            heading2_style=common.first_non_null(
+                heading2_style, self.heading2_style
+            ),
+            heading3_style=common.first_non_null(
+                heading3_style, self.heading3_style
+            ),
             text_style=common.first_non_null(text_style, self.text_style),
         )
 
     @property
     def is_light_theme(self) -> bool:
-        return self.primary_palette.background.perceived_brightness >= 0.5
+        return self.background_palette.background.perceived_brightness >= 0.5
 
     @property
     def primary_color(self) -> rio.Color:
         return self.primary_palette.background
 
     @property
     def secondary_color(self) -> rio.Color:
```

### Comparing `rio_ui-0.5.9/src/rio/user_settings_module.py` & `rio_ui-0.6/rio/user_settings_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     ```python
     # Create a dataclass that inherits from rio.UserSettings. This indicates to
     # Rio that these are settings and should be persisted.
     class MySettings(rio.UserSettings):
         language: str = "en"
 
-
     # Attach the settings to the app. This way the settings will be available in
     # all sessions. They will be loaded automatically from the user whenever
     # they connect or start the app.
     app = rio.App(
         ...,
         default_attachments=[
             MySettings(),
@@ -68,17 +67,18 @@
     you can think of.
 
     Warning: Since settings are stored on the user's device, you should never
     trust them to be valid. A malicious actor could modify them to intentionally
     trigger bugs in your app. Always validate the values before using them.
 
     ## Attributes
-        section_name: If provided, the settings file will contain a section with
-            this name. This allows you to keep the configuration file organized.
-            If `None`, the settings will be stored outside of any section.
+
+    section_name: If provided, the settings file will contain a section with
+        this name. This allows you to keep the configuration file organized.
+        If `None`, the settings will be stored outside of any section.
     """
 
     # Any values from this class will be stored in the configuration file under
     # this section. This has to be set to a string. If empty, the values will be
     # set outside of any sections.
     section_name: ClassVar[str] = ""
 
@@ -135,15 +135,17 @@
             settings_vars[field_name] = field_value
 
         return self
 
     def __setattr__(self, name: str, value: Any) -> None:
         # These attributes doesn't exist yet during the constructor
         dct = vars(self)
-        dirty_attribute_names = dct.setdefault("_rio_dirty_attribute_names_", set())
+        dirty_attribute_names = dct.setdefault(
+            "_rio_dirty_attribute_names_", set()
+        )
 
         # Set the attribute
         dct[name] = value
 
         # Don't synchronize internal attributes
         if name in __class__.__annotations__:
             return
```

### Comparing `rio_ui-0.5.9/src/rio/world_units.py` & `rio_ui-0.6/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/OFL.txt` & `rio_ui-0.6/rio/assets/hosted/fonts/Noto Sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/LICENSE.txt` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.6/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.6/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.6/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.6/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/cli/__init__.py` & `rio_ui-0.6/rio/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 _logger = logging.getLogger(__name__)
 
 
 from typing import Literal
 
-import imy.package_metadata
 import introspection
 import revel
 from revel import *  # type: ignore
 
 import rio.snippets
 
 from . import project, project_setup, run_project
@@ -28,15 +27,15 @@
     details="""
 Rio is a framework for building reactive apps and websites in Python. It's
 designed to be easy to use, and to get out of your way as much as possible.
 
 This is the command line interface for Rio. You can use it to easily create new
 projects, run them, and more.
 """,
-    version=imy.package_metadata.get_package_version("rio-ui"),
+    version=rio.__version__,
 )
 
 
 @app.command(
     aliases={"init", "create"},
     summary="Create a new Rio project",
     details="""
@@ -194,19 +193,26 @@
 import rio
 
 from .. import components as comps
 
 
 class {class_name}(rio.Component):
     def build(self) -> rio.Component:
-        return rio.Markdown('''
-            ## This is a sample component
-
-            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
-            ''')
+        return rio.Markdown(
+            '''
+## This is a Sample Page
+
+Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
+incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
+nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
+Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
+fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
+culpa qui officia deserunt mollit anim id est laborum.
+            '''
+        )
 """
             )
         else:
             file_path.write_text(
                 f"""from __future__ import annotations
 
 from dataclasses import KW_ONLY, field
```

### Comparing `rio_ui-0.5.9/src/rio/cli/cli_instance.py` & `rio_ui-0.6/rio/cli/cli_instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
         # Nope, create a new instance
         self = cls._instance = super(CliInstance, cls).__new__(cls)
 
         # Read the config
         try:
             config_dir = Path(platformdirs.user_config_dir("rio"))
-            self._config = tomlkit.loads((config_dir / "config.toml").read_text())
+            self._config = tomlkit.loads(
+                (config_dir / "config.toml").read_text()
+            )
         except FileNotFoundError:
             self._config = tomlkit.document()
         except OSError as err:
             fatal(f"Couldn't read Rio's configuration: {err}")
 
         # Api client
         self._api_client = None
```

### Comparing `rio_ui-0.5.9/src/rio/cli/nice_traceback.py` & `rio_ui-0.6/rio/cli/nice_traceback.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,17 @@
     frame_filter: Callable[[traceback.FrameSummary], bool] = lambda _: True,
 ) -> str:
     def format_inner(err: BaseException) -> None:
         # Chain to the cause or context if there is one
         if err.__cause__ is not None:
             format_inner(err.__cause__)
             out.write("\n\n")
-            out.write(f"The above exception was the direct cause of the following:\n\n")
+            out.write(
+                f"The above exception was the direct cause of the following:\n\n"
+            )
             include_header = False
 
         elif err.__context__ is not None:
             format_inner(err.__context__)
             out.write("\n\n")
             out.write(
                 f"During handling of the above exception, another exception occurred:\n\n"
```

### Comparing `rio_ui-0.5.9/src/rio/cli/project.py` & `rio_ui-0.6/rio/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         # just strings which are appended to the end of the file, one per line.
         self.rioignore_additions: list[str] = []
 
     def get_key(
         self,
         section_name: str,
         key_name: str,
-        type: Type[T],
+        key_type: Type[T],
         default_value: Any,
     ) -> T:
         """
         Fetches the value of a key from the `rio.toml` file. If the key is
         missing, and a default value was provided it is returned instead.
 
         If the default value is `DEFAULT_FATAL`, an error is displayed and the
@@ -99,17 +99,17 @@
 
             if default_value is DEFAULT_KEYERROR:
                 raise KeyError(key_name)
 
             value = default_value
 
         # Make sure the value is the correct type
-        if not isinstance(value, type):
+        if not isinstance(value, key_type):
             fatal(
-                f"`rio.toml` contains an invalid value for `{key_name}`: expected {type}, got {type(value)}",
+                f"`rio.toml` contains an invalid value for `{key_name}`: expected {key_type}, got {type(value)}",
                 status_code=1,
             )
 
         # Done
         return value
 
     def set_key(self, section_name: str, key_name: str, value: Any) -> None:
@@ -196,15 +196,17 @@
             allowed_chars = "abcdefghijklmnopqrstuvwxyz0123456789-"
             normalized = re.sub("[^" + allowed_chars + "]", "-", name.lower())
 
             if name == normalized:
                 break
 
             normalized = re.sub("-+", "-", normalized)
-            print(f"`{name}` cannot be used for app names. Is `{normalized}` okay?")
+            print(
+                f"`{name}` cannot be used for app names. Is `{normalized}` okay?"
+            )
 
             if revel.select_yes_no("", default_value=True):
                 name = normalized
                 break
 
         # Store the name
         self.set_key("deploy", "name", name)
@@ -292,22 +294,28 @@
 
         # No such file. Offer to create one
         except FileNotFoundError:
             warning(
                 f"You don't appear to be inside of a [bold primary]Rio[/] project. Would you like to create one?"
             )
 
+            import sys
+
+            sys.stdout.write(revel.Fore.RESET)
+            revel.print()
+            revel.input("[yellow]Foo[/]")
+
             if not revel.select_yes_no("", default_value=True):
                 fatal(
                     f"Couldn't find `rio.toml`.",
                     status_code=1,
                 )
 
-            rio_toml_dict, dirty_keys = RioProject._create_toml_contents_interactively(
-                project_dir
+            rio_toml_dict, dirty_keys = (
+                RioProject._create_toml_contents_interactively(project_dir)
             )
 
         # Anything OS related
         except OSError as e:
             fatal(
                 f"Cannot read `{rio_toml_path}`: {e}",
                 status_code=1,
```

### Comparing `rio_ui-0.5.9/src/rio/cli/project_setup.py` & `rio_ui-0.6/rio/cli/project_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             build=pages.{page_component_name},
         ),"""
         )
 
     page_string = "\n".join(page_strings)
 
     # Imports
-    default_theme = rio.Theme.from_color()
+    default_theme = rio.Theme.from_colors()
     buffer = io.StringIO()
 
     buffer.write(
         f"""
 from __future__ import annotations
 
 from pathlib import Path
@@ -132,16 +132,18 @@
     buffer.write(
         f"""
 
 # Define a theme for Rio to use.
 #
 # You can modify the colors here to adapt the appearance of your app or website.
 # The most important parameters are listed, but more are available! You can find
-# them all in the docs TODO: Add link.
-theme = rio.Theme.from_color(
+# them all in the docs
+#
+# https://rio.dev/docs/api/theme
+theme = rio.Theme.from_colors(
     primary_color=rio.Color.from_hex("{default_theme.primary_color.hex}"),
     secondary_color=rio.Color.from_hex("{default_theme.secondary_color.hex}"),
     light=True,
 )
 
 
 # Create the Rio app
@@ -278,15 +280,17 @@
     if needs_isort:
         formatted_code = isort.code(buffer.getvalue())
         out.write(formatted_code)
     else:
         out.write(buffer.getvalue())
 
 
-def generate_dependencies_file(project_dir: Path, dependencies: dict[str, str]) -> None:
+def generate_dependencies_file(
+    project_dir: Path, dependencies: dict[str, str]
+) -> None:
     """
     Writes a `requirements.txt` file with the given dependencies. Does nothing
     if there are no dependencies.
     """
     # Anything to do?
     if not dependencies:
         return
@@ -323,24 +327,28 @@
 
     # Create the target directory
     project_dir = Path.cwd() / dashed_name
     project_dir.mkdir(parents=True, exist_ok=True)
 
     # If the project directory already exists it must be empty
     if any(project_dir.iterdir()):
-        fatal(f"The project directory `{project_dir}` already exists and is not empty")
+        fatal(
+            f"The project directory `{project_dir}` already exists and is not empty"
+        )
 
     # Generate /rio.toml
     with open(project_dir / "rio.toml", "w") as f:
         f.write("# This is the configuration file for Rio,\n")
         f.write("# an easy to use app & web framework for Python.\n")
         f.write("\n")
         f.write(f"[app]\n")
         f.write(f'app_type = "{type}"  # This is either "website" or "app"\n')
-        f.write(f'main_module = "{module_name}"  # The name of your Python module\n')
+        f.write(
+            f'main_module = "{module_name}"  # The name of your Python module\n'
+        )
 
     # Create the main module and its subdirectories
     main_module_dir = project_dir / module_name
     assets_dir = main_module_dir / "assets"
     components_dir = main_module_dir / "components"
     pages_dir = main_module_dir / "pages"
 
@@ -430,22 +438,22 @@
 # Run the app
 {module_name}.app.run_in_window()
 """
             )
 
     # Report success
     #
-    # TODO: Add a command to install dependencies? Activate the venv?
+    # TODO: Other tools like poetry!? Add a command to activate the venv?
     print()
     success(f"The project has been created!")
     success(f"You can find it at `{project_dir.resolve()}`")
     print()
     print(f"To see your new project in action, run the following commands:")
     print()
     print(f"[dim]>[/] cd {revel.shell_escape(project_dir.resolve())}")
 
     if template.dependencies:
         print(
             f"[dim]>[/] python -m pip install -r requirements.txt  [bold]# Don't forget to install dependencies![/]"
-        )  # TODO: Figure out the correct python command?
+        )
 
     print(f"[dim]>[/] rio run")
```

### Comparing `rio_ui-0.5.9/src/rio/cli/rio_api.py` & `rio_ui-0.6/rio/cli/rio_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         if file is not None:
             files = {"file": file}
         else:
             files = None
 
         # Make the request
         #
-        # TODO: Which exception can this throw?
+        # TODO: Which exceptions can this throw?
         response = await self._http_client.request(
             method,
             f"{BASE_URL}/{endpoint}",
             headers=headers,
             json=json,
             files=files,
         )
```

### Comparing `rio_ui-0.5.9/src/rio/cli/rioignore.py` & `rio_ui-0.6/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/cli/tomlconfig.py` & `rio_ui-0.6/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/cli/run_project/app_loading.py` & `rio_ui-0.6/rio/cli/run_project/app_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     project_directory: Path,
     theme: rio.Theme | Tuple[rio.Theme, rio.Theme],
 ) -> rio.App:
     """
     Creates an app that displays the given error message.
     """
     return rio.App(
-        build=functools.partial(make_error_message_component, err, project_directory),
+        build=functools.partial(
+            make_error_message_component, err, project_directory
+        ),
         theme=theme,
     )
 
 
 def import_app_module(proj: project.RioProject) -> types.ModuleType:
     """
     Python's importing is bizarre. This function tries to hide all of that and
@@ -154,15 +156,17 @@
 
     if len(apps) == 0:
         raise AppLoadError(
             f"Cannot find your app. {main_file_reference} needs to to define a variable that is a Rio app. Something like `app = rio.App(...)`"
         )
 
     if len(apps) > 1:
-        variables_string = "`" + "`, `".join(var_name for var_name, _ in apps) + "`"
+        variables_string = (
+            "`" + "`, `".join(var_name for var_name, _ in apps) + "`"
+        )
         raise AppLoadError(
             f"{main_file_reference} defines multiple Rio apps: {variables_string}. Please make sure there is exactly one."
         )
 
     app = apps[0][1]
 
     # Explicitly set the asset directory because it can't reliably be
```

### Comparing `rio_ui-0.5.9/src/rio/cli/run_project/arbiter.py` & `rio_ui-0.6/rio/cli/run_project/arbiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,26 +80,28 @@
         self.run_in_window = run_in_window
 
         # Workers communicate with the `RunningApp` by pushing events into this
         # queue.
         self._event_queue: asyncio.Queue[run_models.Event] = asyncio.Queue()
 
         # If running, contains the various workers
-        self._file_watcher_worker: file_watcher_worker.FileWatcherWorker | None = None
+        self._file_watcher_worker: (
+            file_watcher_worker.FileWatcherWorker | None
+        ) = None
         self._uvicorn_worker: uvicorn_worker.UvicornWorker | None = None
         self._webview_worker: webview_worker.WebViewWorker | None = None
 
         self._file_watcher_task: asyncio.Task[None] | None = None
         self._uvicorn_task: asyncio.Task[None] | None = None
         self._arbiter_task: asyncio.Task[None] | None = None
 
         # The app to use for creating apps. This keeps the theme consistent if
         # for-example the user's app crashes and then a mock-app is injected.
         self._app_theme: Union[rio.Theme, tuple[rio.Theme, rio.Theme]] = (
-            rio.Theme.pair_from_color()
+            rio.Theme.pair_from_colors()
         )
 
         # Prefer to consistently run on the same port, as that makes it easier
         # to connect to - this way old browser tabs don't get invalidated
         # constantly.
         if port is None:
             if common.port_is_free(self._host, 8000):
@@ -122,15 +124,17 @@
         # The mainloop used by the arbiter. This is set once asyncio is running.
         self._mainloop: asyncio.AbstractEventLoop | None = None
 
     def push_event(self, event: run_models.Event) -> None:
         """
         Pushes an event into the event queue. Threadsafe.
         """
-        assert self._mainloop is not None, "Can't push events before asyncio is running"
+        assert (
+            self._mainloop is not None
+        ), "Can't push events before asyncio is running"
         rio.cli._logger.debug(f"Pushing arbiter event `{event}`")
         self._mainloop.call_soon_threadsafe(self._event_queue.put_nowait, event)
 
     @property
     def _host(self) -> str:
         return "0.0.0.0" if self.public else "127.0.0.1"
 
@@ -147,15 +151,19 @@
         else:
             local_ip = "127.0.0.1"
 
         return f"http://{local_ip}:{self.port}"
 
     @property
     def running_tasks(self) -> Iterator[asyncio.Task[None]]:
-        for task in (self._uvicorn_task, self._file_watcher_task, self._arbiter_task):
+        for task in (
+            self._uvicorn_task,
+            self._file_watcher_task,
+            self._arbiter_task,
+        ):
             if task is not None:
                 yield task
 
     def stop(self, *, keyboard_interrupt: bool) -> None:
         """
         Stops the app. This function can safely be called more than once, and at
         any point in time.
@@ -188,15 +196,17 @@
             for task in self.running_tasks:
                 task.cancel()
 
         self._mainloop.call_soon_threadsafe(cancel_all_tasks)
 
         # Stop the webview
         if self._webview_worker is not None:
-            rio.cli._logger.debug("Stopping the webview because the app is stopping")
+            rio.cli._logger.debug(
+                "Stopping the webview because the app is stopping"
+            )
             self._webview_worker.request_stop()
 
     def try_load_app(self) -> tuple[rio.App, Exception | None]:
         """
         Tries to load the user's app. If it fails, a dummy app is created and
         returned, unless running in release mode.
 
@@ -234,15 +244,17 @@
     def run(self) -> None:
         assert not self._stop_requested.is_set()
         assert not self._server_is_ready.is_set()
 
         # Handle keyboard interrupts. KeyboardInterrupt exceptions are very
         # annoying to handle in async code, so instead we'll use a signal
         # handler.
-        signal.signal(signal.SIGINT, lambda *_: self.stop(keyboard_interrupt=True))
+        signal.signal(
+            signal.SIGINT, lambda *_: self.stop(keyboard_interrupt=True)
+        )
 
         # Do as much work as possible in asyncio land
         asyncio_thread = threading.Thread(
             target=lambda: asyncio.run(
                 self._run_async(),
             ),
             name="arbiter function of rio run",
@@ -290,15 +302,17 @@
 
                 if self._stop_requested.is_set():
                     break
 
         # Make sure the main thread stays alive until the asyncio thread is
         # done. Otherwise we get weird errors like "Can't start thread during
         # interpreter shutdown" from asyncio.
-        rio.cli._logger.debug("The arbiter is waiting for the asyncio thread to finish")
+        rio.cli._logger.debug(
+            "The arbiter is waiting for the asyncio thread to finish"
+        )
         asyncio_thread.join()
 
         rio.cli._logger.debug("Arbiter shutdown complete")
 
     async def _run_async(self) -> None:
         # Publish the task, so it can be cancelled
         self._arbiter_task = asyncio.current_task()
@@ -395,25 +409,29 @@
                 apply_monkeypatches()
 
             # Try to load the app
             app, _ = self.try_load_app()
 
             # Start the file watcher
             if self.debug_mode:
-                self._file_watcher_worker = file_watcher_worker.FileWatcherWorker(
-                    push_event=self.push_event,
-                    proj=self.proj,
+                self._file_watcher_worker = (
+                    file_watcher_worker.FileWatcherWorker(
+                        push_event=self.push_event,
+                        proj=self.proj,
+                    )
                 )
                 self._file_watcher_task = asyncio.create_task(
                     self._file_watcher_worker.run(),
                     name="File watcher",
                 )
 
             # Start the uvicorn worker
-            uvicorn_is_ready_or_has_failed: asyncio.Future[None] = asyncio.Future()
+            uvicorn_is_ready_or_has_failed: asyncio.Future[None] = (
+                asyncio.Future()
+            )
 
             self._uvicorn_worker = uvicorn_worker.UvicornWorker(
                 push_event=self.push_event,
                 app=app,
                 socket=sock,
                 quiet=self.quiet,
                 debug_mode=self.debug_mode,
@@ -427,15 +445,17 @@
             )
 
             # Wait for the server to be ready or fails to start
             rio.cli._logger.debug("Waiting for uvicorn to be ready or to fail")
             await uvicorn_is_ready_or_has_failed
 
             # Let everyone else know that the server is ready
-            rio.cli._logger.debug("App startup complete and ready for connections")
+            rio.cli._logger.debug(
+                "App startup complete and ready for connections"
+            )
             self._server_is_ready.set()
 
             # The app has just successfully started. Inform the user
             if self.debug_mode:
                 revel.warning("Debug mode is enabled.")
                 revel.warning(
                     "Debug mode includes helpful tools for development, but is slower and disables some safety checks. Never use it in production!"
@@ -443,16 +463,20 @@
                 revel.warning("Run with `--release` to disable debug mode.")
                 print()
 
             if self.public:
                 revel.warning(
                     f"Running in public mode. All devices on your network can access the app."
                 )
-                revel.warning(f"Only run in public mode if you trust your network!")
-                revel.warning(f"Run without `--public` to limit access to this device.")
+                revel.warning(
+                    f"Only run in public mode if you trust your network!"
+                )
+                revel.warning(
+                    f"Run without `--public` to limit access to this device."
+                )
                 print()
             elif not self.run_in_window:
                 print(
                     f"[dim]Running in [/]local[dim] mode. Only this device can access the app.[/]"
                 )
 
             if not self.run_in_window:
@@ -514,15 +538,17 @@
         rio.cli._logger.debug("Spawning traceback popups")
 
         popup_html = app_loading.make_traceback_html(
             err=err,
             project_directory=self.proj.project_directory,
         )
 
-        for session in self._uvicorn_worker.app_server._active_session_tokens.values():
+        for (
+            session
+        ) in self._uvicorn_worker.app_server._active_session_tokens.values():
             self._evaluate_javascript_in_session_if_connected(
                 session,
                 f"""
 // Override the popup with the traceback message
 let popup = document.querySelector(".rio-connection-lost-popup");
 popup.innerHTML = {json.dumps(popup_html)};
```

### Comparing `rio_ui-0.5.9/src/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.6/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.6/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/cli/run_project/webview_worker.py` & `rio_ui-0.6/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/components/__init__.py` & `rio_ui-0.6/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/components/app_root.py` & `rio_ui-0.6/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/components/auto_form.py` & `rio_ui-0.6/rio/components/auto_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 @dataclass
 class AutoFormChangeEvent:
     field_name: str
     value: Any
 
 
 class AutoForm(component.Component):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     # TODO
     value: Any
     _: KW_ONLY
     on_change: rio.EventHandler[[AutoFormChangeEvent]] = None
 
     def __post_init__(self) -> None:
         # Make sure the passed value is a dataclass
@@ -103,15 +109,17 @@
             return rio.Dropdown(
                 mapping,
                 selected_value=value,
                 on_change=lambda e: self._update_value(field_name, e.value),
             )
 
         # Unsupported type
-        raise TypeError(f"AutoForm does not support fields of type `{field_type}`")
+        raise TypeError(
+            f"AutoForm does not support fields of type `{field_type}`"
+        )
 
     def build(self) -> rio.Component:
         grid = rio.Grid(
             row_spacing=0.5,
             column_spacing=1,
         )
 
@@ -119,15 +127,17 @@
         for ii, field in enumerate(dataclasses.fields(self.value)):
             field_py_name = field.name
             field_type = field.type
             field_nicename = prettify_name(field_py_name)
 
             # Skip fields that are not supported
             try:
-                input_component = self._build_input_field(field_py_name, field_type)
+                input_component = self._build_input_field(
+                    field_py_name, field_type
+                )
             except TypeError:
                 continue
 
             # Add a label
             grid.add(
                 rio.Text(text=field_nicename, align_x=0),
                 ii,
```

### Comparing `rio_ui-0.5.9/src/rio/components/banner.py` & `rio_ui-0.6/rio/components/banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     "Banner",
 ]
 
 
 @final
 class Banner(component.Component):
     r"""
-    # Banner
-
     Displays a short message to the user.
 
     Banners can either show a short text message to the users, or disappear
     entirely if no message is set. Use them to inform the user about the result
     of an action, to give feedback on their input, or anything else that needs
     to be communicated.
 
@@ -28,30 +26,30 @@
     levels control the appearance of the notification bar, and allow you to
     quickly communicate the nature of the message to the user.
 
 
     ## Attributes
 
     `text`: The text to display. If `None` or empty, the banner will disappear
-            entirely.
+        entirely.
 
     `style`: Controls the appearance of the banner. The style is one of
-            `info`, `success`, `warning` and `danger`. Depending on the value
-            the banner may change its colors and icon.
+        `info`, `success`, `warning` and `danger`. Depending on the value the
+        banner may change its colors and icon.
 
     `markup`: Whether the text should be interpreted as Markdown. If `True`, the
-            text will be rendered as Markdown, otherwise it will be rendered as
-            plain text.
+        text will be rendered as Markdown, otherwise it will be rendered as
+        plain text.
 
     `multiline`: Whether long text may be wrapped over multiple lines.
-            Multiline banners are also styled slightly differently to make the
-            icon fit their larger size. Use `"\n"` to add a line break.
+        Multiline banners are also styled slightly differently to make the icon
+        fit their larger size. Use `"\n"` to add a line break.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a banner with the text "This is a
     banner":
 
     ```python
     rio.Banner(text="This is a banner", style="info")
     ```
@@ -85,14 +83,15 @@
 
     text: str | None
     style: Literal["info", "success", "warning", "danger"]
 
     _: KW_ONLY
     markup: bool = False
     multiline: bool = False
+    icon: str | None = None
 
     def build(self) -> rio.Component:
         # Early out: Nothing to show
         if self.text is None:
             return rio.Spacer(width=0, height=0)
 
         text = self.text.strip()
@@ -111,14 +110,17 @@
             icon = "material/warning"
         elif self.style == "danger":
             style_name = "danger"
             icon = "material/error"
         else:
             raise ValueError(f"Invalid style: {self.style}")
 
+        if self.icon is not None:
+            icon = self.icon
+
         # Prepare the text child
         if self.markup:
             text_child = rio.Markdown(
                 text,
                 width="grow",
             )
         else:
```

### Comparing `rio_ui-0.5.9/src/rio/components/build_failed.py` & `rio_ui-0.6/rio/components/build_failed.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["BuildFailed"]
 
 
 class BuildFailed(FundamentalComponent):
     """
-    Used as a placeholder in case a component's `build` function throws an error.
+    Used as a placeholder in case a component's `build` function throws an
+    error.
+
+
+    ## Metadata
+
+    public: False
     """
 
     error_summary: str
     error_details: str
 
     # Debug details can contain sensitive information. Sending these to the
     # client is fine during development, but mustn't happen in production.
```

### Comparing `rio_ui-0.5.9/src/rio/components/button.py` & `rio_ui-0.6/rio/components/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,116 +19,95 @@
 CHILD_MARGIN_Y = 0.3
 INITIALLY_DISABLED_FOR = 0.25
 
 
 @final
 class Button(Component):
     """
-    # Button
-
     A clickable button.
 
     The `Button` component allows the user to trigger an action by clicking on
     it. You can use it to trigger a function call, navigate to a different page,
     or perform other actions.
 
+
     ## Attributes
 
     `content`: The text or child component to display inside of the button.
 
     `icon`: The name of an icon to display on the button, in the form
         "set/name:variant". See the `Icon` component for details of how
         icons work in Rio.
 
     `shape`: The shape of the button. This can be one of:
-        - `pill`: A rectangle where the left and right sides are completely round.
-        - `rounded`: A rectangle with rounded corners.
-        - `rectangle`: A rectangle with sharp corners.
+
+        - `"pill"`: A rectangle where the left and right sides are completely
+            round.
+        - `"rounded"`: A rectangle with rounded corners.
+        - `"rectangle"`: A rectangle with sharp corners.
 
     `style`: Controls the button's appearance. This can be one of:
-        - `major`: A highly visible button with bold visuals.
-        - `minor`: A less visible button that blends into the background.
-        - `plain`: A button with no background or border. Use this to make
-                the button look like a link.
+
+        - `"major"`: A highly visible button with bold visuals.
+        - `"minor"`: A less visible button that blends into the background.
+        - `"plain"`: A button with no background or border. Use this to make the
+            button look like a link.
 
     `color`: The color scheme to use for the button.
 
     `is_sensitive`: Whether the button should respond to user input.
 
     `is_loading`: Whether the button should display a loading indicator. Use
         this to indicate to the user that an action is currently running.
 
     `initially_disabled_for`: The number of seconds the button should be
         disabled for after it is first rendered. This is useful to prevent
-        the user from accidentally triggering an action when the page is
-        first loaded.
+        the user from accidentally pressing a button that suddenly appeared.
 
     `on_press`: Triggered when the user clicks on the button.
 
 
-    ## Example
+    ## Examples
 
-    This minimal example will simply display a `Button` with the text "Click
-    me!" and a castle icon:
+    This code creates a button with the caption "Click me!":
 
     ```python
-    rio.Button(content="Click me!", icon="material/castle")
+    rio.Button(
+        "Click me!",
+        on_press=lambda: print("Button pressed!"),
+    )
     ```
 
-    `Button`s are commonly used to trigger actions. You can easily achieve this
-    by adding a lambda function call to `on_press`:
+    You can make it a little fancier by adding an icon:
 
     ```python
-    class MyComponent(rio.Component):
-        def build(self) -> rio.Component:
-            return rio.Button(
-                content="Click me!",
-                on_press=lambda: print("Button pressed!"),
-            )
+    rio.Button(
+        "Click me!",
+        icon="material/mouse",
+        on_press=lambda: print("Button pressed!"),
+    )
     ```
 
-    If you want to do more than e.g. just print a message, you can use a method
-    call instead of a lambda function:
+    You can even put other components inside of the button. Here's a button with
+    a progress bar that slowly fills up as you click it:
 
     ```python
-    class MyComponent(rio.Component):
-        def on_press_button(self) -> None:
-            # You can do whatever you want here, like printing
-            print("Button pressed!")
+    class ProgressButton(rio.Component):
+        clicks: int = 0
 
-        def build(self) -> rio.Component:
-            return rio.Button(
-                content="Click me!",
-                on_press=self.on_press_button,
-            )
-    ```
-
-    `Button`s are commonly used to trigger actions. You can easily achieve this
-    by adding a function call to on_press. You can use a function call to update
-    the banner text signaling that the button was pressed:
-
-    ```python
-    class MyComponent(rio.Component):
-        banner_text: str = ""
-
-        def on_press_button(self) -> None:
-            self.banner_text = "Button pressed!"
-            # Do whatever you want here
+        def _on_button_press(self) -> None:
+            self.clicks += 1
 
         def build(self) -> rio.Component:
-            return rio.Column(
-                rio.Banner(
-                    text=self.banner_text,
-                    style="info",
-                ),
-                rio.Button(
-                    content="Click me!",
-                    on_press=self.on_press_button,
+            return rio.Button(
+                rio.Column(
+                    rio.Text("Click repeatedly to fill up the progress bar"),
+                    rio.ProgressBar(self.clicks/10, width=15, height=1),
                 ),
-                spacing=1,
+                on_press=self._on_button_press,
             )
     ```
     """
 
     content: str | rio.Component = ""
     _: KW_ONLY
     icon: str | None = None
@@ -242,22 +221,23 @@
     It is similar to the `Button` component, but it is specifically designed to
     display an icon, and it has a round shape.
 
 
     ## Attributes
 
     `icon`: The name of an icon to display on the button, in the form
-            "set/name:variant". See the `Icon` component for details of how
+            `"set/name:variant"`. See the `Icon` component for details of how
             icons work in Rio.
 
     `style`: Controls the button's appearance. This can be one of:
-    - `major`: A highly visible button with bold visuals.
-    - `minor`: A less visible button that blends into the background.
-    - `plain`: A button with no background or border. Use this to make
-                       the button look like a link.
+
+        - `major`: A highly visible button with bold visuals.
+        - `minor`: A less visible button that blends into the background.
+        - `plain`: A button with no background or border. Use this to make
+                        the button look like a link.
 
     `color`: The color scheme to use for the button.
 
     `is_sensitive`: Whether the button should respond to user input.
 
     `initially_disabled_for`: The number of seconds the button should be
             disabled for after it is first rendered. This is useful to prevent
@@ -266,15 +246,15 @@
 
     `size`: The size of the button. This is the diameter of the button in
             font-size units.
 
     `on_press`: Triggered when the user clicks on the button.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a `IconButton` with a castle icon:
 
     ```python
     rio.IconButton(icon="material/castle")
     ```
 
@@ -390,16 +370,16 @@
             height=self.size,
             initially_disabled_for=self.initially_disabled_for,
             # Make sure the button has a square aspect ratio
             align_x=0.5,
             align_y=0.5,
         )
 
-    def get_debug_details(self) -> dict[str, Any]:
-        result = super().get_debug_details()
+    def _get_debug_details(self) -> dict[str, Any]:
+        result = super()._get_debug_details()
 
         # `width` & `height` are replaced with `size`
         del result["width"]
         del result["height"]
 
         return result
```

### Comparing `rio_ui-0.5.9/src/rio/components/card.py` & `rio_ui-0.6/rio/components/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     "Card",
 ]
 
 
 @final
 class Card(FundamentalComponent):
     """
-    # Card
-
     A container that visually encompasses its child components.
 
     Cards are used to group related components together, and to visually
     separate them from other components, allowing you to display them in a
     structured way.
 
     Cards are also often used as large buttons. They can be configured to
@@ -31,35 +29,39 @@
 
 
     ## Attributes
 
     `content`: The component to display inside the card.
 
     `corner_radius`: The radius of the card's corners. If set to `None`, it
-            is picked from the active theme.
+        is picked from the active theme.
 
     `on_press`: An event handler that is called when the card is clicked.
-            Note that attaching an even handler will also modify the appearance
-            of the card, to signal the possible interaction to the user. See
-            `elevate_on_hover` and `colorize_on_hover` for details.
+        Note that attaching an even handler will also modify the appearance
+        of the card, to signal the possible interaction to the user. See
+        `elevate_on_hover` and `colorize_on_hover` for details.
+
+    `ripple`: Whether the card should display a ripple effect when clicked.
+        If set to `None` the card will ripple if an `on_press` event handler is
+        attached.
 
     `elevate_on_hover`: Whether the card should elevate slightly when the
-            mouse hovers over it. If set to `None` the card will elevate if
-            an `on_press` event handler is attached.
+        mouse hovers over it. If set to `None` the card will elevate if
+        an `on_press` event handler is attached.
 
     `colorize_on_hover`: Whether the card should change its color when the
-            mouse hovers over it. If set to `None` the card will change its
-            color if an `on_press` event handler is attached.
+        mouse hovers over it. If set to `None` the card will change its
+        color if an `on_press` event handler is attached.
 
     `color`: The color scheme to use for the card. The color scheme controls
-            the background color of the card, and the color of the text and
-            icons inside it. Check `rio.Color` for details.
+        the background color of the card, and the color of the text and
+        icons inside it. Check `rio.Color` for details.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a `Card` with the castle icon
     in it:
 
     ```python
     rio.Card(content=rio.Icon("material/castle"))
     ```
@@ -116,14 +118,15 @@
     ```
     """
 
     content: rio.Component
     _: KW_ONLY
     corner_radius: float | tuple[float, float, float, float] | None = None
     on_press: rio.EventHandler[[]] = None
+    ripple: bool | None = None
     elevate_on_hover: bool | None = None
     colorize_on_hover: bool | None = None
     color: rio.ColorSet = "neutral"
 
     async def _on_message(self, msg: Any) -> None:
         # Trigger the press event
         await self.call_event_handler(self.on_press)
@@ -140,16 +143,19 @@
         return {
             "corner_radius": (
                 thm.corner_radius_medium
                 if self.corner_radius is None
                 else self.corner_radius
             ),
             "reportPress": report_press,
+            "ripple": report_press if self.ripple is None else self.ripple,
             "elevate_on_hover": (
-                report_press if self.elevate_on_hover is None else self.elevate_on_hover
+                report_press
+                if self.elevate_on_hover is None
+                else self.elevate_on_hover
             ),
             "colorize_on_hover": (
                 report_press
                 if self.colorize_on_hover is None
                 else self.colorize_on_hover
             ),
             "color": color,
```

### Comparing `rio_ui-0.5.9/src/rio/components/class_container.py` & `rio_ui-0.6/rio/components/class_container.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,34 @@
 __all__ = [
     "ClassContainer",
 ]
 
 
 class ClassContainer(FundamentalComponent):
     """
-    # ClassContainer
-
     A Component which holds a single child.
 
     Component which holds a single child, and applies a list of CSS classes to
     it. This is enough to implement several components, preventing the need to
     create a whole bunch of almost identical JavaScript components.
 
     This component is only intended for internal use and is not part of the
     public API.
 
+
     ## Attributes
 
     `content`: The child component to apply the classes to.
 
     `classes`: The list of classes to apply to the child component.
     """
 
     content: rio.Component | None
     classes: list[str]
 
-    def get_debug_details(self) -> dict[str, Any]:
-        result = super().get_debug_details()
+    def _get_debug_details(self) -> dict[str, Any]:
+        result = super()._get_debug_details()
         result.pop("classes")
         return result
 
 
 ClassContainer._unique_id = "ClassContainer-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/color_picker.py` & `rio_ui-0.6/rio/components/color_picker.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,99 +14,78 @@
     "ColorChangeEvent",
 ]
 
 
 @final
 @dataclass
 class ColorChangeEvent:
+    """
+    The argument for the `on_change` handler of a `ColorPicker`.
+
+    ## Attributes
+
+    `color`: The new `color` of the `ColorPicker`.
+    """
+
     color: rio.Color
 
 
 @final
 class ColorPicker(FundamentalComponent):
     """
-    # ColorPicker
-
     Allows the user to pick a RGB(A) color.
 
-    `ColorPicker` is a component that allows the user to pick a color. It
+    `ColorPicker` is a component that allows the user to input a color. It
     displays a combination of colorful areas and sliders that the user can
     interact with to pick a color, and optionally an opacity slider to pick
     opacity.
 
 
     ## Attributes
 
     `color`: The color that the user has picked.
 
     `pick_opacity`: Whether to allow the user to pick opacity. If `False`,
-            the opacity slider will be hidden and the color value will be forced
-            to be fully opaque.
+        the opacity slider will be hidden and the color value will be forced
+        to be fully opaque.
 
     `on_change`: This event is triggered whenever the user changes the color.
 
 
-    ## Example
-
-    This minimal example will simply display a `ColorPicker` with the default
-    color red:
-
-    ```python
-    rio.ColorPicker(rio.Color.from_hex("#ff0000"))
-    ```
+    ## Examples
 
-    `ColorPicker`s are commonly used to let the user select a color. You can
-    easily achieve this by using state bindings to save the color in a variable
-    and using it in your application:
+    This small example will print a message whenever the user changes the
+    selected color:
 
     ```python
-    class MyComponent(rio.Component):
-        color: rio.Color = rio.Color.from_hex("#ff0000")
+    def print_selected_color(event: rio.ColorChangeEvent):
+        print('You selected the color', event.color)
 
-        def build(self) -> rio.Component:
-            return rio.ColorPicker(
-                color=self.bind().color,
-                pick_opacity=True,
-            )
-    ```
-
-    If you want to make your `ColorPicker` more interactive, you can easily
-    achieve this by adding a lambda function call to on_change:
-
-    ```python
-    class MyComponent(rio.Component):
-        color: rio.Color = rio.Color.from_hex("#ff0000")
-
-        def build(self) -> rio.Component:
-            return rio.ColorPicker(
-                color=self.bind().color,
-                pick_opacity=True,
-                on_change=lambda event: print(f"selected color: {event.color}"),
-            )
+    rio.ColorPicker(
+        rio.Color.from_hex("#ff0000"),
+        on_change=print_selected_color,
+    )
     ```
 
-    You can use an event handler to react to changes in the color. This example
-    will print the color to the console whenever the user changes it:
+    This one utilizes a attribute binding to use the selected color as the fill for
+    an `Icon`:
 
     ```python
-    class MyComponent(rio.Component):
-        color: rio.Color = rio.Color.from_rgb(0.5, 0.5, 0.5)
-
-        def on_change_color(self, event: rio.ColorChangeEvent) -> None:
-            # You can do whatever you want in this method
-            self.color = event.color
-            print(f"Selected color: {event.color}")
+    class ButtonColorizer(rio.Component):
+        color: rio.Color = rio.Color.BLUE
 
         def build(self) -> rio.Component:
-            return rio.Card(
+            return rio.Row(
                 rio.ColorPicker(
-                    color=self.color,
-                    pick_opacity=True,
-                    on_change=self.on_change_color,
+                    color=self.bind().color,
                 ),
+                rio.Icon(
+                    'material/star',
+                    fill=self.color,
+                )
             )
     ```
     """
 
     color: rio.Color
     _: KW_ONLY
     pick_opacity: bool = False
```

### Comparing `rio_ui-0.5.9/src/rio/components/component.py` & `rio_ui-0.6/rio/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing_extensions import Self, dataclass_transform
 from uniserde import Jsonable, JsonDoc
 
 import rio
 
 from .. import event, global_state, inspection
 from ..dataclass import RioDataclassMeta, class_local_fields, internal_field
-from ..state_properties import StateBindingMaker, StateProperty
+from ..state_properties import AttributeBindingMaker, StateProperty
 
 __all__ = ["Component"]
 
 
 T = TypeVar("T")
 
 
@@ -85,15 +85,17 @@
             inspect.Parameter.VAR_POSITIONAL,
             inspect.Parameter.VAR_KEYWORD,
         )
     )
     # fmt: on
 
     # Discard parameters that don't correspond to state properties
-    properties_set_by_creator.intersection_update(type(component)._state_properties_)
+    properties_set_by_creator.intersection_update(
+        type(component)._state_properties_
+    )
 
     return properties_set_by_creator
 
 
 C = typing.TypeVar("C", bound="Component")
 
 
@@ -108,15 +110,17 @@
     _state_properties_: dict[str, StateProperty]
 
     # Maps event tags to the methods that handle them. The methods aren't bound
     # to the instance yet, so make sure to pass `self` when calling them
     #
     # The assigned value is needed so that the `Component` class itself has a
     # valid value. All subclasses override this value in `__init_subclass__`.
-    _rio_event_handlers_: defaultdict[event.EventTag, list[tuple[Callable, Any]]]
+    _rio_event_handlers_: defaultdict[
+        event.EventTag, list[tuple[Callable, Any]]
+    ]
 
     # Whether this component class is built into Rio, rather than user defined,
     # or from a library.
     _rio_builtin_: bool
 
     def __init__(cls, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -272,16 +276,14 @@
 
 
 # Using `metaclass=ComponentMeta` makes this an abstract class, but since
 # pyright is too stupid to understand that, we have to additionally inherit from
 # `abc.ABC`
 class Component(abc.ABC, metaclass=ComponentMeta):
     """
-    # Component
-
     Base class for all `rio` components.
 
     Components are the building blocks of `rio` apps. `rio` ships with many
     useful components out of the box, but you can also subclass a component to
     create your own.
 
 
@@ -338,43 +340,43 @@
         both specified, `margin_bottom` is used for the bottom side, while
         the other sides use `margin`.
 
     `width`: How much horizontal space this component should request during
         layouting. This can be either a number, or one of the special
         values:
 
-    - If `"natural"`, the component will request the minimum amount it
-        requires to fit on the screen. For example a `Text` will request
-        however much space the characters of that text require. A `Row`
-        would request the sum of the widths of its children.
-
-    - If `"grow"`, the component will request all the remaining space in its parent.
-
-    - Please note that the space a `Component` receives during layouting
-        may not match the request. As a general rule, for example, containers
-        try to pass on all available space to children. If you really want a
-        `Component` to only take up as much space as requested, consider
-        specifying an alignment.
+        - If `"natural"`, the component will request the minimum amount it
+          requires to fit on the screen. For example a `Text` will request
+          however much space the characters of that text require. A `Row`
+          would request the sum of the widths of its children.
+
+        - If `"grow"`, the component will request all the remaining space in its parent.
+
+        - Please note that the space a `Component` receives during layouting
+          may not match the request. As a general rule, for example, containers
+          try to pass on all available space to children. If you really want a
+          `Component` to only take up as much space as requested, consider
+          specifying an alignment.
 
     `height`: How much vertical space this component should request during
         layouting. This can be either a number, or one of the special values:
 
-    - If `"natural"`, the component will request the minimum amount it
-        requires to fit on the screen. For example a `Text` will request
-        however much space the characters of that text require. A `Row`
-        would request the height of its tallest child.
-
-    - If `"grow"`, the component will request all the remaining space in its
-        parent.
-
-    - Please note that the space a `Component` receives during layouting
-        may not match the request. As a general rule for example, containers
-        try to pass on all available space to children. If you really want a
-        `Component` to only take up as much space as requested, consider
-        specifying an alignment.
+        - If `"natural"`, the component will request the minimum amount it
+          requires to fit on the screen. For example a `Text` will request
+          however much space the characters of that text require. A `Row`
+          would request the height of its tallest child.
+
+        - If `"grow"`, the component will request all the remaining space in its
+          parent.
+
+        - Please note that the space a `Component` receives during layouting
+          may not match the request. As a general rule for example, containers
+          try to pass on all available space to children. If you really want a
+          `Component` to only take up as much space as requested, consider
+          specifying an alignment.
 
     `align_x`: How this component should be aligned horizontally, if it
         receives more space than it requested. This can be a number between
         0 and 1, where 0 means left-aligned, 0.5 means centered, and 1 means
         right-aligned.
 
     `align_y`: How this component should be aligned vertically, if it receives
@@ -460,15 +462,15 @@
         Return the session this component is part of.
         """
         return self._session_
 
     # There isn't really a good type annotation for this... Self is the closest
     # thing
     def bind(self) -> Self:
-        return StateBindingMaker(self)  # type: ignore
+        return AttributeBindingMaker(self)  # type: ignore
 
     def _custom_serialize(self) -> JsonDoc:
         """
         Return any additional properties to be serialized, which cannot be
         deduced automatically from the type annotations.
         """
         return {}
@@ -549,15 +551,17 @@
         else:
             build_result = self.session._weak_component_data_by_component[
                 self
             ].build_result
             yield from build_result._iter_component_tree()
 
     async def _on_message(self, msg: Jsonable, /) -> None:
-        raise RuntimeError(f"{type(self).__name__} received unexpected message `{msg}`")
+        raise RuntimeError(
+            f"{type(self).__name__} received unexpected message `{msg}`"
+        )
 
     def _is_in_component_tree(self, cache: dict[rio.Component, bool]) -> bool:
         """
         Returns whether this component is directly or indirectly connected to the
         component tree of a session.
 
         This operation is fast, but has to walk up the component tree to make sure
@@ -585,15 +589,17 @@
             builder = self._weak_builder_()
             if builder is None:
                 result = False
 
             # Has the builder since created new build output, and this component
             # isn't part of it anymore?
             else:
-                parent_data = self.session._weak_component_data_by_component[builder]
+                parent_data = self.session._weak_component_data_by_component[
+                    builder
+                ]
                 result = (
                     parent_data.build_generation == self._build_generation_
                     and builder._is_in_component_tree(cache)
                 )
 
         # Cache the result and return
         cache[self] = result
@@ -620,16 +626,24 @@
     ) -> None:
         """
         Calls an even handler, awaiting it if necessary.
 
         Call an event handler, if one is present. Await it if necessary. Log and
         discard any exceptions. If `event_data` is present, it will be passed to
         the event handler.
+
+        ## Parameters
+
+        `handler`: The event handler (function) to call.
+
+        `event_data`: Arguments to pass to the event handler.
         """
-        await self.session._call_event_handler(handler, *event_data, refresh=False)
+        await self.session._call_event_handler(
+            handler, *event_data, refresh=False
+        )
 
     async def force_refresh(self) -> None:
         """
         Force a rebuild of this component.
 
         Most of the time components update automatically when their state
         changes. However, some state mutations are invisible to `Rio`: For
@@ -651,15 +665,15 @@
         self.session._register_dirty_component(
             self,
             include_children_recursively=False,
         )
 
         await self.session._refresh()
 
-    def get_debug_details(self) -> dict[str, Any]:
+    def _get_debug_details(self) -> dict[str, Any]:
         """
         Used by Rio's debugger to decide which properties to display to a user,
         when they select a component.
         """
         result = {}
 
         for prop in self._state_properties_:
```

### Comparing `rio_ui-0.5.9/src/rio/components/component_tree.py` & `rio_ui-0.6/rio/components/component_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,28 +11,34 @@
 
 
 class ComponentTree(FundamentalComponent):
     """
     Note: This component makes not attempt to request the correct amount of
     space. Specify a width/height manually, or make sure it's in a properly
     sized parent.
+
+    ## Metadata
+
+    public: False
     """
 
     _: KW_ONLY
 
     # Triggered whenever the user selects a component in the tree. The passed
     # value is the component's ID.
     on_select_component: rio.EventHandler[int] = None
 
     async def _on_message(self, msg: Any) -> None:
         # Parse the message
         assert isinstance(msg, dict), msg
         selected_component_id = msg["selectedComponentId"]
 
         # Trigger the press event
-        await self.call_event_handler(self.on_select_component, selected_component_id)
+        await self.call_event_handler(
+            self.on_select_component, selected_component_id
+        )
 
         # Refresh the session
         await self.session._refresh()
 
 
 ComponentTree._unique_id = "ComponentTree-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/container.py` & `rio_ui-0.6/rio/components/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,27 @@
     "Container",
 ]
 
 
 @final
 class Container(Component):
     """
-    # Container
-
     A component holding a single child.
 
     `Container` is a simple container which holds a single child component. It
     is useful for when you receive a component as child and wish to add
     additional layout attributes such as a margin.
 
 
     ## Attributes
 
     `content`: The component to place inside the container.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a `container` with the text "Hello
     World!":
 
     ```python
     rio.Container(rio.Text("Hello World!"))
     ```
```

### Comparing `rio_ui-0.5.9/src/rio/components/devel_component.py` & `rio_ui-0.6/rio/components/devel_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 _SOURCE_DIRECTORY: Path | None = None
 
 _CSS_SOURCE: str = ""
 _JS_SOURCE: str = ""
 
 
 class DevelComponent(FundamentalComponent):
-    # TODO
+    """
+    ## Metadata
+
+    public: False
+    """
+
     children: list[rio.Component] = field(default_factory=list)
 
     def __init__(
         self,
         *,
         children: Iterable[rio.Component],
         key: str | None = None,
@@ -90,16 +95,20 @@
         if not ts_path.exists():
             raise RuntimeError(
                 "Missing `script.ts` in `DevelComponent` source directory"
             )
 
         # Compile the two, in parallel
         print("DevelComponent: Compiling `DevelComponent` component source")
-        css_path = Path(tempfile.NamedTemporaryFile(suffix=".css", delete=False).name)
-        js_path = Path(tempfile.NamedTemporaryFile(suffix=".js", delete=False).name)
+        css_path = Path(
+            tempfile.NamedTemporaryFile(suffix=".css", delete=False).name
+        )
+        js_path = Path(
+            tempfile.NamedTemporaryFile(suffix=".js", delete=False).name
+        )
 
         tasks = [
             ("sass", str(scss_path), str(css_path)),
             ("tsc", str(ts_path), "--outFile", str(js_path)),
         ]
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
```

### Comparing `rio_ui-0.5.9/src/rio/components/drawer.py` & `rio_ui-0.6/rio/components/drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,28 @@
     "DrawerOpenOrCloseEvent",
 ]
 
 
 @final
 @dataclass
 class DrawerOpenOrCloseEvent:
+    """
+    The argument for the `on_open_or_close` handler of a `Drawer`.
+
+    ## Attributes
+
+    `is_open`: The new `is_open` state of the `Drawer`.
+    """
+
     is_open: bool
 
 
 @final
 class Drawer(FundamentalComponent):
     """
-    # Drawer
-
     A container which slides in from the edge of the screen.
 
     Drawers are containers which can either be completely hidden from view, or
     be made visible by sliding in from the edge of the screen. They are commonly
     used for navigation on smaller displays.
 
     Drawers take two children: The `anchor` is always visible and positions the
@@ -57,15 +63,15 @@
     `is_open`: Whether the drawer is currently open.
 
     `is_user_openable`: Whether the user can open or close the drawer. If this
         is `False`, the drawer can only be opened or closed
         programmatically.
 
 
-    ## Example
+    ## Examples
 
     A simple drawer with a button as the anchor and some text as content:
 
     ```python
     rio.Drawer(
         anchor=rio.Button("Click Me!"),
         content=rio.Text("It was clickbait!"),
@@ -113,15 +119,17 @@
             )
 
         if "is_open" in delta_state and not self.is_user_openable:
             raise AssertionError(
                 "Frontend tried to change value of `Drawer.is_open` even though `is_user_openable` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_open_or_close event
         try:
             is_open = delta_state["is_open"]
         except KeyError:
             pass
         else:
             assert isinstance(is_open, bool), (is_open, type(is_open))
```

### Comparing `rio_ui-0.5.9/src/rio/components/dropdown.py` & `rio_ui-0.6/rio/components/dropdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,69 +17,76 @@
 
 T = TypeVar("T")
 
 
 @final
 @dataclass
 class DropdownChangeEvent(Generic[T]):
+    """
+    The argument for the `on_change` handler of a `Dropdown`.
+
+    ## Attributes
+
+    `value`: The new `selected_value` of the `Dropdown`.
+    """
+
     value: T
 
 
 @final
 class Dropdown(FundamentalComponent, Generic[T]):
     """
-    # Dropdown
-
     A dropdown menu allowing the user to select one of several options.
 
     Dropdowns present the user with a list of options, allowing them to select
     exactly one. In their default state dropdowns are compact and display the
     currently selected option. When activated, a popup menu appears with a list
     of all available options.
 
 
     ## Attributes
 
     `options`: A mapping from option names to values. The names are displayed
-            in the dropdown menu, and the corresponding value is returned when
-            the user selects the option. The values must be comparable.
+        in the dropdown menu, and the corresponding value is returned when
+        the user selects the option. The values must be comparable.
 
     `label`: A short text to display next to the dropdown.
 
     `selected_value`: The value of the currently selected option.
 
     `is_sensitive`: Whether the dropdown should respond to user input.
 
     `is_valid`: Visually displays to the user whether the current option is
         valid. You can use this to signal to the user that their input needs
         to be changed.
 
     `on_change`: Triggered whenever the user selects an option.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a dropdown with three options:
 
     ```python
     rio.Dropdown(["a", "b", "c"])
     ```
 
-    In a `Component` class, you can use state bindings to keep your input value
-    updated and track any changes. Here's a quick example with a `Dropdown`:
+    In a `Component` class, you can use attribute bindings to keep your input
+    value updated and track any changes. Here's a quick example with a
+    `Dropdown`:
 
     ```python
     class MyComponent(rio.Component):
         value: str = "b"
 
         def build(self) -> rio.Component:
             return rio.Dropdown(
                 options=["a", "b", "c"],
                 label="Dropdown",
-                selected_value=self.bind().value,  # State binding
+                selected_value=self.bind().value,  # Attribute binding
                 on_change=lambda event: print(event.value),
             )
     ```
 
     If you want to do more than e.g. just print a message, you can use a method
     call instead of a lambda function:
 
@@ -157,28 +164,28 @@
         self.options = options
         self.label = label
         self.on_change = on_change
         self.is_sensitive = is_sensitive
         self.is_valid = is_valid
 
         # This is an unsafe assignment, because the value could be `None`. This
-        # will be fixed in `__post_init__`, once the state bindings have been
+        # will be fixed in `__post_init__`, once the attribute bindings have been
         # initialized.
         self.selected_value = selected_value  # type: ignore
 
     def __post_init__(self) -> None:
         # Make sure a value is selected
         if self.selected_value is None:
             self.selected_value = next(iter(self.options.values()))
 
     def _fetch_selected_name(self) -> str:
         # The frontend works with names, not values. Get the corresponding
         # name.
 
-        # Avoid hammering a potential state binding
+        # Avoid hammering a potential attribute binding
         selected_value = self.selected_value
 
         # Fetch the name
         for name, value in self.options.items():
             if value == selected_value:
                 return name
         else:
@@ -202,15 +209,17 @@
         try:
             selected_value = self.options[msg["name"]]
         except KeyError:
             # Invalid names may be sent due to lag between the frontend and
             # backend. Ignore them.
             return
 
-        self._apply_delta_state_from_frontend({"selected_value": selected_value})
+        self._apply_delta_state_from_frontend(
+            {"selected_value": selected_value}
+        )
 
         # Trigger the event
         await self.call_event_handler(
             self.on_change, DropdownChangeEvent(self.selected_value)
         )
 
         # Refresh the session
```

### Comparing `rio_ui-0.5.9/src/rio/components/flow_container.py` & `rio_ui-0.6/rio/components/flow_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 __all__ = ["FlowContainer"]
 
 
 @final
 class FlowContainer(FundamentalComponent):
     """
-    # FlowContainer
-
     A container that lays out its children in a horizontal or vertical flow.
 
     `FlowContainer` is a container that lays out its children in a horizontal or
     vertical flow. It is similar to `Container`, but allows you to specify
     spacing between the children.
 
 
@@ -32,15 +30,15 @@
 
     `column_spacing`: The horizontal spacing between the children.
 
     `justify`: The horizontal alignment of the children. Possible values are:
         `left`, `center`, `right`, `justified` and `grow`.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will show a container with a horizontal flow:
 
     ```python
     rio.FlowContainer(
         rio.Text("Hello"),
         rio.Text("World!"),
@@ -56,15 +54,17 @@
     justify: Literal["left", "center", "right", "justified", "grow"]
 
     def __init__(
         self,
         *children: rio.Component,
         row_spacing: float = 0.0,
         column_spacing: float = 0.0,
-        justify: Literal["left", "center", "right", "justified", "grow"] = "center",
+        justify: Literal[
+            "left", "center", "right", "justified", "grow"
+        ] = "center",
         key: str | None = None,
         margin: float | None = None,
         margin_x: float | None = None,
         margin_y: float | None = None,
         margin_left: float | None = None,
         margin_top: float | None = None,
         margin_right: float | None = None,
@@ -95,13 +95,25 @@
         self.column_spacing = column_spacing
         self.row_spacing = row_spacing
         self.justify = justify
 
     def add(self, child: rio.Component) -> Self:
         """
         Appends a child component.
+
+        Appends a child component to the end and then returns the
+        `FlowContainer`, which makes method chaining possible:
+
+        ```python
+        rio.FlowContainer().add(child1).add(child2)
+        ```
+
+
+        ## Parameters
+
+        `child`: The child component to append.
         """
         self.children.append(child)
         return self
 
 
 FlowContainer._unique_id = "FlowContainer-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/fundamental_component.py` & `rio_ui-0.6/rio/components/fundamental_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,17 @@
         if javascript_source:
             message_source += JAVASCRIPT_SOURCE_TEMPLATE % {
                 "js_source": javascript_source,
                 "js_user_class_name": cls.__name__,
                 "js_wrapper_class_name": f"{cls.__name__}Wrapper",
                 "cls_unique_id": cls._unique_id,
                 "child_attribute_names": json.dumps(
-                    inspection.get_child_component_containing_attribute_names(cls)
+                    inspection.get_child_component_containing_attribute_names(
+                        cls
+                    )
                 ),
             }
 
         css_source = cls.build_css_source(sess)
         if css_source:
             escaped_css_source = json.dumps(css_source)
             message_source += CSS_SOURCE_TEMPLATE % {
@@ -140,18 +142,22 @@
         the frontend is valid. If the frontend tries to change the state in a
         way that isn't allowed, this function should throw an error.
         """
         raise AssertionError(
             f"Frontend tried to change the state of a `{type(self).__name__}`"
         )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         pass
 
-    def _apply_delta_state_from_frontend(self, delta_state: dict[str, Any]) -> None:
+    def _apply_delta_state_from_frontend(
+        self, delta_state: dict[str, Any]
+    ) -> None:
         """
         Applies the delta state received from the frontend without marking the
         component as dirty.
         """
         # Since the new state is coming from JS, we know two things:
         # 1. There's no need to send the state back to JS
         # 2. There's no need to re-build this component, since it's a
@@ -164,9 +170,15 @@
             setattr(self, attr_name, attr_value)
 
         if not was_already_dirty:
             self.session._dirty_components.discard(self)
 
 
 class KeyboardFocusableFundamentalComponent(FundamentalComponent):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     async def grab_keyboard_focus(self) -> None:
         await self.session._remote_set_keyboard_focus(self._id)
```

### Comparing `rio_ui-0.5.9/src/rio/components/grid.py` & `rio_ui-0.6/rio/components/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,29 @@
     width: int = 1
     height: int = 1
 
 
 @final
 class Grid(FundamentalComponent):
     """
-    # Grid
-
     A container which arranges its children in a table-like grid.
 
     Grids arrange their children in a table-like grid. Each child is placed in
     one or more cells of the grid. You can add children to the grid either by
     passing them in as a list or by using the `grid_add` method.
 
 
     ## Attributes
 
     `row_spacing`: The amount of space between rows of the grid.
 
     `column_spacing`: The amount of space between columns of the grid.
 
 
-    ## Example
+    ## Examples
 
     This code creates a grid layout with two rows and two columns, and adds
     children to the grid by passing them in as a list:
 
     ```python
     rio.Grid(
         [rio.Text("Hello"), rio.Text("World!")],  # 1. Row
@@ -128,15 +126,17 @@
         self.row_spacing = row_spacing
         self.column_spacing = column_spacing
 
         # JS can only work with lists of Components, so we'll store the
         # components and their positions separately
         self._children, self._child_positions = self._add_initial_children(rows)
 
-        self._properties_set_by_creator_.update(["_children", "_child_positions"])
+        self._properties_set_by_creator_.update(
+            ["_children", "_child_positions"]
+        )
 
     def _add_initial_children(
         self,
         children: Iterable[rio.Component | Iterable[rio.Component]],
     ) -> tuple[list[rio.Component], list[GridChildPosition]]:
         """
         Adds the children added in the constructor to the component. This is
@@ -186,44 +186,53 @@
         child: rio.Component,
         row: int,
         column: int,
         *,
         width: int = 1,
         height: int = 1,
     ) -> Self:
-        assert isinstance(child, rio.Component), child
         """
         Add a child to the grid at a specified position.
 
-        Args:
-            child: The child component to add to the grid.
+        Appends a child component to the end and then returns the
+        `Grid`, which makes method chaining possible.
 
-            row: The row in which to place the child.
 
-            column: The column in which to place the child.
+        ## Parameters
 
-            width: The number of columns the child should take up.
+        `child`: The child component to add to the grid.
 
-            height: The number of rows the child should take up.
+        `row`: The row in which to place the child.
 
+        `column`: The column in which to place the child.
 
-        Example:
-            ```python
-            grid = rio.Grid(row_spacing=1, column_spacing=1)
-            grid.add_child(rio.Text("Hello"), row=0, column=0)
-            ```
+        `width`: The number of columns the child should take up.
+
+        `height`: The number of rows the child should take up.
+
+
+        ## Example
+
+        ```python
+        grid = rio.Grid(row_spacing=1, column_spacing=1)
+        grid.add_child(rio.Text("Hello"), row=0, column=0)
+        ```
         """
+        assert isinstance(child, rio.Component), child
+
         if width <= 0:
             raise ValueError("Children have to take up at least one column")
 
         if height <= 0:
             raise ValueError("Children have to take up at least one row")
 
         self._children.append(child)
-        self._child_positions.append(GridChildPosition(row, column, width, height))
+        self._child_positions.append(
+            GridChildPosition(row, column, width, height)
+        )
 
         # Return self for chaining
         return self
 
     def _custom_serialize(self) -> JsonDoc:
         return {
             "_children": [child._id for child in self._children],
```

### Comparing `rio_ui-0.5.9/src/rio/components/icon.py` & `rio_ui-0.6/rio/components/icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     "Icon",
 ]
 
 
 @final
 class Icon(FundamentalComponent):
     """
-    # Icon
-
     Displays one of many pre-bundled icons.
 
     Icons are a great way to add polish to your app. A good icon can help your
     users understand your app and immediately recognize what a component does.
 
     Rio includes hundreds of free icons, allowing you to easily add them to your
     app without having to find or create your own. The `Icon` component displays
@@ -52,25 +50,24 @@
         `icon-set/name:variant`. You can browse all available icons in Rio's
         debugger sidebar.
 
     `fill`: The color scheme of the icon. The text color is used if no fill is
         specified.
 
 
-    ## Example
+    ## Examples
 
-    This minimal example will simply display an Icon:
+    This minimal example will display the icon named "castle" from the
+    "material" icon set:
 
     ```python
     rio.Icon("material/castle")
     ```
 
-    You can also specify the fill, width and height of the icon. This example
-    will display a simple `Icon` named "castle" from the `material` icon set,
-    filled in red color and of size 2.5 x 2.5:
+    You can also specify the color, width and height of the icon:
 
     ```python
     rio.Icon(
         "material/castle",
         fill=rio.Color.from_hex("ff0000"),
         height=2.5,
         width=2.5,
@@ -109,15 +106,15 @@
         - They must have a `viewBox` attribute, but no height or width
         - They must contain exactly one XML root node: `<svg>...</svg>`. This
           also goes for comments!
         - Rio colors paths by assigning a `fill` to the SVG root. This only
           works as long as the SVG paths don't have a `<style>` assigned
           already.
 
-        Args:
+        ## Parameters
             set_name: The name of the new icon set. This will be used to access
                 the icons.
 
             icon_set_archive_path: The path to the `.tar.xz` archive containing
             the icon
                 set.
         """
@@ -146,30 +143,29 @@
         - They must have a `viewBox` attribute, but no height or width
         - They must contain exactly one XML root node: `<svg>...</svg>`. This
           also goes for comments!
         - Rio colors paths by assigning a `fill` to the SVG root. This only
           works as long as the SVG paths don't have a `<style>` assigned
           already.
 
-        Args:
+        ## Parameters
             icon_source: The path to the SVG file containing the icon.
 
             set_name: The name of the new icon set. This will be used to access
                 the icons.
 
             icon_name: The name of the icon. This will be used to access the
                 icon.
 
             variant_name: The name of the variant. This will be used to access
                 the icon. If not specified, the default variant will be used.
         """
 
         # Try to load the icon
-        with open(icon_source) as f:
-            svg_source = f.read()
+        svg_source = icon_source.read_text(encoding="utf8")
 
         # Add it to the icon registry's cache
         if variant_name is None:
             name = f"{set_name}/{icon_name}"
         else:
             name = f"{set_name}/{icon_name}:{variant_name}"
 
@@ -225,15 +221,17 @@
         # Serialize the fill. This isn't automatically handled because it's a
         # Union.
         if isinstance(self.fill, fills.Fill):
             fill = self.fill._serialize(self.session)
         elif isinstance(self.fill, color.Color):
             fill = self.fill.rgba
         else:
-            assert isinstance(self.fill, str), f"Unsupported fill type: {self.fill}"
+            assert isinstance(
+                self.fill, str
+            ), f"Unsupported fill type: {self.fill}"
             fill = self.fill
 
         # Serialize
         return {
             "svgSource": svg_source,
             "fill": fill,
         }
```

### Comparing `rio_ui-0.5.9/src/rio/components/image.py` & `rio_ui-0.6/rio/components/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
 from typing import Literal, final
 
-from uniserde import JsonDoc
+from uniserde import Jsonable, JsonDoc
 
 from .. import assets
 from ..common import EventHandler, ImageLike
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["Image"]
 
 
 @final
 class Image(FundamentalComponent):
     """
-    # Image
-
-    Displays an image file.
+    Displays a raster image or SVG.
 
     `Image` does just what you'd expect: it displays a single image. The image
     can be loaded from a URL or a local file.
 
-    `Note` that the resolution of the image does not affect the size at which it
+    Note that the resolution of the image does not affect the size at which it
     is displayed. The `Image` component is flexible with its space requirements,
     it adapts to the space allocated by its parent component.
 
     The image can be scaled to fit the shape in one of three ways:
 
     - `fit`: The image is scaled to fit entirely inside the shape, while
       maintaining its aspect ratio. This is the default.
@@ -37,48 +35,46 @@
 
 
     ## Attributes
 
     `image`: The image to display.
 
     `fill_mode`: How the image should be scaled to fit the shape. If `fit`,
-            the image is scaled to fit entirely inside the shape. If `stretch`,
-            the image is stretched to fill the shape exactly, possibly
-            distorting it in the process. If `zoom`, the image is scaled to fill
-            the shape entirely, possibly overflowing.
+        the image is scaled to fit entirely inside the shape. If `stretch`,
+        the image is stretched to fill the shape exactly, possibly
+        distorting it in the process. If `zoom`, the image is scaled to fill
+        the shape entirely, possibly overflowing.
 
-    `on_error`: Triggered when the image fails to load.
+    `on_error`: A function, triggered if the image fails to load.
 
     `corner_radius`: How round to make the corners of the image. If a single
-            number is given, all four corners will be rounded equally. If a
-            tuple of four numbers is given, they will be interpreted as the
-            radii of the top-left, top-right, bottom-right, and bottom-left
-            corners, in that order.
+        number is given, all four corners will be rounded equally. If a
+        tuple of four numbers is given, they will be interpreted as the
+        radii of the top-left, top-right, bottom-right, and bottom-left
+        corners, in that order.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display an image with the URL
     "https://example.com/image.png":
 
     ```python
     rio.Image(rio.URL("https://example.com/image.png"))
-    ````
+    ```
 
     This example demonstrates how to display an `Image` using a Path object.
     The image will be scaled to fit the shape, and the corners will be rounded
     with a radius of 2:
 
     ```python
     from pathlib import Path
 
-    PATH = Path(__file__).parent
-
     rio.Image(
-        PATH / "example_image.png",
+        Path("example_image.png"),
         fill_mode="fit",
         width=20,
         height=20,
         corner_radius=2,
     )
     ```
     """
@@ -106,12 +102,12 @@
 
         return {
             "imageUrl": self._get_image_asset()._serialize(self.session),
             "reportError": self.on_error is not None,
             "corner_radius": corner_radius,
         }
 
-    async def _on_message(self, message: JsonDoc) -> None:
+    async def _on_message(self, message: Jsonable) -> None:
         await self.call_event_handler(self.on_error)
 
 
 Image._unique_id = "Image-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/key_event_listener.py` & `rio_ui-0.6/rio/components/key_event_listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -565,14 +565,32 @@
 ModifierKey = Literal["alt", "control", "meta", "shift"]
 
 _MODIFIERS = ("control", "shift", "alt", "meta")
 
 
 @dataclass(frozen=True)
 class _KeyUpDownEvent:
+    """
+    ## Attributes
+
+    `hardware_key`: The name of the physical button on the keyboard.
+
+    `software_key`: The name of the button. Depending on the user's keyboard
+        layout, this may differ from the `hardware_key`. (For example, if the
+        physical keyboard has a QWERTY layout but the OS is configured to use
+        Dvorak.)
+
+    `text`: The text that pressing this button produces. For example, Shift+1
+        produces the text "!". If the button doesn't produce any text, like F1
+        for example, this will be an empty string.
+
+    `modifiers`: The names of the modifier keys (control, shift, alt, meta) that
+        were pressed when the event occurred.
+    """
+
     hardware_key: HardwareKey
     software_key: SoftwareKey | str
     text: str
     modifiers: frozenset[ModifierKey]
 
     @classmethod
     def _from_json(cls, json_data: dict[str, Any]):
@@ -588,47 +606,55 @@
         keys.append(self.software_key)
 
         return " + ".join(keys)
 
 
 @final
 class KeyDownEvent(_KeyUpDownEvent):
-    pass
+    """
+    The argument for the `on_key_down` handler of a `KeyEventListener`.
+    """
 
 
 @final
 class KeyUpEvent(_KeyUpDownEvent):
-    pass
+    """
+    The argument for the `on_key_up` handler of a `KeyEventListener`.
+    """
 
 
 @final
 class KeyPressEvent(_KeyUpDownEvent):
-    pass
+    """
+    The argument for the `on_key_press` handler of a `KeyEventListener`.
+    """
 
 
 @final
 class KeyEventListener(KeyboardFocusableFundamentalComponent):
     """
     Calls an event handler when a key is pressed or released.
 
     `KeyEventListener` is a container for a single child component. It listens
     for keyboard events and calls corresponding event handlers when they occur.
 
     Keep in mind that `KeyEventListener` will only report events that have not
     been handled by a child component. For example, typing into a `TextInput`
     will not trigger a `KeyEventListener`.
 
+
     ## Attributes
-        content: The child component.
 
-        on_key_down: A function to call when a key is pressed down.
+    `content`: The child component.
 
-        on_key_up: A function to call when a key is released.
+    `on_key_down`: A function to call when a key is pressed down.
 
-        on_key_press: A function to call repeatedly while a key is held down.
+    `on_key_up`: A function to call when a key is released.
+
+    `on_key_press`: A function to call repeatedly while a key is held down.
     """
 
     content: rio.Component
     _: KW_ONLY
     on_key_down: rio.EventHandler[KeyDownEvent] = None
     on_key_up: rio.EventHandler[KeyUpEvent] = None
     on_key_press: rio.EventHandler[KeyPressEvent] = None
@@ -663,14 +689,16 @@
         elif msg_type == "KeyPress":
             await self.call_event_handler(
                 self.on_key_press,
                 KeyPressEvent._from_json(msg),
             )
 
         else:
-            raise ValueError(f"{__class__.__name__} encountered unknown message: {msg}")
+            raise ValueError(
+                f"{__class__.__name__} encountered unknown message: {msg}"
+            )
 
         # Refresh the session
         await self.session._refresh()
 
 
 KeyEventListener._unique_id = "KeyEventListener-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/labeled_column.py` & `rio_ui-0.6/rio/components/labeled_column.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,41 +12,38 @@
 
 __all__ = ["LabeledColumn"]
 
 
 @final
 class LabeledColumn(Component):
     """
-    # LabeledColumn
-
     A container that lays out its children in a column, with labels for each child.
 
     `LabeledColumn` is a container that lays out its children in a column, with
     labels for each child. It is similar to `Column`, but allows you to specify
     labels for each child.
 
 
-    ## Attributes
-
-    `content`: The components to place inside the container, with labels.
-
-
     ## Example
 
     This minimal example will show a container with a column layout and labels:
 
     ```python
     rio.LabeledColumn(
         {
             "First Name": rio.TextInput(),
             "Last Name": rio.TextInput(),
             "Age": rio.TextInput(),
         }
     )
     ```
+
+    ## Metadata
+
+    public: False
     """
 
     _child_list: list[Component] = field(init=False)
 
     def __init__(
         self,
         content: Mapping[str, rio.Component],
@@ -89,14 +86,17 @@
     def content(self, children: Mapping[str, Component]) -> None:
         self._content = dict(children)
         self._child_list = list(children.values())
 
     def add(self, label: str, child: rio.Component) -> Self:
         """
         Appends a child component.
+
+        Appends a child component to the end and then returns the
+        `LabeledColumn`, which makes method chaining possible.
         """
         self._content[label] = child
         self._child_list.append(child)
 
         return self
 
     def build(self) -> Component:
```

### Comparing `rio_ui-0.5.9/src/rio/components/linear_containers.py` & `rio_ui-0.6/rio/components/linear_containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,24 @@
     proportions: Literal["homogeneous"] | Sequence[float] | None = None
 
     # Don't let @dataclass generate a constructor
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def add(self, child: rio.Component) -> Self:
-        """
-        Appends a child component.
-        """
         self.children.append(child)
         return self
 
     def _custom_serialize(self) -> JsonDoc:
         return {"proportions": self.proportions}  # type: ignore[variance]
 
 
 @final
 class Row(_LinearContainer):
     """
-    # Row
-
     A container that lays out its children horizontally.
 
     `Row`s are one of the most common components in Rio. They take any number of
     children and lay them out horizontally, with the first one on the left, the
     second one to its right, and so on. All components in `Row`s occupy the full
     height of their parent.
 
@@ -77,35 +72,36 @@
             spacing is added before the first child or after the last child.
 
     `proportions`: If set, the children will grow according to these proportions.
         - `homogeneous`: All children will grow equally.
         - A list of floats: Each child will grow according to its proportion.
         - `None`: Allows all child components to expand as much as they need.
 
-    ## Example
+    ## Examples
 
     This minimal example will display a `Row` with two text components:
 
     ```python
     rio.Row(rio.Text("Hello"), rio.Text("World!"))
     ```
 
-    `Row`s are commonly used to line up multiple components horizontally. In this example, we're
-    using an Icon and two Text components in a Row and wrap them in a Card.
+    `Row`s are commonly used to line up multiple components horizontally. In
+    this example, we're using an Icon and two Text components in a Row and wrap
+    them in a Card.
 
     ```python
     class MyComponent(rio.Component):
         def build(self) -> rio.Component:
             return rio.Card(
                 content=rio.Row(
                     rio.Icon(icon="material/castle"),
                     rio.Text("Hello"),
                     rio.Text("World!"),
                     spacing=1,
-                    # align card content in the center
+                    # Align card content in the center
                     # to avoid undefined space
                     align_x=0.5,
                 ),
             )
     ```
     """
 
@@ -142,23 +138,38 @@
             align_y=align_y,
         )
 
         self.children = list(children)
         self.spacing = spacing
         self.proportions = proportions
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+
+        Appends a child component to the end and then returns the `Row`, which
+        makes method chaining possible:
+
+        ```python
+        rio.Row().add(child1).add(child2)
+        ```
+
+        ## Parameters
+
+        `child`: The child component to append.
+        """
+        return super().add(child)
+
 
 Row._unique_id = "Row-builtin"
 
 
 @final
 class Column(_LinearContainer):
     """
-    # Column
-
     A container that lays out its children vertically.
 
     `Column`s are one of the most common components in Rio. They take any number
     of children and lay them out vertically, with the first one at the top, the
     second one below that, and so on. All components in `Column`s occupy the
     full width of their parent.
 
@@ -186,23 +197,23 @@
 
 
     ## Attributes
 
     `children`: The components to place in this `Column`.
 
     `spacing`: How much empty space to leave between two adjacent children. No
-            spacing is added before the first child or after the last child.
+        spacing is added before the first child or after the last child.
 
     `proportions`: If set, the children will grow according to these proportions.
         - `homogeneous`: All children will grow equally.
         - A list of floats: Each child will grow according to its proportion.
         - `None`: Allows all child components to expand as much as they need.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will display a `Column` with two text components:
 
     ```python
     rio.Column(rio.Text("Hello"), rio.Text("World!"))
     ```
 
@@ -216,15 +227,15 @@
             return rio.Card(
                 content=rio.Column(
                     rio.Icon("material/castle"),
                     rio.Text("Hello"),
                     rio.Text("World!"),
                     spacing=1,
                     # Align card content in the center to avoid undefined space
-                    align_x=0.5,
+                    align_y=0.5,
                 ),
             )
     ```
     """
 
     def __init__(
         self,
@@ -259,9 +270,26 @@
             align_y=align_y,
         )
 
         self.children = list(children)
         self.spacing = spacing
         self.proportions = proportions
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+
+        Appends a child component to the end and then returns the `Column`,
+        which makes method chaining possible:
+
+        ```python
+        rio.Column().add(child1).add(child2)
+        ```
+
+        ## Parameters
+
+        `child`: The child component to append.
+        """
+        return super().add(child)
+
 
 Column._unique_id = "Column-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/link.py` & `rio_ui-0.6/rio/components/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,32 @@
     "Link",
 ]
 
 
 @final
 class Link(FundamentalComponent):
     """
-    # Link
-
     Navigates to a page or URL when clicked.
 
     `Link`s display a short text, or arbitrary component, and navigate to a page
     or URL when clicked.
 
 
     ## Attributes
 
-
     `child_text`: The text to display inside the link.
 
     `child_component`: The component to display inside the link.
 
     `target_url`: The page or URL to navigate to when clicked.
 
     `open_in_new_tab`: Whether to open the link in a new tab. Defaults to `False`.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display a link with the URL
     "https://example.com" and a text "Click me!":
 
     ```python
     rio.Link("Click me!", "https://example.com")
     ```
@@ -72,15 +69,15 @@
         margin_bottom: float | None = None,
         width: float | Literal["natural", "grow"] = "natural",
         height: float | Literal["natural", "grow"] = "natural",
         align_x: float | None = None,
         align_y: float | None = None,
     ):
         """
-        Args:
+        ## Parameters
             content: The text or component to display inside the link.
 
             target_url: The page or URL to navigate to when clicked.
         """
         super().__init__(
             key=key,
             margin=margin,
@@ -102,15 +99,17 @@
         else:
             self.child_text = None
             self.child_component = content
 
         self.target_url = target_url
         self.open_in_new_tab = open_in_new_tab
 
-        self._properties_set_by_creator_.update(("child_text", "child_component"))
+        self._properties_set_by_creator_.update(
+            ("child_text", "child_component")
+        )
 
     async def _on_message(self, msg: Any) -> None:
         assert isinstance(msg, dict), msg
 
         if "page" in msg:
             # Navigate to the link. Note that this allows the client to inject
             # a, possibly malicious, link. This is fine, because the client can
```

### Comparing `rio_ui-0.5.9/src/rio/components/list_items.py` & `rio_ui-0.6/rio/components/list_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,28 @@
     "CustomListItem",
 ]
 
 
 @final
 class HeadingListItem(FundamentalComponent):
     """
-    # HeadingListItem
-
     A simple list item with only a header.
 
     `HeadingListItem`s are the easiest way to create list items, which can take
     care of the most primitive task: Display a text. If your want a more generic
     list item with additional children, you can use the `SimpleListItem`. Or if
     you want to build a more complex list item, you can use the
     `CustomListItem`.
 
     ## Attributes
 
-    `text`: The text to display.
+    `text`: The text to display
 
-    ## Example
+
+    ## Examples
 
     This minimal example will simply display a list item with the text "Click
     me!":
 
     ```python
     rio.HeadingListItem("Click me!", key="item1")
     ```
@@ -81,37 +80,37 @@
 
 SeparatorListItem._unique_id = "SeparatorListItem-builtin"
 
 
 @final
 class SimpleListItem(Component):
     """
-    # SimpleListItem
-
     A simple list item with a header and optional secondary text and children.
 
     `SimpleListItem`s are a convenient way to create list items, which can
     take care of the most common tasks: Display a text, optional secondary text
     and even additional children (e.g. icons or buttons) to the left and right.
     Most children are optional so you can only add whichever parts you need.
 
+
     ## Attributes
 
     `text`: The text to display.
 
     `secondary_text`: Additional text to display below the primary text. This
         text may span multiple lines (use `"\\n"` to add a line break).
 
     `left_child`: A component to display on the left side of the list item.
 
     `right_child`: A component to display on the right side of the list item.
 
     `on_press`: Triggered when the list item is pressed.
 
-    ## Example
+
+    ## Examples
 
     This minimal example will simply display a list item with the text "Click
     me!":
 
     ```python
     rio.SimpleListItem("Click me!", key="item1")
     ```
@@ -233,35 +232,34 @@
             key="",
         )
 
 
 @final
 class CustomListItem(FundamentalComponent):
     """
-    # CustomListItem
-
     A list item with custom content.
 
     Most of the time the `SimpleListItem` will do the job. With
     `CustomListItems` you can build more complex list items. You can add any
     component to the list item. This can be e.g. a `Row`, `Column`, `Text`,
     `Icon`, `Image` or any other component.
 
+
     ## Attributes
 
     `content`: The content to display.
 
     `on_press`: Triggered when the list item is pressed.
 
     `key`: A unique key to identify the list item. This is used to avoid
         unintentional reconciliation with other items when the list is
         updated.
 
 
-    ## Example
+    ## Examples
 
     Instead of using the `SimpleListItem` you can use the `CustomListItem` to create
     a custom list item. This can be useful if you want to add more complex content
     to the list item. You can add any component to the list item.
 
     ```python
     class MyCustomListItemComponent(rio.Component):
```

### Comparing `rio_ui-0.5.9/src/rio/components/list_view.py` & `rio_ui-0.6/rio/components/list_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 __all__ = ["ListView"]
 
 
 @final
 class ListView(FundamentalComponent):
     """
-    # ListView
-
     Vertically arranges and styles its children.
 
     A container which arranges its children in a vertical list. It is similar to `Column`,
     but it is optimized for displaying large numbers of items.
 
+
     ## Attributes
 
     `children`: The children to display in the list.
 
     `key`: A unique key for this component. If the key changes, the component will be
             destroyed and recreated. This is useful for components which maintain state
             across rebuilds.
 
-    ## Example
+
+    ## Examples
 
     A minimal example of a `ListView` with two items will be shown:
 
     ```python
     rio.ListView(
         rio.SimpleListItem("Product 1", key="item1"),
         rio.SimpleListItem("Product 2", key="item2"),
@@ -110,13 +110,24 @@
         )
 
         self.children = list(children)
 
     def add(self, child: rio.Component) -> Self:
         """
         Appends a child component.
+
+        Appends a child component to the end and then returns the `ListView`,
+        which makes method chaining possible:
+
+        ```python
+        rio.ListView().add(child1).add(child2)
+        ```
+
+        ## Parameters
+
+        `child`: The child component to append.
         """
         self.children.append(child)
         return self
 
 
 ListView._unique_id = "ListView-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/markdown.py` & `rio_ui-0.6/rio/components/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
     "Markdown",
 ]
 
 
 @final
 class Markdown(FundamentalComponent):
     """
-    # Markdown
-
     Displays Markdown-formatted text.
 
     `Markdown` displays text formatted using markdown. Markdown is a
     lightweight markup language that allows you to write text with simple
     formatting, such as **bold**, *italics*, and links.
 
     Markdown is a great way to write text that is both human-readable, yet
@@ -33,15 +31,15 @@
         specify a language explicitly.
 
         Inline code will always use the default language, since they are too
         short to reliably guess the language - so make sure to set a default
         language if you want your inline code to be syntax-highlighted.
 
 
-    ## Example
+    ## Examples
 
     This minimal example will simply display the bold text "Hello World!":
 
     ```python
     rio.Markdown("**Hello World!**")
     ```
     """
```

### Comparing `rio_ui-0.5.9/src/rio/components/media_player.py` & `rio_ui-0.6/rio/components/media_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,71 +13,69 @@
 
 __all__ = ["MediaPlayer"]
 
 
 @final
 class MediaPlayer(KeyboardFocusableFundamentalComponent):
     """
-    # MediaPlayer
-
     Plays audio and video.
 
     `MediaPlayer` plays back audio and video files. It can play local files and
     URLs.
 
     Note that the `MediaPlayer` component doesn't reserve any space for itself,
     it simply makes do with the space it is given by its parent component.
 
 
     ## Attributes
+
     `media`: The media to play. This can be a file path, URL, or bytes.
 
-    `media_type`: The mime type of the media file. May help the browser to
-            play the file correctly.
+    `media_type`: The mime type of the media file. May help the browser play the
+        file correctly.
 
     `loop`: Whether to automatically restart from the beginning when the
-            playback ends.
+        playback ends.
 
     `autoplay`: Whether to start playing the media automatically, without
-            requiring the user to press "Play".
+        requiring the user to press "Play".
 
     `controls`: Whether to display controls like a Play/Pause button, volume
-            slider, etc.
+        slider, etc.
 
     `muted`: Whether to mute the audio.
 
     `volume`: The volume to play the audio at. 1.0 is the native volume;
-            larger numbers increase the volume, smaller numbers decrease it.
+        larger numbers increase the volume, smaller numbers decrease it.
+
+    `background`: The background fill. This is visible when playing audio or
+        when the video doesn't use up all the available space.
 
     `on_playback_end`: An event handler to call when the media finishes
-            playing.
+        playing.
 
     `on_error`: An event handler to call when an error occurs, for example if
-            the file format isn't supported.
+        the file format isn't supported.
 
 
-    ## Example
+    ## Examples
 
-    A minimal example of a `MediaPlayer` playing a local file will be shown:
+    A minimal example of a `MediaPlayer` playing a media file from the internet:
 
     ```python
     rio.MediaPlayer(rio.URL("https://example.com/example_video.mp4"))
     ```
 
     You can use a local file as well:
 
     ```python
     from pathlib import Path
 
-    PATH = Path(__file__).parent
-
-    rio.MediaPlayer(PATH / "example_video.mp4")
+    rio.MediaPlayer(Path("example_video.mp4"))
     ```
-
-
     """
 
     media: pathlib.Path | rio.URL | bytes
     media_type: str | None
     loop: bool
     autoplay: bool
     controls: bool
@@ -149,15 +147,15 @@
 
     def _validate_delta_state_from_frontend(self, delta_state: JsonDoc) -> None:
         if not set(delta_state) <= {"muted", "volume"}:
             raise AssertionError(
                 f"Frontend tried to change `{type(self).__name__}` state: {delta_state}"
             )
 
-    async def _on_message(self, message: JsonDoc) -> None:
+    async def _on_message(self, message: JsonDoc) -> None:  # type: ignore
         if message["type"] == "playbackEnd":
             await self.call_event_handler(self.on_playback_end)
         elif message["type"] == "error":
             await self.call_event_handler(self.on_error)
         else:
             await super()._on_message(message)
```

### Comparing `rio_ui-0.5.9/src/rio/components/mouse_event_listener.py` & `rio_ui-0.6/rio/components/mouse_event_listener.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,108 +29,163 @@
 class MouseButton(enum.Enum):
     LEFT = "left"
     MIDDLE = "middle"
     RIGHT = "right"
 
 
 @dataclass
-class _MouseUpDownEvent:
+class _ButtonEvent:
     button: MouseButton
+
+
+@dataclass
+class _PositionedEvent:
+    """
+    ## Attributes
+
+    `x`: The x coordinate of the mouse when the event was triggered, relative to
+        the left side of the window.
+
+    `y`: The y coordinate of the mouse when the event was triggered, relative to
+        the top of the window. (So a larger `y` means further down.)
+    """
+
     x: float
     y: float
 
 
 @final
-class PressEvent(_MouseUpDownEvent):
-    pass
+@dataclass
+class PressEvent(_ButtonEvent, _PositionedEvent):
+    """
+    The argument for the `on_press` handler of a `MouseEventListener`.
 
+    ## Attributes
 
-@final
-class MouseDownEvent(_MouseUpDownEvent):
-    pass
+    `button`: The mouse button that was pressed.
+    """
 
 
 @final
-class MouseUpEvent(_MouseUpDownEvent):
-    pass
+@dataclass
+class MouseDownEvent(_ButtonEvent, _PositionedEvent):
+    """
+    The argument for the `on_mouse_down` handler of a `MouseEventListener`.
 
+    ## Attributes
 
+    `button`: The mouse button that was pressed.
+    """
+
+
+@final
 @dataclass
-class _MousePositionedEvent:
-    x: float
-    y: float
+class MouseUpEvent(_ButtonEvent, _PositionedEvent):
+    """
+    The argument for the `on_mouse_up` handler of a `MouseEventListener`.
+
+    ## Attributes
+
+    `button`: The mouse button that was released.
+    """
 
 
 @final
-class MouseMoveEvent(_MousePositionedEvent):
-    pass
+class MouseMoveEvent(_PositionedEvent):
+    """
+    The argument for the `on_mouse_move` handler of a `MouseEventListener`.
+    """
 
 
 @final
-class MouseEnterEvent(_MousePositionedEvent):
-    pass
+class MouseEnterEvent(_PositionedEvent):
+    """
+    The argument for the `on_mouse_enter` handler of a `MouseEventListener`.
+    """
 
 
 @final
-class MouseLeaveEvent(_MousePositionedEvent):
-    pass
+class MouseLeaveEvent(_PositionedEvent):
+    """
+    The argument for the `on_mouse_leave` handler of a `MouseEventListener`.
+    """
 
 
 @dataclass
-class _DragEvent:
-    button: MouseButton
-    x: float
-    y: float
+class _DragEvent(_ButtonEvent, _PositionedEvent):
+    """
+    ## Attributes
+
+    `component`: The component located under the mouse cursor when the event
+        happened.
+    """
+
     component: rio.Component
 
 
 @final
 class DragStartEvent(_DragEvent):
-    pass
+    """
+    The argument for the `on_drag_start` handler of a `MouseEventListener`.
+    """
 
 
 @final
 class DragMoveEvent(_DragEvent):
-    pass
+    """
+    The argument for the `on_drag_move` handler of a `MouseEventListener`.
+    """
 
 
 @final
 class DragEndEvent(_DragEvent):
-    pass
+    """
+    The argument for the `on_drag_end` handler of a `MouseEventListener`.
+    """
 
 
 @final
 class MouseEventListener(FundamentalComponent):
     """
     Allows you to listen for mouse events on a component.
 
     `MouseEventListeners` take a single child component and display it. They
     then listen for any mouse activity on the child component and report it
     through their event handlers.
 
+
     ## Attributes
-        content: The child component to display.
 
-        on_press: Similar to `on_mouse_up`, but performs additional subtle
-            checks, such as that the left mouse button was pressed.
+    `content`: The child component to display.
+
+    `on_press`: Similar to `on_mouse_up`, but performs additional subtle
+        checks, such as that the left mouse button was pressed.
+
+    `on_mouse_down`: Triggered when a mouse button is pressed down while
+        the mouse is placed over the child component.
 
-        on_mouse_down: Triggered when a mouse button is pressed down while
-            the mouse is placed over the child component.
+    `on_mouse_up`: Triggered when a mouse button is released while the
+        mouse is placed over the child component.
 
-        on_mouse_up: Triggered when a mouse button is released while the
-            mouse is placed over the child component.
+    `on_mouse_move`: Triggered when the mouse is moved while located over
+        the child component.
 
-        on_mouse_move: Triggered when the mouse is moved while located over
-            the child component.
+    `on_mouse_enter`: Triggered when the mouse previously was not located
+        over the child component, but now is.
 
-        on_mouse_enter: Triggered when the mouse previously was not located
-            over the child component, but now is.
+    `on_mouse_leave`: Triggered when the mouse previously was located over
+        the child component, but now is not.
 
-        on_mouse_leave: Triggered when the mouse previously was located over
-            the child component, but now is not.
+    `on_drag_start`: Triggered when the user starts dragging the mouse, i.e.
+        moving it while holding down a mouse button.
+
+    `on_drag_move`: Triggered when the user moves the mouse while holding down a
+        mouse button.
+
+    `on_drag_end`: Triggered then the user stops dragging the mouse.
     """
 
     content: rio.Component
     _: KW_ONLY
     on_press: rio.EventHandler[PressEvent] = None
     on_mouse_down: rio.EventHandler[MouseDownEvent] = None
     on_mouse_up: rio.EventHandler[MouseUpEvent] = None
@@ -222,41 +277,49 @@
         elif msg_type == "dragStart":
             await self.call_event_handler(
                 self.on_drag_start,
                 DragStartEvent(
                     button=msg["button"],
                     x=msg["x"],
                     y=msg["y"],
-                    component=self.session._weak_components_by_id[msg["component"]],
+                    component=self.session._weak_components_by_id[
+                        msg["component"]
+                    ],
                 ),
             )
 
         elif msg_type == "dragMove":
             await self.call_event_handler(
                 self.on_drag_move,
                 DragMoveEvent(
                     button=msg["button"],
                     x=msg["x"],
                     y=msg["y"],
-                    component=self.session._weak_components_by_id[msg["component"]],
+                    component=self.session._weak_components_by_id[
+                        msg["component"]
+                    ],
                 ),
             )
 
         elif msg_type == "dragEnd":
             await self.call_event_handler(
                 self.on_drag_end,
                 DragEndEvent(
                     button=msg["button"],
                     x=msg["x"],
                     y=msg["y"],
-                    component=self.session._weak_components_by_id[msg["component"]],
+                    component=self.session._weak_components_by_id[
+                        msg["component"]
+                    ],
                 ),
             )
 
         else:
-            raise ValueError(f"{__class__.__name__} encountered unknown message: {msg}")
+            raise ValueError(
+                f"{__class__.__name__} encountered unknown message: {msg}"
+            )
 
         # Refresh the session
         await self.session._refresh()
 
 
 MouseEventListener._unique_id = "MouseEventListener-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/multi_line_text_input.py` & `rio_ui-0.6/rio/components/multi_line_text_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 class MultiLineTextInputConfirmEvent:
     text: str
 
 
 @final
 class MultiLineTextInput(KeyboardFocusableFundamentalComponent):
     """
-    # MultiLineTextInput
-
     A user-editable text field.
 
     It's similar to `TextInput`, but it allows the user to enter multiple lines of text.
 
     `MultiLineTextInput` allows the user to enter a short text. The text can either be
     shown in plain text or other sensitive information.
 
@@ -46,25 +44,25 @@
     `text`: The text currently entered by the user.
 
     `label`: A short text to display next to the text input.
 
     `is_sensitive`: Whether the text input should respond to user input.
 
     `is_valid`: Visually displays to the user whether the current text is
-            valid. You can use this to signal to the user that their input needs
-            to be changed.
+        valid. You can use this to signal to the user that their input needs
+        to be changed.
 
     `on_change`: Triggered when the user changes the text.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
-            such as by pressing the "Enter" key. You can use this to trigger
-            followup actions, such as logging in or submitting a form.
+        such as by pressing the "Enter" key. You can use this to trigger
+        followup actions, such as logging in or submitting a form.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of `MultiLineTextInput` with a default text of "" will be shown:
     `Note`: The text will not be updated if the user changes the text in the input field.
 
     ```python
     rio.MultiLineTextInput(text="")
     ```
@@ -75,15 +73,15 @@
 
     ```python
     class MyComponent(rio.Component):
         text: str = ""
 
         def build(self) -> rio.Component:
             return rio.MultiLineTextInput(
-                text=self.bind().text,  # state binding
+                text=self.bind().text,  # attribute binding
                 label="Write your comments here",
                 on_change=lambda event: print(event.text),
             )
     ```
 
     You can also use a method for updating the input text and do whatever you want.
     Note that methods are handy if you want to do more than just updating the input
@@ -121,15 +119,17 @@
             )
 
         if "text" in delta_state and not self.is_sensitive:
             raise AssertionError(
                 f"Frontend tried to set `MultiLineTextInput.text` even though `is_sensitive` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_change event
         try:
             new_value = delta_state["text"]
         except KeyError:
             pass
         else:
             assert isinstance(new_value, str), new_value
```

### Comparing `rio_ui-0.5.9/src/rio/components/node_input.py` & `rio_ui-0.6/rio/components/node_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 __all__ = [
     "NodeInput",
 ]
 
 
 @final
 class NodeInput(FundamentalComponent):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     name: str
     color: rio.Color
 
     def __init__(
         self,
         name: str,
         color: rio.Color,
```

### Comparing `rio_ui-0.5.9/src/rio/components/node_output.py` & `rio_ui-0.6/rio/components/node_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 __all__ = [
     "NodeOutput",
 ]
 
 
 @final
 class NodeOutput(FundamentalComponent):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     name: str
     color: rio.Color
 
     def __init__(
         self,
         name: str,
         color: rio.Color,
```

### Comparing `rio_ui-0.5.9/src/rio/components/number_input.py` & `rio_ui-0.6/rio/components/number_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,42 @@
     "m": 1_000_000,
 }
 
 
 @final
 @dataclass
 class NumberInputChangeEvent:
+    """
+    The argument for the `on_change` handler of a `NumberInput`.
+
+    ## Attributes
+
+    `value`: The new `value` of the `NumberInput`.
+    """
+
     value: float
 
 
 @final
 @dataclass
 class NumberInputConfirmEvent:
+    """
+    The argument for the `on_confirm` handler of a `NumberInput`.
+
+    ## Attributes
+
+    `value`: The new `value` of the `NumberInput`.
+    """
+
     value: float
 
 
 @final
 class NumberInput(Component):
     """
-    # NumberInput
-
     Like `TextInput`, but specifically for inputting numbers.
 
     `NumberInput` allows the user to enter a number. This is similar to the
     `TextInput` component, but with some goodies for handling numbers. The value
     is automatically parsed and formatted according to the user's locale, and
     you can specify minimum and maximum values to limit the user's input.
 
@@ -56,70 +70,72 @@
     ## Attributes
 
     `value`: The number currently entered by the user.
 
     `label`: A short text to display next to the text input.
 
     `prefix_text`: A short text to display before the text input. Useful for
-            displaying currency symbols or other prefixed units.
+        displaying currency symbols or other prefixed units.
 
     `suffix_text`: A short text to display after the text input. Useful for
-            displaying currency names or units.
+        displaying currency names or units.
 
     `minimum`: The minimum value the number can be set to.
 
     `maximum`: The maximum value the number can be set to.
 
     `decimals`: The number of decimals to accept. If the user enters more
-            decimals, they will be rounded off. If this value is equal to `0`,
-            the input's `value` is guaranteed to be an integer, rather than
-            float.
+        decimals, they will be rounded off. If this value is equal to `0`, the
+        input's `value` is guaranteed to be an integer, rather than float.
 
     `is_sensitive`: Whether the text input should respond to user input.
 
     `is_valid`: Visually displays to the user whether the current text is
-            valid. You can use this to signal to the user that their input needs
-            to be changed.
+        valid. You can use this to signal to the user that their input needs to
+        be changed.
 
     `on_change`: Triggered when the user changes the number.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
-            such as by pressing the "Enter" key.
+        such as by pressing the "Enter" key.
 
 
-    ## Example
+    ## Examples
 
-    A minimal example of `NumberInput` with a default value of 20.00 will be shown:
-    Note: The text will not be updated if the user changes the value in the input field.
+    A minimal example of `NumberInput` with a default value of 20.00 will be
+    shown: Note: The text will not be updated if the user changes the value in
+    the input field.
 
     ```python
     rio.NumberInput(value=20.00)
     ```
 
-    You can easily bind state variables to track changes. If you want to make your `NumberInput` more
-    responsive, you can easily achieve this by adding a lambda function call to e.g. on_change:
+    You can easily bind state variables to track changes. If you want to make
+    your `NumberInput` more responsive, you can easily achieve this by adding a
+    lambda function call to e.g. on_change:
 
     ```python
     class MyComponent(rio.Component):
         value: float = 0.0
 
         def build(self) -> rio.Component:
             return rio.NumberInput(
-                value=self.bind().value,  # state binding
+                value=self.bind().value,  # attribute binding
                 label="price",
                 prefix_text="$",
                 minimum=0,
                 decimals=2,
                 on_change=lambda event: print(f"value: {event.value}"),
             )
     ```
 
-    You can also use a method for updating the input value and do whatever you want. Note that methods
-    are handy if you want to do more than just updating the input value. For example run async code or
-    update other components based on the input text:
+    You can also use a method for updating the input value and do whatever you
+    want. Note that methods are handy if you want to do more than just updating
+    the input value. For example run async code or update other components based
+    on the input text:
 
     ```python
     class MyComponent(rio.Component):
         value: float = 0.0
 
         def on_change_update_value(self, event: rio.NumberInputChangeEvent):
             self.value = event.value
@@ -186,15 +202,17 @@
             except KeyError:
                 pass
             else:
                 raw_value = raw_value[:-1].rstrip()
 
         # Try to parse the number
         try:
-            value = float(raw_value.replace(self.session._decimal_separator, "."))
+            value = float(
+                raw_value.replace(self.session._decimal_separator, ".")
+            )
         except ValueError:
             self.value = self.value  # Force the old value to stay
             return False
 
         # Apply the multiplier
         value *= multiplier
```

### Comparing `rio_ui-0.5.9/src/rio/components/overlay.py` & `rio_ui-0.6/rio/components/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     "Overlay",
 ]
 
 
 @final
 class Overlay(FundamentalComponent):
     """
-    # Overlay
-
     Displays its child above all other components.
 
     The overlay component takes a single child component, and displays it above
     all other components on the page. The child will not scroll with the rest of
     the page and is exempt from layouting.
 
     Components inside of overlays are allocated the entire screen, and are
@@ -30,17 +28,18 @@
     ## Attributes
 
     `content`: The component to display in the overlay. It will take up the
         entire size of the screen, so make sure to use properties such as
         `align_x` and `align_y` to position it as needed.
 
 
-    ## Example
+    ## Examples
 
-    A simple example will display an `Overlay` with the text "Hello, world!" centered on the screen:
+    A simple example will display an `Overlay` with the text "Hello, world!"
+    centered on the screen:
 
     ```python
     rio.Overlay(
         rio.Text("Hello, world!"),
         align_x=0.5,
         align_y=0.5,
     )
@@ -58,16 +57,16 @@
         # parameters, as the underlying HTML `Overlay` element will force itself
         # to span the entire screen, ignoring them.
 
         super().__init__(key=key)
 
         self.content = content
 
-    def get_debug_details(self) -> dict[str, Any]:
-        result = super().get_debug_details()
+    def _get_debug_details(self) -> dict[str, Any]:
+        result = super()._get_debug_details()
 
         # Overlays intentionally remove a lot of common properties, because they
         # would behave in unexpected ways.
         del result["width"]
         del result["height"]
         del result["margin"]
         del result["margin_x"]
```

### Comparing `rio_ui-0.5.9/src/rio/components/page_view.py` & `rio_ui-0.6/rio/components/page_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
         align_y=0.35,
     )
 
 
 @final
 class PageView(Component):
     """
-    # PageView
-
     Placeholders for pages.
 
     Rio apps can consist of many pages. You might have a welcome page, a
     settings page, a login, and so on. Page views act as placeholders, that
     don't have an appearance of their own, but instead look up the currently
     active page, and display that.
 
@@ -67,15 +65,15 @@
 
     `fallback_build`: A callback that is called if the current URL does not
         correspond to any page in the application. It should return a Rio
         component that is displayed instead. If not specified Rio will
         display a default error page.
 
 
-    ## Example
+    ## Examples
 
     A minimal example:
 
     ```python
     app = rio.App(
         build=lambda: rio.Column(
             rio.Text("Welcome to my page!"),
@@ -102,18 +100,18 @@
     ```
 
     This will display "This is the home page" when navigating to the root URL,
     but "This is a subpage" when navigating to "/subpage". Note that on both
     pages the text "Welcome to my page!" is displayed above the page content.
     That's because it's not part of the `PageView`.
 
-    # TODO: Link to the routing/multipage how-to page
-
     """
 
+    # TODO: Link to the routing/multipage how-to page
+
     _: KW_ONLY
 
     fallback_build: Callable[[], rio.Component] | None = None
 
     # How many other PageViews are above this one in the component tree. Zero
     # for top-level PageViews, 1 for the next level, and so on.
     #
```

### Comparing `rio_ui-0.5.9/src/rio/components/plot.py` & `rio_ui-0.6/rio/components/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,39 +19,37 @@
 
 __all__ = ["Plot"]
 
 
 @final
 class Plot(FundamentalComponent):
     """
-    # Plot
-
     Displays a `matplotlib`, `seaborn` or `plotly` plot.
 
 
     ## Attributes
 
     `figure`: The plot figure to display.
 
     `background`: The background color of the plot. If `None`, a color from
         the theme is used.
 
     `corner_radius`: The corner radius of the plot
 
 
-    ## Example
+    ## Examples
 
     A minimal example with a plotly plot:
 
     ```python
     import plotly.graph_objects as go
 
     fig = go.Figure()
 
-    # create your own plot here (add traces, ect.)
+    # Create your own plot here (add traces, ect.)
 
     rio.Plot(fig)
     ```
 
     You can easily show plots defined in your build function by passing
     the figure to the `Plot` component.
 
@@ -71,15 +69,17 @@
             fig = px.line(df, x="x", y="y", title="sample figure")
 
             return rio.Plot(fig)
     ```
     """
 
     figure: (
-        plotly.graph_objects.Figure | matplotlib.figure.Figure | matplotlib.axes.Axes
+        plotly.graph_objects.Figure
+        | matplotlib.figure.Figure
+        | matplotlib.axes.Axes
     )
     background: rio.Fill | None
     corner_radius: float | tuple[float, float, float, float] | None
 
     def __init__(
         self,
         figure: (
@@ -115,15 +115,17 @@
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
         )
 
         self.figure = figure
-        self.background = None if background is None else rio.Fill._try_from(background)
+        self.background = (
+            None if background is None else rio.Fill._try_from(background)
+        )
 
         if corner_radius is None:
             self.corner_radius = self.session.theme.corner_radius_small
         else:
             self.corner_radius = corner_radius
 
     def _custom_serialize(self) -> JsonDoc:
```

### Comparing `rio_ui-0.5.9/src/rio/components/popup.py` & `rio_ui-0.6/rio/components/popup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,22 +14,24 @@
     "PopupOpenOrCloseEvent",
 ]
 
 
 @final
 @dataclass
 class PopupOpenOrCloseEvent:
+    """
+    The argument for the `on_open_or_close` handler of a `Popup`.
+    """
+
     is_open: bool
 
 
 @final
 class Popup(FundamentalComponent):
     """
-    # Popup
-
     A container which floats above other components.
 
     Popups are containers which float above the page when open. This allows you
     to keep your app clean by default, but present additional information or
     controls when needed.
 
     They take two children: The `anchor` is always visible and positions the
@@ -46,36 +48,34 @@
     `anchor`: A component which is always visible and positions the popup.
 
     `content`: A component which is only visible when the popup is open.
 
     `direction`: The direction into which the popup opens.
 
     `alignment`: The alignment of the popup within the anchor. If the popup
-            opens to the left or right, this is the vertical alignment, with `0`
-            being the top and `1` being the bottom. If the popup opens to the
-            top or bottom, this is the horizontal alignment, with `0` being the
-            left and `1` being the right. Has no effect if the popup opens
-            centered.
+        opens to the left or right, this is the vertical alignment, with `0`
+        being the top and `1` being the bottom. If the popup opens to the top or
+        bottom, this is the horizontal alignment, with `0` being the left and
+        `1` being the right. Has no effect if the popup opens centered.
 
     `gap`: How much space to leave between the popup and the anchor. Has no
-            effect popup opens centered.
+        effect popup opens centered.
 
     `is_open`: Whether the popup is currently open.
 
     `on_open_or_close`: Triggered when the popup is opened or closed.
 
 
-    ## Example
+    ## Examples
 
     A simple popup with a button as the anchor and a text input as the content:
-
-    TODO: add example
-
     """
 
+    # TODO: add example
+
     anchor: rio.Component
     content: rio.Component
     _: KW_ONLY
     color: rio.ColorSet = "neutral"
     direction: Literal["left", "top", "right", "bottom", "center"] = "center"
     alignment: float = 0.5
     gap: float = 0.8
@@ -84,15 +84,17 @@
 
     def _validate_delta_state_from_frontend(self, delta_state: JsonDoc) -> None:
         if not set(delta_state) <= {"is_open"}:
             raise AssertionError(
                 f"Frontend tried to change `{type(self).__name__}` state: {delta_state}"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_open_or_close event
         try:
             is_open = delta_state["is_open"]
         except KeyError:
             pass
         else:
             assert isinstance(is_open, bool), is_open
```

### Comparing `rio_ui-0.5.9/src/rio/components/progress_bar.py` & `rio_ui-0.6/rio/components/progress_bar.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,33 +6,31 @@
     "ProgressBar",
 ]
 
 
 @final
 class ProgressBar(FundamentalComponent):
     """
-    # ProgressBar
-
     A progress indicator in the shape of a horizontal bar.
 
     `ProgressBar` conveys to the user that activity is ongoing. It can either
     display the exact progress as a fraction from 0 to 1, or it can display an
     indeterminate progress animation, which is useful when the exact progress
     isn't known.
 
     The circular counterpart to this component is the `ProgressCircle`.
 
 
     ## Attributes
 
     `progress`: The progress to display, as a fraction from 0 to 1. If `None`,
-            the progress indicator will be indeterminate.
+        the progress indicator will be indeterminate.
 
 
-    ## Example
+    ## Examples
 
     A minimal example displaying a progress bar that is 50% complete.
 
     ```python
     rio.ProgressBar(progress=0.5)
     ```
     """
```

### Comparing `rio_ui-0.5.9/src/rio/components/progress_circle.py` & `rio_ui-0.6/rio/components/progress_circle.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     "ProgressCircle",
 ]
 
 
 @final
 class ProgressCircle(FundamentalComponent):
     """
-    # ProgressCircle
-
     A progress indicator in the shape of a circle.
 
     `ProgressCircle` conveys to the user that activity is ongoing. It can either
     display the exact progress as a fraction from 0 to 1, or it can display an
     indeterminate progress animation, which is useful when the exact progress
     isn't known.
 
@@ -29,26 +27,22 @@
 
     The linear counterpart to this component is the `ProgressBar`.
 
 
     ## Attributes
 
     `progress`: The progress to display, as a fraction from 0 to 1. If `None`,
-            the progress indicator will be indeterminate.
+        the progress indicator will be indeterminate.
 
     `color`: The color scheme of the progress indicator. Keeping the default
-                is recommended, but it may make sense to change the color in
-                case the default is hard to perceive on your background.
-
-    `size`: The size of the progress indicator. This is equivalent to setting
-            a component's `width` and `height` to the same value.
-
+        is recommended, but it may make sense to change the color in
+        case the default is hard to perceive on your background.
 
 
-    ## Example
+    ## Examples
 
     A minimal example displaying a progress circle that is 50% complete.
 
     ```python
     rio.ProgressCircle(progress=0.5)
     ```
     """
@@ -70,15 +64,15 @@
         margin_top: float | None = None,
         margin_right: float | None = None,
         margin_bottom: float | None = None,
         align_x: float | None = None,
         align_y: float | None = None,
     ):
         """
-        Args:
+        ## Parameters
             progress: The progress to display, as a fraction from 0 to 1. If `None`,
                 the progress indicator will be indeterminate.
 
             color: The color scheme of the progress indicator. Keeping the default
                 is recommended, but it may make sense to change the color in case
                 the default is hard to perceive on your background.
```

### Comparing `rio_ui-0.5.9/src/rio/components/rectangle.py` & `rio_ui-0.6/rio/components/rectangle.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,53 +15,87 @@
     "Rectangle",
 ]
 
 
 @final
 class Rectangle(FundamentalComponent):
     """
-    # Rectangle
-
     A customizable rectangle shape.
 
     Rectangles are versatile components that can be used to build up more
     complex elements. While not particularly interesting on their own, combining
     a rectangle with other components allows you to quickly create custom
     buttons, cards, or anything els you may need in your app.
 
-    Rectangles also act as a simple source of animations. They accept two
-    styles: A default style for when the user isn't interacting with them, and a
-    hover style for when the mouse hovers above them. This, along with their
+    Rectangles also act as a simple source of animations. They have two styles:
+    A default style for when the user isn't interacting with them, and a hover
+    style for when the mouse hovers above them. This, along with their
     `transition_time` attribute allows you to make your app feel dynamic and
     alive.
 
 
     ## Attributes
 
     `content`: The component to display inside the rectangle.
 
-    `style`: How the rectangle should appear when the user isn't interacting
-        with it.
+    `fill`: The background color/image/gradient of the rectangle.
+
+    `stroke_width`: The width of the rectangle's outline.
+
+    `stroke_color`: The color of the rectangle's outline.
+
+    `corner_radius`: The rectangle's corner radius. Can be a single number or a
+        sequence of 4 numbers.
+
+    `shadow_radius`: The corner radius of the rectangle's shadow.
+
+    `shadow_offset_x`: The horizontal offset of the rectangle's shadow. A
+        negative value moves the shadow to the left side of the rectangle.
+
+    `shadow_offset_y`: The vertical offset of the rectangle's shadow. A
+        negative value moves the shadow above the rectangle.
+
+    `shadow_color`: The color of the rectangle's shadow.
+
+    `hover_fill`: The rectangle's `fill` while the cursor is hovering over it.
+
+    `hover_stroke_width`: The rectangle's `stroke_width` while the cursor is
+        hovering over it.
+
+    `hover_stroke_color`: The rectangle's `stroke_color` while the cursor is
+        hovering over it.
+
+    `hover_corner_radius`: The rectangle's `corner_radius` while the cursor is
+        hovering over it.
 
-    `hover_style`: The style of the rectangle when the mouse hovers above it.
-        If set to `None`, the rectangle will not change its appearance when
-        hovered.
+    `hover_shadow_radius`: The rectangle's `shadow_radius` while the cursor is
+        hovering over it.
+
+    `hover_shadow_offset_x`: The rectangle's `shadow_offset_x` while the cursor
+        is hovering over it.
+
+    `hover_shadow_offset_y`: The rectangle's `shadow_offset_y` while the cursor
+        is hovering over it.
+
+    `hover_shadow_color`: The rectangle's `shadow_color` while the cursor is
+        hovering over it.
 
     `transition_time`: How many seconds it should take for the rectangle to
-        transition between its styles.
+        transition between its regular and hover styles.
 
     `cursor`: The cursor to display when the mouse hovers above the rectangle.
 
     `ripple`: Whether to display a Material Design ripple effect when the
         rectangle is hovered or clicked.
 
 
-    ## Example
+    ## Examples
 
-    A minimal example of a rectangle with a text and red background will be shown:
+    A minimal example of a rectangle with a text and red background will be
+    shown:
 
     ```python
     rio.Rectangle(
         content=rio.Text("Hello World!"),
         fill=rio.Color.from_hex("ff0000"),
     )
     ```
@@ -86,48 +120,51 @@
     _: KW_ONLY
     content: rio.Component | None = None
     transition_time: float = 1.0
     cursor: rio.CursorStyle = cursor_style.CursorStyle.DEFAULT
     ripple: bool = False
 
     fill: rio.FillLike
-    stroke_color: rio.Color = Color.BLACK
     stroke_width: float = 0.0
+    stroke_color: rio.Color = Color.BLACK
     corner_radius: float | tuple[float, float, float, float] = 0.0
-    shadow_color: rio.Color = Color.BLACK
     shadow_radius: float = 0.0
     shadow_offset_x: float = 0.0
     shadow_offset_y: float = 0.0
+    shadow_color: rio.Color = Color.BLACK
 
     hover_fill: rio.FillLike | None = None
-    hover_stroke_color: rio.Color | None = None
     hover_stroke_width: float | None = None
+    hover_stroke_color: rio.Color | None = None
     hover_corner_radius: float | tuple[float, float, float, float] | None = None
-    hover_shadow_color: rio.Color | None = None
     hover_shadow_radius: float | None = None
     hover_shadow_offset_x: float | None = None
     hover_shadow_offset_y: float | None = None
+    hover_shadow_color: rio.Color | None = None
 
     def __post_init__(self):
         self.fill = rio.Fill._try_from(self.fill)
 
     def _custom_serialize(self) -> JsonDoc:
         return {
             # Regular
             "fill": rio.Fill._try_from(self.fill)._serialize(self._session_),
             "corner_radius": (
                 self.corner_radius
-                if self.corner_radius is None or isinstance(self.corner_radius, tuple)
+                if self.corner_radius is None
+                or isinstance(self.corner_radius, tuple)
                 else (self.corner_radius,) * 4
             ),
             # Hover
             "hover_fill": (
                 None
                 if self.hover_fill is None
-                else rio.Fill._try_from(self.hover_fill)._serialize(self._session_)
+                else rio.Fill._try_from(self.hover_fill)._serialize(
+                    self._session_
+                )
             ),
             "hover_corner_radius": (
                 self.hover_corner_radius
                 if self.hover_corner_radius is None
                 or isinstance(self.hover_corner_radius, tuple)
                 else (self.hover_corner_radius,) * 4
             ),
```

### Comparing `rio_ui-0.5.9/src/rio/components/revealer.py` & `rio_ui-0.6/rio/components/revealer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,47 +16,52 @@
 
 T = TypeVar("T")
 
 
 @final
 @dataclass
 class RevealerChangeEvent:
+    """
+    The argument for the `on_change` handler of a `Revealer`.
+
+    ## Attributes
+
+    `is_open`: The new `is_open` state of the `Revealer`.
+    """
+
     is_open: bool
 
 
 @final
 class Revealer(FundamentalComponent):
     """
-    # Revealer
-
     A component that can be used to hide and reveal content.
 
     `Revealer` is a versatile component that can be used to hide and reveal
     content. It can be used to create collapsible sections, or to hide and
     reveal content based on user input.
 
 
     ## Attributes
 
     `header`: The header of the `Revealer`. If `None`, the `Revealer` will be
-            hidden by default.
+        hidden by default.
 
     `content`: The content to display when the `Revealer` is open.
 
     `header_style`: The style of the header. Can be one of `"heading1"`,
-            `"heading2"`, `"heading3"`, or `"text"`.
+        `"heading2"`, `"heading3"`, or `"text"`.
 
     `is_open`: Whether the `Revealer` is open or not.
 
     `on_change`: An event handler that is called when the `Revealer` is opened
-            or closed. The event handler receives a `RevealerChangeEvent` as
-            input.
+        or closed. The event handler receives a `RevealerChangeEvent` as input.
 
 
-    ## Example
+    ## Examples
 
     A simple `Revealer` that displays "Hello" when opened:
 
     ```python
     rio.Revealer(header="Click to reveal", content=rio.Text("Hello"))
     ```
 
@@ -99,15 +104,17 @@
             )
 
         if "is_open" in delta_state and self.header is None:
             raise AssertionError(
                 f"Frontend tried to set `Revealer.is_open` even though it has no `header`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_change event
         try:
             new_value = delta_state["is_open"]
         except KeyError:
             pass
         else:
             assert isinstance(new_value, bool), new_value
```

### Comparing `rio_ui-0.5.9/src/rio/components/root_components.py` & `rio_ui-0.6/rio/components/root_components.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 # that is never re-built, which is convenient in many ways:
 # 1. Every component except for the root component itself has a valid builder
 # 2. The JS code is simpler because the root component can't have an
 #    alignment or margin
 # 3. Children of non-fundamental components are automatically initialized
 #    correctly, so we don't need to duplicate that logic here
 class HighLevelRootComponent(Component):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     build_function: Callable[[], Component]
     build_connection_lost_message_function: Callable[[], Component]
 
     def build(self) -> Component:
         # Spawn a debugger if running in debug mode
 
         if self.session._app_server.debug_mode:
@@ -41,13 +47,19 @@
             user_content,
             common.safe_build(self.build_connection_lost_message_function),
             debugger=debugger,
         )
 
 
 class FundamentalRootComponent(FundamentalComponent):
+    """
+    ## Metadata
+
+    public: False
+    """
+
     content: Component
     connection_lost_component: Component
     debugger: Component | None
 
 
 FundamentalRootComponent._unique_id = "FundamentalRootComponent-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/scroll_container.py` & `rio_ui-0.6/rio/components/scroll_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 __all__ = ["ScrollContainer"]
 
 
 @final
 class ScrollContainer(FundamentalComponent):
     """
-    # ScrollContainer
-
-    Displays a scroll bar if its child grows too large.
+    Displays a scroll bar if its content grows too large.
 
     `ScrollContainer` is a container which displays a scroll bar if its child
     component grows too large. It can scroll vertically and/or horizontally.
 
 
     ## Attributes
 
@@ -36,15 +34,15 @@
         `"never"` disables vertical scrolling altogether.
 
     `sticky_bottom`: If `True`, when the user has scrolled to the bottom and
         the content of the `ScrollContainer` grows larger, the scroll bar
         will automatically scroll to the bottom again.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of `ScrollContainer` displaying an icon:
 
     ```python
     rio.ScrollContainer(
         content=rio.Icon("material/castle", width=50, height=50),
         height=10,
```

### Comparing `rio_ui-0.5.9/src/rio/components/scroll_target.py` & `rio_ui-0.6/rio/components/scroll_target.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 from __future__ import annotations
 
+from dataclasses import KW_ONLY
 from typing import final
 
+from uniserde import JsonDoc
+
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["ScrollTarget"]
 
 
 @final
 class ScrollTarget(FundamentalComponent):
     """
-    # ScrollTarget
-
     Allows browsers to scroll to a specific component via URL fragment.
 
     `ScrollTarget` is a container which can be referenced by a URL fragment,
     which allows browsers to scroll to it when the page is loaded. For example,
     if your website contains a `ScrollTarget` with the ID `"my-section"`, then a
     browser visiting `https://your.website/#my-section` will immediately scroll
     it into view.
 
 
     ## Attributes
 
     `id`: The ID of the `ScrollTarget`. This must be unique among all
-            `ScrollTarget`s on the page.
+        `ScrollTarget`s on the page.
 
     `content`: The child component to display inside the `ScrollTarget`.
 
 
-    ## Example
+    ## Examples
 
-    A minimal example of `ScrollTarget` displaying an icon:
+    A minimal example of `ScrollTarget` displaying a heading:
 
-    #TODO: Better example
     ```python
     rio.ScrollTarget(
-        id="my-section",
-        content=rio.Icon("material/castle", width=50, height=50),
+        id="chapter-1",
+        content=rio.Text('Chapter 1', style='heading1'),
     )
     ```
     """
 
     id: str
     content: rio.Component | None = None
+    _: KW_ONLY
+    copy_button_content: str | rio.Component | None = "¶"
+    copy_button_spacing: float = 0.5
+
+    def _custom_serialize(self) -> JsonDoc:
+        button_content = self.copy_button_content
+
+        return {
+            "copy_button_content": button_content._id
+            if isinstance(button_content, rio.Component)
+            else None,
+            "copy_button_text": button_content
+            if isinstance(button_content, str)
+            else None,
+        }
 
 
 ScrollTarget._unique_id = "ScrollTarget-builtin"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rio_ui-0.5.9/src/rio/components/separator.py` & `rio_ui-0.6/rio/components/separator.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,30 +11,28 @@
     "Separator",
 ]
 
 
 @final
 class Separator(FundamentalComponent):
     """
-    # Separator
-
     A line to separate content.
 
     `Separator` is a horizontal or vertical line that can be used to separate content. It
     can be styled with a color. By default, it is a thin line with a light gray
     color.
 
 
     ## Attributes
 
     `color`: The color of the `Separator`. If `None`, the color will be
-            determined by the theme.
+        determined by the theme.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of `Separator`:
 
     ```python
     rio.Separator()
     ```
```

### Comparing `rio_ui-0.5.9/src/rio/components/slider.py` & `rio_ui-0.6/rio/components/slider.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 class SliderChangeEvent:
     value: float
 
 
 @final
 class Slider(FundamentalComponent):
     """
-    # Slider
-
     A component for selecting a single value from a range.
 
     The `Slider` components allows the user to select a single real number value
     by dragging a handle along a line. The value can be any number within a
     range you can specify.
 
 
@@ -37,20 +35,22 @@
 
     `minimum`: The minimum value the slider can be set to.
 
     `maximum`: The maximum value the slider can be set to.
 
     `value`: The current value of the slider.
 
+    `step`: The step size between slider values.
+
     `is_sensitive`: Whether the slider should respond to user input.
 
     `on_change`: A callback that is called when the value of the slider changes.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Slider` ranging from 0 to 100 will be shown:
 
     ```python
     rio.Slider(minimum=0, maximum=100)
     ```
 
@@ -59,18 +59,18 @@
 
     ```python
     class MyComponent(rio.Component):
         value: int = 0
 
         def build(self) -> rio.Component:
             return rio.Slider(
-                value=self.bind().value,  # state binding
+                value=self.bind().value,  # attribute binding
                 minimum=0,
                 maximum=100,
-                step_size=1,
+                step=1,
                 on_change=lambda event: print(f"value: {event.value}"),
             )
     ```
 
     You can also use a method for updating the input value and do whatever you want. Note that methods
     are handy if you want to do more than just updating the input value. For example run async code or
     update other components based on the input text:
@@ -84,34 +84,34 @@
             print(f"value: {self.value}")
 
         def build(self) -> rio.Component:
             return rio.Slider(
                 value=self.value,
                 minimum=0,
                 maximum=100,
-                step_size=1,
+                step=1,
                 on_change=self.on_change,
             )
     ```
     """
 
     minimum: float
     maximum: float
     value: float
-    step_size: float
+    step: float
     is_sensitive: bool
     on_change: rio.EventHandler[SliderChangeEvent]
 
     def __init__(
         self,
         *,
         minimum: float = 0,
         maximum: float = 1,
-        step_size: float = 0,
-        value: float | None = None,
+        step: float = 0,
+        value: float = 0.5,
         is_sensitive: bool = True,
         on_change: rio.EventHandler[SliderChangeEvent] = None,
         key: str | None = None,
         margin: float | None = None,
         margin_x: float | None = None,
         margin_y: float | None = None,
         margin_left: float | None = None,
@@ -136,67 +136,66 @@
             height=height,
             align_x=align_x,
             align_y=align_y,
         )
 
         self.minimum = minimum
         self.maximum = maximum
-        self.step_size = step_size
-        self.value = value  # type: ignore  Possibly assigning None. Fixed in __post_init__ below
+        self.step = step
+        self.value = value
         self.is_sensitive = is_sensitive
         self.on_change = on_change
 
     def __post_init__(self) -> None:
-        # Don't hammer potential state bindings
+        # Don't hammer potential attribute bindings
         minimum = self.minimum
         maximum = self.maximum
-        step_size = self.step_size
+        step = self.step
         value = self.value
 
         initial_value = value
 
         if maximum <= minimum:
             raise ValueError(
                 f"`maximum` must be greater than `minimum`. Got {maximum} <= {minimum}"
             )
 
-        if step_size < 0:
+        if step < 0:
             raise ValueError(
-                f"`step_size` must be greater than or equal to 0. Got {step_size}"
+                f"`step` must be greater than or equal to 0. Got {step}"
             )
 
-        if value is None:
-            value = minimum + (maximum - minimum) / 2
-
-        if step_size != 0:
-            value = round(value / step_size) * step_size
+        if step != 0:
+            value = round(value / step) * step
 
         value = min(maximum, max(minimum, value))
 
         # Only assign the value if it has in fact changed, as this causes a
         # refresh. If the value is bound to the parent and the parent rebuilds
         # this creates an infinite loop.
         if value != initial_value:
             self.value = value
 
-    # TODO: When `minimum` or `maximum` is changed, make sure the value is still within
-    # the range
+    # TODO: When `minimum` or `maximum` is changed, make sure the value is still
+    # within the range
 
     def _validate_delta_state_from_frontend(self, delta_state: JsonDoc) -> None:
         if not set(delta_state) <= {"value"}:
             raise AssertionError(
                 f"Frontend tried to change `{type(self).__name__}` state: {delta_state}"
             )
 
         if "value" in delta_state and not self.is_sensitive:
             raise AssertionError(
                 f"Frontend tried to set `Slider.value` even though `is_sensitive` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_change event
         try:
             new_value = delta_state["value"]
         except KeyError:
             pass
         else:
             assert isinstance(new_value, (int, float)), new_value
```

### Comparing `rio_ui-0.5.9/src/rio/components/slideshow.py` & `rio_ui-0.6/rio/components/slideshow.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,48 +14,44 @@
     "Slideshow",
 ]
 
 
 @final
 class Slideshow(FundamentalComponent):
     """
-    # Slideshow
-
-    Prominently switch between multiple components based on a timer.
+    Prominently switches between multiple components based on a timer.
 
     The `Slideshow` component is a container that can hold multiple components,
     and will display them one after the other, with smooth transitions in
     between. These are very useful for displaying a series of demos or news to
     visitors.
 
 
     ## Attributes
 
     `children`: The components to transition between.
 
     `linger_time`: The time in seconds to display each component before
-            switching to the next one.
+        switching to the next one.
 
     `corner_radius`: How rounded the slideshow's corners should be. If set to
-            `None`, the slideshow will use a default corner radius from the
-            current theme.
+        `None`, the slideshow will use a default corner radius from the current
+        theme.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of `Slideshow` displaying two images will be shown:
 
     ```python
     from pathlib import Path
 
-    PATH = Path(__file__).parent
-
     rio.Slideshow(
-        rio.Image(PATH / "first.jpg"),
-        rio.Image(PATH / "second.jpg"),
+        rio.Image(Path("first.jpg")),
+        rio.Image(Path("second.jpg")),
         linger_time=5,
     )
     ```
     """
 
     children: list[rio.Component]
     _: KW_ONLY
```

### Comparing `rio_ui-0.5.9/src/rio/components/spacer.py` & `rio_ui-0.6/rio/components/spacer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,26 @@
     "Spacer",
 ]
 
 
 @final
 class Spacer(class_container.ClassContainer):
     """
-    # Spacer
-
     Adds empty space.
 
     Spacers are invisible components which add empty space between other
     components. While similar effects can often be achieved using margins and
     alignment, code with spacers can sometimes be easier to read.
 
     Note that unlike most components in Rio, `Spacer` does not have a `natural`
     size. Therefore it defaults to a width and height of `grow`, as that is how
     they're frequently used.
 
-    ## Example
+
+    ## Examples
 
     A minimal example of `Spacer` will be shown:
 
     ```python
     rio.Spacer(height=5)
     ```
     """
@@ -37,15 +36,15 @@
         self,
         *,
         width: float | Literal["grow"] = "grow",
         height: float | Literal["grow"] = "grow",
         key: str | None = None,
     ):
         """
-        Args:
+        ## Parameters
             width: How much space the spacer should take up horizontally.
             height: How much space the spacer should take up vertically.
         """
 
         super().__init__(
             None,
             ["rio-spacer"],
```

### Comparing `rio_ui-0.5.9/src/rio/components/stack.py` & `rio_ui-0.6/rio/components/stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 
 __all__ = ["Stack"]
 
 
 @final
 class Stack(FundamentalComponent):
     """
-    # Stack
-
     A container that stacks its children in the Z direction.
 
     `Stacks` are similar to rows and columns, but they stack their children in
     the Z direction instead of the X or Y direction. In other words, the stack's
     children overlap each other, with the first one at the bottom, the second
     one above that, and so on.
 
 
     ## Attributes
 
     `children`: The components to place in this `Stack`.
 
-    ## Example
+
+    ## Examples
 
     A minimal example of `Stack` will be shown. This example will create a stack
     of three icons, each with a different size and color. The first icon will be
     at the bottom, the second one above that, and the third one at the top:
 
     ```python
     rio.Stack(
@@ -95,13 +94,24 @@
         )
 
         self.children = list(children)
 
     def add(self, child: rio.Component) -> Self:
         """
         Appends a child component.
+
+        Appends a child component to the end and then returns the `Stack`, which
+        makes method chaining possible:
+
+        ```python
+        rio.Stack().add(child1).add(child2)
+        ```
+
+        ## Parameters
+
+        `child`: The child component to append.
         """
         self.children.append(child)
         return self
 
 
 Stack._unique_id = "Stack-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/switch.py` & `rio_ui-0.6/rio/components/switch.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 class SwitchChangeEvent:
     is_on: bool
 
 
 @final
 class Switch(FundamentalComponent):
     """
-    # Switch
-
     An input for `True` / `False` values.
 
     Switches allow the user to toggle between an "on" and an "off" state. They
     thus correspond to a Python `bool` value. Use them to allow the user to
     enable or disable certain features, or to select between two options.
 
 
@@ -38,15 +36,15 @@
     `is_on`: Whether the switch is currently in the "on" state.
 
     `is_sensitive`: Whether the switch should respond to user input.
 
     `on_change`: Triggered when the user toggles the switch.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Switch` will be shown:
 
     ```python
     rio.Switch(is_on=True)
     ```
 
@@ -98,15 +96,17 @@
             )
 
         if "is_on" in delta_state and not self.is_sensitive:
             raise AssertionError(
                 f"Frontend tried to set `Switch.is_on` even though `is_sensitive` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_change event
         try:
             new_value = delta_state["is_on"]
         except KeyError:
             pass
         else:
             assert isinstance(new_value, bool), new_value
```

### Comparing `rio_ui-0.5.9/src/rio/components/switcher.py` & `rio_ui-0.6/rio/components/switcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,36 @@
     "Switcher",
 ]
 
 
 @final
 class Switcher(FundamentalComponent):
     """
-    # Switcher
-
     A container which can switch between different components.
 
     A `Switcher` is a container which can switch between different components.
     It is commonly used to switch between different views or modes. The
     `content` attribute can be used to change the currently displayed component.
 
+
     ## Attributes
 
     `content`: The currently displayed component.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Switcher` will be shown:
-    TODO: check if this is the correct example
 
     ```python
     rio.Switcher(content=rio.Text("Hello, world!"))
     ```
+
+    ## Metadata
+
+    `experimental`: True
     """
 
     content: rio.Component | None
 
 
 Switcher._unique_id = "Switcher-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/switcher_bar.py` & `rio_ui-0.6/rio/components/switcher_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,45 +24,41 @@
 class SwitcherBarChangeEvent(Generic[T]):
     value: T | None
 
 
 @final
 class SwitcherBar(FundamentalComponent, Generic[T]):
     """
-    # SwitcherBar
-
     A bar of options which can be switched between.
 
     A `SwitcherBar` is a bar of options which can be switched between. It is
     commonly used to switch between different views or modes.
 
 
     ## Attributes
 
     `values`: The list of values which can be selected.
 
     `names`: The list of names to display for each value. If `None`, the
         string representation of each value is used.
 
-    `icons`: The list of icons to display for each value.
-
     `color`: The color of the switcher bar.
 
     `orientation`: The orientation of the switcher bar.
 
     `spacing`: The spacing between options.
 
     `selected_value`: The currently selected value.
 
     `allow_none`: Whether the switcher bar can have no value selected.
 
     `on_change`: Triggered whenever the selected value changes.
 
 
-    ## Example
+    ## Examples
 
     A simple switcher bar with three options:
 
     ```python
     rio.SwitcherBar(
         values=[1, 2, 3],
         names=["A-SwitchName", "B-SwitchName", "C-SwitchName"],
@@ -120,14 +116,18 @@
                     ),
                 ),
                 width="grow",
                 corner_radius=0,
                 color="background",
             )
     ```
+
+    ## Metadata
+
+    `experimental`: True
     """
 
     names: list[str]
     values: list[T]
     icon_svg_sources: list[str | None]
     color: rio.ColorSet
     orientation: Literal["horizontal", "vertical"]
@@ -201,15 +201,16 @@
             self.icon_svg_sources = [None] * len(values)
         else:
             if len(icons) != len(values):
                 raise ValueError("`icons` must be the same length as `values`.")
 
             registry = icon_registry.IconRegistry.get_singleton()
             self.icon_svg_sources = [
-                None if icon is None else registry.get_icon_svg(icon) for icon in icons
+                None if icon is None else registry.get_icon_svg(icon)
+                for icon in icons
             ]
 
         self.selected_value = selected_value
 
     def __post_init__(self) -> None:
         # Make sure a value is selected, if needed
         if self.selected_value is None and not self.allow_none:
@@ -219,15 +220,15 @@
         # None is fine
         if self.selected_value is None:
             assert self.allow_none
             return None
 
         # The frontend works with names, not values. Get the corresponding name.
 
-        # Avoid hammering a potential state binding
+        # Avoid hammering a potential attribute binding
         selected_value = self.selected_value
 
         # Fetch the name
         for name, value in zip(self.names, self.values):
             if value == selected_value:
                 return name
         else:
```

### Comparing `rio_ui-0.5.9/src/rio/components/table.py` & `rio_ui-0.6/rio/components/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
 TableValue = int | float | str
 
 
 @final
 class Table(FundamentalComponent):
     """
-    # Table
-
     A table of data.
 
     Tables are a way to display data in a grid, with rows and columns. They are
     very useful for displaying data that is naturally tabular, such as
     spreadsheets, databases, or CSV files. Tables can be sorted by clicking on
     the column headers.
 
@@ -36,15 +34,15 @@
     ## Attributes
 
     `data`: The data to display.
 
     `show_row_numbers`: Whether to show row numbers on the left side of the table.
 
 
-    ## Example
+    ## Examples
 
     A simple table with some data:
 
     ```python
     rio.Table(
         data={
             "Name": ["Alice", "Bob", "Charlie"],
@@ -65,27 +63,29 @@
     show_row_numbers: bool = True
 
     def _custom_serialize(self) -> JsonDoc:
         return {
             "data": self._data_to_json(),  # type: ignore[variance]
         }
 
-    def _data_to_json(self) -> dict[str, list[TableValue]] | list[list[TableValue]]:
+    def _data_to_json(
+        self,
+    ) -> dict[str, list[TableValue]] | list[list[TableValue]]:
         data = self.data
 
         if isinstance(data, maybes.PANDAS_DATAFRAME_TYPES):
             return data.to_dict(orient="list")  # type: ignore
 
         if isinstance(data, maybes.POLARS_DATAFRAME_TYPES):
-            return data.to_dict(as_series=False)
+            return data.to_dict(as_series=False)  # type: ignore
 
         if isinstance(data, Mapping):
             return dict(data)  # type: ignore[wtf]
 
         if isinstance(data, maybes.NUMPY_ARRAY_TYPES):
-            return data.tolist()
+            return data.tolist()  # type: ignore
 
         data = cast(Iterable[Iterable[TableValue]], data)
         return [row if isinstance(row, list) else list(row) for row in data]
 
 
 Table._unique_id = "Table-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/text.py` & `rio_ui-0.6/rio/components/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,53 +12,49 @@
     "Text",
 ]
 
 
 @final
 class Text(FundamentalComponent):
     """
-    # Text
-
     Displays unformatted text.
 
     `Text` displays text without any formatting, making it one of the most
     commonly used components in Rio.
 
     While the text itself is unformatted, you can still control the style of
     the text using the `style` attribute. This allows you to change the font
     size, color, and more.
 
 
     ## Attributes
 
     `text`: The text to display.
 
-    `multiline`: Whether the text may be split into multiple lines if not
-        enough space is available.
-
     `selectable`: Whether the text can be selected by the user.
 
     `style`: The style of the text. This can either be a `TextStyle` instance,
         or one of the built-in styles: `heading1`, `heading2`, `heading3`,
         `text` or `dim`.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Text` will be shown:
 
     ```python
     rio.Text("Hello, world!")
     ```
     """
 
     text: str
     selectable: bool = True
     style: (
-        Literal["heading1", "heading2", "heading3", "text", "dim"] | rio.TextStyle
+        Literal["heading1", "heading2", "heading3", "text", "dim"]
+        | rio.TextStyle
     ) = "text"
     justify: Literal["left", "right", "center", "justify"] = "center"
     wrap: bool | Literal["ellipsize"] = False
 
     def _custom_serialize(self) -> JsonDoc:
         # Serialization doesn't handle unions. Hence the custom serialization
         # here
```

### Comparing `rio_ui-0.5.9/src/rio/components/text_input.py` & `rio_ui-0.6/rio/components/text_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,42 @@
     "TextInputConfirmEvent",
 ]
 
 
 @final
 @dataclass
 class TextInputChangeEvent:
+    """
+    The argument for the `on_change` handler of a `TextInput`.
+
+    ## Attributes
+
+    `text`: The new `text` of the `TextInput`.
+    """
+
     text: str
 
 
 @final
 @dataclass
 class TextInputConfirmEvent:
+    """
+    The argument for the `on_confirm` handler of a `TextInput`.
+
+    ## Attributes
+
+    `text`: The new `text` of the `TextInput`.
+    """
+
     text: str
 
 
 @final
 class TextInput(KeyboardFocusableFundamentalComponent):
     """
-    # TextInput
-
     A user-editable text field.
 
     `TextInput` allows the user to enter a short text. The text can either be
     shown in plain text, or hidden when used for passwords or other sensitive
     information.
 
 
@@ -64,41 +78,44 @@
     `on_change`: Triggered when the user changes the text.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
             such as by pressing the "Enter" key. You can use this to trigger
             followup actions, such as logging in or submitting a form.
 
 
-    ## Example
+    ## Examples
 
-    A simple `TextInput` with a default value of "John Doe" and a label:
-    Note: The value will not be updated if the user changes the value in the input field.
+    A simple `TextInput` with a default value of "John Doe" and a label. (Note:
+    The value will not be updated if the user changes the value in the input
+    field.)
 
     ```python
     rio.TextInput(text="John Doe", label="Name")
     ```
 
-    You can easily bind state variables to track changes. If you want to make your TextInput more
-    responsive, you can easily achieve this by adding a lambda function call to e.g. on_change:
+    You can easily bind state variables to track changes. If you want to make
+    your TextInput more responsive, you can easily achieve this by adding a
+    lambda function call to e.g. `on_change`:
 
     ```python
     class MyComponent(rio.Component):
         text: str = ""
 
         def build(self) -> rio.Component:
             return rio.TextInput(
-                text=self.bind().text,  # state binding
+                text=self.bind().text,  # attribute binding
                 label="Name",
                 on_change=lambda event: print(f"Name: {event.text}"),
             )
     ```
 
-    You can also use a method for updating the input text and do whatever you want. Note that methods
-    are handy if you want to do more than just updating the input text. For example run async code or
-    update other components based on the input text:
+    You can also use a method for updating the input text and do whatever you
+    want. Note that methods are handy if you want to do more than just updating
+    the input text. For example run async code or update other components based
+    on the input text:
 
     ```python
     class MyComponent(rio.Component):
         text: str = ""
 
         def on_change_update_text(self, event: rio.TextInputChangeEvent):
             self.text = event.text
@@ -131,15 +148,17 @@
             )
 
         if "text" in delta_state and not self.is_sensitive:
             raise AssertionError(
                 f"Frontend tried to set `TextInput.text` even though `is_sensitive` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_change event
         try:
             new_value = delta_state["text"]
         except KeyError:
             pass
         else:
             assert isinstance(new_value, str), new_value
```

### Comparing `rio_ui-0.5.9/src/rio/components/theme_context_switcher.py` & `rio_ui-0.6/rio/components/theme_context_switcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,37 +12,39 @@
     "ThemeContextSwitcher",
 ]
 
 
 @final
 class ThemeContextSwitcher(FundamentalComponent):
     """
-    # ThemeContextSwitcher
-
     A container which can switch between different components.
 
     A `ThemeContextSwitcher` is a container which can switch between different
     components. It is commonly used to switch between different themes. The
     `content` attribute can be used to change the currently displayed component.
 
+    You can find more details on theming on the [theming how-to
+    page](https://rio.dev/docs/howto/theming).
 
     ## Attributes
 
     `content`: The currently displayed component.
 
     `color`: The color of the switcher bar.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `ThemeContextSwitcher` will be shown:
-    TODO: check if this is the correct example
 
     ```python
-    rio.ThemeContextSwitcher(content=rio.Button("Button"), color="secondary")
+    rio.ThemeContextSwitcher(
+        content=rio.Button("Button"),
+        color="secondary"
+    )
     ```
     """
 
     content: rio.Component
     color: rio.ColorSet
 
     def _custom_serialize(self) -> JsonDoc:
```

### Comparing `rio_ui-0.5.9/src/rio/components/tooltip.py` & `rio_ui-0.6/rio/components/tooltip.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from typing import Literal, final
+from typing import TYPE_CHECKING, Literal, final
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Tooltip",
 ]
 
 
 @final
 class Tooltip(FundamentalComponent):
     """
-    # Tooltip
-
     A small pop-up window that appears when the user hovers over an element.
 
     `Tooltip` is a small pop-up window that appears when the user hovers over an
     element. It is commonly used to provide additional information about the
     element, such as a description or a hint.
 
 
@@ -29,32 +27,35 @@
 
     `tip`: The text or component to display in the tooltip.
 
     `position`: The position of the tooltip relative to the anchor. It can be
         one of the following values: `left`, `top`, `right`, `bottom`.
 
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Tooltip` will be shown:
 
     ```python
     rio.Tooltip(
         anchor=rio.Icon("material/info"),
         tip="This is a tooltip.",
         position="top",
     )
     ```
     """
 
     anchor: rio.Component
-    tip_text: str | None
-    tip_component: rio.Component | None
+    tip: str | rio.Component
     position: Literal["left", "top", "right", "bottom"]
 
+    # Hide internal attributes from the IDE
+    if not TYPE_CHECKING:
+        _tip_component: rio.Component | None
+
     # Impute a Text instance if a string is passed in as the tip
     def __init__(
         self,
         anchor: rio.Component,
         tip: str | rio.Component,
         position: Literal["left", "top", "right", "bottom"],
         *,
@@ -83,25 +84,27 @@
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
         )
 
         self.anchor = anchor
+        self.tip = tip
 
         if isinstance(tip, str):
-            self.tip_text = tip
-            self.tip_component = None
+            self._tip_text = tip
+            self._tip_component = None
         else:
-            self.tip_text = None
-            self.tip_component = tip
+            self._tip_text = None
+            self._tip_component = tip
 
         self.position = position
 
-        self._properties_set_by_creator_.update(("tip_text", "tip_component"))
+        self._properties_set_by_creator_.add("_tip_component")
 
     def __post_init__(self):
-        if isinstance(self.tip_text, str):
-            self.tip_component = rio.Text(self.tip_text)
+        # FIXME: This breaks attribute bindings
+        if isinstance(self._tip_text, str):
+            self._tip_component = rio.Text(self._tip_text)
 
 
 Tooltip._unique_id = "Tooltip-builtin"
```

### Comparing `rio_ui-0.5.9/src/rio/components/website.py` & `rio_ui-0.6/rio/components/website.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,24 @@
     "Website",
 ]
 
 
 @final
 class Website(FundamentalComponent):
     """
-    # Website
-
     Displays a website.
 
     `Website` takes a URL as input and displays that website in your app.
 
+
     ## Attributes
+    `url`: The URL of the website you want to display.
 
-        `url`: The URL of the website you want to display.
 
-    ## Example
+    ## Examples
 
     A minimal example of a `Website` will be shown:
 
     ```python
     rio.Website(url=rio.URL("https://www.example.com"))
     ```
     """
```

### Comparing `rio_ui-0.5.9/src/rio/debug/monkeypatches.py` & `rio_ui-0.6/rio/debug/monkeypatches.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from pathlib import Path
 from typing import *  # type: ignore
 
 import introspection.typing
 
 from .. import components, global_state
 from ..components.component import Component, ComponentMeta
-from ..state_properties import PleaseTurnThisIntoAStateBinding, StateProperty
+from ..state_properties import (
+    PleaseTurnThisIntoAnAttributeBinding,
+    StateProperty,
+)
 
 __all__ = [
     "apply_monkeypatches",
 ]
 
 
 def apply_monkeypatches() -> None:
@@ -19,15 +22,17 @@
     by `rio run` when running in debug mode.
     """
     introspection.wrap_method(Component_bind, Component, "bind")
     introspection.wrap_method(ComponentMeta_call, ComponentMeta, "__call__")
     introspection.wrap_method(StateProperty_get, StateProperty, "__get__")
     introspection.wrap_method(StateProperty_set, StateProperty, "__set__")
     introspection.wrap_method(LinearContainer_init, components.Row, "__init__")
-    introspection.wrap_method(LinearContainer_init, components.Column, "__init__")
+    introspection.wrap_method(
+        LinearContainer_init, components.Column, "__init__"
+    )
     introspection.wrap_method(ListView_init, components.ListView, "__init__")
 
 
 def Component_bind(wrapped_method, self: Component):
     if global_state.currently_building_session is None:
         raise RuntimeError(
             "`.bind()` can only be called inside of the `build()` method"
@@ -93,15 +98,15 @@
 def StateProperty_set(
     wrapped_method,
     self: StateProperty,
     instance: Component,
     value: object,
 ):
     # Type check the value
-    if not isinstance(value, PleaseTurnThisIntoAStateBinding):
+    if not isinstance(value, PleaseTurnThisIntoAnAttributeBinding):
         try:
             annotation = self._resolved_annotation
         except AttributeError:
             annotation = introspection.typing.resolve_forward_refs(
                 self._raw_annotation,
                 self._module,
                 mode="ast",
@@ -152,23 +157,30 @@
 ):
     # Proportions related checks
     if proportions is not None and not isinstance(proportions, str):
         proportions = list(proportions)
 
         # Make sure the number of proportions matches the number of children
         if len(proportions) != len(children):
+            if len(proportions) == 1:
+                proportions_str = f"one proportion was {proportions}"
+            else:
+                proportions_str = f"{len(proportions)} proportions were"
+
             raise ValueError(
-                f"The component has {len(children)} children, but {len(proportions)} proportions were provided."
+                f"The component has {len(children)} children, but {proportions_str} provided."
             )
 
         # The sum of all proportions must exceed 0
         if proportions and sum(proportions) <= 0:
-            # TODO: While this handles a lenght of zero children fine, JS
+            # TODO: While this handles a length of zero children fine, JS
             # probably doesn't!
-            raise ValueError("The sum of all proportions must be greater than 0.")
+            raise ValueError(
+                "The sum of all proportions must be greater than 0."
+            )
 
         # Every proportion must be positive
         for proportion in proportions:
             if proportion < 0:
                 raise ValueError(
                     f"{proportion} is not a valid proportion. All proportions must be greater than or equal to zero."
                 )
```

### Comparing `rio_ui-0.5.9/src/rio/debug/typing_utils.py` & `rio_ui-0.6/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/debug/validator.py` & `rio_ui-0.6/rio/debug/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,31 @@
         # Don't modify the original dict
         delta_state = copy.deepcopy(delta_state)
 
         # Get the component type
         try:
             type = delta_state.pop("_type_")
         except KeyError:
-            raise ValidationError(f"Component with id `{id}` is missing `_type_` field")
+            raise ValidationError(
+                f"Component with id `{id}` is missing `_type_` field"
+            )
 
         if not isinstance(type, str):
             raise ValidationError(
                 f"Component with id `{id}` has non-string type `{type}`"
             )
 
         if (
             type
             not in inspection.get_child_component_containing_attribute_names_for_builtin_components()
             and type not in registered_html_components
         ):
-            raise ValidationError(f"Component with id `{id}` has unknown type `{type}`")
+            raise ValidationError(
+                f"Component with id `{id}` has unknown type `{type}`"
+            )
 
         # Construct the result
         return cls(
             id=id,
             type=type,
             state=delta_state,
         )
@@ -219,15 +223,15 @@
         visited_ids: set[int] = set()
 
         to_do = [self.root_component]
 
         while to_do:
             current = to_do.pop()
 
-            # TODO Use this opportunity to detect cycles?
+            # Use this opportunity to detect cycles
             if current.id in visited_ids:
                 print(
                     f"Warning: Validator found a cycle in the component tree involving component with id `{current.id}`"
                 )
                 continue
 
             # Mark the current component as visited
@@ -267,15 +271,17 @@
                 continue
 
             if isinstance(value, int):
                 result[name] = self.as_json(self.components_by_id[value])
                 continue
 
             assert isinstance(value, list), value
-            result[name] = [self.as_json(self.components_by_id[id]) for id in value]
+            result[name] = [
+                self.as_json(self.components_by_id[id]) for id in value
+            ]
 
         return result
 
     def handle_incoming_message(self, msg: Any) -> None:
         """
         Process a message passed from Client -> Server.
 
@@ -328,15 +334,21 @@
         # Update the individual component states
         for component_id, delta_state in msg["deltaStates"].items():
             # Make sure the delta state isn't empty. While this isn't
             # technically invalid, the frontend relies on values such as the
             # margin and alignment to be present. This works, because those
             # values are generated by python regardless of whether they have
             # changed.
-            required_keys = {"_type_", "_margin_", "_size_", "_align_", "_grow_"}
+            required_keys = {
+                "_type_",
+                "_margin_",
+                "_size_",
+                "_align_",
+                "_grow_",
+            }
             missing_keys = required_keys - set(delta_state.keys())
 
             if missing_keys:
                 delta_state_nice = json.dumps(delta_state, indent=4)
                 raise ValidationError(
                     f"Delta state for with id `{component_id}` is missing required keys `{missing_keys}`. The full delta state follows:\n{delta_state_nice}"
                 )
@@ -369,15 +381,17 @@
 
                 # Update the component's state
                 component.state.update(delta_state)
 
         # Update the root component if requested
         if msg["rootComponentId"] is not None:
             try:
-                self.root_component = self.components_by_id[msg["rootComponentId"]]
+                self.root_component = self.components_by_id[
+                    msg["rootComponentId"]
+                ]
             except KeyError:
                 raise ValidationError(
                     f"Attempted to set root component to unknown component with id `{msg['rootComponentId']}`"
                 ) from None
 
         # If no root component is known yet, this message has to contain one
         if self.root_component is None:
@@ -407,27 +421,31 @@
         # Look for any components which were sent in the message, but are not
         # actually used in the component tree
         ids_sent = set(msg["deltaStates"].keys())
         ids_existing = set(self.components_by_id.keys())
         ids_superfluous = sorted(ids_sent - ids_existing)
 
         if ids_superfluous:
-            print(f"Validator Warning: Message contained superfluous component ids:")
+            print(
+                f"Validator Warning: Message contained superfluous component ids:"
+            )
 
             for id in ids_superfluous:
                 delta_state = msg["deltaStates"][id]
                 print(
                     f'-  {delta_state.get("_type_", "unknown type")} #{id}  -  {delta_state}'
                 )
 
         # Dump the client state if requested
         self.dump_client_state()
 
     def _handle_outgoing_evaluateJavascript(self, msg: Any):
         # Is this message registering a new component class?
-        match = re.search(r"window.componentClasses\['(.*)'\]", msg["javaScriptSource"])
+        match = re.search(
+            r"window.componentClasses\['(.*)'\]", msg["javaScriptSource"]
+        )
 
         if match is None:
             return
 
         # Remember the component class as registered
         self.registered_html_components.add(match.group(1))
```

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/component_details.py` & `rio_ui-0.6/rio/debug/client_side_debugger/component_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,18 +113,14 @@
                 column_index,
                 width=width,
             )
 
         # Any values which should be displayed right in the title
         header_accessories = []
 
-        # TODO: Display this only if rio itself (not the app!) is in debug mode
-        # if self.session._app_server.debug_mode:
-        #     header_accessories.append(rio.Text(f"#{target._id}", style="dim"))
-
         if target.key is not None:
             header_accessories = [
                 rio.Icon("material/key", fill="dim"),
                 rio.Text(
                     target.key,
                     style="dim",
                     justify="left",
@@ -170,15 +166,15 @@
 
         row_index_before_properties = row_index
         row_index += 1
 
         # Custom properties
         #
         # Make sure to skip any which already have custom tailored cells
-        debug_details = target.get_debug_details()
+        debug_details = target._get_debug_details()
         for prop_name, prop_value in debug_details.items():
             # Some values have special handling below
             if prop_name in (
                 "key",
                 "width",
                 "height",
                 "margin",
@@ -226,16 +222,20 @@
 
                 py_height_str = repr(py_height_str)
 
             # Spacing to separate the table from the rest
             row_index += 1
 
             # Header
-            result.add(rio.Text("width", style="dim", justify="left"), row_index, 1)
-            result.add(rio.Text("height", style="dim", justify="left"), row_index, 2)
+            result.add(
+                rio.Text("width", style="dim", justify="left"), row_index, 1
+            )
+            result.add(
+                rio.Text("height", style="dim", justify="left"), row_index, 2
+            )
             row_index += 1
 
             # The size as specified in Python
             add_cell("python", 0, True)
             add_cell(py_width_str, 1, False)
             add_cell(py_height_str, 2, False)
             row_index += 1
@@ -305,28 +305,28 @@
 
             add_cell("align_y", 2, True)
             add_cell(str(debug_details.get("align_y", "-")), 3, False)
             row_index += 1
 
         # Link to docs
         if type(target)._rio_builtin_:
-            docs_url = rio.docs.documentation_url(type(target).__name__)
+            docs_url = rio.docs.build_documentation_url(type(target).__name__)
             link_color = self.session.theme.secondary_color
 
             result.add(
                 rio.Link(
                     rio.Row(
                         rio.Icon("material/library-books", fill=link_color),
                         rio.Text("Docs", style=rio.TextStyle(fill=link_color)),
                         spacing=0.5,
                         align_x=0,
                     ),
                     docs_url,
                     # TODO: Support icons in links
-                    # new_tab=True,  # TODO: Support this
+                    open_in_new_tab=True,
                     margin_top=0.2,
                 ),
                 row_index,
                 0,
                 width=2,
             )
             row_index += 1
```

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/debugger.py` & `rio_ui-0.6/rio/debug/client_side_debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/deploy_page.py` & `rio_ui-0.6/rio/debug/client_side_debugger/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/icons_page.py` & `rio_ui-0.6/rio/debug/client_side_debugger/icons_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,17 +124,19 @@
 class IconsPage(rio.Component):
     _: KW_ONLY
     search_text: str = ""
     matches: list[tuple[str, str, tuple[str | None, ...]]] = dataclasses.field(
         default_factory=list
     )
 
-    selected_icon: str | None = None  # The selected icon, **including the icon set**
-    selected_icon_available_variants: tuple[str | None, ...] = dataclasses.field(
-        default_factory=tuple
+    selected_icon: str | None = (
+        None  # The selected icon, **including the icon set**
+    )
+    selected_icon_available_variants: tuple[str | None, ...] = (
+        dataclasses.field(default_factory=tuple)
     )
     selected_variant: str | None = None
     selected_fill: Literal[
         "primary",
         "secondary",
         "success",
         "warning",
@@ -173,17 +175,15 @@
             other_icon_set,
             other_icon_name,
             available_variants,
         ) in get_available_icons():
             if icon_name == other_icon_name and icon_set == other_icon_set:
                 break
         else:
-            assert (
-                False
-            ), f"There is no icon named `{icon_name}` in the `{icon_set}` icon set"
+            assert False, f"There is no icon named `{icon_name}` in the `{icon_set}` icon set"
 
         # Delegate to the regular function for this
         self._on_select_icon(icon_set, icon_name, available_variants)
 
         # Set any state that wasn't handled by the previous call
         self.search_text = icon_name
         self.selected_variant = icon_variant
@@ -236,24 +236,38 @@
         # If there is variations of this icon allow the user to select one
         # if len(self.selected_icon_available_variants) > 1:
         if True:
             variant_buttons = []
 
             for variant in self.selected_icon_available_variants:
                 full_name = (
-                    f"{self.selected_icon}:{variant}" if variant else self.selected_icon
+                    f"{self.selected_icon}:{variant}"
+                    if variant
+                    else self.selected_icon
                 )
 
+                if self.selected_fill == "dim":
+                    color = (
+                        self.session.theme.neutral_palette.foreground.replace(
+                            opacity=0.5
+                        )
+                    )
+                else:
+                    color = self.selected_fill
+
                 variant_buttons.append(
                     rio.Container(
                         rio.IconButton(
                             full_name,
                             style=(
-                                "minor" if variant == self.selected_variant else "plain"
+                                "minor"
+                                if variant == self.selected_variant
+                                else "plain"
                             ),
+                            color=color,
                             on_press=functools.partial(
                                 self._on_select_variant, variant
                             ),
                         ),
                         width="grow",
                         align_y=0.5,
                     )
@@ -343,15 +357,18 @@
                 is_selected = self.selected_icon == f"{icon_set}/{icon_name}"
 
                 results.append(
                     rio.IconButton(
                         f"{icon_set}/{icon_name}",
                         style="minor" if is_selected else "plain",
                         on_press=functools.partial(
-                            self._on_select_icon, icon_set, icon_name, icon_variants
+                            self._on_select_icon,
+                            icon_set,
+                            icon_name,
+                            icon_variants,
                         ),
                         key=f"{icon_set}/{icon_name}",
                     ),
                 )
 
             children.append(
                 rio.FlowContainer(
```

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/layout_preview.py` & `rio_ui-0.6/rio/debug/client_side_debugger/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/project_page.py` & `rio_ui-0.6/rio/debug/client_side_debugger/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/sample_icons_grid.py` & `rio_ui-0.6/rio/debug/client_side_debugger/sample_icons_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 GRID_N_COLUMNS = 6
 
 
 # Choose icons to display
 def find_icons_to_display() -> Iterable[str]:
     # Get a list of all available icons
     names_and_variants: list[tuple[str, str | None]] = list(
-        rio.icon_registry.IconRegistry.get_singleton().all_icons_in_set(ICON_SET)
+        rio.icon_registry.IconRegistry.get_singleton().all_icons_in_set(
+            ICON_SET
+        )
     )
 
     # Choose some at random
     result = random.sample(names_and_variants, GRID_N_ROWS * GRID_N_COLUMNS)
 
     # Convert to strings
     for name, variant in result:
         yield (
-            f"{ICON_SET}/{name}" if variant is None else f"{ICON_SET}/{name}:{variant}"
+            f"{ICON_SET}/{name}"
+            if variant is None
+            else f"{ICON_SET}/{name}:{variant}"
         )
 
 
 DISPLAYED_ICON_NAMES: list[str] = list(find_icons_to_display())
 
 
 class SampleIconsGrid(rio.Component):
```

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/theme_picker_page.py` & `rio_ui-0.6/rio/debug/client_side_debugger/theme_picker_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,127 @@
 import functools
 import io
 from typing import *  # type: ignore
 
 import rio
 
 
+def colors_equal(color1: rio.Color, color2: rio.Color) -> bool:
+    """
+    Returns `True` if the two colors are equal and `False` otherwise. Since
+    color values are stored as floats, this function applies a small fudge
+    factor to account for floating point differences.
+    """
+    epsilon = 1e-6
+
+    return (
+        abs(color1.red - color2.red) < epsilon
+        and abs(color1.green - color2.green) < epsilon
+        and abs(color1.blue - color2.blue) < epsilon
+        and abs(color1.opacity - color2.opacity) < epsilon
+    )
+
+
+def get_minimum_theme_kwargs(theme: rio.Theme) -> dict[str, Any]:
+    """
+    Given a theme, returns a dictionary with the minimum set of keyword
+    arguments required to recreate it.
+    """
+    # This is more complex than it might seem at first, because many colors are
+    # derived from other colors. For example, the neutral color is derived from
+    # the primary one.
+    result: dict[str, Any] = {}
+
+    # Light / dark mode can impact some colors. Make sure to get that value
+    # first.
+    if not theme.is_light_theme:
+        result["light"] = False
+
+    # Some colors don't depend on anything else
+    reference_theme = rio.Theme.from_colors(**result)
+
+    if not colors_equal(theme.primary_color, reference_theme.primary_color):
+        result["primary_color"] = theme.primary_color
+
+    if not colors_equal(theme.secondary_color, reference_theme.secondary_color):
+        result["secondary_color"] = theme.secondary_color
+
+    if not colors_equal(theme.disabled_color, reference_theme.disabled_color):
+        result["disabled_color"] = theme.disabled_color
+
+    if not colors_equal(theme.success_color, reference_theme.success_color):
+        result["success_color"] = theme.success_color
+
+    if not colors_equal(theme.warning_color, reference_theme.warning_color):
+        result["warning_color"] = theme.warning_color
+
+    if not colors_equal(theme.danger_color, reference_theme.danger_color):
+        result["danger_color"] = theme.danger_color
+
+    if not colors_equal(theme.hud_color, reference_theme.hud_color):
+        result["hud_color"] = theme.hud_color
+
+    # These depend on the previously defined ones
+    reference_theme = rio.Theme.from_colors(**result)
+
+    if not colors_equal(
+        theme.background_color, reference_theme.background_color
+    ):
+        result["background_color"] = theme.background_color
+
+    if not colors_equal(theme.neutral_color, reference_theme.neutral_color):
+        result["neutral_color"] = theme.neutral_color
+
+    # Header fill
+    #
+    # This is nontrivial, because there are many kinds of fill, and some of them
+    # can be hard to serialize. Only support solid colors for now.
+    heading_color = theme.heading1_style.fill
+    reference_heading_color = reference_theme.heading1_style.fill
+
+    assert isinstance(heading_color, rio.Color), heading_color
+    assert isinstance(
+        reference_heading_color, rio.Color
+    ), reference_heading_color
+
+    if isinstance(heading_color, rio.Color) and not colors_equal(
+        heading_color, reference_heading_color
+    ):
+        result["heading_fill"] = heading_color
+
+    # Corner radii
+    if theme.corner_radius_large != reference_theme.corner_radius_large:
+        result["corner_radius_large"] = theme.corner_radius_large
+
+    if theme.corner_radius_medium != reference_theme.corner_radius_medium:
+        result["corner_radius_medium"] = theme.corner_radius_medium
+
+    if theme.corner_radius_small != reference_theme.corner_radius_small:
+        result["corner_radius_small"] = theme.corner_radius_small
+
+    return result
+
+
 async def update_and_apply_theme(
     session: rio.Session,
     theme_replacements: dict[str, Any],
 ) -> None:
     """
     Overrides the session's theme with the given one, and makes sure to update
     all components so they use the new theme.
     """
 
-    # Build the new theme
-    updated_theme = session.theme.replace(**theme_replacements)
+    # Determine the kwargs to use for the theme
+    theme_kwargs = get_minimum_theme_kwargs(session.theme)
+    theme_kwargs.update(theme_replacements)
 
-    # The theme theme itself can preserve some values. For example, the primary
-    # color is encoded in the heading text style, so just replacing the primary
-    # palette won't make it go away.
-    #
-    # When passing the values, make sure to only change those that have been
-    # changed relative to the default,
-    #
-    # Take care of that.
-    new_theme = rio.Theme.from_color(
-        primary_color=updated_theme.primary_color,
-        secondary_color=updated_theme.secondary_color,
-        background_color=updated_theme.background_color,
-        neutral_color=updated_theme.neutral_color,
-        hud_color=updated_theme.hud_color,
-        disabled_color=updated_theme.disabled_color,
-        success_color=updated_theme.success_color,
-        warning_color=updated_theme.warning_color,
-        danger_color=updated_theme.danger_color,
-        corner_radius_small=updated_theme.corner_radius_small,
-        corner_radius_medium=updated_theme.corner_radius_medium,
-        corner_radius_large=updated_theme.corner_radius_large,
-        color_headings="auto",  # TODO: How to decide this?
-        light=updated_theme.background_color.perceived_brightness > 0.5,
-    )
+    # Build the new theme
+    new_theme = rio.Theme.from_colors(**theme_kwargs)
 
-    # Apply the theme
+    # Apply it
     await session._apply_theme(new_theme)
 
     # The application itself isn't enough, because some components will have
     # read theme values and used them to set e.g. their corner radii. Dirty
     # every component to force a full rebuild.
     for component in session._weak_components_by_id.values():
         session._register_dirty_component(
@@ -58,138 +133,99 @@
     await session._refresh()
 
 
 def get_source_for_theme(theme: rio.Theme, *, create_theme_pair: bool) -> str:
     """
     Given a theme, returns a string that can be used to recreate it.
     """
-    # Find all values that differ from the defaults
-    default_theme = rio.Theme.from_color()
-    changed_kwargs = {}
-
-    if theme.primary_color != default_theme.primary_color:
-        changed_kwargs["primary_color"] = theme.primary_color
-
-    if theme.secondary_color != default_theme.secondary_color:
-        changed_kwargs["secondary_color"] = theme.secondary_color
-
-    if theme.background_color != default_theme.background_color:
-        changed_kwargs["background_color"] = theme.background_color
-
-    if theme.neutral_color != default_theme.neutral_color:
-        changed_kwargs["neutral_color"] = theme.neutral_color
-
-    if theme.hud_color != default_theme.hud_color:
-        changed_kwargs["hud_color"] = theme.hud_color
-
-    if theme.disabled_color != default_theme.disabled_color:
-        changed_kwargs["disabled_color"] = theme.disabled_color
-
-    if theme.success_color != default_theme.success_color:
-        changed_kwargs["success_color"] = theme.success_color
-
-    if theme.warning_color != default_theme.warning_color:
-        changed_kwargs["warning_color"] = theme.warning_color
-
-    if theme.danger_color != default_theme.danger_color:
-        changed_kwargs["danger_color"] = theme.danger_color
-
-    if theme.corner_radius_small != default_theme.corner_radius_small:
-        changed_kwargs["corner_radius_small"] = round(theme.corner_radius_small, 1)
-
-    if theme.corner_radius_medium != default_theme.corner_radius_medium:
-        changed_kwargs["corner_radius_medium"] = round(theme.corner_radius_medium, 1)
-
-    if theme.corner_radius_large != default_theme.corner_radius_large:
-        changed_kwargs["corner_radius_large"] = round(theme.corner_radius_large, 1)
-
-    if theme.neutral_color.perceived_brightness < 0.5:
-        changed_kwargs["light"] = False
+    # Find all parameters which must be passed to create this theme
+    theme_parameters = get_minimum_theme_kwargs(theme)
 
     # Build the source
     theme_or_themes = "themes" if create_theme_pair else "theme"
     result = io.StringIO()
     result.write(f"# Create the {theme_or_themes}\n")
 
     if create_theme_pair:
-        result.write("themes = rio.Theme.pair_from_color(")
+        result.write("themes = rio.Theme.pair_from_colors(")
     else:
-        result.write("theme = rio.Theme.from_color(")
+        result.write("theme = rio.Theme.from_colors(")
 
-    if changed_kwargs:
+    if theme_parameters:
         result.write("\n")
 
-        for key, value in changed_kwargs.items():
+        for key, value in theme_parameters.items():
             result.write(f"    {key}=")
 
             if isinstance(value, rio.Color):
                 hex_value = value.hex
                 if len(hex_value) == 8 and hex_value.endswith("ff"):
                     hex_value = hex_value[:-2]
 
                 result.write(f"rio.Color.from_hex({hex_value!r})")
+            elif isinstance(value, bool):
+                result.write("True" if value else "False")
             elif isinstance(value, (int, float)):
-                result.write(repr(value))
+                result.write(f"{value:.2f}")
             else:
                 raise NotImplementedError(f"Unsupported type: {type(value)}")
 
             result.write(",\n")
 
     result.write(")\n")
     result.write("\n")
-    result.write(f"# And apply {'them' if create_theme_pair else 'it'} to your app\n")
+    result.write(
+        f"# And apply {'them' if create_theme_pair else 'it'} to your app\n"
+    )
     result.write("app = rio.App(\n")
     result.write("    ...\n")
     result.write(f"    theme={theme_or_themes},\n")
     result.write("    ...\n")
     result.write(")")
 
     # Done
     return result.getvalue()
 
 
 class PalettePicker(rio.Component):  #
     shared_open_key: str
 
     palette_nicename: str
-    palette_attribute_name: str
-
-    is_colorful_palette: bool
+    palette_slug: str
 
     pick_opacity: bool = False
 
     round_top: bool = False
     round_bottom: bool = False
 
     @property
     def palette(self) -> rio.Palette:
-        return getattr(self.session.theme, self.palette_attribute_name)
+        return getattr(self.session.theme, f"{self.palette_slug}_palette")
 
     async def _on_color_change(self, event: rio.ColorChangeEvent) -> None:
         await update_and_apply_theme(
             self.session,
             {
-                self.palette_attribute_name: rio.Palette._from_color(
-                    event.color,
-                    colorful=self.is_colorful_palette,
-                )
+                f"{self.palette_slug}_color": event.color,
             },
         )
 
     def _on_press(self, event: rio.PressEvent) -> None:
         # Toggle the popup
         if self.shared_open_key == self.palette_nicename:
             self.shared_open_key = ""
         else:
             self.shared_open_key = self.palette_nicename
 
     def build(self) -> rio.Component:
         palette = self.palette
 
-        top_radius = self.session.theme.corner_radius_medium if self.round_top else 0
+        top_radius = (
+            self.session.theme.corner_radius_medium if self.round_top else 0
+        )
         bottom_radius = (
             self.session.theme.corner_radius_medium if self.round_bottom else 0
         )
 
         return rio.Popup(
             anchor=rio.MouseEventListener(
                 rio.Rectangle(
@@ -257,18 +293,17 @@
     create_dark_theme: bool = False
 
     @rio.event.on_populate
     async def _on_populate(self) -> None:
         if self.theme_variants_are_initialized:
             return
 
-        current_theme_is_light = (
-            self.session.theme.background_color.perceived_brightness > 0.5
-        )
+        self.theme_variants_are_initialized = True
 
+        current_theme_is_light = self.session.theme.is_light_theme
         self.create_light_theme = current_theme_is_light
         self.create_dark_theme = not current_theme_is_light
 
     async def _on_radius_change(
         self,
         radius_name: str,
         event: rio.SliderChangeEvent,
@@ -276,159 +311,170 @@
         await update_and_apply_theme(
             self.session,
             {
                 radius_name: event.value,
             },
         )
 
-    def _toggle_create_light_theme(self) -> None:
+    async def _toggle_create_light_theme(self) -> None:
         self.create_light_theme = not self.create_light_theme
 
         if not self.create_light_theme and not self.create_dark_theme:
             self.create_dark_theme = True
 
-    def _toggle_create_dark_theme(self) -> None:
+        await update_and_apply_theme(
+            self.session,
+            {
+                "light": self.session.theme.is_light_theme
+                and self.create_light_theme,
+            },
+        )
+
+    async def _toggle_create_dark_theme(self) -> None:
         self.create_dark_theme = not self.create_dark_theme
 
         if not self.create_light_theme and not self.create_dark_theme:
             self.create_light_theme = True
 
+        await update_and_apply_theme(
+            self.session,
+            {
+                "light": self.session.theme.is_light_theme
+                or not self.create_dark_theme,
+            },
+        )
+
     def build(self) -> rio.Component:
         # Prepare the radius sliders
         slider_min = 0
         slider_max = 4
         radius_sliders = rio.Grid(
             (
-                rio.Text("Small"),
+                rio.Text(
+                    "Small",
+                    justify="left",
+                ),
                 rio.Slider(
                     value=self.session.theme.corner_radius_small,
                     minimum=slider_min,
                     maximum=slider_max,
                     width="grow",
                     on_change=functools.partial(
                         self._on_radius_change,
                         "corner_radius_small",
                     ),
                 ),
             ),
             (
-                rio.Text("Medium"),
+                rio.Text(
+                    "Medium",
+                    justify="left",
+                ),
                 rio.Slider(
                     value=self.session.theme.corner_radius_medium,
                     minimum=slider_min,
                     maximum=slider_max,
                     width="grow",
                     on_change=functools.partial(
                         self._on_radius_change,
                         "corner_radius_medium",
                     ),
                 ),
             ),
             (
-                rio.Text("Large"),
+                rio.Text(
+                    "Large",
+                    justify="left",
+                ),
                 rio.Slider(
                     value=self.session.theme.corner_radius_large,
                     minimum=slider_min,
                     maximum=slider_max,
                     width="grow",
                     on_change=functools.partial(
                         self._on_radius_change,
                         "corner_radius_large",
                     ),
                 ),
             ),
+            row_spacing=0.5,
         )
 
         # Combine everything
         return rio.ScrollContainer(
             content=rio.Column(
                 # Main Colors
-                # rio.Text(
-                #     "Theme Colors",
-                #     style="heading3",
-                #     margin_bottom=1,
-                #     justify='left',
-                # ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Primary",
-                    palette_attribute_name="primary_palette",
-                    is_colorful_palette=False,
+                    palette_slug="primary",
                     round_top=True,
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Secondary",
-                    palette_attribute_name="secondary_palette",
-                    is_colorful_palette=False,
+                    palette_slug="secondary",
                     round_bottom=True,
                 ),
                 # Neutral Colors
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Background",
-                    palette_attribute_name="background_palette",
-                    is_colorful_palette=False,
+                    palette_slug="background",
                     margin_top=1,
                     round_top=True,
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Neutral",
-                    palette_attribute_name="neutral_palette",
-                    is_colorful_palette=False,
+                    palette_slug="neutral",
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="HUD",
-                    palette_attribute_name="hud_palette",
-                    is_colorful_palette=False,
+                    palette_slug="hud",
                     pick_opacity=True,
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Disabled",
-                    palette_attribute_name="disabled_palette",
-                    is_colorful_palette=False,
+                    palette_slug="disabled",
                     round_bottom=True,
                 ),
                 # Semantic Colors
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Success",
-                    palette_attribute_name="success_palette",
-                    is_colorful_palette=True,
+                    palette_slug="success",
                     margin_top=1,
                     round_top=True,
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Warning",
-                    palette_attribute_name="warning_palette",
-                    is_colorful_palette=True,
+                    palette_slug="warning",
                 ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Danger",
-                    palette_attribute_name="danger_palette",
-                    is_colorful_palette=True,
+                    palette_slug="danger",
                     round_bottom=True,
                 ),
                 # Corner radii
                 rio.Text(
                     "Corner Radii",
                     style="heading3",
                     margin_top=1,
                     margin_bottom=1,
                     justify="left",
                 ),
                 radius_sliders,
                 # Theme Variants
                 rio.Text(
-                    "Theme Variants",
+                    "Variants",
                     style="heading3",
                     margin_top=1,
                     margin_bottom=1,
                     justify="left",
                 ),
                 rio.Row(
                     rio.Spacer(),
@@ -443,22 +489,24 @@
                         style="minor" if self.create_dark_theme else "plain",
                         on_press=self._toggle_create_dark_theme,
                     ),
                     rio.Spacer(),
                 ),
                 # Code Sample
                 rio.Text(
-                    "Code Sample",
+                    "Code",
                     style="heading3",
                     margin_top=1,
-                    # margin_bottom=1,  Not used for now, since markdown has an oddly large margin anyway
+                    margin_bottom=1,
                     justify="left",
                 ),
                 rio.Markdown(
                     f"""
+Use this code to recreate the current theme in your app:
+
 ```python
 {get_source_for_theme(self.session.theme, create_theme_pair=self.create_light_theme and self.create_dark_theme)}
 ```
                     """,
                 ),
                 margin=1,
                 align_y=0,
```

### Comparing `rio_ui-0.5.9/src/rio/debug/client_side_debugger/tree_page.py` & `rio_ui-0.6/rio/debug/client_side_debugger/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 
     try:
         return original_method(*args, **kwargs)
     finally:
         asyncio.windows_events.tasks = tasks_module  # type: ignore
 
 
-introspection.wrap_method(asyncio.windows_events.IocpProactor, accept)
+introspection.wrap_method(asyncio.windows_events.IocpProactor, accept)  # type: ignore
```

### Comparing `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/README.md` & `rio_ui-0.6/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/__init__.py` & `rio_ui-0.6/rio/snippets/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import copy
+import urllib.parse
 import functools
 import json
 import re
 from dataclasses import dataclass
 from pathlib import Path
 from typing import *  # type: ignore
 
@@ -83,15 +84,15 @@
     def is_binary_snippet(self) -> bool:
         return not self.is_text_snippet
 
     @staticmethod
     def from_path(group: str, name: str, file_path: Path) -> Snippet:
         # Read the contents if it's a text snippet
         if file_path.suffix in (".txt", ".md", ".py", ".json"):
-            raw_code = file_path.read_text()
+            raw_code = file_path.read_text(encoding="utf-8")
         else:
             raw_code = None
 
         return Snippet(
             group=group,
             name=name,
             file_path=file_path,
@@ -210,15 +211,15 @@
     ## Raises
 
     `KeyError`: If there is no group with the given name.
     """
     all_groups = _get_all_snippet_paths()
     group_dict = all_groups.get(group, {})
 
-    return (
+    return tuple(
         Snippet.from_path(group, name, file_path)
         for name, file_path in group_dict.items()
     )
 
 
 @functools.lru_cache(maxsize=None)
 def get_snippet(group: str, name: str) -> Snippet:
@@ -351,19 +352,23 @@
             elif snippet.file_path.suffix == ".py":
                 other_python_files.append(snippet)
 
             else:
                 assert False, f"Unrecognized snippet file `{snippet.file_path}`"
 
         # Create the project template
-        assert readme_snippet is not None, f"`README.md` snippet not found for `{name}`"
+        assert (
+            readme_snippet is not None
+        ), f"`README.md` snippet not found for `{name}`"
         assert (
             thumbnail_snippet is not None
         ), f"`thumbnail.svg` snippet not found for {name}"
-        assert metadata is not None, f"`meta.json` snippet not found for `{name}`"
+        assert (
+            metadata is not None
+        ), f"`meta.json` snippet not found for `{name}`"
         assert (
             root_init_snippet is not None
         ), f"`root_init.py` snippet not found for `{name}`"
 
         return ProjectTemplate(
             name=name,
             level=metadata.level,
@@ -415,7 +420,74 @@
                 ],
             )
         )
 
     # This function can't simply yield, because of the `lru_cache`. Instead,
     # return something immutable.
     return tuple(result)
+
+
+@dataclass
+class HowtoGuide:
+    """
+    Represents a how-to guide.
+    """
+
+    # A URL-safe unique identifier for the how-to guide
+    slug: str
+
+    # A human-readable name of the how-to guide
+    title: str
+
+    # The markdown source of the how-to guide. This does not contain a title
+    markdown_source: str
+
+    @staticmethod
+    def from_snippet(snip: Snippet) -> HowtoGuide:
+        """
+        Creates a `Howto` instance from a snippet. The snippet must contain
+        the howto's markdown source and start with a # heading.
+        """
+        # Split the markdown source into title and content
+        full_source = snip.stripped_code()
+        lines = full_source.split("\n", 1)
+        assert (
+            len(lines) == 2
+        ), f"Snippet `{snip.name}` is either missing a title or the content"
+        title, content = lines
+
+        # Clean up the title
+        title = title.strip()
+        assert title.startswith(
+            "#"
+        ), f"The source for snippet `{snip.name}` does not start with a heading?"
+        title = title[1:].strip()
+
+        # Clean up the content
+        content = content.strip()
+
+        # Derive the slug from the snippet's name
+        assert snip.name.endswith(".md"), snip.name
+        slug = snip.name[:-3]
+        assert slug == urllib.parse.quote(slug), slug
+
+        # Build the result
+        return HowtoGuide(
+            slug=slug,
+            title=title,
+            markdown_source=content,
+        )
+
+
+@functools.lru_cache(maxsize=None)
+def get_howto_guides() -> Iterable[HowtoGuide]:
+    """
+    Iterates over all available how-to guides.
+    """
+    result = []
+
+    for snip in all_snippets_in_group("howtos"):
+        result.append(HowtoGuide.from_snippet(snip))
+
+    # This function can't simply yield, because of the `lru_cache`. Instead,
+    # return something immutable.
+    return tuple(result)
```

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,57 +8,70 @@
 
 # </additional-imports>
 
 
 # <component>
 class CryptoCard(rio.Component):
     """
-    The CryptoCard class is a component of a dashboard application, designed to handle
-    and display cryptocurrency-related data. It uses the rio library to create
-    interactive dashboard components and pandas DataFrame to store cryptocurrency data.
-
-    The build method creates a rio.Card component that displays a line plot of the last
-    50 data points of the cryptocurrency, the cryptocurrency's logo, the name and ticker
-    symbol of the cryptocurrency, the amount of the cryptocurrency, and the amount of
-    the cryptocurrency in USD. The layout of the card is a grid with 4 rows and 2 columns.
+    Handle and display cryptocurrency-related data.
 
-    If there is no data available for the cryptocurrency, a message is printed to the console.
+    Show a card with a line plot of the last 50 data points of the
+    cryptocurrency, the cryptocurrency's logo, the name and ticker symbol of the
+    cryptocurrency, the amount of the cryptocurrency, and the amount of the
+    cryptocurrency in USD.
 
 
     ## Attributes
-        data: A pandas DataFrame that holds the cryptocurrency data.
-        coin: A string representing the name of the cryptocurrency.
-        coin_amount: A float representing the amount of the cryptocurrency.
-        coin_ticker: A string representing the ticker symbol of the cryptocurrency.
-        logo_url: A string representing the URL of the cryptocurrency's logo.
-
-    ## Layout
-    ```
-    ╔══════════════════ CARD ════════════════════╗
-    ║ ┏━━━━━━━━━━━━━┳━━ GRID ━━━━━━━━━━━━━━━━━━┓ ║
-    ║ ┃             ┃                          ┃ ║
-    ║ ┃ Image       ┃ Plot                     ┃ ║
-    ║ ┃             ┃                          ┃ ║
-    ║ ┣━━━━━━━━━━━━━╋━━━━━━━━━━━━━━━━━━━━━━━━━━┫ ║
-    ║ ┃ Coin Ticker ┃ Coin Amount              ┃ ║
-    ║ ┣━━━━━━━━━━━━━╋━━━━━━━━━━━━━━━━━━━━━━━━━━┫ ║
-    ║ ┃ Coin Name   ┃ Coin Amount in USD       ┃ ║
-    ║ ┗━━━━━━━━━━━━━┻━━━━━━━━━━━━━━━━━━━━━━━━━━┛ ║
-    ╚════════════════════════════════════════════╝
-    ```
+
+    `data`: Historical data of the fetched crypto coins.
+
+    `coin`: Name of the selected coin.
+
+    `coin_amount`: Representing the amount of the selected coin.
+
+    `coin_ticker`: Representing the ticker symbol of the cryptocurrency.
+
+    `logo_url`: Representing the URL of the cryptocurrency's logo.
     """
 
     data: pd.DataFrame
     coin: str
     coin_amount: float
     coin_ticker: str
     color: str
     logo_url: str
 
     def build(self) -> rio.Component:
+        """
+        Create a card with a line plot of the last 50 data points of the
+        cryptocurrency, the cryptocurrency's logo, the name and ticker symbol of
+        the cryptocurrency, the amount of the cryptocurrency, and the amount of
+        the cryptocurrency in USD.
+
+        See the approx. layout below:
+        ```
+        ╔══════════════════════════════ Card ═════════════════════════════╗
+        ║ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━ Grid ━━━━━━━━━━━━━━━━━━━━━━━━━━━┓ ║
+        ║ ┃ ┏━━━━━━ Image ━━━━━┓ ┏━━━━━━━━━━━━━━ Plot ━━━━━━━━━━━━━━━━┓ ┃ ║
+        ║ ┃ ┃ e.g. BTC Logo    ┃ ┃ e.g. line plot of BTC data         ┃ ┃ ║
+        ║ ┃ ┃                  ┃ ┃                                    ┃ ┃ ║
+        ║ ┃ ┃                  ┃ ┃                                    ┃ ┃ ║
+        ║ ┃ ┃                  ┃ ┃                                    ┃ ┃ ║
+        ║ ┃ ┗━━━━━━━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ ┃ ║
+        ║ ┃ ┏━━━━━━ Text ━━━━━━┓ ┏━━━━━━━━━━━━━━ Text ━━━━━━━━━━━━━━━━┓ ┃ ║
+        ║ ┃ ┃ Coin Ticker      ┃ ┃ Coin Amount                        ┃ ┃ ║
+        ║ ┃ ┗━━━━━━━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ ┃ ║
+        ║ ┃ ┏━━━━━━ Text ━━━━━━┓ ┏━━━━━━━━━━━━━━ Text ━━━━━━━━━━━━━━━━┓ ┃ ║
+        ║ ┃ ┃ Coin Name        ┃ ┃ Coin Amount in USD                 ┃ ┃ ║
+        ║ ┃ ┗━━━━━━━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ ┃ ║
+        ║ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ ║
+        ╚═════════════════════════════════════════════════════════════════╝
+        ```
+        """
+        # create a line plot of the last 50 data points of the selected coin
         fig = px.line(
             self.data[self.coin].iloc[-50:],
             color_discrete_sequence=[self.color],
             height=200,
             width=200,
         )
 
@@ -71,32 +84,23 @@
 
         # strip down the rest of the plot
         fig.update_layout(
             showlegend=False,
             margin=dict(t=10, l=10, b=10, r=10),
         )
 
+        # create a grid layout for the card
+        # The grid will have 4 rows and 3 columns
+        # Because the width of the plot is bigger, we get a ratio of 2:1
         grid = rio.Grid(
             column_spacing=0.5,
             row_spacing=1,
             margin=2,
         )
 
-        # Create a grid layout for the card
-        # The grid will have 4 rows and 2 columns
-        # Because the width of the plot is bigger, the second column will be wider
-        # like shown below:
-
-        ############################################
-        # Icon        | Plot                       #
-        # Icon        | Plot                       #
-        # Coin Ticker | Coin Amount                #
-        # Coin Name   | Coin Amount in USD         #
-        ############################################
-
         # Image with grid height 2
         grid.add(
             rio.Image(
                 rio.URL(
                     self.logo_url
                 ),  # logo_url = e.g. "https://cryptologos.cc/logos/bitcoin-btc-logo.svg?v=029"
                 height=2,
```

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 
 @dataclass
 class MenuItems:
     """
     MenuItems data model.
 
     ## Attributes
-        name: The name of the menu item.
-        description: The description of the menu item.
-        price: The price of the menu item.
-        category: The category of the menu item.
+
+    `name`: The name of the menu item.
+
+    `description`: The description of the menu item.
+
+    `price`: The price of the menu item.
+
+    `category`: The category of the menu item.
     """
 
     name: str
     description: str
     price: float
     category: str
 
     @staticmethod
     def new_empty() -> "MenuItems":
         """
-        Creates a new empty MenuItems object.
-
-        Returns:
-            MenuItems: A new empty MenuItems object.
+        Creates a new empty MenuItems object. Which is used for creating new menu item.
         """
         return MenuItems(
             name="",
             description="",
             price=0.0,
             category="",
         )
 
 
-# initial data
+# initialize some data
 MENUITEMSET: list[MenuItems] = [
     MenuItems(
         name="Hamburger",
         description="A classic hamburger with lettuce, tomato, and onions",
         price=4.99,
         category="Burgers",
     ),
```

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,16 @@
         # Spawn components for the fields
         field_components: list[rio.Component] = []
 
         for index, field in enumerate(self.fields):
             field_components.append(
                 comps.Field(
                     value=field,
-                    dim=self.winner is not None and index not in self.winning_indices,
+                    dim=self.winner is not None
+                    and index not in self.winning_indices,
                     on_press=functools.partial(self.on_press, index),
                 )
             )
 
         # Come up with a status message
         if self.winner in ("X", "O"):
             message = f"{self.winner} has won!"
```

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
         # Spawn components for the fields
         field_components: list[rio.Component] = []
 
         for index, field in enumerate(self.fields):
             field_components.append(
                 comps.Field(
                     value=field,
-                    dim=self.winner is not None and index not in self.winning_indices,
+                    dim=self.winner is not None
+                    and index not in self.winning_indices,
                     on_press=functools.partial(self.on_press, index),
                 )
             )
 
         # Come up with a status message
         if self.winner in ("X", "O"):
             message = f"{self.winner} has won!"
```

### Comparing `rio_ui-0.5.9/tests/test_custom_components.py` & `rio_ui-0.6/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_docstring_code_blocks.py` & `rio_ui-0.6/tests/test_docstring_code_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 import subprocess
 import tempfile
 from typing import *  # type: ignore
 
 import black
+import imy.docstrings
 import pyright
 import pytest
 
 import rio
-import rio.docs
 
 CODE_BLOCK_PATTERN = re.compile(r"```.*?\n(.*?)\n```", re.DOTALL)
 
 
 def all_components() -> list[Type[rio.Component]]:
     """
     Iterates over all components that ship with Rio.
@@ -28,15 +28,15 @@
     return result
 
 
 def get_code_blocks(comp: Type[rio.Component]) -> list[str]:
     """
     Returns a list of all code blocks in the docstring of a component.
     """
-    docs = rio.docs.ClassDocs.parse(comp)
+    docs = imy.docstrings.ClassDocs.from_class(comp)
 
     # No docs?
     if docs.details is None:
         return []
 
     # Find any contained code blocks
     result: list[str] = []
```

### Comparing `rio_ui-0.5.9/tests/test_events.py` & `rio_ui-0.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_project_templates.py` & `rio_ui-0.6/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_reconciliation.py` & `rio_ui-0.6/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_refresh.py` & `rio_ui-0.6/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_session.py` & `rio_ui-0.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_state_bindings.py` & `rio_ui-0.6/tests/test_attribute_bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import cast
 
 from utils import create_mockapp
 
 import rio
-from rio.state_properties import PleaseTurnThisIntoAStateBinding
+from rio.state_properties import PleaseTurnThisIntoAnAttributeBinding
 
 
 class Parent(rio.Component):
     text: str = ""
 
     def build(self):
         return rio.Text(self.bind().text)
@@ -17,25 +17,25 @@
     text: str = ""
 
     def build(self):
         return Parent(self.bind().text)
 
 
 async def test_bindings_arent_created_too_early():
-    # There was a time when state bindings were created in `Component.__init__`,
+    # There was a time when attribute bindings were created in `Component.__init__`,
     # thus skipping any properties that were only assigned later.
     class IHaveACustomInit(rio.Component):
         text: str
 
         def __init__(self, *args, text: str, **kwargs):
             super().__init__(*args, **kwargs)
 
             # `Component.__init__`` has already run, but we haven't assigned
             # `self.text` yet. Do it now and assert that it still becomes a
-            # state binding.
+            # attribute binding.
             self.text = text
 
         def build(self) -> rio.Component:
             return rio.Text(self.text)
 
     class Container(rio.Component):
         text: str = "hi"
@@ -49,16 +49,16 @@
 
         assert child_component.text == "hi"
 
         root_component.text = "bye"
         assert child_component.text == "bye"
 
 
-async def test_init_receives_state_bindings_as_input():
-    # For a while we considered initializing state bindings before calling a
+async def test_init_receives_attribute_bindings_as_input():
+    # For a while we considered initializing attribute bindings before calling a
     # component's `__init__` and passing the values of the bindings as arguments
     # into `__init__`. But ultimately we decided against it, because some
     # components may want to use state properties/bindings in their __init__. So
     # make sure the `__init__` actually receives a
     # `PleaseTurnThisIntoAStateBinding` object as input.
     size_value = None
 
@@ -75,15 +75,15 @@
     class Container(rio.Component):
         size: float
 
         def build(self) -> rio.Component:
             return Square(self.bind().size)
 
     async with create_mockapp(lambda: Container(7)):
-        assert isinstance(size_value, PleaseTurnThisIntoAStateBinding)
+        assert isinstance(size_value, PleaseTurnThisIntoAnAttributeBinding)
 
 
 async def test_binding_assignment_on_child():
     async with create_mockapp(Parent) as app:
         root_component = app.get_component(Parent)
         text_component = app.get_build_output(root_component, rio.Text)
 
@@ -119,15 +119,16 @@
                 rio.Text(self.bind().text),
                 rio.Text(self.bind().text),
             )
 
     async with create_mockapp(Root) as app:
         root_component = app.get_component(Root)
         text1, text2 = cast(
-            list[rio.Text], app.get_build_output(root_component, rio.Column).children
+            list[rio.Text],
+            app.get_build_output(root_component, rio.Column).children,
         )
 
         assert not app.dirty_components
 
         text1.text = "Hello"
 
         assert app.dirty_components == {root_component, text1, text2}
```

### Comparing `rio_ui-0.5.9/tests/test_user_settings.py` & `rio_ui-0.6/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.9/tests/test_zzz_guardrails.py` & `rio_ui-0.6/tests/test_zzz_guardrails.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ):
     _ = rio.PageView(fallback_build=component_cls)
 
 
 @pytest.mark.parametrize(
     "component_cls",
     [
-        rio.Rectangle,
+        rio.Dropdown,
         rio.Text,
     ],
 )
 @enable_component_instantiation
 def test_component_class_cant_be_used_as_build_function(
     component_cls: type[rio.Component],
 ):
@@ -78,15 +78,17 @@
 
 
 async def test_init_cannot_read_state_properties():
     # Accessing state properties in `__init__` is not allowed because state
     # bindings aren't initialized yet at that point. In development mode, trying
     # to access a state property in `__init__` should raise an exception.
     init_executed = False
-    accessing_foo_raised_exception = accessing_margin_top_raised_exception = False
+    accessing_foo_raised_exception = accessing_margin_top_raised_exception = (
+        False
+    )
 
     class IllegalComponent(rio.Component):
         foo: int
 
         def __init__(self, foo: int):
             super().__init__()
```

### Comparing `rio_ui-0.5.9/tests/utils.py` & `rio_ui-0.6/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,34 +90,42 @@
     def last_component_state_changes(
         self,
     ) -> Mapping[rio.Component, Mapping[str, object]]:
         for message in reversed(self.outgoing_messages):
             if message["method"] == "updateComponentStates":
                 delta_states: dict = message["params"]["deltaStates"]  # type: ignore
                 return {
-                    self.session._weak_components_by_id[int(component_id)]: delta
+                    self.session._weak_components_by_id[
+                        int(component_id)
+                    ]: delta
                     for component_id, delta in delta_states.items()
                     if int(component_id) != self.session._root_component._id
                 }
 
         return {}
 
     def get_root_component(self) -> rio.Component:
         sess = self.session
 
         high_level_root = sess._root_component
-        assert isinstance(high_level_root, HighLevelRootComponent), high_level_root
+        assert isinstance(
+            high_level_root, HighLevelRootComponent
+        ), high_level_root
 
         low_level_root = sess._weak_component_data_by_component[
             high_level_root
         ].build_result
-        assert isinstance(low_level_root, FundamentalRootComponent), low_level_root
+        assert isinstance(
+            low_level_root, FundamentalRootComponent
+        ), low_level_root
 
         scroll_container = low_level_root.content
-        assert isinstance(scroll_container, rio.ScrollContainer), scroll_container
+        assert isinstance(
+            scroll_container, rio.ScrollContainer
+        ), scroll_container
 
         return scroll_container.content
 
     def get_components(self, component_type: type[C]) -> Iterator[C]:
         root_component = self.get_root_component()
 
         for component in root_component._iter_component_tree():
@@ -131,18 +139,22 @@
             raise AssertionError(f"No component of type {component_type} found")
 
     def get_build_output(
         self,
         component: rio.Component,
         type_: type[C] | None = None,
     ) -> C:
-        result = self.session._weak_component_data_by_component[component].build_result
+        result = self.session._weak_component_data_by_component[
+            component
+        ].build_result
 
         if type_ is not None:
-            assert type(result) is type_, f"Expected {type_}, got {type(result)}"
+            assert (
+                type(result) is type_
+            ), f"Expected {type_}, got {type(result)}"
 
         return result  # type: ignore
 
     async def refresh(self) -> None:
         await self.session._refresh()
 
 
@@ -176,15 +188,17 @@
         headers={"accept": "text/html"},
     )
     await app_server._serve_index(fake_request, "")
 
     [[session_token, session]] = app_server._active_session_tokens.items()
 
     if use_ordered_dirty_set:
-        session._dirty_components = ordered_set.OrderedSet(session._dirty_components)  # type: ignore
+        session._dirty_components = ordered_set.OrderedSet(
+            session._dirty_components
+        )  # type: ignore
 
     mock_app = MockApp(session, user_settings=user_settings)
 
     fake_websocket: Any = types.SimpleNamespace(
         client="1.2.3.4",
         accept=lambda: _make_awaitable(),
         send_text=mock_app._send_message,
@@ -196,15 +210,17 @@
 
     async def serve_websocket():
         try:
             await app_server._serve_websocket(fake_websocket, session_token)
         except asyncio.CancelledError:
             pass
         except Exception as error:
-            test_task.cancel(f"Exception in AppServer._serve_websocket: {error}")
+            test_task.cancel(
+                f"Exception in AppServer._serve_websocket: {error}"
+            )
         else:
             test_task.cancel(
                 "AppServer._serve_websocket exited unexpectedly. An exception"
                 " must have occurred in the `init_coro`."
             )
 
     server_task = asyncio.create_task(serve_websocket())
@@ -241,15 +257,17 @@
         )
         session._decimal_separator = "."
         session._thousands_separator = ","
         session._send_message = _fake_send_message
         session._receive_message = _fake_receive_message
 
         rio.global_state.currently_building_session = session
-        session._root_component = HighLevelRootComponent(build, lambda: rio.Text(""))
+        session._root_component = HighLevelRootComponent(
+            build, lambda: rio.Text("")
+        )
 
         rio.global_state.currently_building_component = session._root_component
         try:
             session._root_component.build()
         finally:
             rio.global_state.currently_building_component = None
             rio.global_state.currently_building_session = None
```

### Comparing `rio_ui-0.5.9/README.md` & `rio_ui-0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,78 @@
-![Rio](https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=)
-![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
-![Discord](https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square)
-![Python Version](https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square)
-![License](https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square)
-![GitHub Stars](https://img.shields.io/github/stars/rio-labs/rio?style=flat-square)
+<p align="center">
+  <img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem; height: 8.8rem"/>
+</p>
+
+<p align="center">
+  <strong>Rio</strong> is an easy to use framework for creating websites and apps and is based <strong>entirely on Python</strong>. 🐍
+  <br>
+  You <strong>won't need a single line of HTML, CSS, or
+  JavaScript</strong> to create beautiful, modern apps.<br><br>
+  <a href="https://rio.dev/get-started">Tutorial</a> - <a href="https://rio.dev/examples">Examples</a> - <a href="https://discord.gg/7ejXaPwhyH">Discord</a> - <a href="https://rio.dev/docs">Docs</a> - <a href="https://github.com/rio-labs/rio">Source Code</a><br><br>
+  Rio brings React-style components to Python. Pull from a wealth of built-in
+  components and combine them to create your own custom components. Then combine
+  those into entire apps. Best of all, Rio apps can run both locally on your
+  machine and on the web.
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=" alt="Rio"/>
+  <img src="https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square" alt="Version"/>
+  <!--
+  <img src="https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square" alt="Discord"/>
+  -->
+  <img src="https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square" alt="Python Version"/>
+  <img src="https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square" alt="License"/>
+  <!--
+  <img src="https://img.shields.io/github/stars/rio-labs/rio?style=flat-square" alt="GitHub Stars"/>
+  -->
+</p>
 
-<!-- https://shields.io/badges -->
+![dall_e_example](https://github.com/rio-labs/rio/assets/41641225/44279406-0c2d-47e2-98b5-4582722054b2)
 
-<img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem" />
-
-🌊 You've arrived at **Rio**, an easy to use framework for creating websites and
-apps.
-
-🐍 Rio is based **entirely on Python**. You **won't need a single line of HTML, CSS, or
-JavaScript** to create beautiful, modern apps.
-
-[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://github.com/rio-labs/rio)
-
-Rio brings React-style components to Python. Pull from a wealth of built-in
-components and combine them to create your own custom components. Then combine
-those into entire apps. Best of all, Rio apps can run both locally on your
-machine and on the web.
 
 ## Features 🧩
 
 -   Modern, **declarative UI** framework
 -   **100% Python** - Zero HTML, CSS, or JavaScript required
 -   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
 -   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
 -   Apps can run **both locally and on the web**
+-   **Dev tools** included
 -   **Open Source & Free forever**
 
+## Example ⌨️
+
+```python
+# Define a component that counts button clicks
+class ButtonClicker(rio.Component):
+    # Define the attributes of the component. Changing these will
+    # affect the GUI.
+    clicks: int = 0
+
+    # Define a method that increments the click count. We'll later
+    # make a button that calls this method whenever it is pressed.
+    def _on_press(self) -> None:
+        self.clicks += 1
+
+    # Define the `build` method. This method essentially tells rio
+    # what a ButtonClicker component looks like. Whenever the state
+    # of the ButtonClicker component changes, rio will call its
+    # `build` method and update the GUI according to the output.
+    def build(self) -> rio.Component:
+        return rio.Column(
+            rio.Button('Click me', on_press=self._on_press),
+            rio.Text(f'You clicked the button {self.clicks} time(s)'),
+        )
+
+# Create an App and tell it to display a ButtonClicker when it starts
+app = rio.App(build=ButtonClicker)
+app.run_in_browser()
+```
+
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
 ```
@@ -53,106 +91,19 @@
 rio new my-project --type website --template "Tic-Tac-Toe"
 cd my-project
 rio run
 ```
 
 You'll have your first app up and running in seconds!
 
-## How it works 🧠
-
-TODO: Minimal example
-
-```python
-from typing import *  # type: ignore
-import rio
-from openai import AsyncOpenAI
-
-client = AsyncOpenAI()
-
-
-class DallEPage(rio.Component):
-    prompt: str = ""
-    image_url: str = ""
-    is_loading: bool = False
-
-    async def get_image(self) -> None:
-        """Get an image by prompt."""
-
-        self.is_loading = True
-        await self.force_refresh()
-
-        if self.prompt == "":
-            self.image_url = ""
-            self.is_loading = False
-            return
-
-        try:
-            response = await client.images.generate(
-                model="dall-e-2",
-                prompt=self.prompt,
-                size="256x256",
-                quality="standard",
-                n=1,
-            )
-            self.image_url = response.data[0].url
-
-        finally:
-            self.is_loading = False
-
-    def build(self) -> rio.Component:
-
-        return rio.Rectangle(
-            content=rio.Card(
-                rio.Column(
-                    rio.Text("DALL-E", style="heading1"),
-                    rio.TextInput(
-                        text=self.bind().prompt,
-                        label="Prompt:",
-                    ),
-                    rio.Button(
-                        "Create Image",
-                        on_press=self.get_image,
-                        is_loading=self.is_loading,
-                    ),
-                    # Add the image to the page if it exists
-                    *(
-                        [
-                            rio.Image(
-                                rio.URL(self.image_url),
-                                height=36,
-                            )
-                        ]
-                        if self.image_url
-                        else []
-                    ),
-                    spacing=1,
-                    margin=2,
-                ),
-                width=40,
-                align_x=0.5,
-                align_y=0.5,
-                margin=2,
-            ),
-            fill=rio.Color.GREY,
-        )
-
-
-# Run the app
-app = rio.App(
-    pages=[
-        rio.Page(
-            name="Home",
-            page_url="",
-            build=DallEPage,
-        ),
-    ],
-)
-```
-
 ## Status: In Development 🚧
 
 Rio is still in development. We're working hard to bring you the best possible
 experience. If you have any feedback, please let us know on [our Discord server](https://discord.gg/7ejXaPwhyH).
 
-## Contributing 🤝
+## Community Support 🤝
+
+For general help using Rio, please refer to the [official Rio documentation](https://rio.dev/docs). For additional help, you can use one of these channels to ask a question:
 
-TODO: Write how someone can contribute to the project. :)
+-   [Discord](https://discord.gg/7ejXaPwhyH) (For live discussion with the Community and Rio team)
+-   [GitHub](https://github.com/rio-labs/rio) (Bug reports, Contributions)
+-   [Community Forum](https://github.com/rio-labs/rio/discussions) (Questions and Discussions)
```

### Comparing `rio_ui-0.5.9/pyproject.toml` & `rio_ui-0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [project]
 name = "rio-ui"
 description = "Build modern Websites and Apps just with Python"
 dynamic = ["version"]
 authors = [
     { name = "Jakob Pinterits", email = "jakob.pinterits@gmail.com" },
-    { name = "Paul Pinterits" },
+    { name = "Paul Pinterits", email = "rawing7@gmail.com" },
 ]
 dependencies = [
     "aiofiles~=23.2.1",
     "fastapi~=0.110",
     "fuzzywuzzy~=0.18.0",
     "gitignore-parser~=0.1.9",
     "httpx~=0.25.1",
-    "imy~=0.2.4",
-    "introspection~=1.7.14",
+    "imy~=0.3.0",
+    "introspection~=1.8",
     "isort~=5.13.2",
     "keyring~=24.3.0",
     "pillow~=10.2.0",
     "pytest~=7.3.1",
     "python-levenshtein~=0.23.0",
     "python-multipart~=0.0.6",
     "pytz~=2024.1",
     "revel~=0.9.0",
     "timer-dict~=1.0.0",
     "tomlkit~=0.12.3",
     "typing-extensions>=4.5.0",
     "unicall~=0.1.5",
-    "uniserde~=0.3.12",
+    "uniserde~=0.3.13",
     "uvicorn[standard]~=0.23.2",
     "watchfiles~=0.21.0",
-    "yarl~=1.9.2",
+    "yarl>=1.9.4",
 ]
 requires-python = ">= 3.10"
 readme = "README.md"
-license.text = "LGPL-3.0" # TODO
+license.text = "LGPL-3.0" # LAUNCH-TODO
 keywords = [
     "web-development",
     "web-framework",
     "framework",
     "functional",
     "type-safe",
     "typing",
@@ -52,16 +52,19 @@
     "rio",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Information Technology",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)", # TODO
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.optional-dependencies]
 window = [
@@ -81,32 +84,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 dev-dependencies = [
     "alt-pytest-asyncio~=0.7.2",
+    "black~=24.4.0",
     "coverage~=7.2.2",
     "pre-commit~=3.1.1",
-    "pyfakefs~=5.3.0",
     "pytest~=7.3.1",
     "pyright~=1.1.350",
+    "requests~=2.31",
     "ruff~=0.4.1",
+    "pandas>=2.2.2",
+    "polars>=0.20.23",
+    "pywebview",
 ]
 managed = true
 
 [tool.rye.scripts]
-build = "npm run-script build"
-dev-build = "npm run-script dev-build"
-publish = "echo FIXME"
-
-[tool.hatch.metadata]
-allow-direct-references = true
+# check-docs = { call = "scripts.check_docs:main" }
+build = "npm run build"
+dev-build = "npm run dev-build"
+publish = { call = "scripts.publish_new_release:main" }
 
 [tool.hatch.version]
-path = "src/rio/__init__.py"
+path = "rio/__init__.py"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/rio"]
+packages = ["rio"]
+artifacts = ["rio/generated/*"]
+
+[tool.hatch.build.targets.sdist]
+artifacts = ["rio/generated/*"]
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+line-length = 80
```

### Comparing `rio_ui-0.5.9/PKG-INFO` & `rio_ui-0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,131 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.5.9
+Version: 0.6
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: documentation, https://rio.dev/docs
-Author: Paul Pinterits
-Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>
+Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: LGPL-3.0
 License-File: LICENSE.txt
 Keywords: app,framework,functional,local-app,modern,react,rio,type-safe,typed,typing,user-interface,web,web-app,web-development,web-framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: fastapi~=0.110
 Requires-Dist: fuzzywuzzy~=0.18.0
 Requires-Dist: gitignore-parser~=0.1.9
 Requires-Dist: httpx~=0.25.1
-Requires-Dist: imy~=0.2.4
-Requires-Dist: introspection~=1.7.14
+Requires-Dist: imy~=0.3.0
+Requires-Dist: introspection~=1.8
 Requires-Dist: isort~=5.13.2
 Requires-Dist: keyring~=24.3.0
 Requires-Dist: pillow~=10.2.0
 Requires-Dist: pytest~=7.3.1
 Requires-Dist: python-levenshtein~=0.23.0
 Requires-Dist: python-multipart~=0.0.6
 Requires-Dist: pytz~=2024.1
 Requires-Dist: revel~=0.9.0
 Requires-Dist: timer-dict~=1.0.0
 Requires-Dist: tomlkit~=0.12.3
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: unicall~=0.1.5
-Requires-Dist: uniserde~=0.3.12
+Requires-Dist: uniserde~=0.3.13
 Requires-Dist: uvicorn[standard]~=0.23.2
 Requires-Dist: watchfiles~=0.21.0
-Requires-Dist: yarl~=1.9.2
+Requires-Dist: yarl>=1.9.4
 Provides-Extra: window
 Requires-Dist: cefpython3~=66.1; (sys_platform == 'win32') and extra == 'window'
 Requires-Dist: platformdirs~=3.11.0; extra == 'window'
 Requires-Dist: pygobject~=3.44.1; (sys_platform == 'linux') and extra == 'window'
 Requires-Dist: pywebview~=4.2.2; extra == 'window'
 Description-Content-Type: text/markdown
 
-![Rio](https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=)
-![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
-![Discord](https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square)
-![Python Version](https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square)
-![License](https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square)
-![GitHub Stars](https://img.shields.io/github/stars/rio-labs/rio?style=flat-square)
+<p align="center">
+  <img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem; height: 8.8rem"/>
+</p>
+
+<p align="center">
+  <strong>Rio</strong> is an easy to use framework for creating websites and apps and is based <strong>entirely on Python</strong>. 🐍
+  <br>
+  You <strong>won't need a single line of HTML, CSS, or
+  JavaScript</strong> to create beautiful, modern apps.<br><br>
+  <a href="https://rio.dev/get-started">Tutorial</a> - <a href="https://rio.dev/examples">Examples</a> - <a href="https://discord.gg/7ejXaPwhyH">Discord</a> - <a href="https://rio.dev/docs">Docs</a> - <a href="https://github.com/rio-labs/rio">Source Code</a><br><br>
+  Rio brings React-style components to Python. Pull from a wealth of built-in
+  components and combine them to create your own custom components. Then combine
+  those into entire apps. Best of all, Rio apps can run both locally on your
+  machine and on the web.
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=" alt="Rio"/>
+  <img src="https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square" alt="Version"/>
+  <!--
+  <img src="https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square" alt="Discord"/>
+  -->
+  <img src="https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square" alt="Python Version"/>
+  <img src="https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square" alt="License"/>
+  <!--
+  <img src="https://img.shields.io/github/stars/rio-labs/rio?style=flat-square" alt="GitHub Stars"/>
+  -->
+</p>
 
-<!-- https://shields.io/badges -->
+![dall_e_example](https://github.com/rio-labs/rio/assets/41641225/44279406-0c2d-47e2-98b5-4582722054b2)
 
-<img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem" />
-
-🌊 You've arrived at **Rio**, an easy to use framework for creating websites and
-apps.
-
-🐍 Rio is based **entirely on Python**. You **won't need a single line of HTML, CSS, or
-JavaScript** to create beautiful, modern apps.
-
-[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://github.com/rio-labs/rio)
-
-Rio brings React-style components to Python. Pull from a wealth of built-in
-components and combine them to create your own custom components. Then combine
-those into entire apps. Best of all, Rio apps can run both locally on your
-machine and on the web.
 
 ## Features 🧩
 
 -   Modern, **declarative UI** framework
 -   **100% Python** - Zero HTML, CSS, or JavaScript required
 -   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
 -   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
 -   Apps can run **both locally and on the web**
+-   **Dev tools** included
 -   **Open Source & Free forever**
 
+## Example ⌨️
+
+```python
+# Define a component that counts button clicks
+class ButtonClicker(rio.Component):
+    # Define the attributes of the component. Changing these will
+    # affect the GUI.
+    clicks: int = 0
+
+    # Define a method that increments the click count. We'll later
+    # make a button that calls this method whenever it is pressed.
+    def _on_press(self) -> None:
+        self.clicks += 1
+
+    # Define the `build` method. This method essentially tells rio
+    # what a ButtonClicker component looks like. Whenever the state
+    # of the ButtonClicker component changes, rio will call its
+    # `build` method and update the GUI according to the output.
+    def build(self) -> rio.Component:
+        return rio.Column(
+            rio.Button('Click me', on_press=self._on_press),
+            rio.Text(f'You clicked the button {self.clicks} time(s)'),
+        )
+
+# Create an App and tell it to display a ButtonClicker when it starts
+app = rio.App(build=ButtonClicker)
+app.run_in_browser()
+```
+
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
 ```
@@ -104,106 +144,19 @@
 rio new my-project --type website --template "Tic-Tac-Toe"
 cd my-project
 rio run
 ```
 
 You'll have your first app up and running in seconds!
 
-## How it works 🧠
-
-TODO: Minimal example
-
-```python
-from typing import *  # type: ignore
-import rio
-from openai import AsyncOpenAI
-
-client = AsyncOpenAI()
-
-
-class DallEPage(rio.Component):
-    prompt: str = ""
-    image_url: str = ""
-    is_loading: bool = False
-
-    async def get_image(self) -> None:
-        """Get an image by prompt."""
-
-        self.is_loading = True
-        await self.force_refresh()
-
-        if self.prompt == "":
-            self.image_url = ""
-            self.is_loading = False
-            return
-
-        try:
-            response = await client.images.generate(
-                model="dall-e-2",
-                prompt=self.prompt,
-                size="256x256",
-                quality="standard",
-                n=1,
-            )
-            self.image_url = response.data[0].url
-
-        finally:
-            self.is_loading = False
-
-    def build(self) -> rio.Component:
-
-        return rio.Rectangle(
-            content=rio.Card(
-                rio.Column(
-                    rio.Text("DALL-E", style="heading1"),
-                    rio.TextInput(
-                        text=self.bind().prompt,
-                        label="Prompt:",
-                    ),
-                    rio.Button(
-                        "Create Image",
-                        on_press=self.get_image,
-                        is_loading=self.is_loading,
-                    ),
-                    # Add the image to the page if it exists
-                    *(
-                        [
-                            rio.Image(
-                                rio.URL(self.image_url),
-                                height=36,
-                            )
-                        ]
-                        if self.image_url
-                        else []
-                    ),
-                    spacing=1,
-                    margin=2,
-                ),
-                width=40,
-                align_x=0.5,
-                align_y=0.5,
-                margin=2,
-            ),
-            fill=rio.Color.GREY,
-        )
-
-
-# Run the app
-app = rio.App(
-    pages=[
-        rio.Page(
-            name="Home",
-            page_url="",
-            build=DallEPage,
-        ),
-    ],
-)
-```
-
 ## Status: In Development 🚧
 
 Rio is still in development. We're working hard to bring you the best possible
 experience. If you have any feedback, please let us know on [our Discord server](https://discord.gg/7ejXaPwhyH).
 
-## Contributing 🤝
+## Community Support 🤝
+
+For general help using Rio, please refer to the [official Rio documentation](https://rio.dev/docs). For additional help, you can use one of these channels to ask a question:
 
-TODO: Write how someone can contribute to the project. :)
+-   [Discord](https://discord.gg/7ejXaPwhyH) (For live discussion with the Community and Rio team)
+-   [GitHub](https://github.com/rio-labs/rio) (Bug reports, Contributions)
+-   [Community Forum](https://github.com/rio-labs/rio/discussions) (Questions and Discussions)
```

