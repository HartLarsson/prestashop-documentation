Class TaxCore
=====================





* Class name: TaxCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/tax/Tax.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L28)


Contents
--------


### Properties

* [$_product_country_tax](#property-$_product_country_tax)
* [$_product_tax_via_rules](#property-$_product_tax_via_rules)
* [$active](#property-$active)
* [$definition](#property-$definition)
* [$deleted](#property-$deleted)
* [$name](#property-$name)
* [$rate](#property-$rate)
* [$webserviceParameters](#property-$webserviceParameters)

### Methods

* [_onStatusChange](#method-_onStatusChange)
* [delete](#method-delete)
* [excludeTaxeOption](#method-excludeTaxeOption)
* [getCarrierTaxRate](#method-getCarrierTaxRate)
* [getProductEcotaxRate](#method-getProductEcotaxRate)
* [getProductTaxRate](#method-getProductTaxRate)
* [getProductTaxRateViaRules](#method-getProductTaxRateViaRules)
* [getTaxIdByName](#method-getTaxIdByName)
* [getTaxes](#method-getTaxes)
* [historize](#method-historize)
* [isUsed](#method-isUsed)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)




Properties
----------


### <a name="property-$_product_country_tax"></a>$_product_country_tax

```php
protected mixed $_product_country_tax = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/tax/Tax.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L59).


### <a name="property-$_product_tax_via_rules"></a>$_product_tax_via_rules

```php
protected mixed $_product_tax_via_rules = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/tax/Tax.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L60).


### <a name="property-$active"></a>$active

```php
public boolean $active
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L37).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'tax', 'primary' => 'id_tax', 'multilang' => true, 'fields' => array('rate' => array('type' => self::TYPE_FLOAT, 'validate' => 'isFloat', 'required' => true), 'active' => array('type' => self::TYPE_BOOL), 'deleted' => array('type' => self::TYPE_BOOL), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 32)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/tax/Tax.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L45).


### <a name="property-$deleted"></a>$deleted

```php
public boolean $deleted
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L40).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L31).


### <a name="property-$rate"></a>$rate

```php
public float $rate
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L34).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectsNodeName' => 'taxes')
```





* Visibility: **protected**
* Source: [classes/tax/Tax.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L62).


Methods
-------


### <a name="method-_onStatusChange"></a>_onStatusChange

```php
mixed TaxCore::_onStatusChange()
```





* Visibility: **protected**
* Source: [classes/tax/Tax.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L117)




### <a name="method-delete"></a>delete

```php
mixed TaxCore::delete()
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L66)




### <a name="method-excludeTaxeOption"></a>excludeTaxeOption

```php
mixed TaxCore::excludeTaxeOption()
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 164](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L164)




### <a name="method-getCarrierTaxRate"></a>getCarrierTaxRate

```php
float TaxCore::getCarrierTaxRate($id_carrier, $id_address)
```

Returns the carrier tax rate



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 209](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L209)


#### Arguments
* $id_carrier **mixed**
* $id_address **mixed**



### <a name="method-getProductEcotaxRate"></a>getProductEcotaxRate

```php
float TaxCore::getProductEcotaxRate($id_address)
```

Returns the ecotax tax rate



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 193](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L193)


#### Arguments
* $id_address **mixed**



### <a name="method-getProductTaxRate"></a>getProductTaxRate

```php
\Tax TaxCore::getProductTaxRate(integer $id_product, $id_address, \Context $context)
```

Returns the product tax



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L249)


#### Arguments
* $id_product **integer**
* $id_address **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-getProductTaxRateViaRules"></a>getProductTaxRateViaRules

```php
\Tax TaxCore::getProductTaxRateViaRules(integer $id_product, integer $id_country, $id_state, $zipcode)
```

Return the product tax rate using the tax rules system



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 229](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L229)


#### Arguments
* $id_product **integer**
* $id_country **integer**
* $id_state **mixed**
* $zipcode **mixed**



### <a name="method-getTaxIdByName"></a>getTaxIdByName

```php
mixed TaxCore::getTaxIdByName(string $tax_name, boolean $active)
```

Return the tax id associated to the specified name



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 175](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L175)


#### Arguments
* $tax_name **string**
* $active **boolean** - (true by default)



### <a name="method-getTaxes"></a>getTaxes

```php
array TaxCore::getTaxes($id_lang, $active_only)
```

Get all available taxes



* Visibility: **public**
* This method is **static**.
* Source: [classes/tax/Tax.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L144)


#### Arguments
* $id_lang **mixed**
* $active_only **mixed**



### <a name="method-historize"></a>historize

```php
mixed TaxCore::historize()
```

Save the object with the field deleted to true

@return bool

* Visibility: **public**
* Source: [classes/tax/Tax.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L82)




### <a name="method-isUsed"></a>isUsed

```php
boolean TaxCore::isUsed()
```

Returns true if the tax is used in an order details



* Visibility: **public**
* Source: [classes/tax/Tax.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L130)




### <a name="method-toggleStatus"></a>toggleStatus

```php
mixed TaxCore::toggleStatus()
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 88](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L88)




### <a name="method-update"></a>update

```php
mixed TaxCore::update($null_values)
```





* Visibility: **public**
* Source: [classes/tax/Tax.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/classes/tax/Tax.php#L96)


#### Arguments
* $null_values **mixed**

