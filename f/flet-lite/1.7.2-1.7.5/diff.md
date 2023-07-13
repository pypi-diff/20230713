# Comparing `tmp/flet_lite-1.7.2.tar.gz` & `tmp/flet_lite-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_lite-1.7.2.tar", last modified: Sun Jul  9 17:31:31 2023, max compression
+gzip compressed data, was "flet_lite-1.7.5.tar", last modified: Thu Jul 13 18:36:30 2023, max compression
```

## Comparing `flet_lite-1.7.2.tar` & `flet_lite-1.7.5.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 17:31:22.000000 flet_lite-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-09 17:31:22.000000 flet_lite-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-09 17:31:31.924562 flet_lite-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 17:31:22.000000 flet_lite-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/manage_client_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_add_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_clean_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_go_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_page_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_remove_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_update_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/cli_tools/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/flet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/append_assets_to_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/edit_control_props.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/tools/platform_specifics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/get_platform_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/pythonista_webview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/run_event_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/setup_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/update_control_on_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/update_page_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.900563 flet_lite-1.7.2/flet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/all_props_posible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/api_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/appbar_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/control_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_all_subcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_control_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_free_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/page_posible_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/view_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/web_host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.904563 flet_lite-1.7.2/flet/web/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4313577 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/development.zip
--rw-r--r--   0 runner    (1001) docker     (123)  4292224 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/dist.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.920562 flet_lite-1.7.2/flet_core/
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/alert_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/animated_switcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/app_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/border.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/border_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/bottom_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/callable_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.920562 flet_lite-1.7.2/flet_core/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/oval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/flet_core/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_axis_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_point_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_point_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/pie_chart_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/circle_avatar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/client_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/constrained_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/control_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/datatable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/divider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/drag_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/draggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/elevated_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/embed_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/file_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/filled_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/filled_tonal_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/flet_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/floating_action_button.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/form_field_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/gesture_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/grid_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/haptic_feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icon_button.py
--rw-r--r--   0 runner    (1001) docker     (123)   362652 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/inline_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/list_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/list_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/local_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/matplotlib_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/navigation_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/navigation_rail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/outlined_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/popup_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/progress_ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/radio_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/responsive_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/scrollable_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/semantics.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/session_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shader_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shake_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/snack_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/template_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/textfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/transparent_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/user_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/vertical_divider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/window_drag_area.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/flet_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 17:31:22.000000 flet_lite-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:31:31.924562 flet_lite-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-09 17:31:22.000000 flet_lite-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.984136 flet_lite-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 18:36:18.000000 flet_lite-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 18:36:18.000000 flet_lite-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-13 18:36:30.984136 flet_lite-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-13 18:36:18.000000 flet_lite-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.948134 flet_lite-1.7.5/flet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.948134 flet_lite-1.7.5/flet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/manage_client_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_add_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_clean_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_go_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_page_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_remove_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/api/push_update_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.948134 flet_lite-1.7.5/flet/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/cli_tools/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/flet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.952134 flet_lite-1.7.5/flet/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/append_assets_to_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/edit_control_props.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.952134 flet_lite-1.7.5/flet/tools/platform_specifics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/platform_specifics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/platform_specifics/get_platform_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/platform_specifics/pythonista_webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/run_event_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/setup_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/update_control_on_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/tools/update_page_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.956134 flet_lite-1.7.5/flet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/all_props_posible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/api_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/appbar_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/control_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/get_all_subcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/get_control_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/get_free_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/page_posible_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/view_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/utils/web_host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.960135 flet_lite-1.7.5/flet/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/web/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4313789 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/web/development.zip
+-rw-r--r--   0 runner    (1001) docker     (123)  4292224 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet/web/dist.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.980136 flet_lite-1.7.5/flet_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/alert_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/animated_switcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/app_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/border.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/border_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/bottom_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/callable_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.980136 flet_lite-1.7.5/flet_core/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/oval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/canvas/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.984136 flet_lite-1.7.5/flet_core/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/chart_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/chart_point_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/line_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/circle_avatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/client_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/constrained_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/control_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/drag_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/draggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/elevated_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/embed_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/filled_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/filled_tonal_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/flet_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/floating_action_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/form_field_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/gesture_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/grid_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/haptic_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/icon_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)   362652 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/inline_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/list_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/list_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/local_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/matplotlib_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/navigation_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/navigation_rail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/outlined_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/popup_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/progress_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/radio_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/responsive_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/scrollable_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/shader_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/shake_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/snack_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/template_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/text_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/text_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/transparent_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/user_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/vertical_divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-13 18:36:18.000000 flet_lite-1.7.5/flet_core/window_drag_area.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:30.984136 flet_lite-1.7.5/flet_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-13 18:36:30.000000 flet_lite-1.7.5/flet_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-13 18:36:30.000000 flet_lite-1.7.5/flet_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:36:30.000000 flet_lite-1.7.5/flet_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 18:36:30.000000 flet_lite-1.7.5/flet_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:36:30.000000 flet_lite-1.7.5/flet_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 18:36:18.000000 flet_lite-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:36:30.984136 flet_lite-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 18:36:18.000000 flet_lite-1.7.5/setup.py
```

### Comparing `flet_lite-1.7.2/LICENSE` & `flet_lite-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/PKG-INFO` & `flet_lite-1.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_lite
-Version: 1.7.2
+Version: 1.7.5
 Summary: A tiny version of flet to work on mobile development
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.7.2/README.md` & `flet_lite-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/.DS_Store` & `flet_lite-1.7.5/flet/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/api/manage_client_pushes.py` & `flet_lite-1.7.5/flet/api/manage_client_pushes.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/api/push_page_update_request.py` & `flet_lite-1.7.5/flet/api/push_page_update_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from ..utils.get_control_data import get_control_props
 from ..utils.appbar_coder import appbar_to_dict
 from ..utils.page_posible_props import all_page_posible_props
 from ..tools.edit_control_props import edit_control_props
 from ..utils.view_coder import view_to_dict
