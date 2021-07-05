# Event Booking Completed

### 

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "Event Booking Completed",
    "booking": {
        "ticketList": [
            {
                "event": {
                    "fakeProductId": "<fakeProductId>"
                },
                "price": {
                    "points": "<points>",
                    "sellingPrice": "<sellingPrice>"
                },
                "quantity": "<quantity>"
            }
        ],
        "total": {
            "currency": "<currency>"
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|currency|string|Currency of the payment for the booking. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|fakeProductId|string|Helper node used by AA Product String Builder to set product to location. This field gets a static value of "event".  With updates to the AA PS extension, this will soon go away.|event|event||||||
|points|integer|Number of points for an item booked or sold.|5000, 2520, 3200|||||||
|quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
