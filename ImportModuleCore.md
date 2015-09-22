ImportModuleCore
===============

ImportModule class, ImportModule.php
Import module management




* Class name: ImportModuleCore
* Namespace: 
* This is an **abstract** class
* Parent class: [Module](ModuleCore)
* This class is defined in classes\module\ImportModule.php line 34





Properties
----------


### $_link

    protected mixed $_link = null





* Visibility: **protected**
* This property is defined in classes\module\ImportModule.php line 36


### $server

    public mixed $server





* Visibility: **public**
* This property is defined in classes\module\ImportModule.php line 38


### $user

    public mixed $user





* Visibility: **public**
* This property is defined in classes\module\ImportModule.php line 40


### $passwd

    public mixed $passwd





* Visibility: **public**
* This property is defined in classes\module\ImportModule.php line 42


### $database

    public mixed $database





* Visibility: **public**
* This property is defined in classes\module\ImportModule.php line 44


### $prefix

    public string $prefix





* Visibility: **public**
* This property is defined in classes\module\ImportModule.php line 47


Methods
-------


### __destruct

    mixed ImportModuleCore::__destruct()





* Visibility: **public**
* This method is defined in classes\module\ImportModule.php line 50




### initDatabaseConnection

    mixed ImportModuleCore::initDatabaseConnection()





* Visibility: **protected**
* This method is defined in classes\module\ImportModule.php line 57




### ExecuteS

    mixed ImportModuleCore::ExecuteS($query)





* Visibility: **public**
* This method is defined in classes\module\ImportModule.php line 75


#### Arguments
* $query **mixed**



### Execute

    mixed ImportModuleCore::Execute($query)





* Visibility: **public**
* This method is defined in classes\module\ImportModule.php line 88


#### Arguments
* $query **mixed**



### getValue

    mixed ImportModuleCore::getValue($query)





* Visibility: **public**
* This method is defined in classes\module\ImportModule.php line 94


#### Arguments
* $query **mixed**



### getImportModulesOnDisk

    mixed ImportModuleCore::getImportModulesOnDisk()





* Visibility: **public**
* This method is **static**.
* This method is defined in classes\module\ImportModule.php line 105




### getDefaultIdLang

    mixed ImportModuleCore::getDefaultIdLang()





* Visibility: **public**
* This method is **abstract**.
* This method is defined in classes\module\ImportModule.php line 116


