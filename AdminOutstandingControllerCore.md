AdminOutstandingControllerCore
===============






* Class name: AdminOutstandingControllerCore
* Namespace: 
* Parent class: [AdminController](AdminControllerCore)
* This class is defined in controllers\admin\AdminOutstandingController.php line 30





Properties
----------


### $object

    public \OrderInvoice $object





* Visibility: **public**
* This property is defined in controllers\admin\AdminOutstandingController.php line 30


Methods
-------


### __construct

    mixed AdminOutstandingControllerCore::__construct()





* Visibility: **public**
* This method is defined in controllers\admin\AdminOutstandingController.php line 32




### initToolbar

    boolean AdminOutstandingControllerCore::initToolbar()

Toolbar initialisation



* Visibility: **public**
* This method is defined in controllers\admin\AdminOutstandingController.php line 119




### printPDFIcons

    string AdminOutstandingControllerCore::printPDFIcons($id_invoice, $tr)

Column callback for print PDF incon



* Visibility: **public**
* This method is defined in controllers\admin\AdminOutstandingController.php line 130


#### Arguments
* $id_invoice **mixed** - &lt;p&gt;integer Invoice ID&lt;/p&gt;
* $tr **mixed** - &lt;p&gt;array Row data&lt;/p&gt;



### printOutstandingCalculation

    mixed AdminOutstandingControllerCore::printOutstandingCalculation($id_invoice, $tr)





* Visibility: **public**
* This method is defined in controllers\admin\AdminOutstandingController.php line 139


#### Arguments
* $id_invoice **mixed**
* $tr **mixed**



### renderView

    mixed AdminOutstandingControllerCore::renderView()

View render



* Visibility: **public**
* This method is defined in controllers\admin\AdminOutstandingController.php line 161


