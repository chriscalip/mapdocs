Drupal\openlayers\Plugin\Interaction\InlineJS\InlineJS
===============

Class InlineJS.




* Class name: InlineJS
* Namespace: Drupal\openlayers\Plugin\Interaction\InlineJS
* Parent class: [Drupal\openlayers\Types\Interaction](Drupal-openlayers-Types-Interaction.md)





Properties
----------


### $options

    protected array $options = array()

The array containing the options.



* Visibility: **protected**


### $machine_name

    public string $machine_name

The unique machine name.



* Visibility: **public**


### $name

    public string $name

The human readable name.



* Visibility: **public**


### $description

    public string $description

A short description.



* Visibility: **public**


### $factory_service

    public string $factory_service

The factory service.



* Visibility: **public**


### $weight

    protected integer $weight





* Visibility: **protected**


### $collection

    protected \Drupal\openlayers\Types\Collection $collection

Holds the Collection object.



* Visibility: **protected**


### $attached

    protected array $attached = array('js' => array(), 'css' => array(), 'library' => array(), 'libraries_load' => array())

Holds all the attachment used by this object.



* Visibility: **protected**


Methods
-------


### __construct

    mixed Drupal\openlayers\Plugin\Interaction\InlineJS\InlineJS::__construct(array $configuration, string $plugin_id, array $plugin_definition, \Drupal\Core\Extension\ModuleHandlerInterface $module_handler, \Drupal\service_container\Messenger\MessengerInterface $messenger, \Drupal\service_container\Legacy\Drupal7 $drupal7)

Constructs an InlineJS plugin.



* Visibility: **public**


#### Arguments
* $configuration **array** - &lt;p&gt;The configuration array.&lt;/p&gt;
* $plugin_id **string** - &lt;p&gt;The plugin id.&lt;/p&gt;
* $plugin_definition **array** - &lt;p&gt;The plugin definition.&lt;/p&gt;
* $module_handler **Drupal\Core\Extension\ModuleHandlerInterface**
* $messenger **Drupal\service_container\Messenger\MessengerInterface**
* $drupal7 **Drupal\service_container\Legacy\Drupal7**



### optionsForm

    mixed Drupal\openlayers\Types\ObjectInterface::optionsForm(array $form, array $form_state)

Provides the options form to configure this object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $form **array** - &lt;p&gt;The form array by reference.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### init

    mixed Drupal\openlayers\Types\ObjectInterface::init()

Initializes the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### optionsFormValidate

    mixed Drupal\openlayers\Types\ObjectInterface::optionsFormValidate(array $form, array $form_state)

Validation callback for the options form.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $form **array** - &lt;p&gt;The form array.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### optionsFormSubmit

    mixed Drupal\openlayers\Types\ObjectInterface::optionsFormSubmit(array $form, array $form_state)

Submit callback for the options form.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $form **array** - &lt;p&gt;The form array.&lt;/p&gt;
* $form_state **array** - &lt;p&gt;The form_state array by reference.&lt;/p&gt;



### preBuild

    mixed Drupal\openlayers\Types\ObjectInterface::preBuild(array $build, \Drupal\openlayers\Types\ObjectInterface $context)

Invoked before an objects render array is built.

Mostly invoked by the map object.

* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $build **array** - &lt;p&gt;The array with the build information.&lt;/p&gt;
* $context **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;The context of the build. Mostly the map object.&lt;/p&gt;



### postBuild

    mixed Drupal\openlayers\Types\ObjectInterface::postBuild(array $build, \Drupal\openlayers\Types\ObjectInterface $context)

Invoked after an objects render array is built.

Mostly invoked by the map object.

* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $build **array** - &lt;p&gt;The array with the build information.&lt;/p&gt;
* $context **[Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)** - &lt;p&gt;The context of the build. Mostly the map object.&lt;/p&gt;



### clearOption

    mixed Drupal\openlayers\Types\ObjectInterface::clearOption(string|array $parents)





* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $parents **string|array**



