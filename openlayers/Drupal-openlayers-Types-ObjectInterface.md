Drupal\openlayers\Types\ObjectInterface
===============

Interface openlayers_object_interface.




* Interface name: ObjectInterface
* Namespace: Drupal\openlayers\Types
* This is an **interface**
* This interface extends: Drupal\Component\Plugin\PluginInspectionInterface





Methods
-------


### init

    mixed Drupal\openlayers\Types\ObjectInterface::init()

Initializes the object.



* Visibility: **public**




### getType

    string|FALSE Drupal\openlayers\Types\ObjectInterface::getType()

The type of this object.



* Visibility: **public**




### clearOption

    mixed Drupal\openlayers\Types\ObjectInterface::clearOption(string|array $parents)





* Visibility: **public**


#### Arguments
* $parents **string|array**



### getOptions

    array Drupal\openlayers\Types\ObjectInterface::getOptions()

Return the options array.



* Visibility: **public**




### setOptions

    mixed Drupal\openlayers\Types\ObjectInterface::setOptions(array $options)

Set the options array.



* Visibility: **public**


#### Arguments
* $options **array** - &lt;p&gt;The options array.&lt;/p&gt;



### getOption

    mixed Drupal\openlayers\Types\ObjectInterface::getOption(string|array $parents, mixed $default_value)

Returns an option.



* Visibility: **public**


#### Arguments
* $parents **string|array**
* $default_value **mixed** - &lt;p&gt;The default value to return if the option isn&#039;t set. Set to NULL if not
defined.&lt;/p&gt;



### setOption

    mixed Drupal\openlayers\Types\ObjectInterface::setOption(string|array $parents, mixed $value)

Set an option.



* Visibility: **public**


#### Arguments
* $parents **string|array**
* $value **mixed** - &lt;p&gt;The value to set.&lt;/p&gt;



### optionsForm

    mixed Drupal\openlayers\Types\ObjectInterface::optionsForm(array $form, array $form_state)

Provides the options form to configure this object.



* Visibility: **public**


#### Arguments
* $form **array** - &lt;p&gt;The form array by reference.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### optionsFormValidate

    mixed Drupal\openlayers\Types\ObjectInterface::optionsFormValidate(array $form, array $form_state)

Validation callback for the options form.



* Visibility: **public**


#### Arguments
* $form **array** - &lt;p&gt;The form array.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### optionsFormSubmit

    mixed Drupal\openlayers\Types\ObjectInterface::optionsFormSubmit(array $form, array $form_state)

Submit callback for the options form.



* Visibility: **public**


#### Arguments
* $form **array** - &lt;p&gt;The form array.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### attached

    array Drupal\openlayers\Types\ObjectInterface::attached()

Returns a list of attachments for building the render array.



* Visibility: **public**




### dependencies

    array Drupal\openlayers\Types\ObjectInterface::dependencies()

Defines dependencies.



* Visibility: **public**




### isAsynchronous

    boolean Drupal\openlayers\Types\ObjectInterface::isAsynchronous()

Whether or not this object has to be processed asynchronously.

If true the map this object relates to won't be processes right away by
Drupals behaviour attach.

* Visibility: **public**




### preBuild

    mixed Drupal\openlayers\Types\ObjectInterface::preBuild(array $build, \Drupal\openlayers\Types\ObjectInterface $context)

Invoked before an objects render array is built.

Mostly invoked by the map object.

* Visibility: **public**


#### Arguments
* $build **array** - &lt;p&gt;The array with the build information.&lt;/p&gt;
* $context **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;The context of the build. Mostly the map object.&lt;/p&gt;



### postBuild

    mixed Drupal\openlayers\Types\ObjectInterface::postBuild(array $build, \Drupal\openlayers\Types\ObjectInterface $context)

Invoked after an objects render array is built.

Mostly invoked by the map object.

* Visibility: **public**


#### Arguments
* $build **array** - &lt;p&gt;The array with the build information.&lt;/p&gt;
* $context **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;The context of the build. Mostly the map object.&lt;/p&gt;



### getExport

    \StdClass Drupal\openlayers\Types\ObjectInterface::getExport()

Return an object, CTools Exportable.



* Visibility: **public**




### getConfiguration

    array Drupal\openlayers\Types\ObjectInterface::getConfiguration()

Return the object configuration.



* Visibility: **public**




### getObjects

    array Drupal\openlayers\Types\ObjectInterface::getObjects(string $type)

Return an array of OL objects indexed by their type.



* Visibility: **public**


#### Arguments
* $type **string**



### getParents

    array Drupal\openlayers\Types\ObjectInterface::getParents()

Returns an array with the maps this object is attached on.



* Visibility: **public**




### getProvider

    string Drupal\openlayers\Types\ObjectInterface::getProvider()

Return the module that provides this plugin.



* Visibility: **public**




### getClassDirectory

    string Drupal\openlayers\Types\ObjectInterface::getClassDirectory()

Returns the path to the plugin directory.



* Visibility: **public**




### getClassPath

    string Drupal\openlayers\Types\ObjectInterface::getClassPath()

Returns the path to the class file.



* Visibility: **public**




### getCollection

    \Drupal\openlayers\Types\Collection Drupal\openlayers\Types\ObjectInterface::getCollection()

Return the Collection object linked to the object.



* Visibility: **public**




### getJS

    array Drupal\openlayers\Types\ObjectInterface::getJS()

Return the JS to insert in the page when building the object.



* Visibility: **public**




### setWeight

    void Drupal\openlayers\Types\ObjectInterface::setWeight(integer $weight)

Set the weight of an object.



* Visibility: **public**


#### Arguments
* $weight **integer**



### getWeight

    integer Drupal\openlayers\Types\ObjectInterface::getWeight()

Get the weight of an object.



* Visibility: **public**




### optionsToObjects

    array<mixed,Object> Drupal\openlayers\Types\ObjectInterface::optionsToObjects()

Return a flat array containing Openlayers Objects from the options array.



* Visibility: **public**




### getName

    string Drupal\openlayers\Types\ObjectInterface::getName()

Return the human name of the object.



* Visibility: **public**




### getMachineName

    string Drupal\openlayers\Types\ObjectInterface::getMachineName()

Return the unique machine name of the object.



* Visibility: **public**




### getDescription

    string Drupal\openlayers\Types\ObjectInterface::getDescription()

Return the description of the object.



* Visibility: **public**




### getPluginDescription

    string Drupal\openlayers\Types\ObjectInterface::getPluginDescription()

Return the description of the object's plugin.



* Visibility: **public**




### i18nStringsRefresh

    mixed Drupal\openlayers\Types\ObjectInterface::i18nStringsRefresh()

Refresh string translations.



* Visibility: **public**




### getFactoryService

    string Drupal\openlayers\Types\ObjectInterface::getFactoryService()

Return the Factory Service of the object.



* Visibility: **public**



