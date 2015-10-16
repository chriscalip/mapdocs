# PHP provisions assets (js,css,div)
## Map Render Flow 1


> $map = Drupal\openlayers\Openlayers::load('map', machine_name);

> $map->build();

>> $map->preBuild();

>> // check async

>> // setup styles

>> Setup Build array

>>> '#attached' => $map->getCollection()->getAttached(); 

>>>> $map has method getCollection from Object inheritance

>>>> instance of Collection does getAttached()

>>>> during getAttached()

>>>>> get all objects attached to collection

>>>>> at each attached object execute attached()

>>>>>> attached provides css,js information

>> $map->postBuild()

