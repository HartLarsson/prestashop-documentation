CartCore
===============






* Class name: CartCore
* Namespace: 
* Parent class: [ObjectModel](ObjectModelCore)
* This class is defined in classes\Cart.php line 27



Constants
----------


### ONLY_PRODUCTS

    const ONLY_PRODUCTS = 1



* This constant is defined in classes\Cart.php line 147


### ONLY_DISCOUNTS

    const ONLY_DISCOUNTS = 2



* This constant is defined in classes\Cart.php line 148


### BOTH

    const BOTH = 3



* This constant is defined in classes\Cart.php line 149


### BOTH_WITHOUT_SHIPPING

    const BOTH_WITHOUT_SHIPPING = 4



* This constant is defined in classes\Cart.php line 150


### ONLY_SHIPPING

    const ONLY_SHIPPING = 5



* This constant is defined in classes\Cart.php line 151


### ONLY_WRAPPING

    const ONLY_WRAPPING = 6



* This constant is defined in classes\Cart.php line 152


### ONLY_PRODUCTS_WITHOUT_SHIPPING

    const ONLY_PRODUCTS_WITHOUT_SHIPPING = 7



* This constant is defined in classes\Cart.php line 153


### ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING

    const ONLY_PHYSICAL_PRODUCTS_WITHOUT_SHIPPING = 8



* This constant is defined in classes\Cart.php line 154


Properties
----------


### $id

    public mixed $id





* Visibility: **public**
* This property is defined in classes\Cart.php line 29


### $id_shop_group

    public mixed $id_shop_group





* Visibility: **public**
* This property is defined in classes\Cart.php line 31


### $id_shop

    public mixed $id_shop





* Visibility: **public**
* This property is defined in classes\Cart.php line 33


### $id_address_delivery

    public integer $id_address_delivery





* Visibility: **public**
* This property is defined in classes\Cart.php line 36


### $id_address_invoice

    public integer $id_address_invoice





* Visibility: **public**
* This property is defined in classes\Cart.php line 39


### $id_currency

    public integer $id_currency





* Visibility: **public**
* This property is defined in classes\Cart.php line 42


### $id_customer

    public integer $id_customer





* Visibility: **public**
* This property is defined in classes\Cart.php line 45


### $id_guest

    public integer $id_guest





* Visibility: **public**
* This property is defined in classes\Cart.php line 48


### $id_lang

    public integer $id_lang





* Visibility: **public**
* This property is defined in classes\Cart.php line 51


### $recyclable

    public boolean $recyclable





* Visibility: **public**
* This property is defined in classes\Cart.php line 54


### $gift

    public boolean $gift





* Visibility: **public**
* This property is defined in classes\Cart.php line 57


### $gift_message

    public string $gift_message





* Visibility: **public**
* This property is defined in classes\Cart.php line 60


### $mobile_theme

    public boolean $mobile_theme





* Visibility: **public**
* This property is defined in classes\Cart.php line 63


### $date_add

    public string $date_add





* Visibility: **public**
* This property is defined in classes\Cart.php line 66


### $secure_key

    public string $secure_key





* Visibility: **public**
* This property is defined in classes\Cart.php line 69


### $id_carrier

    public integer $id_carrier





* Visibility: **public**
* This property is defined in classes\Cart.php line 72


### $date_upd

    public string $date_upd





* Visibility: **public**
* This property is defined in classes\Cart.php line 75


### $checkedTos

    public mixed $checkedTos = false





* Visibility: **public**
* This property is defined in classes\Cart.php line 77


### $pictures

    public mixed $pictures





* Visibility: **public**
* This property is defined in classes\Cart.php line 78


### $textFields

    public mixed $textFields





* Visibility: **public**
* This property is defined in classes\Cart.php line 79


### $delivery_option

    public mixed $delivery_option





* Visibility: **public**
* This property is defined in classes\Cart.php line 81


### $allow_seperated_package

    public boolean $allow_seperated_package = false





* Visibility: **public**
* This property is defined in classes\Cart.php line 84