+from ..utils.control_coder import control_to_dict
 import jsonpickle, json, flet
 
 
 def push_page_update_request (page_class):
     """Request to remove a control"""
     push_data = {
         "ok" : True,
         "action" : "page_update",
         "props" : {},
         "appbar" : None,
-        "views" : []
+        "views" : [],
+        "overlay" : []
     }
 
     edit_control_props(control=page_class)
     
     for p in all_page_posible_props:
         if hasattr(page_class, p):
             push_data['props'][p] = getattr(page_class, p)
@@ -30,9 +32,12 @@
             page_class.__dict__[i] = "center"
 
     if page_class.appbar != None:
         push_data['appbar'] = appbar_to_dict(page_class.appbar)
     
     for v in page_class.views:
         push_data["views"].append(view_to_dict(view=v))
+    
+    for olc in page_class.overlay:
+        push_data['overlay'].append (control_to_dict(control=olc, overlay=True))
 
     page_class.api_host.add_update_on_wait (push_data)
```

### Comparing `flet_lite-1.7.2/flet/cli_tools/publish.py` & `flet_lite-1.7.5/flet/cli_tools/publish.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/flet.py` & `flet_lite-1.7.5/flet/flet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal
 from .page import Page
-import signal, sys
+import signal, sys, shutil, os
 
 
 WEB_BROWSER = "web_browser"
 FLET_APP = "flet_app"
 FLET_APP_WEB = "flet_app_web"
 FLET_APP_HIDDEN = "flet_app_hidden"
 
@@ -34,14 +34,16 @@
     # Define a signal handler function
     def signal_handler(signal, frame):
         print("""
 Program is closed!
 Give the project a rate at github if you did like it: https://github.com/SKbarbon/flet_lite
 Create an issue if there is one: https://github.com/SKbarbon/flet_lite/issues
 """)
+        if os.path.isdir ("web") and os.path.isfile("web/index.html"):
+            shutil.rmtree("web")
         sys.exit()
 
     # Set the signal handler for SIGINT (Ctrl+C)
     signal.signal(signal.SIGINT, signal_handler)
 
     # open a loop so the threads of the two hosts not closed.
     still_open = True
```

### Comparing `flet_lite-1.7.2/flet/page.py` & `flet_lite-1.7.5/flet/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         
         # page class's flet props
         self.appbar = None
         self.route = "/"
         self.last_control_number = 0
         self.__controls_are_pushed = [] # The controls that did be on the page at least once.
         self.views = []
+        self.overlay = []
         self.controls = []
         self.controls_dict_numbers = {}
     
     def start_target (self):
         """When the host and client browser are ready, this is will be called to start the target function."""
         print("Connected to a browser..")
         try:
@@ -75,14 +76,16 @@
             control.page = self
             control.parent = parent
             control.flet_lite_number = self.last_control_number
             self.last_control_number = self.last_control_number + 1
             self.controls_dict_numbers[f'{control.flet_lite_number}'] = control
             self.__controls_are_pushed.append(control)
             control = control.build()
+        
+        control.is_overlay = False
         control.flet_lite_number = self.last_control_number
         control.parent = parent
         control.page = self
 
         push_add_request(controls=[control], page_class=self)
         if control not in self.__controls_are_pushed:
             self.__controls_are_pushed.append(control)
@@ -95,29 +98,46 @@
         self.last_control_number = self.last_control_number + 1
 
         if hasattr (control, "controls"):
             for I in control.controls:
                 self.add(I, parent=control.flet_lite_number)
         elif hasattr(control, "content"):
             if control.content != None:
-                self.add(control=control.content, parent=control.flet_lite_number)
+                self.add(control=control.content, parent=control.flet_lite_number)    
+
+    def setup_overlay_control (self, c:flet.Control):
+        c.flet_lite_number = self.last_control_number
+        self.last_control_number = self.last_control_number + 1
+
+        c.page = self
+        c.is_overlay = True
+        c.parent = "page"
+
+        self.controls_dict_numbers[f"{c.flet_lite_number}"] = c
+
+        return c
+
     
     def update (self, *controls):
         # push the controls that are not pushed yet
         for con in self.controls:
             if con not in self.__controls_are_pushed:
                 self.add(con)
         
         for sub_con in get_all_subControls_on_the_page(parent=self):
             if sub_con not in self.__controls_are_pushed:
                 if hasattr(sub_con, "parent"):
                     self.add(sub_con, parent=sub_con.parent.flet_lite_number)
                 else:
                     self.add(sub_con)
         
