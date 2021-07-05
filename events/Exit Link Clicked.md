# Exit Link Clicked

### 

## Javascript Code
```js
window.appEventData987 = window.appEventData987 || [];
appEventData987.push({
  "event": "Exit Link Clicked",
    "linkInfo": {
        "linkContainer": "<linkContainer>",
        "linkId": "<linkId>",
        "linkRegion": "<linkRegion>",
        "linkTarget": "<linkTarget>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkContainer|string|Indicates the container for a clicked link within the hierarchy \[Site &gt; Page &gt; Region &gt; Container &gt; linkID\]|Best Friends - Best Jeans, Puppy Love, Sail Away, Mens, Kids, Kids : Tops|||||||
|linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkRegion|string|Indicates the region on page for a clicked link within the hierarchy \[Site &gt; Page &gt; Region &gt; Container &gt; linkID\]|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||
|linkTarget|string|HREF of the link.  Primarily useful for exit link tracking. |https:\/\/www.usda.gov. https:\/\/msnbc.com|||||||
