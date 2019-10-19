This patch addresses changes that were introduced in Magento 2.3.3 that resulted in problems with extensions and customizations of the product collection feature that rely on method chaining contracts.  
The `addAttributeToFilter` method (in file `app/code/Magento/Catalog/Model/ResourceModel/Product/Collection.php`) was refactored without a return statement, which broke the method-chaining that is used extensively in customizations of this feature.  
This patch refactors the method to add the missing return statement and ensure that method chaining works.
