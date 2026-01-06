## We have updated the enum type of Shopify Shop Access. Please check the existing record using below SQL.

Validate the data of Enumeration Type using below SQL.
```
SELECT COUNT(*) FROM ENUMERATION_TYPE WHERE ENUM_TYPE_ID = "ShopifyShopAccessScope";
```
If the count is 0. Please import the below data.
```
<moqui.basic.EnumerationType description="Shopify Shop Access Scope" enumTypeId="ShopifyShopAccessScope"/>
```

Then validate the data of Enumeration using the below SQL.
```
SELECT COUNT(*) FROM ENUMERATION WHERE ENUM_TYPE_ID = "SHOPIFY_SHOP_ACCESS";
```
If the count is grater then 0. Please run the below SQL.
```
UPDATE ENUMERATION SET ENUM_TYPE_ID = "ShopifyShopAccessScope" WHERE ENUM_TYPE_ID = "SHOPIFY_SHOP_ACCESS";
```

-----------------
