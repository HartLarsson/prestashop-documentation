Class ConfigurationCore
=====================





* Class name: ConfigurationCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Configuration.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L27)


Contents
--------


### Properties

* [$_cache](#property-$_cache)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$definition](#property-$definition)
* [$id](#property-$id)
* [$id_shop](#property-$id_shop)
* [$id_shop_group](#property-$id_shop_group)
* [$name](#property-$name)
* [$types](#property-$types)
* [$value](#property-$value)
* [$webserviceParameters](#property-$webserviceParameters)
* [$db](#property-$db)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$force_id](#property-$force_id)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id_lang](#property-$id_lang)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [clearCache](#method-clearCache)
* [configurationIsLoaded](#method-configurationIsLoaded)
* [delete](#method-delete)
* [deleteByName](#method-deleteByName)
* [deleteFromContext](#method-deleteFromContext)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateObject](#method-duplicateObject)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [get](#method-get)
* [getAssociatedShops](#method-getAssociatedShops)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getGlobalValue](#method-getGlobalValue)
* [getIdByName](#method-getIdByName)
* [getInt](#method-getInt)
* [getMultiShopValues](#method-getMultiShopValues)
* [getMultiple](#method-getMultiple)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasContext](#method-hasContext)
* [hasKey](#method-hasKey)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangKey](#method-isLangKey)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [isOverridenByCurrentContext](#method-isOverridenByCurrentContext)
* [loadConfiguration](#method-loadConfiguration)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [set](#method-set)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [sqlRestriction](#method-sqlRestriction)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateGlobalValue](#method-updateGlobalValue)
* [updateMultishopTable](#method-updateMultishopTable)
* [updateValue](#method-updateValue)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)




Properties
----------


### <a name="property-$_cache"></a>$_cache

```php
protected array $_cache = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Configuration.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L64).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/Configuration.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L41).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* Source: [classes/Configuration.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L44).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'configuration', 'primary' => 'id_configuration', 'multilang' => true, 'fields' => array('name' => array('type' => self::TYPE_STRING, 'validate' => 'isConfigName', 'required' => true, 'size' => 254), 'id_shop_group' => array('type' => self::TYPE_NOTHING, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_NOTHING, 'validate' => 'isUnsignedId'), 'value' => array('type' => self::TYPE_STRING), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Configuration.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L49).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/Configuration.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L29).


### <a name="property-$id_shop"></a>$id_shop

```php
public mixed $id_shop
```





* Visibility: **public**
* Source: [classes/Configuration.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L35).


### <a name="property-$id_shop_group"></a>$id_shop_group

```php
public mixed $id_shop_group
```





* Visibility: **public**
* Source: [classes/Configuration.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L34).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Configuration.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L32).


### <a name="property-$types"></a>$types

```php
protected array $types = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Configuration.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L67).


### <a name="property-$value"></a>$value

```php
public string $value
```





* Visibility: **public**
* Source: [classes/Configuration.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L38).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('fields' => array('value' => array()))
```





* Visibility: **protected**
* Source: [classes/Configuration.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L69).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 141](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L141).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 131](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L131).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L106).


### <a name="property-$force_id"></a>$force_id

```php
public \boolean, $force_id = false
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 146](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L146).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L64).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L58).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L120).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 136](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L136).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 174](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L174)


#### Arguments
* $id **integer** - Existing object id in order to load object (optional)
* $id_lang **integer** - Required if object is multilingual (optional)
* $id_shop **integer** - ID shop for objects with multishop on langs



### <a name="method-add"></a>add

```php
boolean ObjectModelCore::add(boolean $autodate, boolean $null_values)
```

Add current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 441](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L441)


#### Arguments
* $autodate **boolean**
* $null_values **boolean**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1227](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1227)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1279](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1279)


#### Arguments
* $id_shops **integer|array**



### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1214](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1214)


#### Arguments
* $all **mixed**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1241](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1241)


#### Arguments
* $all **mixed**



### <a name="method-configurationIsLoaded"></a>configurationIsLoaded

```php
mixed ConfigurationCore::configurationIsLoaded()
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 107](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L107)




### <a name="method-delete"></a>delete

```php
boolean ObjectModelCore::delete()
```

Delete current object from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 706](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L706)




### <a name="method-deleteByName"></a>deleteByName

```php
boolean ConfigurationCore::deleteByName(string $key)
```

Delete a configuration key in database (with or without language management)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 417](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L417)


#### Arguments
* $key **string** - Key to delete



### <a name="method-deleteFromContext"></a>deleteFromContext

```php
mixed ConfigurationCore::deleteFromContext(string $key)
```

Delete configuration key from current context.



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 444](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L444)


#### Arguments
* $key **string**



### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1410](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1410)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 752](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L752)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 997](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L997)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateObject"></a>duplicateObject

```php
\new ObjectModelCore::duplicateObject()
```

Duplicate current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 532](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L532)




### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1323](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1323)


#### Arguments
* $id **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1447](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1447)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 331](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L331)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes, $purify)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 378](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L378)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**
* $purify **mixed**



### <a name="method-get"></a>get

```php
string ConfigurationCore::get(string $key, integer $id_lang, $id_shop_group, $id_shop)
```

Get a single configuration value (in one language only)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 162](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L162)


#### Arguments
* $key **string** - Key wanted
* $id_lang **integer** - Language ID
* $id_shop_group **mixed**
* $id_shop **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1308](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1308)




### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1553](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1553)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1660](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1660)


#### Arguments
* $field_name **mixed**
* $id_lang **null**



### <a name="method-getFields"></a>getFields

```php
array ObjectModelCore::getFields()
```

Prepare fields for ObjectModel class (add, update)
All fields are verified (pSQL, intval.

..)

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 259](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L259)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ConfigurationCore::getFieldsLang()
```





* Visibility: **public**
* Source: [classes/Configuration.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L79)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1206](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1206)


#### Arguments
* $all **mixed**



### <a name="method-getFieldsShop"></a>getFieldsShop

```php
array ObjectModelCore::getFieldsShop()
```

Prepare fields for multishop
Fields are not validated here, we considere they are already validated in getFields() method, this
not the best solution but this is the only one possible for retro compatibility.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 282](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L282)




### <a name="method-getGlobalValue"></a>getGlobalValue

```php
mixed ConfigurationCore::getGlobalValue($key, $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 192](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L192)


#### Arguments
* $key **mixed**
* $id_lang **mixed**



### <a name="method-getIdByName"></a>getIdByName

```php
mixed ConfigurationCore::getIdByName(string $key, integer $id_shop_group, integer $id_shop)
```

Return ID a configuration key



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L93)


#### Arguments
* $key **string**
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-getInt"></a>getInt

```php
array ConfigurationCore::getInt(string $key, integer $id_shop_group, integer $id_shop)
```

Get a single configuration value (in multiple languages)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 205](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L205)


#### Arguments
* $key **string** - Key wanted
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-getMultiShopValues"></a>getMultiShopValues

```php
array ConfigurationCore::getMultiShopValues(string $key, integer $id_lang)
```

Get a single configuration value for all shops



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 221](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L221)


#### Arguments
* $key **string** - Key wanted
* $id_lang **integer**



### <a name="method-getMultiple"></a>getMultiple

```php
array ConfigurationCore::getMultiple(array $keys, integer $id_lang, $id_shop_group, $id_shop)
```

Get several configuration values (in one language only)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 238](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L238)


#### Arguments
* $keys **array** - Keys wanted
* $id_lang **integer** - Language ID
* $id_shop_group **mixed**
* $id_shop **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 787](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L787)


#### Arguments
* $fields_array **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $class)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 154](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L154)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
array ConfigurationCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```

This method is override to allow TranslatedConfiguration entity



* Visibility: **public**
* Source: [classes/Configuration.php line 552](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L552)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed ObjectModelCore::getWebserviceParameters($ws_params_attribute_name)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1069](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1069)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasContext"></a>hasContext

```php
mixed ConfigurationCore::hasContext(string $key, integer $id_lang, integer $context)
```

Check if configuration var is defined in given context



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 472](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L472)


#### Arguments
* $key **string**
* $id_lang **integer**
* $context **integer**



### <a name="method-hasKey"></a>hasKey

```php
boolean ConfigurationCore::hasKey(string $key, integer $id_lang, integer $id_shop_group, integer $id_shop)
```

Check if key exists in configuration



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 264](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L264)


#### Arguments
* $key **string**
* $id_lang **integer**
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1348](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1348)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1485](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1485)


#### Arguments
* $data **array**
* $id_lang **integer**



### <a name="method-hydrateCollection"></a>hydrateCollection

```php
array ObjectModelCore::hydrateCollection(string $class, array $datas, integer $id_lang)
```

Fill (hydrate) a list of objects in order to get a collection of these objects



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1504](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1504)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1256](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1256)


#### Arguments
* $id_shop **integer**



### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean ObjectModelCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1465](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1465)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangKey"></a>isLangKey

```php
boolean ConfigurationCore::isLangKey(string $key)
```

Check if a key was loaded as multi lang



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 521](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L521)


#### Arguments
* $key **string**



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1365](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1365)




### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1360](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1360)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1355](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1355)




### <a name="method-isOverridenByCurrentContext"></a>isOverridenByCurrentContext

```php
mixed ConfigurationCore::isOverridenByCurrentContext($key)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 496](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L496)


#### Arguments
* $key **mixed**



### <a name="method-loadConfiguration"></a>loadConfiguration

```php
mixed ConfigurationCore::loadConfiguration()
```

Load all configuration data



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 126](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L126)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 803](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L803)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 429](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L429)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-set"></a>set

```php
mixed ConfigurationCore::set(string $key, mixed $values, integer $id_shop_group, integer $id_shop)
```

Set TEMPORARY a single configuration value (in one language only)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 282](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L282)


#### Arguments
* $key **string** - Key wanted
* $values **mixed** - $values is an array if the configuration is multilingual, a single string else.
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1591](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1591)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1686](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1686)


#### Arguments
* $fields **array**



### <a name="method-sqlRestriction"></a>sqlRestriction

```php
string ConfigurationCore::sqlRestriction(integer $id_shop_group, integer $id_shop)
```

Add SQL restriction on shops for configuration table



* Visibility: **protected**
* This method is **static**.
* Source: [classes/Configuration.php line 533](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L533)


#### Arguments
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 768](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L768)




### <a name="method-update"></a>update

```php
boolean ObjectModelCore::update(boolean $null_values)
```

Update current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 588](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L588)


#### Arguments
* $null_values **boolean**



### <a name="method-updateGlobalValue"></a>updateGlobalValue

```php
boolean ConfigurationCore::updateGlobalValue(string $key, mixed $values, boolean $html)
```

Update configuration key for global context only



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 314](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L314)


#### Arguments
* $key **string**
* $values **mixed**
* $html **boolean**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1380](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1380)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-updateValue"></a>updateValue

```php
boolean ConfigurationCore::updateValue(string $key, mixed $values, boolean $html, integer $id_shop_group, integer $id_shop)
```

Update configuration key and value into database (automatically insert if key does not exist)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Configuration.php line 329](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/Configuration.php#L329)


#### Arguments
* $key **string** - Key
* $values **mixed** - $values is an array if the configuration is multilingual, a single string else.
* $html **boolean** - Specify if html is authorized in value
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1015](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1015)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1021](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1021)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang, $skip, $human_errors)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 914](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L914)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**
* $skip **mixed**
* $human_errors **mixed**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string ObjectModelCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 841](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L841)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsLang"></a>validateFieldsLang

```php
boolean|string ObjectModelCore::validateFieldsLang(boolean $die, boolean $error_return)
```

Check for multilingual fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 870](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L870)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1183](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.10/classes/ObjectModel.php#L1183)


#### Arguments
* $htmlentities **mixed**


