# Content Share

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Share",
    "social": {
        "shareMethod": "<shareMethod>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|social.shareMethod|string|Captures the platform name where content from Capital Group is shared, e.g., LinkedIn, Facebook, Twitter, Embed, Print|LinkedIn, Facebook, Twitter, Embed, Print|||||||

## Attached Notes

<p>This event is used capture analytics that focus on share content on LinkedIn, Twitter , Email, Print, facebook&nbsp;</p>
