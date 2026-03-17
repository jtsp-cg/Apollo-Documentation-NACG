# Fire Other Click

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Fire Other Click",
    "linkName": {
        "customLinkName": "<customLinkName>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkName.customLinkName|string|Track Activity without Page Load
Fire other click adobe Adobe analytics beacon call.
This scheme is useful when user don't want to fire page load call and want to do operation as other click|selfservicecompleted|||||||




