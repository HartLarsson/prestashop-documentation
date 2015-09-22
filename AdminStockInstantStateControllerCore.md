AdminStockInstantStateControllerCore
===============






* Class name: AdminStockInstantStateControllerCore
* Namespace: 
* Parent class: [AdminController](AdminControllerCore)
* This class is defined in controllers\admin\AdminStockInstantStateController.php line 31





Properties
----------


### $stock_instant_state_warehouses

    protected mixed $stock_instant_state_warehouses = array()





* Visibility: **protected**
* This property is defined in controllers\admin\AdminStockInstantStateController.php line 33


### $object

    public \Stock $object





* Visibility: **public**
* This property is defined in controllers\admin\AdminStockInstantStateController.php line 31


Methods
-------


### __construct

    mixed AdminStockInstantStateControllerCore::__construct()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 35




### initPageHeaderToolbar

    mixed AdminStockInstantStateControllerCore::initPageHeaderToolbar()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 110




### renderList

    mixed AdminStockInstantStateControllerCore::renderList()

AdminController::renderList() override



* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 143




### renderDetails

    mixed AdminStockInstantStateControllerCore::renderDetails()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 206




### getList

    mixed AdminStockInstantStateControllerCore::getList(integer $id_lang, string|null $order_by, string|null $order_way, integer $start, integer|null $limit, integer|boolean $id_lang_shop)

AdminController::getList() override



* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 270


#### Arguments
* $id_lang **integer**
* $order_by **string|null**
* $order_way **string|null**
* $start **integer**
* $limit **integer|null**
* $id_lang_shop **integer|boolean**



### valuationCmp

    boolean AdminStockInstantStateControllerCore::valuationCmp(array $n, array $m)

CMP



* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 382


#### Arguments
* $n **array**
* $m **array**



### realQuantityCmp

    boolean AdminStockInstantStateControllerCore::realQuantityCmp(array $n, array $m)

CMP



* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 399


#### Arguments
* $n **array**
* $m **array**



### getCurrentCoverageWarehouse

    integer AdminStockInstantStateControllerCore::getCurrentCoverageWarehouse()

Gets the current warehouse used



* Visibility: **protected**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 413




### initToolbar

    mixed AdminStockInstantStateControllerCore::initToolbar()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 429




### renderCSV

    mixed AdminStockInstantStateControllerCore::renderCSV()

Exports CSV



* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 453




### initContent

    mixed AdminStockInstantStateControllerCore::initContent()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 529




### initProcess

    mixed AdminStockInstantStateControllerCore::initProcess()





* Visibility: **public**
* This method is defined in controllers\admin\AdminStockInstantStateController.php line 538


