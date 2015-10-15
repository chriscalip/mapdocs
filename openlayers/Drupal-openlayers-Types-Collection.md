Drupal\openlayers\Types\Collection
===============

Class Collection.




* Class name: Collection
* Namespace: Drupal\openlayers\Types
* Parent class: Drupal\Component\Plugin\PluginBase





Properties
----------


### $objects

    protected array<mixed,\Drupal\openlayers\Types\ObjectInterface> $objects = array()





* Visibility: **protected**


Methods
-------


### import

    mixed Drupal\openlayers\Types\Collection::import(array<mixed,\Drupal\openlayers\Types\ObjectInterface> $import)

Import a flat list of Openlayers Objects.



* Visibility: **public**


#### Arguments
* $import **array&lt;mixed,\Drupal\openlayers\Types\ObjectInterface&gt;** - &lt;p&gt;The array of objects to import.&lt;/p&gt;



### append

    mixed Drupal\openlayers\Types\Collection::append(\Drupal\openlayers\Types\ObjectInterface $object)

Add object to this collection.



* Visibility: **public**


#### Arguments
* $object **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;Object instance to add to this collection.&lt;/p&gt;



### prepend

    mixed Drupal\openlayers\Types\Collection::prepend(\Drupal\openlayers\Types\ObjectInterface $object)

Add object to this collection.



* Visibility: **public**


#### Arguments
* $object **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;Object instance to add to this collection.&lt;/p&gt;



### delete

    mixed Drupal\openlayers\Types\Collection::delete(\Drupal\openlayers\Types\ObjectInterface $object)

Remove object from this collection.



* Visibility: **public**


#### Arguments
* $object **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;Object instance to remove from this collection.&lt;/p&gt;



### clear

    mixed Drupal\openlayers\Types\Collection::clear(array $types)

Remove object type.



* Visibility: **public**


#### Arguments
* $types **array** - &lt;p&gt;The types of objects to remove.&lt;/p&gt;



### getAttached

    array Drupal\openlayers\Types\Collection::getAttached()

Returns an array with all the attachments of the collection objects.



* Visibility: **public**




### getJS

    array Drupal\openlayers\Types\Collection::getJS()

Array with all the JS settings of the collection objects.



* Visibility: **public**




### getObjects

    array Drupal\openlayers\Types\Collection::getObjects(string $type)

Array with all the collection objects.



* Visibility: **public**


#### Arguments
* $type **string** - &lt;p&gt;Type to filter for. If set only a list with objects of this type is
  returned.&lt;/p&gt;



### getFlatList

    array<mixed,\Drupal\openlayers\Types\Object> Drupal\openlayers\Types\Collection::getFlatList(array $types)

Return an array with all the collection objects.



* Visibility: **public**


#### Arguments
* $types **array** - &lt;p&gt;Array of type to filter for. If set, only a list with objects of this
  type is returned.&lt;/p&gt;



### merge

    mixed Drupal\openlayers\Types\Collection::merge(\Drupal\openlayers\Types\Collection $collection)

Merges another collection into this one.



* Visibility: **public**


#### Arguments
* $collection **[Drupal\openlayers\Types\Collection](Drupal-openlayers-Types-Collection.md)** - &lt;p&gt;The collection to merge into this one.&lt;/p&gt;



### getExport

    array Drupal\openlayers\Types\Collection::getExport()

Get the collection as an export array with id's instead of objects.



* Visibility: **public**