### $_nbProducts

    protected mixed $_nbProducts = array()





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 86


### $_isVirtualCart

    protected mixed $_isVirtualCart = array()





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 87


### $_products

    protected mixed $_products = null





* Visibility: **protected**
* This property is defined in classes\Cart.php line 89


### $_totalWeight

    protected mixed $_totalWeight = array()





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 90


### $_taxCalculationMethod

    protected mixed $_taxCalculationMethod = PS_TAX_EXC





* Visibility: **protected**
* This property is defined in classes\Cart.php line 91


### $_carriers

    protected mixed $_carriers = null





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 92


### $_taxes_rate

    protected mixed $_taxes_rate = null





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 93


### $_attributesLists

    protected mixed $_attributesLists = array()





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 94


### $_customer

    protected \Customer $_customer = null





* Visibility: **protected**
* This property is **static**.
* This property is defined in classes\Cart.php line 97


### $definition

    public mixed $definition = array('table' => 'cart', 'primary' => 'id_cart', 'fields' => array('id_shop_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_address_delivery' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_address_invoice' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_carrier' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_currency' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_customer' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_guest' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_lang' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'recyclable' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift_message' => array('type' => self::TYPE_STRING, 'validate' => 'isMessage'), 'mobile_theme' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'delivery_option' => array('type' => self::TYPE_STRING), 'secure_key' => array('type' => self::TYPE_STRING, 'size' => 32), 'allow_seperated_package' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))





* Visibility: **public**
* This property is **static**.
* This property is defined in classes\Cart.php line 102


### $webserviceParameters

    protected mixed $webserviceParameters = array('fields' => array('id_address_delivery' => array('xlink_resource' => 'addresses'), 'id_address_invoice' => array('xlink_resource' => 'addresses'), 'id_currency' => array('xlink_resource' => 'currencies'), 'id_customer' => array('xlink_resource' => 'customers'), 'id_guest' => array('xlink_resource' => 'guests'), 'id_lang' => array('xlink_resource' => 'languages')), 'associations' => array('cart_rows' => array('resource' => 'cart_row', 'virtual_entity' => true, 'fields' => array('id_product' => array('required' => true, 'xlink_resource' => 'products'), 'id_product_attribute' => array('required' => true, 'xlink_resource' => 'combinations'), 'id_address_delivery' => array('required' => true, 'xlink_resource' => 'addresses'), 'quantity' => array('required' => true)))))





* Visibility: **protected**
* This property is defined in classes\Cart.php line 127


Methods
-------


### __construct

    mixed CartCore::__construct($id, $id_lang)





* Visibility: **public**
* This method is defined in classes\Cart.php line 156


#### Arguments
* $id **mixed**
* $id_lang **mixed**



### setTaxCalculationMethod

    mixed CartCore::setTaxCalculationMethod()





* Visibility: **public**
* This method is defined in classes\Cart.php line 182




### add

    mixed CartCore::add($autodate, $null_values)





* Visibility: **public**
* This method is defined in classes\Cart.php line 187


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### update

    mixed CartCore::update($null_values)





* Visibility: **public**
* This method is defined in classes\Cart.php line 202


#### Arguments
* $null_values **mixed**



### updateAddressId

    mixed CartCore::updateAddressId(integer $id_address, integer $id_address_new)

Update the address id of the cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 225


#### Arguments
* $id_address **integer** - &lt;p&gt;Current address id to change&lt;/p&gt;
* $id_address_new **integer** - &lt;p&gt;New address id&lt;/p&gt;



### delete

    mixed CartCore::delete()





* Visibility: **public**
* This method is defined in classes\Cart.php line 253




### getTaxesAverageUsed

    mixed CartCore::getTaxesAverageUsed($id_cart)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 293


#### Arguments
* $id_cart **mixed**



### getAverageProductsTaxRate

    mixed CartCore::getAverageProductsTaxRate($cart_amount_te, $cart_amount_ti)

The arguments are optional and only serve as return values in case caller needs the details.



* Visibility: **public**
* This method is defined in classes\Cart.php line 341


#### Arguments
* $cart_amount_te **mixed**
* $cart_amount_ti **mixed**



### getDiscounts

    mixed CartCore::getDiscounts($lite, $refresh)





* Visibility: **public**
* This method is defined in classes\Cart.php line 358


#### Arguments
* $lite **mixed**
* $refresh **mixed**



### getCartRules

    mixed CartCore::getCartRules($filter)





* Visibility: **public**
* This method is defined in classes\Cart.php line 364


#### Arguments
* $filter **mixed**



### getOrderedCartRulesIds

    array CartCore::getOrderedCartRulesIds($filter)

Return the cart rules Ids on the cart.



* Visibility: **public**
* This method is defined in classes\Cart.php line 414


#### Arguments
* $filter **mixed**



### getDiscountsCustomer

    mixed CartCore::getDiscountsCustomer($id_cart_rule)





* Visibility: **public**
* This method is defined in classes\Cart.php line 440


#### Arguments
* $id_cart_rule **mixed**



### getLastProduct

    mixed CartCore::getLastProduct()





* Visibility: **public**
* This method is defined in classes\Cart.php line 457




### getProducts

    mixed CartCore::getProducts($refresh, $id_product, $id_country)

Return cart products



* Visibility: **public**
* This method is defined in classes\Cart.php line 486


#### Arguments
* $refresh **mixed**
* $id_product **mixed**
* $id_country **mixed**



### cacheSomeAttributesLists

    mixed CartCore::cacheSomeAttributesLists($ipa_list, $id_lang)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 747


#### Arguments
* $ipa_list **mixed**
* $id_lang **mixed**



### nbProducts

    mixed CartCore::nbProducts()

Return cart products quantity



* Visibility: **public**
* This method is defined in classes\Cart.php line 806




### getNbProducts

    mixed CartCore::getNbProducts($id)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 815


#### Arguments
* $id **mixed**



### addDiscount

    mixed CartCore::addDiscount($id_cart_rule)





* Visibility: **public**
* This method is defined in classes\Cart.php line 834


#### Arguments
* $id_cart_rule **mixed**



### addCartRule

    mixed CartCore::addCartRule($id_cart_rule)





* Visibility: **public**
* This method is defined in classes\Cart.php line 840


#### Arguments
* $id_cart_rule **mixed**



### containsProduct

    mixed CartCore::containsProduct($id_product, $id_product_attribute, $id_customization, $id_address_delivery)





* Visibility: **public**
* This method is defined in classes\Cart.php line 878


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_customization **mixed**
* $id_address_delivery **mixed**



### updateQty

    mixed CartCore::updateQty(integer $quantity, integer $id_product, integer $id_product_attribute, $id_customization, string $operator, $id_address_delivery, \Shop $shop, $auto_add_cart_rule)

Update product quantity



* Visibility: **public**
* This method is defined in classes\Cart.php line 913


#### Arguments
* $quantity **integer** - &lt;p&gt;Quantity to add (or substract)&lt;/p&gt;
* $id_product **integer** - &lt;p&gt;Product ID&lt;/p&gt;
* $id_product_attribute **integer** - &lt;p&gt;Attribute ID if needed&lt;/p&gt;
* $id_customization **mixed**
* $operator **string** - &lt;p&gt;Indicate if quantity must be increased or decreased&lt;/p&gt;
* $id_address_delivery **mixed**
* $shop **[Shop](ShopCore)**
* $auto_add_cart_rule **mixed**



### _updateCustomizationQuantity

    mixed CartCore::_updateCustomizationQuantity($quantity, $id_customization, $id_product, $id_product_attribute, $id_address_delivery, $operator)





* Visibility: **protected**
* This method is defined in classes\Cart.php line 1089


#### Arguments
* $quantity **mixed**
* $id_customization **mixed**
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**
* $operator **mixed**



### _addCustomization

    boolean CartCore::_addCustomization(integer $id_product, integer $id_product_attribute, integer $index, integer $type, string $field, integer $quantity)

Add customization item to database



* Visibility: **public**
* This method is defined in classes\Cart.php line 1152


#### Arguments
* $id_product **integer**
* $id_product_attribute **integer**
* $index **integer**
* $type **integer**
* $field **string**
* $quantity **integer**



### orderExists

    boolean CartCore::orderExists()

Check if order has already been placed



* Visibility: **public**
* This method is defined in classes\Cart.php line 1202




### deleteDiscount

    mixed CartCore::deleteDiscount($id_cart_rule)





* Visibility: **public**
* This method is defined in classes\Cart.php line 1216


#### Arguments
* $id_cart_rule **mixed**



### removeCartRule

    mixed CartCore::removeCartRule($id_cart_rule)





* Visibility: **public**
* This method is defined in classes\Cart.php line 1222


#### Arguments
* $id_cart_rule **mixed**



### deleteProduct

    boolean CartCore::deleteProduct(integer $id_product, integer $id_product_attribute, integer $id_customization, $id_address_delivery)

Delete a product from the cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 1252


#### Arguments
* $id_product **integer** - &lt;p&gt;Product ID&lt;/p&gt;
* $id_product_attribute **integer** - &lt;p&gt;Attribute ID if needed&lt;/p&gt;
* $id_customization **integer** - &lt;p&gt;Customization id&lt;/p&gt;
* $id_address_delivery **mixed**



### _deleteCustomization

    boolean CartCore::_deleteCustomization(integer $id_customization, $id_product, $id_product_attribute, $id_address_delivery)

Delete a customization from the cart. If customization is a Picture,
then the image is also deleted



* Visibility: **protected**
* This method is defined in classes\Cart.php line 1338


#### Arguments
* $id_customization **integer**
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**



### getTotalCart

    mixed CartCore::getTotalCart($id_cart, $use_tax_display, $type)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 1384


#### Arguments
* $id_cart **mixed**
* $use_tax_display **mixed**
* $type **mixed**



### getOrderTotalUsingTaxCalculationMethod

    mixed CartCore::getOrderTotalUsingTaxCalculationMethod($id_cart)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 1396


#### Arguments
* $id_cart **mixed**



### getOrderTotal

    float CartCore::getOrderTotal($with_taxes, integer $type, $products, $id_carrier, boolean $use_cache)

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
* This method is defined in classes\Cart.php line 1419


#### Arguments
* $with_taxes **mixed**
* $type **integer** - &lt;p&gt;Total type&lt;/p&gt;
* $products **mixed**
* $id_carrier **mixed**
* $use_cache **boolean** - &lt;p&gt;Allow using cache of the method CartRule::getContextualValue&lt;/p&gt;



### getGiftWrappingPrice

    float CartCore::getGiftWrappingPrice(boolean $with_taxes, $id_address)

Get the gift wrapping price



* Visibility: **public**
* This method is defined in classes\Cart.php line 1695


#### Arguments
* $with_taxes **boolean** - &lt;p&gt;With or without taxes&lt;/p&gt;
* $id_address **mixed**



### getNbOfPackages

    integer CartCore::getNbOfPackages()

Get the number of packages



* Visibility: **public**
* This method is defined in classes\Cart.php line 1743




### getPackageList

    array CartCore::getPackageList($flush)

Get products grouped by package and by addresses to be sent individualy (one package = one shipping cost).



* Visibility: **public**
* This method is defined in classes\Cart.php line 1771


#### Arguments
* $flush **mixed**



### getPackageIdWarehouse

    mixed CartCore::getPackageIdWarehouse($package, $id_carrier)





* Visibility: **public**
* This method is defined in classes\Cart.php line 2010


#### Arguments
* $package **mixed**
* $id_carrier **mixed**



### getDeliveryOptionList

    array CartCore::getDeliveryOptionList(\Country $default_country, boolean $flush)

Get all deliveries options available for the current cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 2063


#### Arguments
* $default_country **[Country](CountryCore)**
* $flush **boolean** - &lt;p&gt;Force flushing cache&lt;/p&gt;



### sortDeliveryOptionList

    integer CartCore::sortDeliveryOptionList($option1, $option2)

Sort list of option delivery by parameters define in the BO



* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 2338


#### Arguments
* $option1 **mixed**
* $option2 **mixed**



### carrierIsSelected

    mixed CartCore::carrierIsSelected($id_carrier, $id_address)





* Visibility: **public**
* This method is defined in classes\Cart.php line 2365


#### Arguments
* $id_carrier **mixed**
* $id_address **mixed**



### simulateCarriersOutput

    mixed CartCore::simulateCarriersOutput(\Country $default_country, boolean $flush)

Get all deliveries options available for the current cart formated like Carriers::getCarriersForOrder
This method was wrote for retrocompatibility with 1.4 theme
New theme need to use Cart::getDeliveryOptionList() to generate carriers option in the checkout process



* Visibility: **public**
* This method is defined in classes\Cart.php line 2396


#### Arguments
* $default_country **[Country](CountryCore)**
* $flush **boolean** - &lt;p&gt;Force flushing cache&lt;/p&gt;



### simulateCarrierSelectedOutput

    mixed CartCore::simulateCarrierSelectedOutput($use_cache)





* Visibility: **public**
* This method is defined in classes\Cart.php line 2444


#### Arguments
* $use_cache **mixed**



### intifier

    integer CartCore::intifier($string, $delimiter)

Translate a string option_delivery identifier ('24,3,') in a int (3240002000)

The  option_delivery identifier is a list of integers separated by a ','.
This method replace the delimiter by a sequence of '0'.
The size of this sequence is fixed by the first digit of the return

* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 2464


#### Arguments
* $string **mixed**
* $delimiter **mixed**



### desintifier

    mixed CartCore::desintifier($int, $delimiter)

Translate a int option_delivery identifier (3240002000) in a string ('24,3,')



* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 2474


#### Arguments
* $int **mixed**
* $delimiter **mixed**



### isMultiAddressDelivery

    boolean CartCore::isMultiAddressDelivery()

Does the cart use multiple address



* Visibility: **public**
* This method is defined in classes\Cart.php line 2486




### getAddressCollection

    mixed CartCore::getAddressCollection()

Get all delivery addresses object for the current cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 2504




### setDeliveryOption

    mixed CartCore::setDeliveryOption($delivery_option)

Set the delivery option and id_carrier, if there is only one carrier



* Visibility: **public**
* This method is defined in classes\Cart.php line 2532


#### Arguments
* $delivery_option **mixed**



### getIdCarrierFromDeliveryOption

    mixed CartCore::getIdCarrierFromDeliveryOption($delivery_option)





* Visibility: **protected**
* This method is defined in classes\Cart.php line 2560


#### Arguments
* $delivery_option **mixed**



### getDeliveryOption

    array|boolean|mixed CartCore::getDeliveryOption(\Country|null $default_country, boolean $dontAutoSelectOptions, boolean $use_cache)

Get the delivery option selected, or if no delivery option was selected,
the cheapest option for each address



* Visibility: **public**
* This method is defined in classes\Cart.php line 2584


#### Arguments
* $default_country **[Country](CountryCore)|null**
* $dontAutoSelectOptions **boolean**
* $use_cache **boolean**



### getTotalShippingCost

    float CartCore::getTotalShippingCost(array|null $delivery_option, boolean $use_tax, \Country|null $default_country)

Return shipping total for the cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 2650


#### Arguments
* $delivery_option **array|null** - &lt;p&gt;Array of the delivery option for each address&lt;/p&gt;
* $use_tax **boolean**
* $default_country **[Country](CountryCore)|null**



### getCarrierCost

    float CartCore::getCarrierCost(integer $id_carrier, boolean $useTax, \Country|null $default_country, array $delivery_option)

Return shipping total of a specific carriers for the cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 2685


#### Arguments
* $id_carrier **integer**
* $useTax **boolean**
* $default_country **[Country](CountryCore)|null**
* $delivery_option **array** - &lt;p&gt;Array of the delivery option for each address&lt;/p&gt;



### getOrderShippingCost

    mixed CartCore::getOrderShippingCost($id_carrier, $use_tax, \Country $default_country, $product_list)





* Visibility: **public**
* This method is defined in classes\Cart.php line 2714


#### Arguments
* $id_carrier **mixed**
* $use_tax **mixed**
* $default_country **[Country](CountryCore)**
* $product_list **mixed**



### getPackageShippingCost

    float CartCore::getPackageShippingCost(integer $id_carrier, boolean $use_tax, \Country|null $default_country, array|null $product_list, integer|null $id_zone)

Return package shipping cost



* Visibility: **public**
* This method is defined in classes\Cart.php line 2732


#### Arguments
* $id_carrier **integer** - &lt;p&gt;Carrier ID (default : current carrier)&lt;/p&gt;
* $use_tax **boolean**
* $default_country **[Country](CountryCore)|null**
* $product_list **array|null** - &lt;p&gt;List of product concerned by the shipping.
                                     If null, all the product of the cart are used to calculate the shipping cost&lt;/p&gt;
* $id_zone **integer|null**



### getTotalWeight

    float CartCore::getTotalWeight($products)

Return cart weight



* Visibility: **public**
* This method is defined in classes\Cart.php line 3044


#### Arguments
* $products **mixed**



### checkDiscountValidity

    boolean|string CartCore::checkDiscountValidity(\CartRule $obj, $discounts, $order_total, $products, $check_cart_discount)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3089


#### Arguments
* $obj **[CartRule](CartRuleCore)**
* $discounts **mixed**
* $order_total **mixed**
* $products **mixed**
* $check_cart_discount **mixed**



### getSummaryDetails

    array CartCore::getSummaryDetails($id_lang, $refresh)

Return useful informations for cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 3103


#### Arguments
* $id_lang **mixed**
* $refresh **mixed**



### checkQuantities

    mixed CartCore::checkQuantities($return_product)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3259


#### Arguments
* $return_product **mixed**



### checkProductsAccess

    mixed CartCore::checkProductsAccess()





* Visibility: **public**
* This method is defined in classes\Cart.php line 3279




### lastNoneOrderedCart

    mixed CartCore::lastNoneOrderedCart($id_customer)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3295


#### Arguments
* $id_customer **mixed**



### isVirtualCart

    boolean CartCore::isVirtualCart($strict)

Check if cart contains only virtual products



* Visibility: **public**
* This method is defined in classes\Cart.php line 3317


#### Arguments
* $strict **mixed**



### getCartByOrderId

    \Cart|boolean CartCore::getCartByOrderId(integer $id_order)

Build cart object from provided id_order



* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3347


#### Arguments
* $id_order **integer**



### getCartIdByOrderId

    mixed CartCore::getCartIdByOrderId($id_order)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3356


#### Arguments
* $id_order **mixed**



### addTextFieldToProduct

    boolean CartCore::addTextFieldToProduct($id_product, $index, $type, $text_value)

Add customer's text



* Visibility: **public**
* This method is defined in classes\Cart.php line 3375


#### Arguments
* $id_product **mixed**
* $index **mixed**
* $type **mixed**
* $text_value **mixed**



### addPictureToProduct

    boolean CartCore::addPictureToProduct($id_product, $index, $type, $file)

Add customer's pictures



* Visibility: **public**
* This method is defined in classes\Cart.php line 3385


#### Arguments
* $id_product **mixed**
* $index **mixed**
* $type **mixed**
* $file **mixed**



### deletePictureToProduct

    boolean CartCore::deletePictureToProduct(integer $id_product, $index)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3396


#### Arguments
* $id_product **integer**
* $index **mixed**



### deleteCustomizationToProduct

    boolean CartCore::deleteCustomizationToProduct(integer $id_product, integer $index)

Remove a customer's customization



* Visibility: **public**
* This method is defined in classes\Cart.php line 3409


#### Arguments
* $id_product **integer**
* $index **integer**



### getProductCustomization

    array CartCore::getProductCustomization(integer $id_product, integer $type, boolean $not_in_cart)

Return custom pictures in this cart for a specified product



* Visibility: **public**
* This method is defined in classes\Cart.php line 3444


#### Arguments
* $id_product **integer**
* $type **integer** - &lt;p&gt;only return customization of this type&lt;/p&gt;
* $not_in_cart **boolean** - &lt;p&gt;only return customizations that are not in cart already&lt;/p&gt;



### getCustomerCarts

    mixed CartCore::getCustomerCarts($id_customer, $with_order)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3463


#### Arguments
* $id_customer **mixed**
* $with_order **mixed**



### replaceZeroByShopName

    mixed CartCore::replaceZeroByShopName($echo, $tr)





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3473


#### Arguments
* $echo **mixed**
* $tr **mixed**



### duplicate

    mixed CartCore::duplicate()





* Visibility: **public**
* This method is defined in classes\Cart.php line 3478




### getWsCartRows

    mixed CartCore::getWsCartRows()





* Visibility: **public**
* This method is defined in classes\Cart.php line 3589




### setWsCartRows

    mixed CartCore::setWsCartRows($values)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3598


#### Arguments
* $values **mixed**



### setProductAddressDelivery

    mixed CartCore::setProductAddressDelivery($id_product, $id_product_attribute, $old_id_address_delivery, $new_id_address_delivery)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3616


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $old_id_address_delivery **mixed**
* $new_id_address_delivery **mixed**



### duplicateProduct

    mixed CartCore::duplicateProduct($id_product, $id_product_attribute, $id_address_delivery, $new_id_address_delivery, $quantity, $keep_quantity)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3683


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_address_delivery **mixed**
* $new_id_address_delivery **mixed**
* $quantity **mixed**
* $keep_quantity **mixed**



### setNoMultishipping

    mixed CartCore::setNoMultishipping()

Update products cart address delivery with the address delivery of the cart



* Visibility: **public**
* This method is defined in classes\Cart.php line 3798




### autosetProductAddress

    mixed CartCore::autosetProductAddress()

Set an address to all products on the cart without address delivery



* Visibility: **public**
* This method is defined in classes\Cart.php line 3871




### deleteAssociations

    mixed CartCore::deleteAssociations()





* Visibility: **public**
* This method is defined in classes\Cart.php line 3901




### isGuestCartByCartId

    boolean CartCore::isGuestCartByCartId(integer $id_cart)

isGuestCartByCartId



* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 3914


#### Arguments
* $id_cart **integer**



### isCarrierInRange

    mixed CartCore::isCarrierInRange($id_carrier, $id_zone)

isCarrierInRange

Check if the specified carrier is in range

* Visibility: **public**
* This method is defined in classes\Cart.php line 3934


#### Arguments
* $id_carrier **mixed**
* $id_zone **mixed**



### isAllProductsInStock

    boolean CartCore::isAllProductsInStock(boolean $ignore_virtual, boolean $exclusive)





* Visibility: **public**
* This method is defined in classes\Cart.php line 3978


#### Arguments
* $ignore_virtual **boolean** - &lt;p&gt;Ignore virtual product&lt;/p&gt;
* $exclusive **boolean** - &lt;p&gt;If true, the validation is exclusive : it must be present product in stock and out of stock&lt;/p&gt;



### addExtraCarriers

    mixed CartCore::addExtraCarriers(array $array)

Execute hook displayCarrierList (extraCarrier) and merge theme to the $array



* Visibility: **public**
* This method is **static**.
* This method is defined in classes\Cart.php line 4011


#### Arguments
* $array **array**



### getDeliveryAddressesWithoutCarriers

    array CartCore::getDeliveryAddressesWithoutCarriers(boolean $return_collection, $error)

Get all the ids of the delivery addresses without carriers



* Visibility: **public**
* This method is defined in classes\Cart.php line 4040


#### Arguments
* $return_collection **boolean** - &lt;p&gt;Return a collection&lt;/p&gt;
* $error **mixed**