+        # push controls that are overlay and still not pushed
+        for overlay_control in self.overlay:
+            self.setup_overlay_control(c=overlay_control)
+        
         # update sub controls
         all_controls_to_update = []
         for control in controls:
             all_controls_to_update.append(control)
             for i in get_all_subControls_on_the_page(control):
                 if i.page != None: i.page = self
                 all_controls_to_update.append(i)
```

### Comparing `flet_lite-1.7.2/flet/publish.py` & `flet_lite-1.7.5/flet/publish.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/tools/append_assets_to_dist.py` & `flet_lite-1.7.5/flet/tools/append_assets_to_dist.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/tools/platform_specifics/pythonista_webview.py` & `flet_lite-1.7.5/flet/tools/platform_specifics/pythonista_webview.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/tools/run_event_function.py` & `flet_lite-1.7.5/flet/tools/run_event_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
             threading.Thread(target=function_, args=[e], daemon=True).start()
     # ----
     if hasattr(control, event_function_name):
         e = Event(target="", name=f"{event_function_name}", data=event_data)
         e.control = control
         e.page = page_class
         if getattr(control, event_function_name) != None:
+            if append_keys != None:
+                for k in append_keys:
+                    setattr(e, k, append_keys[k])
             if not hasattr(getattr(control, event_function_name), "__dict__"):
                 do_event_function()
             elif getattr(control, event_function_name).__dict__ == {}:
-                if append_keys != None:
-                    for k in append_keys:
-                        setattr(e, k, append_keys[k])
                 do_event_function()
             elif getattr(control, event_function_name).__dict__['_EventHandler__handlers'] != {}:
                 do_event_function()
```

### Comparing `flet_lite-1.7.2/flet/tools/setup_web.py` & `flet_lite-1.7.5/flet/tools/setup_web.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/tools/update_page_info.py` & `flet_lite-1.7.5/flet/tools/update_page_info.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/all_props_posible.py` & `flet_lite-1.7.5/flet/utils/all_props_posible.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,9 +18,12 @@
         "value", "weight", "autofocus",
         "border_width", "can_reveal_password", "counter_text",
         "cursor_color", "cursor_height", "cursor_radius", "cursor_width",
         "dense", "error_style", "filled", "focused_bgcolor", "focused_border_color", 
         "helper_style", "helper_text", "hint_text", "label", "max_length", "max_lines",
         "min_lines", "multiline", "password", "read_only", "prefix_text", "text_size",
         "expand", "disabled", "alignment", "width", "height", "border_radius", "text",
-        "scroll", "auto_scroll", "icon", "name", "src", "src_base64"
+        "scroll", "auto_scroll", "icon", "name", "src", "src_base64",
+        "allowed_extensions", "allow_multiple", "dialog_title", "file_name",
+        "file_type", "initial_directory", "state", "autoplay", "balance", "playback_rate",
+        "volume"
     ]
```

### Comparing `flet_lite-1.7.2/flet/utils/api_host.py` & `flet_lite-1.7.5/flet/utils/api_host.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/appbar_coder.py` & `flet_lite-1.7.5/flet/utils/appbar_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/control_coder.py` & `flet_lite-1.7.5/flet/utils/control_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/get_all_subcontrols.py` & `flet_lite-1.7.5/flet/utils/get_all_subcontrols.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/get_control_data.py` & `flet_lite-1.7.5/flet/utils/get_control_data.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/page_posible_props.py` & `flet_lite-1.7.5/flet/utils/page_posible_props.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/view_coder.py` & `flet_lite-1.7.5/flet/utils/view_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/utils/web_host.py` & `flet_lite-1.7.5/flet/utils/web_host.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/web/.DS_Store` & `flet_lite-1.7.5/flet/web/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet/web/development.zip` & `flet_lite-1.7.5/flet/web/development.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 4313577 bytes, number of entries: 129
-drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 10:44 dist/
--rwxr-xr-x  2.0 unx      263 bX defN 23-Jul-07 10:44 __MACOSX/._dist
+Zip file size: 4313789 bytes, number of entries: 129
+drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-13 16:57 dist/
+-rwxr-xr-x  2.0 unx      263 bX defN 23-Jul-13 16:57 __MACOSX/._dist
 -rw-r--r--  2.0 unx       92 bX defN 23-Jun-14 17:06 dist/version.json
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._version.json
 -rw-r--r--  2.0 unx       32 bX defN 23-Jun-14 17:06 dist/.last_build_id
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._.last_build_id
 -rw-r--r--  2.0 unx     3521 bX defN 23-Jun-18 18:19 dist/index.html
 -rw-r--r--  2.0 unx      219 bX defN 23-Jun-18 18:19 __MACOSX/dist/._index.html
 -rw-r--r--  2.0 unx     6148 bX defN 23-Jul-06 14:40 dist/.DS_Store
 -rw-r--r--  2.0 unx      120 bX defN 23-Jul-06 14:40 __MACOSX/dist/._.DS_Store
