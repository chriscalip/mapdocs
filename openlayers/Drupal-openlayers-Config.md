Drupal\openlayers\Config
===============

Class openlayers_config.




* Class name: Config
* Namespace: Drupal\openlayers







Methods
-------


### defaults

    array|null Drupal\openlayers\Config::defaults(string $key)

Get default configuration.



* Visibility: **protected**
* This method is **static**.


#### Arguments
* $key **string** - &lt;p&gt;Key to get. If not provided, returns the full array.&lt;/p&gt;



### get

    mixed Drupal\openlayers\Config::get(string|array $parents, string|array $default_value)

Fetches a configuration value.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $parents **string|array** - &lt;p&gt;The path to the configuration value. Strings use dots as path separator.&lt;/p&gt;
* $default_value **string|array** - &lt;p&gt;The default value to use if the config value isn&#039;t set.&lt;/p&gt;



### set

    array Drupal\openlayers\Config::set(string|array $parents, mixed $value)

Sets a configuration value.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $parents **string|array** - &lt;p&gt;The path to the configuration value. Strings use dots as path separator.&lt;/p&gt;
* $value **mixed** - &lt;p&gt;The  value to set.&lt;/p&gt;



### clear

    array Drupal\openlayers\Config::clear(string|array $parents)

Removes a configuration value.



* Visibility: **public**
* This method is **static**.


#### Arguments
* $parents **string|array** - &lt;p&gt;The path to the configuration value. Strings use dots as path separator.&lt;/p&gt;


