This patch resolves an issue with the Async and Bulk APIs, which in certain versions of Magento do not provide the information needed to update or create data for specific stores.  
Without this patch, the Async/Bulk REST APIs will support the default store view scope only.

Affected Magento versions are: Magento Open Source v2.3.2, 2.3.1

(This patch is also known as MAGETWO-99902.)