-drwx------  2.0 unx        0 bx stor 23-Jul-07 12:22 dist/app/
--rwx------  2.0 unx      220 bX defN 23-Jul-07 12:22 __MACOSX/dist/._app
+drwx------  2.0 unx        0 bx stor 23-Jul-13 16:57 dist/app/
+-rwx------  2.0 unx      220 bX defN 23-Jul-13 16:57 __MACOSX/dist/._app
 -rw-r--r--  2.0 unx  5440180 bX defN 23-Jun-14 17:06 dist/main.dart.js
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._main.dart.js
 -rw-r--r--  2.0 unx    14240 bX defN 23-Jun-14 17:06 dist/flutter.js
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._flutter.js
 -rw-r--r--  2.0 unx     8319 bX defN 23-Jun-14 17:06 dist/flutter_service_worker.js
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._flutter_service_worker.js
 -rw-r--r--  2.0 unx     1573 bX defN 23-Jun-14 17:06 dist/python-worker.js
@@ -27,25 +27,25 @@
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/._manifest.json
 -rw-r--r--  2.0 unx  2125653 bX defN 23-Jun-15 19:03 dist/app.tar.gz
 -rw-r--r--  2.0 unx      319 bX defN 23-Jun-15 19:03 __MACOSX/dist/._app.tar.gz
 drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-15 19:03 dist/assets/
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/._assets
 -rw-r--r--  2.0 unx      744 bX defN 23-Jun-14 17:06 dist/python.js
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/._python.js
-drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-05 07:44 dist/app/tools/
--rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-05 07:44 __MACOSX/dist/app/._tools
+drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 18:44 dist/app/tools/
+-rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/._tools
 -rw-r--r--  2.0 unx     6148 bX defN 23-Jul-03 17:16 dist/app/.DS_Store
 -rw-r--r--  2.0 unx      120 bX defN 23-Jul-03 17:16 __MACOSX/dist/app/._.DS_Store
-drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 11:05 dist/app/flet_utils/
--rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 11:05 __MACOSX/dist/app/._flet_utils
+drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 18:44 dist/app/flet_utils/
+-rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/._flet_utils
 -rw-r--r--  2.0 unx       13 bX defN 23-Jun-15 19:03 dist/app/requirements.txt
-drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 10:41 dist/app/api/
--rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 10:41 __MACOSX/dist/app/._api
--rw-r--r--  2.0 unx     3207 bX defN 23-Jul-07 11:10 dist/app/main.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 11:10 __MACOSX/dist/app/._main.py
+drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 18:44 dist/app/api/
+-rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/._api
+-rw-r--r--  2.0 unx     3207 bX defN 23-Jul-13 14:00 dist/app/main.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 14:00 __MACOSX/dist/app/._main.py
 -rw-r--r--  2.0 unx    17040 bX defN 23-Jun-14 17:06 dist/icons/loading-animation.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/icons/._loading-animation.png
 -rw-r--r--  2.0 unx     4699 bX defN 23-Jun-14 17:06 dist/icons/apple-touch-icon-192.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/icons/._apple-touch-icon-192.png
 -rw-r--r--  2.0 unx     6622 bX defN 23-Jun-14 17:06 dist/icons/icon-192.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/icons/._icon-192.png
 -rw-r--r--  2.0 unx     4128 bX defN 23-Jun-14 17:06 dist/icons/icon-maskable-192.png
