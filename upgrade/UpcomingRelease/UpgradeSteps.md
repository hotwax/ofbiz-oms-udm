## We have updated the enum type of Shopify Shop Access. Please check the existing record using below SQL.

```
SELECT COUNT(*) FROM ENUMERATION WHERE ENUM_TYPE_ID = "SHOPIFY_SHOP_ACCESS";
```

If the count is grater then 0 then import the below data.
```
<moqui.basic.EnumerationType description="Shopify Shop Access Scope" enumTypeId="ShopifyShopAccessScope"/>
<moqui.basic.Enumeration description="Shopify Shop No Access" enumCode="SHOP_NO" enumId="SHOP_NO_ACCESS" enumTypeId="ShopifyShopAccessScope"/>
<moqui.basic.Enumeration description="Shopify Shop Read Only Access" enumCode="SHOP_READ" enumId="SHOP_READ_ACCESS" enumTypeId="ShopifyShopAccessScope"/>
<moqui.basic.Enumeration description="Shopify Shop Read and Write Access" enumCode="SHOP_READ_WRITE" enumId="SHOP_RW_ACCESS" enumTypeId="ShopifyShopAccessScope"/>
```

-----------------
