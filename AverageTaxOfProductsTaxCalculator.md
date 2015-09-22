AverageTaxOfProductsTaxCalculator
===============






* Class name: AverageTaxOfProductsTaxCalculator
* Namespace: 
* This class is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 3





Properties
----------


### $id_order

    private mixed $id_order





* Visibility: **private**
* This property is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 5


### $configuration

    private mixed $configuration





* Visibility: **private**
* This property is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 6


### $db

    private mixed $db





* Visibility: **private**
* This property is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 7


### $computation_method

    public mixed $computation_method = 'average_tax_of_products'





* Visibility: **public**
* This property is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 9


Methods
-------


### __construct

    mixed AverageTaxOfProductsTaxCalculator::__construct(\Core_Foundation_Database_DatabaseInterface $db, \Core_Business_ConfigurationInterface $configuration)





* Visibility: **public**
* This method is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 11


#### Arguments
* $db **[Core_Foundation_Database_DatabaseInterface](Core_Foundation_Database_DatabaseInterface)**
* $configuration **[Core_Business_ConfigurationInterface](Core_Business_ConfigurationInterface)**



### getProductTaxes

    mixed AverageTaxOfProductsTaxCalculator::getProductTaxes()





* Visibility: **private**
* This method is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 17




### setIdOrder

    mixed AverageTaxOfProductsTaxCalculator::setIdOrder($id_order)





* Visibility: **public**
* This method is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 30


#### Arguments
* $id_order **mixed**



### getTaxesAmount

    mixed AverageTaxOfProductsTaxCalculator::getTaxesAmount($price_before_tax, $price_after_tax, $round_precision, $round_mode)





* Visibility: **public**
* This method is defined in classes\tax\AverageTaxOfProductsTaxCalculator.php line 36


#### Arguments
* $price_before_tax **mixed**
* $price_after_tax **mixed**
* $round_precision **mixed**
* $round_mode **mixed**

