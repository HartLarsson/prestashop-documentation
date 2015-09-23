Class StoreCore
=====================





* Class name: StoreCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Store.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L28)


Contents
--------


### Properties

* [$active](#property-$active)
* [$address1](#property-$address1)
* [$address2](#property-$address2)
* [$city](#property-$city)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$email](#property-$email)
* [$fax](#property-$fax)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsValidate](#property-$fieldsValidate)
* [$hours](#property-$hours)
* [$id_country](#property-$id_country)
* [$id_state](#property-$id_state)
* [$identifier](#property-$identifier)
* [$latitude](#property-$latitude)
* [$longitude](#property-$longitude)
* [$name](#property-$name)
* [$note](#property-$note)
* [$phone](#property-$phone)
* [$postcode](#property-$postcode)
* [$table](#property-$table)
* [$webserviceParameters](#property-$webserviceParameters)
* [$_cache](#property-$_cache)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$id](#property-$id)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$langMultiShop](#property-$langMultiShop)
* [$tables](#property-$tables)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [getFields](#method-getFields)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsValidateLang](#method-getFieldsValidateLang)
* [getIdentifier](#method-getIdentifier)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [getWsHours](#method-getWsHours)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToGroupShop](#method-isAssociatedToGroupShop)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setWsHours](#method-setWsHours)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)




Properties
----------


### <a name="property-$active"></a>$active

```php
public boolean $active = true
```





* Visibility: **public**
* Source: [classes/Store.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L79).


### <a name="property-$address1"></a>$address1

```php
public string $address1
```





* Visibility: **public**
* Source: [classes/Store.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L40).


### <a name="property-$address2"></a>$address2

```php
public string $address2
```





* Visibility: **public**
* Source: [classes/Store.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L43).


### <a name="property-$city"></a>$city

```php
public string $city
```





* Visibility: **public**
* Source: [classes/Store.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L49).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/Store.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L73).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* Source: [classes/Store.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L76).


### <a name="property-$email"></a>$email

```php
public string $email
```





* Visibility: **public**
* Source: [classes/Store.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L70).


### <a name="property-$fax"></a>$fax

```php
public string $fax
```





* Visibility: **public**
* Source: [classes/Store.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L64).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array('id_country', 'name', 'address1', 'city', 'active')
```





* Visibility: **protected**
* Source: [classes/Store.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L81).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array('name' => 128, 'address1' => 128, 'address2' => 128, 'postcode' => 12, 'city' => 64, 'latitude' => 12, 'longitude' => 12, 'hours' => 254, 'phone' => 16, 'fax' => 16, 'email' => 128, 'note' => 65000)
```





* Visibility: **protected**
* Source: [classes/Store.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L82).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array('id_country' => 'isUnsignedId', 'id_state' => 'isNullOrUnsignedId', 'name' => 'isGenericName', 'address1' => 'isAddress', 'address2' => 'isAddress', 'city' => 'isCityName', 'latitude' => 'isCoordinate', 'longitude' => 'isCoordinate', 'hours' => 'isSerializedArray', 'phone' => 'isPhoneNumber', 'fax' => 'isPhoneNumber', 'note' => 'isCleanHtml', 'email' => 'isEmail', 'active' => 'isBool')
```





* Visibility: **protected**
* Source: [classes/Store.php line 83](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L83).


### <a name="property-$hours"></a>$hours

```php
public string $hours
```





* Visibility: **public**
* Source: [classes/Store.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L58).


### <a name="property-$id_country"></a>$id_country

```php
public integer $id_country
```





* Visibility: **public**
* Source: [classes/Store.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L31).


### <a name="property-$id_state"></a>$id_state

```php
public integer $id_state
```





* Visibility: **public**
* Source: [classes/Store.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L34).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier = 'id_store'
```





* Visibility: **protected**
* Source: [classes/Store.php line 88](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L88).


### <a name="property-$latitude"></a>$latitude

```php
public float $latitude
```





* Visibility: **public**
* Source: [classes/Store.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L52).


### <a name="property-$longitude"></a>$longitude

```php
public float $longitude
```





* Visibility: **public**
* Source: [classes/Store.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L55).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Store.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L37).


### <a name="property-$note"></a>$note

```php
public string $note
```





* Visibility: **public**
* Source: [classes/Store.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L67).


### <a name="property-$phone"></a>$phone

```php
public string $phone
```





* Visibility: **public**
* Source: [classes/Store.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L61).


### <a name="property-$postcode"></a>$postcode

```php
public string $postcode
```





* Visibility: **public**
* Source: [classes/Store.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L46).


### <a name="property-$table"></a>$table

```php
protected mixed $table = 'store'
```





* Visibility: **protected**
* Source: [classes/Store.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L87).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('fields' => array('id_country' => array('xlink_resource' => 'countries'), 'id_state' => array('xlink_resource' => 'states'), 'hours' => array('getter' => 'getWsHours', 'setter' => 'setWsHours')))
```





* Visibility: **protected**
* Source: [classes/Store.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L90).


### <a name="property-$_cache"></a>$_cache

```php
protected mixed $_cache = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L75).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected \fieldsRequiredDatabase $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L50).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected array $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L59).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected array $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L62).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected array $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L65).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L31).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L34).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L36).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L78).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L81).


### <a name="property-$langMultiShop"></a>$langMultiShop

```php
protected mixed $langMultiShop = false
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L67).


### <a name="property-$tables"></a>$tables

```php
protected array $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L70).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed StoreCore::__construct($id_store, $id_lang)
```





* Visibility: **public**
* Source: [classes/Store.php line 123](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L123)


#### Arguments
* $id_store **mixed**
* $id_lang **mixed**



### <a name="method-add"></a>add

```php
mixed ObjectModelCore::add($autodate, $nullValues)
```

Add current object to database

return boolean Insertion result

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 202](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L202)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 780](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L780)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops, string $type)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 828](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L828)


#### Arguments
* $id_shops **integer|array**
* $type **string**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 794](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L794)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
mixed ObjectModelCore::delete()
```

Delete current object from database

return boolean Deletion result

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 349](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L349)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage()
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 898](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L898)




### <a name="method-deleteSelection"></a>deleteSelection

```php
mixed ObjectModelCore::deleteSelection($selection)
```

Delete several objects from database

return boolean Deletion result

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 387](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L387)


#### Arguments
* $selection **mixed**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $className, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 558](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L558)


#### Arguments
* $field **mixed**
* $className **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 868](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L868)


#### Arguments
* $id **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase($id_entity, $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 931](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L931)


#### Arguments
* $id_entity **mixed** - entity id
* $table **mixed**



### <a name="method-getFields"></a>getFields

```php
mixed StoreCore::getFields()
```





* Visibility: **public**
* Source: [classes/Store.php line 98](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L98)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L772)


#### Arguments
* $all **mixed**



### <a name="method-getFieldsValidateLang"></a>getFieldsValidateLang

```php
array ObjectModelCore::getFieldsValidateLang()
```

Get list of fields related to language to validate



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 975](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L975)




