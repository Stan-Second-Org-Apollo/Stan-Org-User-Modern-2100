# Product Viewed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "Product Viewed",
    "product": [
        {
            "fulfillment": {
                "isBopusOnly": "<isBopusOnly>"
            },
            "isThirdPartyProduct": "<isThirdPartyProduct>",
            "price": {
                "sellingPrice": "<sellingPrice>"
            },
            "productInfo": {
                "businessUnit": "<businessUnit>",
                "discountAmount": "<discountAmount>",
                "fulfillmentOptions": "<fulfillmentOptions>",
                "isFeatured": "<isFeatured>",
                "isOutOfStock": "<isOutOfStock>",
                "isSKuAvailable": "<isSKuAvailable>",
                "productID": "<productID>",
                "quantityAvailable": "<quantityAvailable>",
                "ratingCountAndAverageCombined": "<ratingCountAndAverageCombined>",
                "sku": "<sku>",
                "status": "<status>"
            }
        }
    ],
    "productInfo": {
        "isBestSeller": "<isBestSeller>",
        "isTopRated": "<isTopRated>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|businessUnit|string|The business unit associated with each product.|Apparel, Shoes, Home|||||||
|discountAmount|string|The product discount amount shown to the visitor for each product.|$20, 10%, $5|||||||
|fulfillmentOptions|string|The product fulfillment options available for each product to view impact on conversion.|Shipped Only, In Store Only, Local Pickup Only, In Store or Ship, Digital \(Email or Text\)|||||||
|isBestSeller|integer|Count of times the product was a best seller product.||||||||
|isBopusOnly|integer|Count of times the user engaged with a product whose only available shipping method was Buy Online Pick Up In Store \(i.e., BOPUS\).||||||||
|isFeatured|integer|Count of times the product was a featured\/boosted product.||||||||
|isOutOfStock|boolean|Boolean flag indicating that an inventoried product is out of stock. |TRUE, FALSE|||||||
|isSKuAvailable|boolean|True\/False flag to indicate if product SKU is known at the time of the event|true, false|||||||
|isThirdPartyProduct|integer|Count of times a user viewed a product page for a third party \(e.g., marketplace vendor\) product.||||||||
|isTopRated|integer|Count of times the product was a top rated product.||||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|quantityAvailable|string|The product quantity available.|1, 10, 100|||||||
|ratingCountAndAverageCombined|string|Combined Rating Count and Rating Average with colon as delimiter|23:4.5, 222:1.7, 1:5, 2:3.5|||||||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|sku|string|Stock Keeping Unit \(SKU\) Unique Identifier of specific item \(typically\) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|status|string|Described the product's status|In Stock, Out of Stcok, Back-Ordered|||||||
