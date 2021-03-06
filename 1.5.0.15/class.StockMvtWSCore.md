Class StockMvtWSCore
=====================

Webservice entity for stock movements



* Class name: StockMvtWSCore
* Parent class: [ObjectModelCore](class.ObjectModelCore.md)
* Source: [classes/stock/StockMvtWS.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L32)


Contents
--------

### Constants

* [FORMAT_COMMON](#constant-FORMAT_COMMON)
* [FORMAT_LANG](#constant-FORMAT_LANG)
* [FORMAT_SHOP](#constant-FORMAT_SHOP)
* [HAS_MANY](#constant-HAS_MANY)
* [HAS_ONE](#constant-HAS_ONE)
* [TYPE_BOOL](#constant-TYPE_BOOL)
* [TYPE_DATE](#constant-TYPE_DATE)
* [TYPE_FLOAT](#constant-TYPE_FLOAT)
* [TYPE_HTML](#constant-TYPE_HTML)
* [TYPE_INT](#constant-TYPE_INT)
* [TYPE_NOTHING](#constant-TYPE_NOTHING)
* [TYPE_STRING](#constant-TYPE_STRING)

### Properties

* [$current_wa](#property-$current_wa)
* [$date_add](#property-$date_add)
* [$db](#property-$db)
* [$def](#property-$def)
* [$definition](#property-$definition)
* [$ean13](#property-$ean13)
* [$employee_firstname](#property-$employee_firstname)
* [$employee_lastname](#property-$employee_lastname)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id](#property-$id)
* [$id_currency](#property-$id_currency)
* [$id_employee](#property-$id_employee)
* [$id_lang](#property-$id_lang)
* [$id_order](#property-$id_order)
* [$id_product](#property-$id_product)
* [$id_product_attribute](#property-$id_product_attribute)
* [$id_shop](#property-$id_shop)
* [$id_shop_list](#property-$id_shop_list)
* [$id_stock](#property-$id_stock)
* [$id_stock_mvt_reason](#property-$id_stock_mvt_reason)
* [$id_supply_order](#property-$id_supply_order)
* [$id_warehouse](#property-$id_warehouse)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$last_wa](#property-$last_wa)
* [$management_type](#property-$management_type)
* [$physical_quantity](#property-$physical_quantity)
* [$price_te](#property-$price_te)
* [$product_name](#property-$product_name)
* [$reference](#property-$reference)
* [$referer](#property-$referer)
* [$sign](#property-$sign)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$tables_assoc](#property-$tables_assoc)
* [$upc](#property-$upc)
* [$update_fields](#property-$update_fields)
* [$webserviceParameters](#property-$webserviceParameters)

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
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAssociatedShops](#method-getAssociatedShops)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWSProductName](#method-getWSProductName)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isMultishop](#method-isMultishop)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateMultishopTable](#method-updateMultishopTable)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)


Constants
----------


### <a name="constant-FORMAT_COMMON"></a>FORMAT_COMMON

```php
const FORMAT_COMMON = 1
```

List of data to format



* Source: [classes/stock/StockMvtWS.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L44).


### <a name="constant-FORMAT_LANG"></a>FORMAT_LANG

```php
const FORMAT_LANG = 2
```





* Source: [classes/stock/StockMvtWS.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L45).


### <a name="constant-FORMAT_SHOP"></a>FORMAT_SHOP

```php
const FORMAT_SHOP = 3
```





* Source: [classes/stock/StockMvtWS.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L46).


### <a name="constant-HAS_MANY"></a>HAS_MANY

```php
const HAS_MANY = 2
```





* Source: [classes/stock/StockMvtWS.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L52).


### <a name="constant-HAS_ONE"></a>HAS_ONE

```php
const HAS_ONE = 1
```

List of association types



* Source: [classes/stock/StockMvtWS.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L51).


### <a name="constant-TYPE_BOOL"></a>TYPE_BOOL

```php
const TYPE_BOOL = 2
```





* Source: [classes/stock/StockMvtWS.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L34).


### <a name="constant-TYPE_DATE"></a>TYPE_DATE

```php
const TYPE_DATE = 5
```





* Source: [classes/stock/StockMvtWS.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L37).


### <a name="constant-TYPE_FLOAT"></a>TYPE_FLOAT

```php
const TYPE_FLOAT = 4
```





* Source: [classes/stock/StockMvtWS.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L36).


### <a name="constant-TYPE_HTML"></a>TYPE_HTML

```php
const TYPE_HTML = 6
```





* Source: [classes/stock/StockMvtWS.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L38).


### <a name="constant-TYPE_INT"></a>TYPE_INT

```php
const TYPE_INT = 1
```

List of field types



* Source: [classes/stock/StockMvtWS.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L33).


### <a name="constant-TYPE_NOTHING"></a>TYPE_NOTHING

```php
const TYPE_NOTHING = 7
```





* Source: [classes/stock/StockMvtWS.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L39).


### <a name="constant-TYPE_STRING"></a>TYPE_STRING

```php
const TYPE_STRING = 3
```





* Source: [classes/stock/StockMvtWS.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L35).


Properties
----------


### <a name="property-$current_wa"></a>$current_wa

```php
public float $current_wa = null
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L94).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L39).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/stock/StockMvtWS.php line 141](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L141).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 131](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L131).


### <a name="property-$definition"></a>$definition

```php
public array $definition = array()
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/stock/StockMvtWS.php line 126](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L126).


### <a name="property-$ean13"></a>$ean13

```php
public string $ean13
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 139](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L139).


### <a name="property-$employee_firstname"></a>$employee_firstname

```php
public string $employee_firstname
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L49).


### <a name="property-$employee_lastname"></a>$employee_lastname

```php
public string $employee_lastname
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L54).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/stock/StockMvtWS.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L106).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L64).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L55).


### <a name="property-$id_currency"></a>$id_currency

```php
public integer $id_currency
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L124).


### <a name="property-$id_employee"></a>$id_employee

```php
public integer $id_employee
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L44).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L58).


### <a name="property-$id_order"></a>$id_order

```php
public integer $id_order = null
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 74](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L74).


### <a name="property-$id_product"></a>$id_product

```php
public integer $id_product
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 109](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L109).


### <a name="property-$id_product_attribute"></a>$id_product_attribute

```php
public integer $id_product_attribute
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L114).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L60).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L62).


### <a name="property-$id_stock"></a>$id_stock

```php
public integer $id_stock
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L59).


### <a name="property-$id_stock_mvt_reason"></a>$id_stock_mvt_reason

```php
public integer $id_stock_mvt_reason
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L69).


### <a name="property-$id_supply_order"></a>$id_supply_order

```php
public integer $id_supply_order = null
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L84).


### <a name="property-$id_warehouse"></a>$id_warehouse

```php
public integer $id_warehouse
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L119).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L120).


### <a name="property-$last_wa"></a>$last_wa

```php
public float $last_wa = null
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 89](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L89).


### <a name="property-$management_type"></a>$management_type

```php
public string $management_type
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 129](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L129).


### <a name="property-$physical_quantity"></a>$physical_quantity

```php
public integer $physical_quantity
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L64).


### <a name="property-$price_te"></a>$price_te

```php
public float $price_te
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 99](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L99).


### <a name="property-$product_name"></a>$product_name

```php
public mixed $product_name
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 134](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L134).


### <a name="property-$reference"></a>$reference

```php
public string $reference
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 149](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L149).


### <a name="property-$referer"></a>$referer

```php
public integer $referer
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 104](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L104).


### <a name="property-$sign"></a>$sign

```php
public integer $sign
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L79).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L111).


### <a name="property-$tables_assoc"></a>$tables_assoc

```php
protected Array $tables_assoc = array('id_product' => array('table' => 's'), 'id_product_attribute' => array('table' => 's'), 'id_warehouse' => array('table' => 's'), 'id_currency' => array('table' => 's'), 'management_type' => array('table' => 'w'), 'ean13' => array('table' => 's'), 'upc' => array('table' => 's'), 'reference' => array('table' => 's'))
```

Associations tables for attributes that require different tables than stated in ObjectModel::definition



* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 206](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L206).


### <a name="property-$upc"></a>$upc

```php
public string $upc
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L144).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 136](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L136).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected array $webserviceParameters = array()
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L114).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed StockMvtWSCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 169](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L169)


#### Arguments
* $id **integer** - Existing object id in order to load object (optional)
* $id_lang **integer** - Required if object is multilingual (optional)
* $id_shop **integer** - ID shop for objects with multishop on langs



### <a name="method-add"></a>add

```php
boolean StockMvtWSCore::add(boolean $autodate, boolean $null_values)
```

Add current object to database



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 437](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L437)


#### Arguments
* $autodate **boolean**
* $null_values **boolean**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed StockMvtWSCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1049](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1049)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean StockMvtWSCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1096](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1096)


#### Arguments
* $id_shops **integer|array**



### <a name="method-clearCache"></a>clearCache

```php
mixed StockMvtWSCore::clearCache($all)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1063](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1063)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
boolean StockMvtWSCore::delete()
```

Delete current object from database



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 633](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L633)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean StockMvtWSCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1223](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1223)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean StockMvtWSCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 679](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L679)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed StockMvtWSCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 879](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L879)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed StockMvtWSCore::duplicateShops($id)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1140](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1140)


#### Arguments
* $id **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean StockMvtWSCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 1260](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1260)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array StockMvtWSCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 335](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L335)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed StockMvtWSCore::formatValue(mixed $value, integer $type, $with_quotes)
```

Format a data



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 381](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L381)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array StockMvtWSCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1125](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1125)




### <a name="method-getDefinition"></a>getDefinition

```php
array StockMvtWSCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 1363](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1363)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed StockMvtWSCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1440](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1440)


#### Arguments
* $field_name **mixed**
* $id_lang **null**



### <a name="method-getFields"></a>getFields

```php
array StockMvtWSCore::getFields()
```

Prepare fields for ObjectModel class (add, update)
All fields are verified (pSQL, intval.

..)

* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 263](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L263)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array StockMvtWSCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 300](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L300)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed StockMvtWSCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1041](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1041)


#### Arguments
* $all **mixed**



### <a name="method-getFieldsShop"></a>getFieldsShop

```php
array StockMvtWSCore::getFieldsShop()
```

Prepare fields for multishop
Fields are not validated here, we considere they are already validated in getFields() method, this
not the best solution but this is the only one possible for retro compatibility.



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 286](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L286)




### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed StockMvtWSCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 711](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L711)


#### Arguments
* $fields_array **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array StockMvtWSCore::getValidationRules(string $class)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 149](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L149)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWSProductName"></a>getWSProductName

```php
mixed StockMvtWSCore::getWSProductName()
```

Webservice : getter for the product name



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 282](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L282)




### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed StockMvtWSCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1015](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1015)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed StockMvtWSCore::getWebserviceParameters($ws_params_attribute_name)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 941](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L941)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean StockMvtWSCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1165](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1165)




### <a name="method-hydrate"></a>hydrate

```php
mixed StockMvtWSCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1295](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1295)


#### Arguments
* $data **array**
* $id_lang **integer**



### <a name="method-hydrateCollection"></a>hydrateCollection

```php
array StockMvtWSCore::hydrateCollection(string $class, array $datas, integer $id_lang)
```

Fill (hydrate) a list of objects in order to get a collection of these objects



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 1314](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1314)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean StockMvtWSCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1078](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1078)


#### Arguments
* $id_shop **integer**



### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean StockMvtWSCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 1278](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1278)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed StockMvtWSCore::isLangMultishop()
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1178](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1178)




### <a name="method-isMultishop"></a>isMultishop

```php
mixed StockMvtWSCore::isMultishop()
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1173](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1173)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed StockMvtWSCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 727](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L727)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
boolean StockMvtWSCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 425](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L425)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed StockMvtWSCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* Source: [classes/stock/StockMvtWS.php line 1386](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1386)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed StockMvtWSCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 1466](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1466)


#### Arguments
* $fields **array**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean StockMvtWSCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 695](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L695)




### <a name="method-update"></a>update

```php
boolean StockMvtWSCore::update(boolean $null_values)
```

Update current object to database



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 521](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L521)


#### Arguments
* $null_values **boolean**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean StockMvtWSCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* Source: [classes/stock/StockMvtWS.php line 1193](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L1193)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-validateControler"></a>validateControler

```php
mixed StockMvtWSCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 894](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L894)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed StockMvtWSCore::validateController($htmlentities)
```





* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 900](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L900)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string StockMvtWSCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 832](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L832)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string StockMvtWSCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 765](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L765)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsLang"></a>validateFieldsLang

```php
boolean|string StockMvtWSCore::validateFieldsLang(boolean $die, boolean $error_return)
```

Check for multilingual fields validity before database interaction



* Visibility: **public**
* Source: [classes/stock/StockMvtWS.php line 794](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.15/classes/stock/StockMvtWS.php#L794)


#### Arguments
* $die **boolean**
* $error_return **boolean**


