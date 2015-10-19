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