### <a name="method-getIdentifier"></a>getIdentifier

```php
string ObjectModelCore::getIdentifier()
```

Get object identifier name



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 964](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L964)




### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields(array $fieldsArray)
```

Prepare multilingual fields for database insertion



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 430](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L430)


#### Arguments
* $fieldsArray **array** - Multilingual fields to prepare
return array Prepared fields for database insertion



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $className)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 89](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L89)


#### Arguments
* $className **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 747](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L747)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed ObjectModelCore::getWebserviceParameters($wsParamsAttributeName)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 617](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L617)


#### Arguments
* $wsParamsAttributeName **mixed**



### <a name="method-getWsHours"></a>getWsHours

```php
mixed StoreCore::getWsHours()
```





* Visibility: **public**
* Source: [classes/Store.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L130)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 987](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L987)


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
* Source: [classes/ObjectModel.php line 1006](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L1006)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToGroupShop"></a>isAssociatedToGroupShop

```php
boolean ObjectModelCore::isAssociatedToGroupShop(integer $id_group_shop)
```

Check if current object is associated to a group shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 854](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L854)


#### Arguments
* $id_group_shop **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 809](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L809)


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
* Source: [classes/ObjectModel.php line 948](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L948)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 888](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L888)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fieldsArray, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 447](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L447)


#### Arguments
* $fields **mixed**
* $fieldsArray **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
mixed ObjectModelCore::save($nullValues, $autodate)
```

Save current object to database (add or update)

return boolean Insertion result

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 192](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L192)


#### Arguments
* $nullValues **mixed**
* $autodate **mixed**



### <a name="method-setWsHours"></a>setWsHours

```php
mixed StoreCore::setWsHours($hours)
```





* Visibility: **public**
* Source: [classes/Store.php line 135](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/Store.php#L135)


#### Arguments
* $hours **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
mixed ObjectModelCore::toggleStatus()
```

Toggle object status in database

return boolean Update result

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 405](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L405)




### <a name="method-update"></a>update

```php
boolean ObjectModelCore::update($nullValues)
```

Update current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 274](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L274)


#### Arguments
* $nullValues **mixed**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 571](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L571)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 577](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L577)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateFields"></a>validateFields

```php
mixed ObjectModelCore::validateFields($die, $errorReturn)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 481](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L481)


#### Arguments
* $die **mixed**
* $errorReturn **mixed**



### <a name="method-validateFieldsLang"></a>validateFieldsLang

```php
mixed ObjectModelCore::validateFieldsLang($die, $errorReturn)
```

Check for multilingual fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 514](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.1/classes/ObjectModel.php#L514)


#### Arguments
* $die **mixed**
* $errorReturn **mixed**

