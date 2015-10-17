# `openlayers_ui`
sub-module `openlayers_ui` that handles all the admin gui.

## Main Administration Pages
`openlayers_ui.module` implements hook_menu to provide menus and `includes/openlayers_ui.admin.inc` provides to form handling the menu page.

Menu Pages

 * admin/structure/openlayers
 * admin/structure/openlayers/settings

## Sub Administration Pages per plugin type

`openlayers_ui` makes use of the schema assets provided by `openlayers` hook_schema and its ctools exportable integration. Each of these exportable plugin types {maps,components,controls,interactions,layers,projections,sources,styles} has a corresponding `ctools_export_ui` class at directory `openlayers_ui/src/Plugin/export_ui` through those classes
menu pages are created.

Given these exportable plugin types {maps,components,controls,interactions,layers,projections,sources,styles}

Legend :

 * [type] : one of the exportable plugin types
 * %      : the machine name of the plugin belonging to the plugin type.

Menu Pages

 * admin/structure/openlayers/[type]
 * admin/structure/openlayers/[type]/add
 * admin/structure/openlayers/[type]/import
 * admin/structure/openlayers/[type]/list
 * admin/structure/openlayers/[type]/list/%
 * admin/structure/openlayers/[type]/list/%/clone
 * admin/structure/openlayers/[type]/list/%/delete
 * admin/structure/openlayers/[type]/list/%/disable
 * admin/structure/openlayers/[type]/list/%/edit
 * admin/structure/openlayers/[type]/list/%/enable
 * admin/structure/openlayers/[type]/list/%/export
 * admin/structure/openlayers/[type]/list/%/revert

Each of these menu pages has a page callback `ctools_export_ui_switcher_page` and forms and other menu-tab information dictated by a corresponding plugin type class. see `openlayers_ui/src/Plugin/export_ui`
