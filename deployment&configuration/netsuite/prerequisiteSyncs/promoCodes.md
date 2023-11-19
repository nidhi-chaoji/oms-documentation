# Setup Promo Codes

## Order level discounts:
If an order has a discount code applied to it, during order sync to NetSuite, HotWax checks if the applied code is available in NetSuite. If the code is available then the exact code is used and the value of the discount is shared as the "Rate". 

In the event that the code is not available in NetSuite, HotWax will use a default discount code 'SHOPIFY DISCOUNT' along with the value of the discount. For this failover to work the discount item must be created in NetSuite first.

1. Go to **Lists > Accounting > Items > New**
2. Select Item Type: **Discount**
3. Enter **'SHOPIFY DISCOUNT'** in the Item Name and Display Name field
4. Enter **0.00** in the Rate field
5. Select Subsidiary
6. In the **Accounting** sub-tab
    - Select Account
    - Check the **'Apply before sales tax'** checkbox

To check promo codes in NetSuite, HotWax syncs promo codes from NetSuite once a day.

### Export Current Promo Codes from NetSuite
Schedule this SuiteScript to export current promo codes in NetSuite that need to be synced to HotWax
```
add SuiteScript here
```

Job to save new promo codes:
```
JOB_IMP_PRMO_CODE
Import Promo Code
FTP Config: IMP_PRMO_CODE
```

### Export Discontinued Promo Codes
Schedule this SuiteScript to export removed promo codes in NetSuite that need to be synced to HotWax
```
add SuiteScript here
```
Job to remove promo codes no longer active in NetSuite:
```
JOB_RMV_PRMO_CODE
Remove Promo Code
IMP_RMV_PRMO_CODE
```

## Discount items
Item level discounts have to be synced as a separate line item in the order using a "SHOPIFY ITEM DISCOUNT" item. The amount of the adjustment is added in the "Amount" field when preparing the CSV for NetSuite and the "Price Level" is always set to "Custom".

To learn more about how discounts are handled on orders, read the full NetSuite integration documentation.

For this sync to work, a blanket ‘discount item’ must be created in NetSuite. If you’re using Shopify this discount code is usually ‘Shopify Discount Item’

This ID of this product in NetSuite needs to be entered into the integration layer so that it can be sent to NetSuite during order sync.

1. Go to **Lists > Accounting > Items > New**
2. Select Item Type: **Discount**
3. Enter **'SHOPIFY DISCOUNT ITEM'** in the Item Name and Display Name field
4. Enter **0.00** in the Rate field
5. Select Subsidiary
6. In the **Accounting** sub-tab
    - Select Account
    - Check the **'Apply before sales tax'** checkbox