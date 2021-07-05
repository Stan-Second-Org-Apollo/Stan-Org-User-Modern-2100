# User Unsubscribed

### 

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "User Unsubscribed",
    "subscription": {
        "unsubscribeMethod": "<unsubscribeMethod>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|unsubscribeMethod|string|Describes the method used to unsubscribe.|footer field, registration opt in, order placed, notification preferences, ESP feed|||||||