@@ -64,68 +64,68 @@
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/assets/._packages
 drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-15 19:03 dist/assets/shaders/
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/assets/._shaders
 -rw-r--r--  2.0 unx      229 bX defN 23-Jun-14 17:06 dist/assets/AssetManifest.smcbin
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/._AssetManifest.smcbin
 drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-15 19:03 dist/assets/fonts/
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/assets/._fonts
--rw-r--r--  2.0 unx     1642 bX defN 23-Jul-07 10:42 dist/app/tools/manage_host_updates.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 10:42 __MACOSX/dist/app/tools/._manage_host_updates.py
--rw-r--r--  2.0 unx      815 bX defN 23-Jul-02 19:40 dist/app/tools/post_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-02 19:40 __MACOSX/dist/app/tools/._post_request.py
--rw-r--r--  2.0 unx      986 bX defN 23-Jul-05 12:09 dist/app/flet_utils/hook_control_events.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-05 12:09 __MACOSX/dist/app/flet_utils/._hook_control_events.py
--rw-r--r--  2.0 unx      389 bX defN 23-Jul-07 10:33 dist/app/flet_utils/manage_page_events.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 10:33 __MACOSX/dist/app/flet_utils/._manage_page_events.py
--rw-r--r--  2.0 unx     1157 bX defN 23-Jul-07 11:27 dist/app/flet_utils/appbar_coder.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 11:27 __MACOSX/dist/app/flet_utils/._appbar_coder.py
--rw-r--r--  2.0 unx     1294 bX defN 23-Jul-06 14:30 dist/app/flet_utils/get_all_subcontrols.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-06 14:30 __MACOSX/dist/app/flet_utils/._get_all_subcontrols.py
--rw-r--r--  2.0 unx       95 bX defN 23-Jul-05 09:48 dist/app/flet_utils/control_actions.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-05 09:48 __MACOSX/dist/app/flet_utils/._control_actions.py
--rw-r--r--  2.0 unx      623 bX defN 23-Jul-06 16:40 dist/app/flet_utils/flet_control_generator.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-06 16:40 __MACOSX/dist/app/flet_utils/._flet_control_generator.py
--rw-r--r--  2.0 unx      471 bX defN 23-Jul-06 14:33 dist/app/flet_utils/append_to_content.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-06 14:33 __MACOSX/dist/app/flet_utils/._append_to_content.py
--rw-r--r--  2.0 unx      973 bX defN 23-Jul-07 12:21 dist/app/flet_utils/view_coder.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 12:21 __MACOSX/dist/app/flet_utils/._view_coder.py
--rw-r--r--  2.0 unx      848 bX defN 23-Jul-07 11:56 dist/app/flet_utils/control_coder.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 11:56 __MACOSX/dist/app/flet_utils/._control_coder.py
--rw-r--r--  2.0 unx       94 bX defN 23-Jul-07 10:42 dist/app/api/manage_route_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 10:42 __MACOSX/dist/app/api/._manage_route_request.py
--rw-r--r--  2.0 unx      957 bX defN 23-Jul-07 12:21 dist/app/api/manage_page_update_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 12:21 __MACOSX/dist/app/api/._manage_page_update_request.py
--rw-r--r--  2.0 unx      416 bX defN 23-Jul-05 08:40 dist/app/api/push_event_to_host.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-05 08:40 __MACOSX/dist/app/api/._push_event_to_host.py
--rw-r--r--  2.0 unx      465 bX defN 23-Jul-05 14:58 dist/app/api/manage_update_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-05 14:58 __MACOSX/dist/app/api/._manage_update_request.py
--rw-r--r--  2.0 unx      358 bX defN 23-Jul-07 11:15 dist/app/api/initialize_page_target.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 11:15 __MACOSX/dist/app/api/._initialize_page_target.py
-drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-22 09:26 dist/app/api/__pycache__/
--rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-22 09:26 __MACOSX/dist/app/api/.___pycache__
--rw-r--r--  2.0 unx      435 bX defN 23-Jul-06 12:46 dist/app/api/manage_clean_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-06 12:46 __MACOSX/dist/app/api/._manage_clean_request.py
--rw-r--r--  2.0 unx      740 bX defN 23-Jul-07 07:47 dist/app/api/manage_remove_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 07:47 __MACOSX/dist/app/api/._manage_remove_request.py
--rw-r--r--  2.0 unx      991 bX defN 23-Jul-06 16:39 dist/app/api/manage_add_request.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-06 16:39 __MACOSX/dist/app/api/._manage_add_request.py
--rw-r--r--  2.0 unx      475 bX defN 23-Jul-05 11:15 dist/app/api/get_host_updates.py
--rw-r--r--  2.0 unx      163 bX defN 23-Jul-05 11:15 __MACOSX/dist/app/api/._get_host_updates.py
+-rw-r--r--  2.0 unx     1642 bX defN 23-Jul-07 18:44 dist/app/tools/manage_host_updates.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/tools/._manage_host_updates.py
+-rw-r--r--  2.0 unx      815 bX defN 23-Jul-07 18:44 dist/app/tools/post_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/tools/._post_request.py
+-rw-r--r--  2.0 unx     1119 bX defN 23-Jul-13 14:23 dist/app/flet_utils/hook_control_events.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 14:23 __MACOSX/dist/app/flet_utils/._hook_control_events.py
+-rw-r--r--  2.0 unx      389 bX defN 23-Jul-07 18:44 dist/app/flet_utils/manage_page_events.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._manage_page_events.py
+-rw-r--r--  2.0 unx     1157 bX defN 23-Jul-07 18:44 dist/app/flet_utils/appbar_coder.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._appbar_coder.py
+-rw-r--r--  2.0 unx     1294 bX defN 23-Jul-07 18:44 dist/app/flet_utils/get_all_subcontrols.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._get_all_subcontrols.py
+-rw-r--r--  2.0 unx       95 bX defN 23-Jul-07 18:44 dist/app/flet_utils/control_actions.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._control_actions.py
+-rw-r--r--  2.0 unx      623 bX defN 23-Jul-13 13:57 dist/app/flet_utils/flet_control_generator.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 13:57 __MACOSX/dist/app/flet_utils/._flet_control_generator.py
+-rw-r--r--  2.0 unx      471 bX defN 23-Jul-07 18:44 dist/app/flet_utils/append_to_content.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._append_to_content.py
+-rw-r--r--  2.0 unx      973 bX defN 23-Jul-07 18:44 dist/app/flet_utils/view_coder.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._view_coder.py
+-rw-r--r--  2.0 unx      848 bX defN 23-Jul-07 18:44 dist/app/flet_utils/control_coder.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/flet_utils/._control_coder.py
+-rw-r--r--  2.0 unx       94 bX defN 23-Jul-07 18:44 dist/app/api/manage_route_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._manage_route_request.py
+-rw-r--r--  2.0 unx     1629 bX defN 23-Jul-13 16:57 dist/app/api/manage_page_update_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 16:57 __MACOSX/dist/app/api/._manage_page_update_request.py
+-rw-r--r--  2.0 unx      416 bX defN 23-Jul-13 14:23 dist/app/api/push_event_to_host.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 14:23 __MACOSX/dist/app/api/._push_event_to_host.py
+-rw-r--r--  2.0 unx      465 bX defN 23-Jul-07 18:44 dist/app/api/manage_update_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._manage_update_request.py
+-rw-r--r--  2.0 unx      358 bX defN 23-Jul-07 18:44 dist/app/api/initialize_page_target.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._initialize_page_target.py
+drwxr-xr-x  2.0 unx        0 bx stor 23-Jul-07 18:44 dist/app/api/__pycache__/
+-rwxr-xr-x  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/.___pycache__
+-rw-r--r--  2.0 unx      435 bX defN 23-Jul-07 18:44 dist/app/api/manage_clean_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._manage_clean_request.py
+-rw-r--r--  2.0 unx      740 bX defN 23-Jul-07 18:44 dist/app/api/manage_remove_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._manage_remove_request.py
+-rw-r--r--  2.0 unx      991 bX defN 23-Jul-13 14:03 dist/app/api/manage_add_request.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-13 14:03 __MACOSX/dist/app/api/._manage_add_request.py
+-rw-r--r--  2.0 unx      475 bX defN 23-Jul-07 18:44 dist/app/api/get_host_updates.py
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/._get_host_updates.py
 drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-15 19:03 dist/assets/packages/window_manager/
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/assets/packages/._window_manager
 -rw-r--r--  2.0 unx     9242 bX defN 23-Jun-14 17:06 dist/assets/shaders/ink_sparkle.frag
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/shaders/._ink_sparkle.frag
 -rw-r--r--  2.0 unx  1261080 bX defN 23-Jun-14 17:06 dist/assets/fonts/MaterialIcons-Regular.otf
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/fonts/._MaterialIcons-Regular.otf
--rw-r--r--  2.0 unx      861 bX defN 23-Jun-22 09:26 dist/app/api/__pycache__/value_update.cpython-311.pyc
--rw-r--r--  2.0 unx      163 bX defN 23-Jun-22 09:26 __MACOSX/dist/app/api/__pycache__/._value_update.cpython-311.pyc
+-rw-r--r--  2.0 unx      861 bX defN 23-Jul-07 18:44 dist/app/api/__pycache__/value_update.cpython-311.pyc
+-rw-r--r--  2.0 unx      163 bX defN 23-Jul-07 18:44 __MACOSX/dist/app/api/__pycache__/._value_update.cpython-311.pyc
 drwxr-xr-x  2.0 unx        0 bx stor 23-Jun-15 19:03 dist/assets/packages/window_manager/images/
 -rwxr-xr-x  2.0 unx      163 bX defN 23-Jun-15 19:03 __MACOSX/dist/assets/packages/window_manager/._images
 -rw-r--r--  2.0 unx      366 bX defN 23-Jun-14 17:06 dist/assets/packages/window_manager/images/ic_chrome_unmaximize.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/packages/window_manager/images/._ic_chrome_unmaximize.png
 -rw-r--r--  2.0 unx      166 bX defN 23-Jun-14 17:06 dist/assets/packages/window_manager/images/ic_chrome_minimize.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/packages/window_manager/images/._ic_chrome_minimize.png
 -rw-r--r--  2.0 unx      271 bX defN 23-Jun-14 17:06 dist/assets/packages/window_manager/images/ic_chrome_maximize.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/packages/window_manager/images/._ic_chrome_maximize.png
 -rw-r--r--  2.0 unx      298 bX defN 23-Jun-14 17:06 dist/assets/packages/window_manager/images/ic_chrome_close.png
 -rw-r--r--  2.0 unx      163 bX defN 23-Jun-14 17:06 __MACOSX/dist/assets/packages/window_manager/images/._ic_chrome_close.png
