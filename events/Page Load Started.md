# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "Page Load Started",
    "page": {
        "dayOfWeek": "<dayOfWeek>",
        "hour": "<hour>",
        "isIncognitoMode": "<isIncognitoMode>",
        "pageName": "<pageName>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|dayOfWeek|string|The day of the week the activity occured.||||||||
|hour|string|The time of activity at the top of the hour.||||||||
|isIncognitoMode|integer|Set on all pages when user is in "incognito mode" in their browser.||||||||
|pageName|string|Describes the page and its content specifically. |product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
