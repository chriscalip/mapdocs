# mapdocs
Technical Overview Notes of 2 Drupal Mapping Modules

- Openlayers
  * <a href="https://www.drupal.org/project/openlayers" target="_blank">link</a>
  * version 7.x-3.x
- Leaflet
  * <a href="https://www.drupal.org/project/leaflet" target="_blank">link</a>
  * new version, currently building.

## Table of Contents

- [openlayers/](#s1)
- [openlayers-overview/](#s2)
  * [execution-flow-php-provisions-assets.md](#s2.1)


<a name="s1"></a>
## openlayers/ folder

Contains Auto Generated docs of openlayers objects

<a name="s2"></a>
## openlayers-overview/ folder

Contains Technical Overview Notes of the drupal <a href="https://www.drupal.org/project/openlayers" target="_blank">openlayers</a> module.

<a name="s2.1"></a>
## execution-flow-php-provisions-assets.md

Describes the execution flow in php when loading an openlayers map; the beginnings of displaying the map. During php page display; the map div is displayed, the provisioning of assets (css,js,etc.. are added) for each object  (
Layers,Sources,Controls,Interactions,Components,Projections,Styles) belonging to the map.
