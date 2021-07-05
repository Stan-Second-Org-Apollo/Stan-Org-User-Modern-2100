# Accommodation Booking Completed

### 

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "Accommodation Booking Completed",
    "booking": {
        "payment": [
            {
                "loyaltyPointsAmount": "<loyaltyPointsAmount>",
                "paymentAmount": "<paymentAmount>"
            }
        ],
        "roomList": [
            {
                "location": {
                    "locationId": "<locationId>"
                },
                "room": {
                    "numAdults": "<numAdults>",
                    "numberInMultiRoomReservation": "<numberInMultiRoomReservation>",
                    "ratePerNight": "<ratePerNight>"
                }
            }
        ],
        "total": {
            "currency": "<currency>"
        },
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|currency|string|Currency of the payment for the booking. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|loyaltyPointsAmount|integer|Number of loyalty points |100, 101, 1000||||0|||
|numAdults|integer|Integer number of adults for the booking.|1, 2, 3, 4, 5||||1|||
|numberInMultiRoomReservation|integer|Integer position of a room in a multi-room booking action.|1, 2, 3||||1|||
|paymentAmount|string|String representation of the payment amount. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|ratePerNight|string|String representation of the price per use-period. Typically nightly rate for a hotel room or monthly rate for an apartment. Positive. Up to two decimal places for cents. No currency symbol.|200, 75.29, 150, 89.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|transactionID|string|Unique identifier of the transaction. Max Length 20. Used as a key for upload of post transaction data. ||^[a-zA-Z0-9]{6,20}$|6|20||||
