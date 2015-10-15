Drupal\openlayers\Openlayers
===============

Class Openlayers.




* Class name: Openlayers
* Namespace: Drupal\openlayers







Methods
-------


### getOLObjectsOptions

    array Drupal\openlayers\Openlayers::getOLObjectsOptions(string $object_type)

Gets a list of available plugin types.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $object_type **string** - &lt;p&gt;The plugin type.&lt;/p&gt;



### loadAllAsOptions

    array Drupal\openlayers\Openlayers::loadAllAsOptions(string $type)

Gets a list of Openlayers exportable.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $type **string** - &lt;p&gt;The plugin .&lt;/p&gt;



### loadExportable

    array Drupal\openlayers\Openlayers::loadExportable(string $object_type, string $export_id)

Load a CTools exportable.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $object_type **string** - &lt;p&gt;Type of object to load:
  map|layer|source|control|interaction|style|component .&lt;/p&gt;
* $export_id **string** - &lt;p&gt;The exportable id.&lt;/p&gt;



### loadAllExportable

    array Drupal\openlayers\Openlayers::loadAllExportable(string $type)

Gets all available OL objects.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $type **string** - &lt;p&gt;The plugin type&lt;/p&gt;



### load

    Object|\Drupal\openlayers\Types\Error Drupal\openlayers\Openlayers::load(string $object_type, array|string|object $export)

Create an object instance for an export.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $object_type **string** - &lt;p&gt;The object type to look up. See openlayers_object_types() for a list of
available object types.&lt;/p&gt;
* $export **array|string|object** - &lt;p&gt;The exported object.&lt;/p&gt;



### loadAll

    array<mixed,\Drupal\openlayers\Types\Object> Drupal\openlayers\Openlayers::loadAll(string $object_type)

Load all objects.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $object_type **string** - &lt;p&gt;Type of object to load:
  map|layer|source|control|interaction|style|component.&lt;/p&gt;



### save

    mixed Drupal\openlayers\Openlayers::save(\Drupal\openlayers\Types\ObjectInterface $object)

Save an object in the database.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $object **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;The object to save.&lt;/p&gt;



### getPluginTypes

    array Drupal\openlayers\Openlayers::getPluginTypes(array $filter)

Return the list of Openlayers plugins type this module provides.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $filter **array** - &lt;p&gt;The values to filter out of the result array.&lt;/p&gt;



### getLibrary

    array|false Drupal\openlayers\Openlayers::getLibrary()

Return information about the Openlayers 3 if installed.



* Visibility: **public**
* This method is **static**.




### getLibraryVersion

    string Drupal\openlayers\Openlayers::getLibraryVersion()

Return the version of the Openlayers library in use.



* Visibility: **public**
* This method is **static**.




### getLocalLibraryVersion

    string Drupal\openlayers\Openlayers::getLocalLibraryVersion()

Return the version of the Openlayers library in use.



* Visibility: **public**
* This method is **static**.




### array_map_recursive

    array Drupal\openlayers\Openlayers::array_map_recursive(callable $func, array $arr)

Apply a function recursively to all the value of an array.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $func **callable** - &lt;p&gt;Function to call.&lt;/p&gt;
* $arr **array** - &lt;p&gt;The array to process.&lt;/p&gt;



### floatval_if_numeric

    float|mixed Drupal\openlayers\Openlayers::floatval_if_numeric(mixed $var)

Ensures a value is of type float or integer if it is a numeric value.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $var **mixed** - &lt;p&gt;The value to type cast if possible.&lt;/p&gt;



### removeEmptyElements

    array Drupal\openlayers\Openlayers::removeEmptyElements(array $array)

Recursively removes empty values from an array.

Empty means empty($value) AND not 0.

* Visibility: **public**
* This method is **static**.


#### Arguments
* $array **array** - &lt;p&gt;The array to clean.&lt;/p&gt;



### positioningOptions

    array Drupal\openlayers\Openlayers::positioningOptions()

Returns an array with positioning options.



* Visibility: **public**
* This method is **static**.




### getGeometryTypes

    array Drupal\openlayers\Openlayers::getGeometryTypes()

The list of geometries available.



* Visibility: **public**
* This method is **static**.




### getAttached

    array Drupal\openlayers\Openlayers::getAttached()

Returns the list of files libraries or js/css files needed according to
the settings.



* Visibility: **public**
* This method is **static**.



