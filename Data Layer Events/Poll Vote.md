# Poll Vote

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Poll Vote",
    "tool": {
        "pollAnswer": "<pollAnswer>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|tool.pollAnswer|string|Captures the user's sentiment poll answer|quiz:hopeful:g, contentModalPopUp:soso:g, quiz:confident:g, quiz:soso:g, contentModalPopUp:hopeful:g|||||||

## Attached Notes

<p>This event is used to capture poll vote analytics when user interact with voting in a poll on tool</p>