### setOption

    mixed Drupal\openlayers\Types\ObjectInterface::setOption(string|array $parents, mixed $value)

Set an option.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $parents **string|array**
* $value **mixed** - &lt;p&gt;The value to set.&lt;/p&gt;



### getOptions

    array Drupal\openlayers\Types\ObjectInterface::getOptions()

Return the options array.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### setOptions

    mixed Drupal\openlayers\Types\ObjectInterface::setOptions(array $options)

Set the options array.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $options **array** - &lt;p&gt;The options array.&lt;/p&gt;



### getExport

    \StdClass Drupal\openlayers\Types\ObjectInterface::getExport()

Return an object, CTools Exportable.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getConfiguration

    array Drupal\openlayers\Types\ObjectInterface::getConfiguration()

Return the object configuration.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getMachineName

    string Drupal\openlayers\Types\ObjectInterface::getMachineName()

Return the unique machine name of the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getName

    string Drupal\openlayers\Types\ObjectInterface::getName()

Return the human name of the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getDescription

    string Drupal\openlayers\Types\ObjectInterface::getDescription()

Return the description of the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getFactoryService

    string Drupal\openlayers\Types\ObjectInterface::getFactoryService()

Return the Factory Service of the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getOption

    mixed Drupal\openlayers\Types\ObjectInterface::getOption(string|array $parents, mixed $default_value)

Returns an option.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $parents **string|array**
* $default_value **mixed** - &lt;p&gt;The default value to return if the option isn&#039;t set. Set to NULL if not
defined.&lt;/p&gt;



### attached

    array Drupal\openlayers\Types\ObjectInterface::attached()

Returns a list of attachments for building the render array.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getObjects

    array Drupal\openlayers\Types\ObjectInterface::getObjects(string $type)

Return an array of OL objects indexed by their type.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $type **string**



### getParents

    array Drupal\openlayers\Types\ObjectInterface::getParents()

Returns an array with the maps this object is attached on.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### dependencies

    array Drupal\openlayers\Types\ObjectInterface::dependencies()

Defines dependencies.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getProvider

    string Drupal\openlayers\Types\ObjectInterface::getProvider()

Return the module that provides this plugin.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getClassDirectory

    string Drupal\openlayers\Types\ObjectInterface::getClassDirectory()

Returns the path to the plugin directory.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getClassPath

    string Drupal\openlayers\Types\ObjectInterface::getClassPath()

Returns the path to the class file.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### isAsynchronous

    boolean Drupal\openlayers\Types\ObjectInterface::isAsynchronous()

Whether or not this object has to be processed asynchronously.

If true the map this object relates to won't be processes right away by
Drupals behaviour attach.

* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getType

    string|FALSE Drupal\openlayers\Types\ObjectInterface::getType()

The type of this object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getCollection

    \Drupal\openlayers\Types\Collection Drupal\openlayers\Types\ObjectInterface::getCollection()

Return the Collection object linked to the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### optionsToObjects

    array<mixed,Object> Drupal\openlayers\Types\ObjectInterface::optionsToObjects()

Return a flat array containing Openlayers Objects from the options array.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getJS

    array Drupal\openlayers\Types\ObjectInterface::getJS()

Return the JS to insert in the page when building the object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### setWeight

    void Drupal\openlayers\Types\ObjectInterface::setWeight(integer $weight)

Set the weight of an object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)


#### Arguments
* $weight **integer**



### getWeight

    integer Drupal\openlayers\Types\ObjectInterface::getWeight()

Get the weight of an object.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### getPluginDescription

    string Drupal\openlayers\Types\ObjectInterface::getPluginDescription()

Return the description of the object's plugin.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)




### i18nStringsRefresh

    mixed Drupal\openlayers\Types\ObjectInterface::i18nStringsRefresh()

Refresh string translations.



* Visibility: **public**
* This method is defined by [Drupal\openlayers\Types\ObjectInterface](Drupal-openlayers-Types-ObjectInterface.md)



