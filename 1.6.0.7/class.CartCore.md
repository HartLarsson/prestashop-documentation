Class CartCore
=====================





* Class name: CartCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Cart.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L27)


Contents
--------

### Constants

* [BOTH](#constant-BOTH)
* [BOTH_WITHOUT_SHIPPING](#constant-BOTH_WITHOUT_SHIPPING)
* [ONLY_DISCOUNTS](#constant-ONLY_DISCOUNTS)
* [ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING](#constant-ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING)
* [ONLY_PRODUCTS](#constant-ONLY_PRODUCTS)
* [ONLY_PRODUCTS_WITHOUT_SHIPPING](#constant-ONLY_PRODUCTS_WITHOUT_SHIPPING)
* [ONLY_SHIPPING](#constant-ONLY_SHIPPING)
* [ONLY_WRAPPING](#constant-ONLY_WRAPPING)

### Properties

* [$_attributesLists](#property-$_attributesLists)
* [$_carriers](#property-$_carriers)
* [$_isVirtualCart](#property-$_isVirtualCart)
* [$_nbProducts](#property-$_nbProducts)
* [$_products](#property-$_products)
* [$_taxCalculationMethod](#property-$_taxCalculationMethod)
* [$_taxes_rate](#property-$_taxes_rate)
* [$_totalWeight](#property-$_totalWeight)
* [$allow_seperated_package](#property-$allow_seperated_package)
* [$checkedTos](#property-$checkedTos)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$definition](#property-$definition)
* [$delivery_option](#property-$delivery_option)
* [$gift](#property-$gift)
* [$gift_message](#property-$gift_message)
* [$id](#property-$id)
* [$id_address_delivery](#property-$id_address_delivery)
* [$id_address_invoice](#property-$id_address_invoice)
* [$id_carrier](#property-$id_carrier)
* [$id_currency](#property-$id_currency)
* [$id_customer](#property-$id_customer)
* [$id_guest](#property-$id_guest)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$id_shop_group](#property-$id_shop_group)
* [$mobile_theme](#property-$mobile_theme)
* [$pictures](#property-$pictures)
* [$recyclable](#property-$recyclable)
* [$secure_key](#property-$secure_key)
* [$textFields](#property-$textFields)
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
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)

### Methods

* [__construct](#method-__construct)
* [_addCustomization](#method-_addCustomization)
* [_deleteCustomization](#method-_deleteCustomization)
* [_updateCustomizationQuantity](#method-_updateCustomizationQuantity)
* [add](#method-add)
* [addCartRule](#method-addCartRule)
* [addDiscount](#method-addDiscount)
* [addExtraCarriers](#method-addExtraCarriers)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [addPictureToProduct](#method-addPictureToProduct)
* [addTextFieldToProduct](#method-addTextFieldToProduct)
* [associateTo](#method-associateTo)
* [autosetProductAddress](#method-autosetProductAddress)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [cacheSomeAttributesLists](#method-cacheSomeAttributesLists)
* [carrierIsSelected](#method-carrierIsSelected)
* [checkDiscountValidity](#method-checkDiscountValidity)
* [checkQuantities](#method-checkQuantities)
* [clearCache](#method-clearCache)
* [containsProduct](#method-containsProduct)
* [delete](#method-delete)
* [deleteAssociations](#method-deleteAssociations)
* [deleteCustomizationToProduct](#method-deleteCustomizationToProduct)
* [deleteDiscount](#method-deleteDiscount)
* [deleteImage](#method-deleteImage)
* [deletePictureToProduct](#method-deletePictureToProduct)
* [deleteProduct](#method-deleteProduct)
* [deleteSelection](#method-deleteSelection)
* [desintifier](#method-desintifier)
* [displayFieldName](#method-displayFieldName)
* [duplicate](#method-duplicate)
* [duplicateObject](#method-duplicateObject)
* [duplicateProduct](#method-duplicateProduct)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAddressCollection](#method-getAddressCollection)
* [getAssociatedShops](#method-getAssociatedShops)
* [getCarrierCost](#method-getCarrierCost)
* [getCartByOrderId](#method-getCartByOrderId)
* [getCartIdByOrderId](#method-getCartIdByOrderId)
* [getCartRules](#method-getCartRules)
* [getCustomerCarts](#method-getCustomerCarts)
* [getDefinition](#method-getDefinition)
* [getDeliveryAddressesWithoutCarriers](#method-getDeliveryAddressesWithoutCarriers)
* [getDeliveryOption](#method-getDeliveryOption)
* [getDeliveryOptionList](#method-getDeliveryOptionList)
* [getDiscounts](#method-getDiscounts)
* [getDiscountsCustomer](#method-getDiscountsCustomer)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getGiftWrappingPrice](#method-getGiftWrappingPrice)
* [getIdCarrierFromDeliveryOption](#method-getIdCarrierFromDeliveryOption)
* [getLastProduct](#method-getLastProduct)
* [getNbOfPackages](#method-getNbOfPackages)
* [getNbProducts](#method-getNbProducts)
* [getOrderShippingCost](#method-getOrderShippingCost)
* [getOrderTotal](#method-getOrderTotal)
* [getOrderTotalUsingTaxCalculationMethod](#method-getOrderTotalUsingTaxCalculationMethod)
* [getPackageIdWarehouse](#method-getPackageIdWarehouse)
* [getPackageList](#method-getPackageList)
* [getPackageShippingCost](#method-getPackageShippingCost)
* [getProductCustomization](#method-getProductCustomization)
* [getProducts](#method-getProducts)
* [getSummaryDetails](#method-getSummaryDetails)
* [getTaxesAverageUsed](#method-getTaxesAverageUsed)
* [getTotalCart](#method-getTotalCart)
* [getTotalShippingCost](#method-getTotalShippingCost)
* [getTotalWeight](#method-getTotalWeight)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [getWsCartRows](#method-getWsCartRows)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [intifier](#method-intifier)
* [isAllProductsInStock](#method-isAllProductsInStock)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCarrierInRange](#method-isCarrierInRange)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isGuestCartByCartId](#method-isGuestCartByCartId)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiAddressDelivery](#method-isMultiAddressDelivery)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [isVirtualCart](#method-isVirtualCart)
* [lastNoneOrderedCart](#method-lastNoneOrderedCart)
* [makeTranslationFields](#method-makeTranslationFields)
* [nbProducts](#method-nbProducts)
* [orderExists](#method-orderExists)
* [removeCartRule](#method-removeCartRule)
* [replaceZeroByShopName](#method-replaceZeroByShopName)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setDeliveryOption](#method-setDeliveryOption)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [setNoMultishipping](#method-setNoMultishipping)
* [setProductAddressDelivery](#method-setProductAddressDelivery)
* [setWsCartRows](#method-setWsCartRows)
* [simulateCarrierSelectedOutput](#method-simulateCarrierSelectedOutput)
* [simulateCarriersOutput](#method-simulateCarriersOutput)
* [sortDeliveryOptionList](#method-sortDeliveryOptionList)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateAddressId](#method-updateAddressId)
* [updateMultishopTable](#method-updateMultishopTable)
* [updateQty](#method-updateQty)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)


Constants
----------


### <a name="constant-BOTH"></a>BOTH

```php
const BOTH = 3
```





* Source: [classes/Cart.php line 146](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L146).


### <a name="constant-BOTH_WITHOUT_SHIPPING"></a>BOTH_WITHOUT_SHIPPING

```php
const BOTH_WITHOUT_SHIPPING = 4
```





* Source: [classes/Cart.php line 147](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L147).


### <a name="constant-ONLY_DISCOUNTS"></a>ONLY_DISCOUNTS

```php
const ONLY_DISCOUNTS = 2
```





* Source: [classes/Cart.php line 145](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L145).


### <a name="constant-ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING"></a>ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING

```php
const ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING = 8
```





* Source: [classes/Cart.php line 151](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L151).


### <a name="constant-ONLY_PRODUCTS"></a>ONLY_PRODUCTS

```php
const ONLY_PRODUCTS = 1
```





* Source: [classes/Cart.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L144).


### <a name="constant-ONLY_PRODUCTS_WITHOUT_SHIPPING"></a>ONLY_PRODUCTS_WITHOUT_SHIPPING

```php
const ONLY_PRODUCTS_WITHOUT_SHIPPING = 7
```





* Source: [classes/Cart.php line 150](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L150).


### <a name="constant-ONLY_SHIPPING"></a>ONLY_SHIPPING

```php
const ONLY_SHIPPING = 5
```





* Source: [classes/Cart.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L148).


### <a name="constant-ONLY_WRAPPING"></a>ONLY_WRAPPING

```php
const ONLY_WRAPPING = 6
```





* Source: [classes/Cart.php line 149](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L149).


Properties
----------


### <a name="property-$_attributesLists"></a>$_attributesLists

```php
protected mixed $_attributesLists = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L94).


### <a name="property-$_carriers"></a>$_carriers

```php
protected mixed $_carriers = null
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L92).


### <a name="property-$_isVirtualCart"></a>$_isVirtualCart

```php
protected mixed $_isVirtualCart = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L87).


### <a name="property-$_nbProducts"></a>$_nbProducts

```php
protected mixed $_nbProducts = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L86).


### <a name="property-$_products"></a>$_products

```php
protected mixed $_products = null
```





* Visibility: **protected**
* Source: [classes/Cart.php line 89](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L89).


### <a name="property-$_taxCalculationMethod"></a>$_taxCalculationMethod

```php
protected mixed $_taxCalculationMethod = PS_TAX_EXC
```





* Visibility: **protected**
* Source: [classes/Cart.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L91).


### <a name="property-$_taxes_rate"></a>$_taxes_rate

```php
protected mixed $_taxes_rate = null
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L93).


### <a name="property-$_totalWeight"></a>$_totalWeight

```php
protected mixed $_totalWeight = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Cart.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L90).


### <a name="property-$allow_seperated_package"></a>$allow_seperated_package

```php
public boolean $allow_seperated_package = false
```





* Visibility: **public**
* Source: [classes/Cart.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L84).


### <a name="property-$checkedTos"></a>$checkedTos

```php
public mixed $checkedTos = false
```





* Visibility: **public**
* Source: [classes/Cart.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L77).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/Cart.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L66).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* Source: [classes/Cart.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L75).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'cart', 'primary' => 'id_cart', 'fields' => array('id_shop_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_address_delivery' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_address_invoice' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_carrier' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_currency' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_customer' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_guest' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_lang' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'recyclable' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift_message' => array('type' => self::TYPE_STRING, 'validate' => 'isMessage'), 'mobile_theme' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'delivery_option' => array('type' => self::TYPE_STRING), 'secure_key' => array('type' => self::TYPE_STRING, 'size' => 32), 'allow_seperated_package' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDateFormat'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDateFormat')))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Cart.php line 99](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L99).


### <a name="property-$delivery_option"></a>$delivery_option

```php
public mixed $delivery_option
```





* Visibility: **public**
* Source: [classes/Cart.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L81).


### <a name="property-$gift"></a>$gift

```php
public boolean $gift
```





* Visibility: **public**
* Source: [classes/Cart.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L57).


### <a name="property-$gift_message"></a>$gift_message

```php
public string $gift_message
```





* Visibility: **public**
* Source: [classes/Cart.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L60).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/Cart.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L29).


### <a name="property-$id_address_delivery"></a>$id_address_delivery

```php
public integer $id_address_delivery
```





* Visibility: **public**
* Source: [classes/Cart.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L36).


### <a name="property-$id_address_invoice"></a>$id_address_invoice

```php
public integer $id_address_invoice
```





* Visibility: **public**
* Source: [classes/Cart.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L39).


### <a name="property-$id_carrier"></a>$id_carrier

```php
public integer $id_carrier
```





* Visibility: **public**
* Source: [classes/Cart.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L72).


### <a name="property-$id_currency"></a>$id_currency

```php
public integer $id_currency
```





* Visibility: **public**
* Source: [classes/Cart.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L42).


### <a name="property-$id_customer"></a>$id_customer

```php
public integer $id_customer
```





* Visibility: **public**
* Source: [classes/Cart.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L45).


### <a name="property-$id_guest"></a>$id_guest

```php
public integer $id_guest
```





* Visibility: **public**
* Source: [classes/Cart.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L48).


### <a name="property-$id_lang"></a>$id_lang

```php
public integer $id_lang
```





* Visibility: **public**
* Source: [classes/Cart.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L51).


### <a name="property-$id_shop"></a>$id_shop

```php
public mixed $id_shop
```





* Visibility: **public**
* Source: [classes/Cart.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L33).


### <a name="property-$id_shop_group"></a>$id_shop_group

```php
public mixed $id_shop_group
```





* Visibility: **public**
* Source: [classes/Cart.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L31).


### <a name="property-$mobile_theme"></a>$mobile_theme

```php
public boolean $mobile_theme
```





* Visibility: **public**
* Source: [classes/Cart.php line 63](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L63).


### <a name="property-$pictures"></a>$pictures

```php
public mixed $pictures
```





* Visibility: **public**
* Source: [classes/Cart.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L78).


### <a name="property-$recyclable"></a>$recyclable

```php
public boolean $recyclable
```





* Visibility: **public**
* Source: [classes/Cart.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L54).


### <a name="property-$secure_key"></a>$secure_key

```php
public string $secure_key
```





* Visibility: **public**
* Source: [classes/Cart.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L69).


### <a name="property-$textFields"></a>$textFields

```php
public mixed $textFields
```





* Visibility: **public**
* Source: [classes/Cart.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L79).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('fields' => array('id_address_delivery' => array('xlink_resource' => 'addresses'), 'id_address_invoice' => array('xlink_resource' => 'addresses'), 'id_currency' => array('xlink_resource' => 'currencies'), 'id_customer' => array('xlink_resource' => 'customers'), 'id_guest' => array('xlink_resource' => 'guests'), 'id_lang' => array('xlink_resource' => 'languages')), 'associations' => array('cart_rows' => array('resource' => 'cart_row', 'virtual_entity' => true, 'fields' => array('id_product' => array('required' => true, 'xlink_resource' => 'products'), 'id_product_attribute' => array('required' => true, 'xlink_resource' => 'combinations'), 'id_address_delivery' => array('required' => true, 'xlink_resource' => 'addresses'), 'quantity' => array('required' => true)))))
```





* Visibility: **protected**
* Source: [classes/Cart.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L124).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 140](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L140).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L130).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L80).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L65).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 95](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L95).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L85).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L100).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L90).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 105](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L105).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 63](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L63).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L61).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L75).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 116](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L116).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L119).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L70).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 110](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L110).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 135](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L135).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed CartCore::__construct($id, $id_lang)
```





* Visibility: **public**
* Source: [classes/Cart.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L153)


#### Arguments
* $id **mixed**
* $id_lang **mixed**



### <a name="method-_addCustomization"></a>_addCustomization

```php
boolean CartCore::_addCustomization(integer $id_product, integer $id_product_attribute, integer $index, integer $type, string $field, integer $quantity)
```

Add customization item to database



* Visibility: **public**
* Source: [classes/Cart.php line 1056](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1056)


#### Arguments
* $id_product **integer**
* $id_product_attribute **integer**
* $index **integer**
* $type **integer**
* $field **string**
* $quantity **integer**



### <a name="method-_deleteCustomization"></a>_deleteCustomization

```php
boolean CartCore::_deleteCustomization(integer $id_customization, $id_product, $id_product_attribute, $id_address_delivery)
```

Delete a customization from the cart. If customization is a Picture,
then the image is also deleted



* Visibility: **protected**
* Source: [classes/Cart.php line 1242](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1242)


#### Arguments
* $id_customization **integer**
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**



### <a name="method-_updateCustomizationQuantity"></a>_updateCustomizationQuantity

```php
mixed CartCore::_updateCustomizationQuantity($quantity, $id_customization, $id_product, $id_product_attribute, $id_address_delivery, $operator)
```





* Visibility: **protected**
* Source: [classes/Cart.php line 992](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L992)


#### Arguments
* $quantity **mixed**
* $id_customization **mixed**
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**
* $operator **mixed**



### <a name="method-add"></a>add

```php
mixed CartCore::add($autodate, $null_values)
```





* Visibility: **public**
* Source: [classes/Cart.php line 177](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L177)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-addCartRule"></a>addCartRule

```php
mixed CartCore::addCartRule($id_cart_rule)
```





* Visibility: **public**
* Source: [classes/Cart.php line 778](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L778)


#### Arguments
* $id_cart_rule **mixed**



### <a name="method-addDiscount"></a>addDiscount

```php
mixed CartCore::addDiscount($id_cart_rule)
```





* Visibility: **public**
* Source: [classes/Cart.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L772)


#### Arguments
* $id_cart_rule **mixed**



### <a name="method-addExtraCarriers"></a>addExtraCarriers

```php
mixed CartCore::addExtraCarriers(array $array)
```

Execute hook displayCarrierList (extraCarrier) and merge theme to the $array



* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3686](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3686)


#### Arguments
* $array **array**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1212](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1212)


#### Arguments
* $fields **mixed**



### <a name="method-addPictureToProduct"></a>addPictureToProduct

```php
boolean CartCore::addPictureToProduct($id_product, $index, $type, $file)
```

Add customer's pictures



* Visibility: **public**
* Source: [classes/Cart.php line 3097](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3097)


#### Arguments
* $id_product **mixed**
* $index **mixed**
* $type **mixed**
* $file **mixed**



### <a name="method-addTextFieldToProduct"></a>addTextFieldToProduct

```php
boolean CartCore::addTextFieldToProduct($id_product, $index, $type, $text_value)
```

Add customer's text



* Visibility: **public**
* Source: [classes/Cart.php line 3087](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3087)


#### Arguments
* $id_product **mixed**
* $index **mixed**
* $type **mixed**
* $text_value **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1264](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1264)


#### Arguments
* $id_shops **integer|array**



### <a name="method-autosetProductAddress"></a>autosetProductAddress

```php
mixed CartCore::autosetProductAddress()
```

Set an address to all products on the cart without address delivery



* Visibility: **public**
* Source: [classes/Cart.php line 3553](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3553)




### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1199](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1199)




### <a name="method-cacheSomeAttributesLists"></a>cacheSomeAttributesLists

```php
mixed CartCore::cacheSomeAttributesLists($ipa_list, $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 687](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L687)


#### Arguments
* $ipa_list **mixed**
* $id_lang **mixed**



### <a name="method-carrierIsSelected"></a>carrierIsSelected

```php
mixed CartCore::carrierIsSelected($id_carrier, $id_address)
```





* Visibility: **public**
* Source: [classes/Cart.php line 2181](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2181)


#### Arguments
* $id_carrier **mixed**
* $id_address **mixed**



### <a name="method-checkDiscountValidity"></a>checkDiscountValidity

```php
mixed CartCore::checkDiscountValidity($obj, $discounts, $order_total, $products, $check_cart_discount)
```





* Visibility: **public**
* Source: [classes/Cart.php line 2859](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2859)


#### Arguments
* $obj **mixed**
* $discounts **mixed**
* $order_total **mixed**
* $products **mixed**
* $check_cart_discount **mixed**



### <a name="method-checkQuantities"></a>checkQuantities

```php
mixed CartCore::checkQuantities()
```





* Visibility: **public**
* Source: [classes/Cart.php line 2999](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2999)




### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1226](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1226)


#### Arguments
* $all **mixed**



### <a name="method-containsProduct"></a>containsProduct

```php
mixed CartCore::containsProduct($id_product, $id_product_attribute, $id_customization, $id_address_delivery)
```





* Visibility: **public**
* Source: [classes/Cart.php line 807](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L807)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_customization **mixed**
* $id_address_delivery **mixed**



### <a name="method-delete"></a>delete

```php
mixed CartCore::delete()
```





* Visibility: **public**
* Source: [classes/Cart.php line 240](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L240)




### <a name="method-deleteAssociations"></a>deleteAssociations

```php
mixed CartCore::deleteAssociations()
```





* Visibility: **public**
* Source: [classes/Cart.php line 3581](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3581)




### <a name="method-deleteCustomizationToProduct"></a>deleteCustomizationToProduct

```php
boolean CartCore::deleteCustomizationToProduct(integer $id_product, integer $index)
```

Remove a customer's customization



* Visibility: **public**
* Source: [classes/Cart.php line 3115](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3115)


#### Arguments
* $id_product **integer**
* $index **integer**



### <a name="method-deleteDiscount"></a>deleteDiscount

```php
mixed CartCore::deleteDiscount($id_cart_rule)
```





* Visibility: **public**
* Source: [classes/Cart.php line 1125](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1125)


#### Arguments
* $id_cart_rule **mixed**



### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1395](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1395)


#### Arguments
* $force_delete **mixed**



### <a name="method-deletePictureToProduct"></a>deletePictureToProduct

```php
mixed CartCore::deletePictureToProduct($id_product, $index)
```





* Visibility: **public**
* Source: [classes/Cart.php line 3102](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3102)


#### Arguments
* $id_product **mixed**
* $index **mixed**



### <a name="method-deleteProduct"></a>deleteProduct

```php
boolean CartCore::deleteProduct(integer $id_product, integer $id_product_attribute, integer $id_customization, $id_address_delivery)
```

Delete a product from the cart



* Visibility: **public**
* Source: [classes/Cart.php line 1159](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1159)


#### Arguments
* $id_product **integer** - Product ID
* $id_product_attribute **integer** - Attribute ID if needed
* $id_customization **integer** - Customization id
* $id_address_delivery **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 737](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L737)


#### Arguments
* $selection **array**



### <a name="method-desintifier"></a>desintifier

```php
mixed CartCore::desintifier($int, $delimiter)
```

Translate a int option_delivery identifier (3240002000) in a string ('24,3,')



* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 2286](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2286)


#### Arguments
* $int **mixed**
* $delimiter **mixed**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 982](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L982)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicate"></a>duplicate

```php
mixed CartCore::duplicate()
```





* Visibility: **public**
* Source: [classes/Cart.php line 3182](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3182)




### <a name="method-duplicateObject"></a>duplicateObject

```php
\new ObjectModelCore::duplicateObject()
```

Duplicate current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 521](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L521)




### <a name="method-duplicateProduct"></a>duplicateProduct

```php
mixed CartCore::duplicateProduct($id_product, $id_product_attribute, $id_address_delivery, $new_id_address_delivery, $quantity, $keep_quantity)
```





* Visibility: **public**
* Source: [classes/Cart.php line 3370](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3370)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**
* $new_id_address_delivery **mixed**
* $quantity **mixed**
* $keep_quantity **mixed**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1308](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1308)


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
* Source: [classes/ObjectModel.php line 1432](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1432)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 325](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L325)


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
* Source: [classes/ObjectModel.php line 372](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L372)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**
* $purify **mixed**



### <a name="method-getAddressCollection"></a>getAddressCollection

```php
mixed CartCore::getAddressCollection()
```

Get all delivery addresses object for the current cart



* Visibility: **public**
* Source: [classes/Cart.php line 2317](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2317)




### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1293](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1293)




### <a name="method-getCarrierCost"></a>getCarrierCost

```php
float CartCore::getCarrierCost(integer $id_carrier, \booleal $useTax, \Country $default_country, array $delivery_option)
```

Return shipping total of a specific carriers for the cart



* Visibility: **public**
* Source: [classes/Cart.php line 2484](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2484)


#### Arguments
* $id_carrier **integer**
* $useTax **booleal**
* $default_country **[Country](class.CountryCore.md)**
* $delivery_option **array** - Array of the delivery option for each address



### <a name="method-getCartByOrderId"></a>getCartByOrderId

```php
\Cart|boolean CartCore::getCartByOrderId(integer $id_order)
```

Build cart object from provided id_order



* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3061](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3061)


#### Arguments
* $id_order **integer**



### <a name="method-getCartIdByOrderId"></a>getCartIdByOrderId

```php
mixed CartCore::getCartIdByOrderId($id_order)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3069](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3069)


#### Arguments
* $id_order **mixed**



### <a name="method-getCartRules"></a>getCartRules

```php
mixed CartCore::getCartRules($filter)
```





* Visibility: **public**
* Source: [classes/Cart.php line 326](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L326)


#### Arguments
* $filter **mixed**



### <a name="method-getCustomerCarts"></a>getCustomerCarts

```php
mixed CartCore::getCustomerCarts($id_customer, $with_order)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3167](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3167)


#### Arguments
* $id_customer **mixed**
* $with_order **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1538](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1538)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getDeliveryAddressesWithoutCarriers"></a>getDeliveryAddressesWithoutCarriers

```php
array CartCore::getDeliveryAddressesWithoutCarriers(boolean $return_collection)
```

Get all the ids of the delivery addresses without carriers



* Visibility: **public**
* Source: [classes/Cart.php line 3717](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3717)


#### Arguments
* $return_collection **boolean** - Return a collection



### <a name="method-getDeliveryOption"></a>getDeliveryOption

```php
array CartCore::getDeliveryOption($default_country, $dontAutoSelectOptions, $use_cache)
```

Get the delivery option seleted, or if no delivery option was selected, the cheapest option for each address



* Visibility: **public**
* Source: [classes/Cart.php line 2384](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2384)


#### Arguments
* $default_country **mixed**
* $dontAutoSelectOptions **mixed**
* $use_cache **mixed**



### <a name="method-getDeliveryOptionList"></a>getDeliveryOptionList

```php
array CartCore::getDeliveryOptionList(\Country $default_country, boolean $flush)
```

Get all deliveries options available for the current cart



* Visibility: **public**
* Source: [classes/Cart.php line 1911](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1911)


#### Arguments
* $default_country **[Country](class.CountryCore.md)**
* $flush **boolean** - Force flushing cache



### <a name="method-getDiscounts"></a>getDiscounts

```php
mixed CartCore::getDiscounts($lite, $refresh)
```





* Visibility: **public**
* Source: [classes/Cart.php line 320](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L320)


#### Arguments
* $lite **mixed**
* $refresh **mixed**



### <a name="method-getDiscountsCustomer"></a>getDiscountsCustomer

```php
mixed CartCore::getDiscountsCustomer($id_cart_rule)
```





* Visibility: **public**
* Source: [classes/Cart.php line 371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L371)


#### Arguments
* $id_cart_rule **mixed**



### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1645](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1645)


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
* Source: [classes/ObjectModel.php line 253](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L253)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 290](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L290)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1191](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1191)


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
* Source: [classes/ObjectModel.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L276)




### <a name="method-getGiftWrappingPrice"></a>getGiftWrappingPrice

```php
float CartCore::getGiftWrappingPrice(boolean $with_taxes, $id_address)
```

Get the gift wrapping price



* Visibility: **public**
* Source: [classes/Cart.php line 1571](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1571)


#### Arguments
* $with_taxes **boolean** - With or without taxes
* $id_address **mixed**



### <a name="method-getIdCarrierFromDeliveryOption"></a>getIdCarrierFromDeliveryOption

```php
mixed CartCore::getIdCarrierFromDeliveryOption($delivery_option)
```





* Visibility: **protected**
* Source: [classes/Cart.php line 2369](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2369)


#### Arguments
* $delivery_option **mixed**



### <a name="method-getLastProduct"></a>getLastProduct

```php
mixed CartCore::getLastProduct()
```





* Visibility: **public**
* Source: [classes/Cart.php line 387](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L387)




### <a name="method-getNbOfPackages"></a>getNbOfPackages

```php
integer CartCore::getNbOfPackages()
```

Get the number of packages



* Visibility: **public**
* Source: [classes/Cart.php line 1597](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1597)




### <a name="method-getNbProducts"></a>getNbProducts

```php
mixed CartCore::getNbProducts($id)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 754](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L754)


#### Arguments
* $id **mixed**



### <a name="method-getOrderShippingCost"></a>getOrderShippingCost

```php
mixed CartCore::getOrderShippingCost($id_carrier, $use_tax, \Country $default_country, $product_list)
```





* Visibility: **public**
* Source: [classes/Cart.php line 2513](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2513)


#### Arguments
* $id_carrier **mixed**
* $use_tax **mixed**
* $default_country **[Country](class.CountryCore.md)**
* $product_list **mixed**



### <a name="method-getOrderTotal"></a>getOrderTotal

```php
float CartCore::getOrderTotal($with_taxes, integer $type, $products, $id_carrier, boolean $use_cache)
```

This function returns the total cart amount

Possible values for $type:
Cart::ONLY_PRODUCTS
Cart::ONLY_DISCOUNTS
Cart::BOTH
Cart::BOTH_WITHOUT_SHIPPING
Cart::ONLY_SHIPPING
Cart::ONLY_WRAPPING
Cart::ONLY_PRODUCTS_WITHOUT_SHIPPING
Cart::ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING

* Visibility: **public**
* Source: [classes/Cart.php line 1320](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1320)


#### Arguments
* $with_taxes **mixed**
* $type **integer** - Total type
* $products **mixed**
* $id_carrier **mixed**
* $use_cache **boolean** - Allow using cache of the method CartRule::getContextualValue



### <a name="method-getOrderTotalUsingTaxCalculationMethod"></a>getOrderTotalUsingTaxCalculationMethod

```php
mixed CartCore::getOrderTotalUsingTaxCalculationMethod($id_cart)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 1297](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1297)


#### Arguments
* $id_cart **mixed**



### <a name="method-getPackageIdWarehouse"></a>getPackageIdWarehouse

```php
mixed CartCore::getPackageIdWarehouse($package, $id_carrier)
```





* Visibility: **public**
* Source: [classes/Cart.php line 1861](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1861)


#### Arguments
* $package **mixed**
* $id_carrier **mixed**



### <a name="method-getPackageList"></a>getPackageList

```php
array CartCore::getPackageList($flush)
```

Get products grouped by package and by addresses to be sent individualy (one package = one shipping cost).



* Visibility: **public**
* Source: [classes/Cart.php line 1622](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1622)


#### Arguments
* $flush **mixed**



### <a name="method-getPackageShippingCost"></a>getPackageShippingCost

```php
float CartCore::getPackageShippingCost(integer $id_carrier, \booleal $use_tax, \Country $default_country, Array $product_list, $id_zone)
```

Return package shipping cost



* Visibility: **public**
* Source: [classes/Cart.php line 2530](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2530)


#### Arguments
* $id_carrier **integer** - Carrier ID (default : current carrier)
* $use_tax **booleal**
* $default_country **[Country](class.CountryCore.md)**
* $product_list **Array**
* $id_zone **mixed**



### <a name="method-getProductCustomization"></a>getProductCustomization

```php
array CartCore::getProductCustomization(integer $id_product, integer $type, boolean $not_in_cart)
```

Return custom pictures in this cart for a specified product



* Visibility: **public**
* Source: [classes/Cart.php line 3149](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3149)


#### Arguments
* $id_product **integer**
* $type **integer** - only return customization of this type
* $not_in_cart **boolean** - only return customizations that are not in cart already



### <a name="method-getProducts"></a>getProducts

```php
mixed CartCore::getProducts($refresh, $id_product, $id_country)
```

Return cart products



* Visibility: **public**
* Source: [classes/Cart.php line 413](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L413)


#### Arguments
* $refresh **mixed**
* $id_product **mixed**
* $id_country **mixed**



### <a name="method-getSummaryDetails"></a>getSummaryDetails

```php
array CartCore::getSummaryDetails($id_lang, $refresh)
```

Return useful informations for cart



* Visibility: **public**
* Source: [classes/Cart.php line 2873](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2873)


#### Arguments
* $id_lang **mixed**
* $refresh **mixed**



### <a name="method-getTaxesAverageUsed"></a>getTaxesAverageUsed

```php
mixed CartCore::getTaxesAverageUsed($id_cart)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 279](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L279)


#### Arguments
* $id_cart **mixed**



### <a name="method-getTotalCart"></a>getTotalCart

```php
mixed CartCore::getTotalCart($id_cart, $use_tax_display, $type)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 1286](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1286)


#### Arguments
* $id_cart **mixed**
* $use_tax_display **mixed**
* $type **mixed**



### <a name="method-getTotalShippingCost"></a>getTotalShippingCost

```php
float CartCore::getTotalShippingCost(array $delivery_option, \booleal $use_tax, \Country $default_country)
```

Return shipping total for the cart



* Visibility: **public**
* Source: [classes/Cart.php line 2454](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2454)


#### Arguments
* $delivery_option **array** - Array of the delivery option for each address
* $use_tax **booleal**
* $default_country **[Country](class.CountryCore.md)**



### <a name="method-getTotalWeight"></a>getTotalWeight

```php
float CartCore::getTotalWeight($products)
```

Return cart weight



* Visibility: **public**
* Source: [classes/Cart.php line 2815](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2815)


#### Arguments
* $products **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L772)


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
* Source: [classes/ObjectModel.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L148)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1132](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1132)


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
* Source: [classes/ObjectModel.php line 1054](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1054)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-getWsCartRows"></a>getWsCartRows

```php
mixed CartCore::getWsCartRows()
```





* Visibility: **public**
* Source: [classes/Cart.php line 3279](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3279)




### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1333](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1333)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1470](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1470)


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
* Source: [classes/ObjectModel.php line 1489](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1489)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-intifier"></a>intifier

```php
integer CartCore::intifier($string, $delimiter)
```

Translate a string option_delivery identifier ('24,3,') in a int (3240002000)

The  option_delivery identifier is a list of integers separated by a ','.
This method replace the delimiter by a sequence of '0'.
The size of this sequence is fixed by the first digit of the return

* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 2276](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2276)


#### Arguments
* $string **mixed**
* $delimiter **mixed**



### <a name="method-isAllProductsInStock"></a>isAllProductsInStock

```php
boolean CartCore::isAllProductsInStock(boolean $ignore_virtual, boolean $exclusive)
```





* Visibility: **public**
* Source: [classes/Cart.php line 3653](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3653)


#### Arguments
* $ignore_virtual **boolean** - Ignore virtual product
* $exclusive **boolean** - If true, the validation is exclusive : it must be present product in stock and out of stock



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1241](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1241)


#### Arguments
* $id_shop **integer**



### <a name="method-isCarrierInRange"></a>isCarrierInRange

```php
mixed CartCore::isCarrierInRange($id_carrier, $id_zone)
```

isCarrierInRange

Check if the specified carrier is in range

* Visibility: **public**
* Source: [classes/Cart.php line 3613](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3613)


#### Arguments
* $id_carrier **mixed**
* $id_zone **mixed**



### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean ObjectModelCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1450](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1450)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isGuestCartByCartId"></a>isGuestCartByCartId

```php
boolean CartCore::isGuestCartByCartId(integer $id_cart)
```

isGuestCartByCartId



* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3594](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3594)


#### Arguments
* $id_cart **integer**



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1350](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1350)




### <a name="method-isMultiAddressDelivery"></a>isMultiAddressDelivery

```php
boolean CartCore::isMultiAddressDelivery()
```

Does the cart use multiple address



* Visibility: **public**
* Source: [classes/Cart.php line 2298](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2298)




### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1345](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1345)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1340](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1340)




### <a name="method-isVirtualCart"></a>isVirtualCart

```php
boolean CartCore::isVirtualCart($strict)
```

Check if cart contains only virtual products



* Visibility: **public**
* Source: [classes/Cart.php line 3032](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3032)


#### Arguments
* $strict **mixed**



### <a name="method-lastNoneOrderedCart"></a>lastNoneOrderedCart

```php
mixed CartCore::lastNoneOrderedCart($id_customer)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3012](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3012)


#### Arguments
* $id_customer **mixed**



### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 788](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L788)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-nbProducts"></a>nbProducts

```php
mixed CartCore::nbProducts()
```

Return cart products quantity



* Visibility: **public**
* Source: [classes/Cart.php line 746](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L746)




### <a name="method-orderExists"></a>orderExists

```php
boolean CartCore::orderExists()
```

Check if order has already been placed



* Visibility: **public**
* Source: [classes/Cart.php line 1111](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1111)




### <a name="method-removeCartRule"></a>removeCartRule

```php
mixed CartCore::removeCartRule($id_cart_rule)
```





* Visibility: **public**
* Source: [classes/Cart.php line 1131](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L1131)


#### Arguments
* $id_cart_rule **mixed**



### <a name="method-replaceZeroByShopName"></a>replaceZeroByShopName

```php
mixed CartCore::replaceZeroByShopName($echo, $tr)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 3177](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3177)


#### Arguments
* $echo **mixed**
* $tr **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 418](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L418)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1576](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1576)




### <a name="method-setDeliveryOption"></a>setDeliveryOption

```php
mixed CartCore::setDeliveryOption($delivery_option)
```

Set the delivery option and id_carrier, if there is only one carrier



* Visibility: **public**
* Source: [classes/Cart.php line 2343](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2343)


#### Arguments
* $delivery_option **mixed**



### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1671](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1671)


#### Arguments
* $fields **array**



### <a name="method-setNoMultishipping"></a>setNoMultishipping

```php
mixed CartCore::setNoMultishipping()
```

Update products cart address delivery with the address delivery of the cart



* Visibility: **public**
* Source: [classes/Cart.php line 3481](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3481)




### <a name="method-setProductAddressDelivery"></a>setProductAddressDelivery

```php
mixed CartCore::setProductAddressDelivery($id_product, $id_product_attribute, $old_id_address_delivery, $new_id_address_delivery)
```





* Visibility: **public**
* Source: [classes/Cart.php line 3306](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3306)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $old_id_address_delivery **mixed**
* $new_id_address_delivery **mixed**



### <a name="method-setWsCartRows"></a>setWsCartRows

```php
mixed CartCore::setWsCartRows($values)
```





* Visibility: **public**
* Source: [classes/Cart.php line 3288](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L3288)


#### Arguments
* $values **mixed**



### <a name="method-simulateCarrierSelectedOutput"></a>simulateCarrierSelectedOutput

```php
mixed CartCore::simulateCarrierSelectedOutput($use_cache)
```





* Visibility: **public**
* Source: [classes/Cart.php line 2257](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2257)


#### Arguments
* $use_cache **mixed**



### <a name="method-simulateCarriersOutput"></a>simulateCarriersOutput

```php
mixed CartCore::simulateCarriersOutput(\Country $default_country, boolean $flush)
```

Get all deliveries options available for the current cart formated like Carriers::getCarriersForOrder
This method was wrote for retrocompatibility with 1.4 theme
New theme need to use Cart::getDeliveryOptionList() to generate carriers option in the checkout process



* Visibility: **public**
* Source: [classes/Cart.php line 2209](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2209)


#### Arguments
* $default_country **[Country](class.CountryCore.md)**
* $flush **boolean** - Force flushing cache



### <a name="method-sortDeliveryOptionList"></a>sortDeliveryOptionList

```php
integer CartCore::sortDeliveryOptionList($option1, $option2)
```

Sort list of option delivery by parameters define in the BO



* Visibility: **public**
* This method is **static**.
* Source: [classes/Cart.php line 2160](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L2160)


#### Arguments
* $option1 **mixed**
* $option2 **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 753](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L753)




### <a name="method-update"></a>update

```php
mixed CartCore::update($null_values)
```





* Visibility: **public**
* Source: [classes/Cart.php line 190](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L190)


#### Arguments
* $null_values **mixed**



### <a name="method-updateAddressId"></a>updateAddressId

```php
mixed CartCore::updateAddressId(integer $id_address, integer $id_address_new)
```

Update the address id of the cart



* Visibility: **public**
* Source: [classes/Cart.php line 211](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L211)


#### Arguments
* $id_address **integer** - Current address id to change
* $id_address_new **integer** - New address id



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1365](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1365)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-updateQty"></a>updateQty

```php
mixed CartCore::updateQty(integer $quantity, integer $id_product, integer $id_product_attribute, $id_customization, string $operator, $id_address_delivery, \Shop $shop, $auto_add_cart_rule)
```

Update product quantity



* Visibility: **public**
* Source: [classes/Cart.php line 839](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/Cart.php#L839)


#### Arguments
* $quantity **integer** - Quantity to add (or substract)
* $id_product **integer** - Product ID
* $id_product_attribute **integer** - Attribute ID if needed
* $id_customization **mixed**
* $operator **string** - Indicate if quantity must be increased or decreased
* $id_address_delivery **mixed**
* $shop **[Shop](class.ShopCore.md)**
* $auto_add_cart_rule **mixed**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1000](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1000)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1006](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1006)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang, $skip, $human_errors)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 899](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L899)


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
* Source: [classes/ObjectModel.php line 826](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L826)


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
* Source: [classes/ObjectModel.php line 855](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L855)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1168](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.7/classes/ObjectModel.php#L1168)


#### Arguments
* $htmlentities **mixed**

