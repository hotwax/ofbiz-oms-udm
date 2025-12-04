# ProductStoreSetting to skip update product type
- To prevent **product type updates** from being applied to specific product stores during Shopify sync, you must create a `ProductStoreSetting` record with the setting type `UPDATE_PRODUCT_TYPE` set to `"true"`.
- Create (or update) your data file with the following entry, replacing **STORE** with the appropriate `productStoreId`:

```xml
<org.apache.ofbiz.product.store.ProductStoreSetting 
    productStoreId="STORE" 
    settingTypeEnumId="UPDATE_PRODUCT_TYPE" 
    settingValue="true"/>