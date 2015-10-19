# PHP provisions assets (js,css,div)
## Map Render Flow 1

<pre>
$object_type = 'map';
$map = Drupal\openlayers\Openlayers::load($object_type, machine_name);
$map->build();
  // Inside $map->build() function
  $map->preBuild();
  // Instead of multiple drupal_add_js this method makes use of '#attached'
  // see https://api.drupal.org/api/drupal/includes%21common.inc/function/drupal_process_attached/7
  '#attached' => $map->getCollection()->getAttached();
  // $map has method getCollection from Object inheritance
  // instance of Collection does getAttached()
  // during getAttached()
  // get all plugin attached to collection
  // at each attached plugin execute attached()
  // attached provides css,js,libraries_load information
  // note plugin OLMap.php provisions openlayers libraries_load
  $map->postBuild()
</pre>

A note about plugin's asset (css,js) weight.

  * libraries/openlayers3/build/ol.js
  * modules/openlayers/js/openlayers.js
  * modules/openlayers/js/openlayers.pluginManager.js
  * modules/openlayers/js/openlayers.behaviors.js

These files weight are declared through openlayers_libraries_info().

While plugin assets (weight) are set via default method from src/Plugin/Types/Object.php

  * modules/openlayers/src/Plugin/Map/OLMap/js/olmap.js
  * modules/openlayers/src/Plugin/Layer/Vector/js/vector.js
  * modules/openlayers/src/Plugin/Layer/Tile/js/tile.js
  * modules/openlayers/src/Plugin/Control/MousePosition/js/mouseposition.js
  * modules/openlayers/src/Plugin/Source/GeoJSON/js/geojson.js
