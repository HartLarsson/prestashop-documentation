Class AdminPdfControllerCore
=====================





* Class name: AdminPdfControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminPdfController.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L27)


Contents
--------



### Methods

* [checkCacheFolder](#method-checkCacheFolder)
* [generateDeliverySlipPDFByIdOrder](#method-generateDeliverySlipPDFByIdOrder)
* [generateDeliverySlipPDFByIdOrderInvoice](#method-generateDeliverySlipPDFByIdOrderInvoice)
* [generateInvoicePDFByIdOrder](#method-generateInvoicePDFByIdOrder)
* [generateInvoicePDFByIdOrderInvoice](#method-generateInvoicePDFByIdOrderInvoice)
* [generatePDF](#method-generatePDF)
* [initProcess](#method-initProcess)
* [postProcess](#method-postProcess)
* [processGenerateDeliverySlipPDF](#method-processGenerateDeliverySlipPDF)
* [processGenerateDeliverySlipsPDF](#method-processGenerateDeliverySlipsPDF)
* [processGenerateInvoicePdf](#method-processGenerateInvoicePdf)
* [processGenerateInvoicesPDF](#method-processGenerateInvoicesPDF)
* [processGenerateInvoicesPDF2](#method-processGenerateInvoicesPDF2)
* [processGenerateOrderSlipPDF](#method-processGenerateOrderSlipPDF)
* [processGenerateOrderSlipsPDF](#method-processGenerateOrderSlipsPDF)
* [processGenerateSupplyOrderFormPDF](#method-processGenerateSupplyOrderFormPDF)






Methods
-------


### <a name="method-checkCacheFolder"></a>checkCacheFolder

```php
mixed AdminPdfControllerCore::checkCacheFolder()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L48)




### <a name="method-generateDeliverySlipPDFByIdOrder"></a>generateDeliverySlipPDFByIdOrder

```php
mixed AdminPdfControllerCore::generateDeliverySlipPDFByIdOrder($id_order)
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 151](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L151)


#### Arguments
* $id_order **mixed**



### <a name="method-generateDeliverySlipPDFByIdOrderInvoice"></a>generateDeliverySlipPDFByIdOrderInvoice

```php
mixed AdminPdfControllerCore::generateDeliverySlipPDFByIdOrderInvoice($id_order_invoice)
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L161)


#### Arguments
* $id_order_invoice **mixed**



### <a name="method-generateInvoicePDFByIdOrder"></a>generateInvoicePDFByIdOrder

```php
mixed AdminPdfControllerCore::generateInvoicePDFByIdOrder($id_order)
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 170](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L170)


#### Arguments
* $id_order **mixed**



### <a name="method-generateInvoicePDFByIdOrderInvoice"></a>generateInvoicePDFByIdOrderInvoice

```php
mixed AdminPdfControllerCore::generateInvoicePDFByIdOrderInvoice($id_order_invoice)
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 181](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L181)


#### Arguments
* $id_order_invoice **mixed**



### <a name="method-generatePDF"></a>generatePDF

```php
mixed AdminPdfControllerCore::generatePDF($object, $template)
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 191](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L191)


#### Arguments
* $object **mixed**
* $template **mixed**



### <a name="method-initProcess"></a>initProcess

```php
mixed AdminPdfControllerCore::initProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L37)




### <a name="method-postProcess"></a>postProcess

```php
mixed AdminPdfControllerCore::postProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L29)




### <a name="method-processGenerateDeliverySlipPDF"></a>processGenerateDeliverySlipPDF

```php
mixed AdminPdfControllerCore::processGenerateDeliverySlipPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L76)




### <a name="method-processGenerateDeliverySlipsPDF"></a>processGenerateDeliverySlipsPDF

```php
mixed AdminPdfControllerCore::processGenerateDeliverySlipsPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 127](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L127)




### <a name="method-processGenerateInvoicePdf"></a>processGenerateInvoicePdf

```php
mixed AdminPdfControllerCore::processGenerateInvoicePdf()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L54)




### <a name="method-processGenerateInvoicesPDF"></a>processGenerateInvoicesPDF

```php
mixed AdminPdfControllerCore::processGenerateInvoicesPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L91)




### <a name="method-processGenerateInvoicesPDF2"></a>processGenerateInvoicesPDF2

```php
mixed AdminPdfControllerCore::processGenerateInvoicesPDF2()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L101)




### <a name="method-processGenerateOrderSlipPDF"></a>processGenerateOrderSlipPDF

```php
mixed AdminPdfControllerCore::processGenerateOrderSlipPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L64)




### <a name="method-processGenerateOrderSlipsPDF"></a>processGenerateOrderSlipsPDF

```php
mixed AdminPdfControllerCore::processGenerateOrderSlipsPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L114)




### <a name="method-processGenerateSupplyOrderFormPDF"></a>processGenerateSupplyOrderFormPDF

```php
mixed AdminPdfControllerCore::processGenerateSupplyOrderFormPDF()
```





* Visibility: **public**
* Source: [controllers/admin/AdminPdfController.php line 137](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminPdfController.php#L137)


