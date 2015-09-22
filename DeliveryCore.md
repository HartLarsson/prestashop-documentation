DeliveryCore
===============






* Class name: DeliveryCore
* Namespace: 
* Parent class: [ObjectModel](ObjectModelCore)
* This class is defined in classes\Delivery.php line 27





Properties
----------


### $id_delivery

    public integer $id_delivery





* Visibility: **public**
* This property is defined in classes\Delivery.php line 30


### $id_shop

    public integer $id_shop





* Visibility: **public**
* This property is defined in classes\Delivery.php line 33


### $id_shop_group

    public integer $id_shop_group





* Visibility: **public**
* This property is defined in classes\Delivery.php line 36


### $id_carrier

    public integer $id_carrier





* Visibility: **public**
* This property is defined in classes\Delivery.php line 39


### $id_range_price

    public integer $id_range_price





* Visibility: **public**
* This property is defined in classes\Delivery.php line 42


### $id_range_weight

    public integer $id_range_weight





* Visibility: **public**
* This property is defined in classes\Delivery.php line 45


### $id_zone

    public integer $id_zone





* Visibility: **public**
* This property is defined in classes\Delivery.php line 48


### $price

    public float $price





* Visibility: **public**
* This property is defined in classes\Delivery.php line 51


### $definition

    public mixed $definition = array('table' => 'delivery', 'primary' => 'id_delivery', 'fields' => array('id_carrier' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_range_price' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_range_weight' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_zone' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_shop' => array('type' => self::TYPE_INT), 'id_shop_group' => array('type' => self::TYPE_INT), 'price' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true)))





* Visibility: **public**
* This property is **static**.
* This property is defined in classes\Delivery.php line 56


### $webserviceParameters

    protected mixed $webserviceParameters = array('objectsNodeName' => 'deliveries', 'fields' => array('id_carrier' => array('xlink_resource' => 'carriers'), 'id_range_price' => array('xlink_resource' => 'price_ranges'), 'id_range_weight' => array('xlink_resource' => 'weight_ranges'), 'id_zone' => array('xlink_resource' => 'zones')))





* Visibility: **protected**
* This property is defined in classes\Delivery.php line 70


Methods
-------


### getFields

    mixed DeliveryCore::getFields()





* Visibility: **public**
* This method is defined in classes\Delivery.php line 80


