# Javascript map is rendered on page.
## Map Render Flow 2

After php page building provisions the page with openlayers javascript files.. A page typically
has these suite of js files enabling a display of an openlayers map :

  * Weight, JS File
  * 6.019 , sites/all/libraries/openlayers3/build/ol.js
  * 8.016 , sites/all/modules/openlayers/js/openlayers.js
  * 12.017 , sites/all/modules/openlayers/js/openlayers.pluginManager.js
  * 14.018 , sites/all/modules/openlayers/js/openlayers.behaviors.js
  * 20.006 , sites/all/modules/openlayers/src/Plugin/Map/OLMap/js/olmap.js
  * 20.007 , sites/all/modules/openlayers/src/Plugin/Layer/Vector/js/vector.js
  * 20.008 , sites/all/modules/openlayers/src/Plugin/Layer/Tile/js/tile.js
  * 20.009 , sites/all/modules/openlayers/src/Plugin/Control/MousePosition/js/mouseposition.js
  * 20.01 , sites/all/modules/openlayers/src/Plugin/Source/GeoJSON/js/geojson.js
  * 20.013 , sites/all/modules/openlayers/src/Plugin/Style/Circle/js/Circle.js
  * 20.012 , sites/all/modules/openlayers/src/Plugin/Source/MapQuest/js/mapquest.js
  * 20.013 , sites/all/modules/openlayers/src/Plugin/Component/InlineJS/js/inlineJS.js
  * 20.014 , sites/all/modules/openlayers/src/Plugin/Control/FullScreen/js/fullscreen.js
  * 20.015 , sites/all/modules/openlayers/src/Plugin/Interaction/DragBox/js/dragbox.js

The lighter the 'Weight' the earlier a 'JS File' is added to the page.
@see php-provisions-assets on how javascript files are added to the page

The ol object is globally available when build/ol.js is added to page. Drupal.openlayers object through js/openlayers.js . Plugin JS files "openlayers/src/Plugin/*" calls in Drupal.openlayers.pluginManager.register function and "register" their various plugin feature to the openlayers.pluginManager.js

The js file openlayers.behaviours.js integrates with drupal.js javascript behaviour api ( https://www.drupal.org/update/modules/6/7#drupal_behaviors ) as it implements an "attach" method, furthermore the attach method calls in Drupal.openlayers.pluginManager.attach which in turn calls in any active plugin attach method. Finally inside the openlayers.behaviours.js attach method is the openlayer.js processMap method call.
