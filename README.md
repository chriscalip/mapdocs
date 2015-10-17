# mapdocs
Technical Overview Notes of 2 Drupal Mapping Modules

- Openlayers, <a href="https://www.drupal.org/project/openlayers" target="_blank">link</a>, version 7.x-3.x
- Leaflet, <a href="https://www.drupal.org/project/leaflet" target="_blank">link</a>, new version, currently building.

## Table of Contents

- [openlayers/](#s1)
- [openlayers-overview/](#s2)
  * [Display of Map; php execution flow](#s2.1)
  * [Configuration Management through Ctools](#s2.2)
  * [Administration Graphical User Interface](#s2.3)

<a name="s1"></a>
## openlayers/ folder

Contains Auto Generated docs of openlayers objects

<a name="s2"></a>
## openlayers-overview/ folder

Contains Technical Overview Notes of the drupal <a href="https://www.drupal.org/project/openlayers" target="_blank">openlayers</a> module.

<a name="s2.1"></a>
## Display of Map; php execution flow
`openlayers-overview/execution-flow-php-provisions-assets.md`

Describes the execution flow in php when loading an openlayers map; the beginnings of displaying the map. During php page display; the map div is displayed, the provisioning of assets (css,js,etc.. are added) for each object  (
Layers,Sources,Controls,Interactions,Components,Projections,Styles) belonging to the map.

<a name="s2.2"></a>
## Configuration Management through Ctools
`openlayers-overview/ctools_export_ui-inventory.md`

Configuration presets – collections of configuration or other types of objects that administrators set up that can then be used in different contexts on a website. In the openlayers module, administrators define maps – objects that are containers for some very complex configuration. These configuration objects are all stored in the database as they are created, but they can also be exported into code, and this is the foundation of the concept of exportables.

For more background on configuration management through ctools. Check this link:
<a href="https://www.drupal.org/node/928026" target="_blank">How to make configuration objects exportable with CTools</a>

The file `openlayers-overview/ctools_export_ui-inventory.md` is an inventory of `ctools_export_ui` integration code that facilitates the configuration management through ctools.

<a name="s2.3"></a>
## Administration Graphical User Interface
`openlayers-overview/admin-graphical-user-interface.md`

Describes the components that facilitate the openlayers admin gui.
