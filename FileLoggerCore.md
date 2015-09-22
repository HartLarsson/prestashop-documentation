FileLoggerCore
===============






* Class name: FileLoggerCore
* Namespace: 
* Parent class: [AbstractLogger](AbstractLoggerCore)
* This class is defined in classes\log\FileLogger.php line 27





Properties
----------


### $filename

    protected mixed $filename = ''





* Visibility: **protected**
* This property is defined in classes\log\FileLogger.php line 29


Methods
-------


### logMessage

    mixed FileLoggerCore::logMessage($message, $level)

Write the message in the log file



* Visibility: **protected**
* This method is defined in classes\log\FileLogger.php line 37


#### Arguments
* $message **mixed**
* $level **mixed**



### setFilename

    mixed FileLoggerCore::setFilename(string $filename)

Check if the specified filename is writable and set the filename



* Visibility: **public**
* This method is defined in classes\log\FileLogger.php line 51


#### Arguments
* $filename **string**



### getFilename

    mixed FileLoggerCore::getFilename()

Log the message



* Visibility: **public**
* This method is defined in classes\log\FileLogger.php line 66