-129 files, 10709645 bytes uncompressed, 4284543 bytes compressed:  60.0%
+129 files, 10710450 bytes uncompressed, 4284755 bytes compressed:  60.0%
```

#### dist/app/flet_utils/hook_control_events.py

```diff
@@ -1,11 +1,13 @@
 import flet
 
 all_actions = [
-    "on_change", "on_submit", "on_focus", "on_blur", "on_hover", "on_click"
+    "on_change", "on_submit", "on_focus", "on_blur", "on_hover", "on_click",
+    "on_result", "on_upload", "on_duration_changed", "on_loaded", "on_position_changed",
+    "on_seek_complete", "on_state_changed"
 ]
 
 
 class HookControlEvents:
     """
     This will search for all control events to hook them into a function.
```

#### dist/app/api/manage_page_update_request.py

```diff
@@ -1,10 +1,11 @@
 from flet_utils.appbar_coder import dict_to_appbar
 from flet_utils.view_coder import dict_to_view
-
+from flet_utils.hook_control_events import HookControlEvents
+from flet_utils.control_coder import dict_to_control
 
 
 def manage_page_update_request (update_dict, main_class):
     for i in update_dict['props']:
             if hasattr(main_class.page, i):
                 if update_dict['props'][i] != None:
                     setattr(main_class.page, i, update_dict['props'][i])
@@ -20,8 +21,22 @@
         for i in update_dict['views']:
             if i['route'] == "/":
                 clear_all = True
                 break
         if clear_all:
             main_class.page.views.clear()
         for v in update_dict['views']:
-            main_class.page.views.append (dict_to_view(view_dict=v, main_class=main_class))
+            main_class.page.views.append (dict_to_view(view_dict=v, main_class=main_class))
+    
+
+    if "overlay" in update_dict:
+        if update_dict['overlay'] == []:
+            main_class.page.overlay.clear()
+        
+        for ovlc in update_dict['overlay']:
+            control = dict_to_control(control_dict=ovlc)
+            main_class.page.overlay.append (control)
+            main_class.all_controls[f'{control.flet_lite_number}'] = control
+            main_class.parents_of_controls[control] = "page"
+            
+            # Hook all the overlay control events.
+            HookControlEvents(control=control, main_class=main_class)
```

### Comparing `flet_lite-1.7.2/flet/web/dist.zip` & `flet_lite-1.7.5/flet/web/dist.zip`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/__init__.py` & `flet_lite-1.7.5/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/alert_dialog.py` & `flet_lite-1.7.5/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/animated_switcher.py` & `flet_lite-1.7.5/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/animation.py` & `flet_lite-1.7.5/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/app_bar.py` & `flet_lite-1.7.5/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/audio.py` & `flet_lite-1.7.5/flet_core/audio.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
         CallableControl.__init__(
             self,
             ref=ref,
             data=data,
         )
 
+        # flet_lite props
+        self.duration = 0
+        self.position = 0
+
         self.src = src
         self.src_base64 = src_base64
         self.autoplay = autoplay
         self.volume = volume
         self.balance = balance
         self.playback_rate = playback_rate
         self.release_mode = release_mode
@@ -112,28 +116,32 @@
 
     async def seek_async(self, position_milliseconds: int):
         await self._call_method_async(
             "seek", params=[str(position_milliseconds)], wait_for_result=False
         )
 
     def get_duration(self) -> Optional[int]:
-        sr = self._call_method("get_duration", [])
-        return int(sr) if sr else None
+        # sr = self._call_method("get_duration", [])
+        # return int(sr) if sr else None
+        return self.duration
 
     async def get_duration_async(self) -> Optional[int]:
-        sr = await self._call_method_async("get_duration", [])
-        return int(sr) if sr else None
+        # sr = await self._call_method_async("get_duration", [])
+        # return int(sr) if sr else None
+        return self.duration
 
     def get_current_position(self) -> Optional[int]:
-        sr = self._call_method("get_current_position", [])
-        return int(sr) if sr else None
+        # sr = self._call_method("get_current_position", [])
+        # return int(sr) if sr else None
+        return self.position
 
     async def get_current_position_async(self) -> Optional[int]:
-        sr = await self._call_method_async("get_current_position", [])
-        return int(sr) if sr else None
+        # sr = await self._call_method_async("get_current_position", [])
+        # return int(sr) if sr else None
+        return self.position
 
     # src
     @property
     def src(self):
         return self._get_attr("src")
 
     @src.setter
```

### Comparing `flet_lite-1.7.2/flet_core/banner.py` & `flet_lite-1.7.5/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/border.py` & `flet_lite-1.7.5/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/border_radius.py` & `flet_lite-1.7.5/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/bottom_sheet.py` & `flet_lite-1.7.5/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/buttons.py` & `flet_lite-1.7.5/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/callable_control.py` & `flet_lite-1.7.5/flet_core/callable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/__init__.py` & `flet_lite-1.7.5/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/arc.py` & `flet_lite-1.7.5/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/canvas.py` & `flet_lite-1.7.5/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/circle.py` & `flet_lite-1.7.5/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/color.py` & `flet_lite-1.7.5/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/fill.py` & `flet_lite-1.7.5/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/line.py` & `flet_lite-1.7.5/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/oval.py` & `flet_lite-1.7.5/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/path.py` & `flet_lite-1.7.5/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/points.py` & `flet_lite-1.7.5/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/rect.py` & `flet_lite-1.7.5/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/shadow.py` & `flet_lite-1.7.5/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/canvas/text.py` & `flet_lite-1.7.5/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/card.py` & `flet_lite-1.7.5/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/bar_chart.py` & `flet_lite-1.7.5/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/bar_chart_group.py` & `flet_lite-1.7.5/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/bar_chart_rod.py` & `flet_lite-1.7.5/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_lite-1.7.5/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/chart_axis.py` & `flet_lite-1.7.5/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/chart_axis_label.py` & `flet_lite-1.7.5/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/chart_point_shape.py` & `flet_lite-1.7.5/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/line_chart.py` & `flet_lite-1.7.5/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/line_chart_data.py` & `flet_lite-1.7.5/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/line_chart_data_point.py` & `flet_lite-1.7.5/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/pie_chart.py` & `flet_lite-1.7.5/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/charts/pie_chart_section.py` & `flet_lite-1.7.5/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/checkbox.py` & `flet_lite-1.7.5/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/circle_avatar.py` & `flet_lite-1.7.5/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/client_storage.py` & `flet_lite-1.7.5/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/clipboard.py` & `flet_lite-1.7.5/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/colors.py` & `flet_lite-1.7.5/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/column.py` & `flet_lite-1.7.5/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/connection.py` & `flet_lite-1.7.5/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/constrained_control.py` & `flet_lite-1.7.5/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/container.py` & `flet_lite-1.7.5/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/control.py` & `flet_lite-1.7.5/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/datatable.py` & `flet_lite-1.7.5/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/divider.py` & `flet_lite-1.7.5/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/drag_target.py` & `flet_lite-1.7.5/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/draggable.py` & `flet_lite-1.7.5/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/dropdown.py` & `flet_lite-1.7.5/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/elevated_button.py` & `flet_lite-1.7.5/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/embed_json_encoder.py` & `flet_lite-1.7.5/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/event_handler.py` & `flet_lite-1.7.5/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/file_picker.py` & `flet_lite-1.7.5/flet_core/file_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,17 +289,17 @@
     def file_type(self) -> FilePickerFileType:
         return self.__file_type
 
     @file_type.setter
     def file_type(self, value: FilePickerFileType):
         self.__file_type = value
         if isinstance(value, FilePickerFileType):
-            self._set_attr("fileType", value.value)
+            self._set_attr("fileType", str(value.value))
         else:
-            self.__set_file_type(value)
+            self.__set_file_type(str(value))
 
     def __set_file_type(self, value: FileTypeString):
         self._set_attr("fileType", value)
 
     # allowed_extensions
     @property
     def allowed_extensions(self) -> Optional[List[str]]:
```

### Comparing `flet_lite-1.7.2/flet_core/filled_button.py` & `flet_lite-1.7.5/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/filled_tonal_button.py` & `flet_lite-1.7.5/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/flet_app.py` & `flet_lite-1.7.5/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/floating_action_button.py` & `flet_lite-1.7.5/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/form_field_control.py` & `flet_lite-1.7.5/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/gesture_detector.py` & `flet_lite-1.7.5/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/gradients.py` & `flet_lite-1.7.5/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/grid_view.py` & `flet_lite-1.7.5/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/haptic_feedback.py` & `flet_lite-1.7.5/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/icon.py` & `flet_lite-1.7.5/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/icon_button.py` & `flet_lite-1.7.5/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/icons.py` & `flet_lite-1.7.5/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/image.py` & `flet_lite-1.7.5/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/list_tile.py` & `flet_lite-1.7.5/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/list_view.py` & `flet_lite-1.7.5/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/local_connection.py` & `flet_lite-1.7.5/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/margin.py` & `flet_lite-1.7.5/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/markdown.py` & `flet_lite-1.7.5/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/matplotlib_chart.py` & `flet_lite-1.7.5/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/navigation_bar.py` & `flet_lite-1.7.5/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/navigation_rail.py` & `flet_lite-1.7.5/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/outlined_button.py` & `flet_lite-1.7.5/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/padding.py` & `flet_lite-1.7.5/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/page.py` & `flet_lite-1.7.5/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/painting.py` & `flet_lite-1.7.5/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/plotly_chart.py` & `flet_lite-1.7.5/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/popup_menu_button.py` & `flet_lite-1.7.5/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/progress_bar.py` & `flet_lite-1.7.5/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/progress_ring.py` & `flet_lite-1.7.5/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/protocol.py` & `flet_lite-1.7.5/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/querystring.py` & `flet_lite-1.7.5/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/radio.py` & `flet_lite-1.7.5/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/radio_group.py` & `flet_lite-1.7.5/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/responsive_row.py` & `flet_lite-1.7.5/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/row.py` & `flet_lite-1.7.5/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/scrollable_control.py` & `flet_lite-1.7.5/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/semantics.py` & `flet_lite-1.7.5/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/session_storage.py` & `flet_lite-1.7.5/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/shader_mask.py` & `flet_lite-1.7.5/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/shadow.py` & `flet_lite-1.7.5/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/shake_detector.py` & `flet_lite-1.7.5/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/slider.py` & `flet_lite-1.7.5/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/snack_bar.py` & `flet_lite-1.7.5/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/stack.py` & `flet_lite-1.7.5/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/switch.py` & `flet_lite-1.7.5/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/tabs.py` & `flet_lite-1.7.5/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/template_route.py` & `flet_lite-1.7.5/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/text.py` & `flet_lite-1.7.5/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/text_button.py` & `flet_lite-1.7.5/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/text_span.py` & `flet_lite-1.7.5/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/text_style.py` & `flet_lite-1.7.5/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/textfield.py` & `flet_lite-1.7.5/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/theme.py` & `flet_lite-1.7.5/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/tooltip.py` & `flet_lite-1.7.5/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/transform.py` & `flet_lite-1.7.5/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/transparent_pointer.py` & `flet_lite-1.7.5/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/types.py` & `flet_lite-1.7.5/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/user_control.py` & `flet_lite-1.7.5/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/vertical_divider.py` & `flet_lite-1.7.5/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/view.py` & `flet_lite-1.7.5/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_core/window_drag_area.py` & `flet_lite-1.7.5/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/flet_lite.egg-info/PKG-INFO` & `flet_lite-1.7.5/flet_lite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-lite
-Version: 1.7.2
+Version: 1.7.5
 Summary: A tiny version of flet to work on mobile development
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.7.2/flet_lite.egg-info/SOURCES.txt` & `flet_lite-1.7.5/flet_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7.2/setup.py` & `flet_lite-1.7.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_descibe = str(f.read())
 
 setup(
     name='flet_lite',
-    version='1.7.2',
+    version='1.7.5',
     author='SKbarbon',
     description='A tiny version of flet to work on mobile development',
     long_description=long_descibe,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_lite',
     install_requires=["flask_cors", "flask", "jsonpickle", "repath"],
     packages=find_packages(include=["flet", "flet_core", "flet.web", "flet/*", "flet.api"]),
```

