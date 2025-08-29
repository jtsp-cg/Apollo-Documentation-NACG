# Page Heartbeat

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Heartbeat",
    "heartbeat": {
        "30secondspagename": "<30secondspagename>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|heartbeat.30secondspagename|string|heartbeat.30secondspagename|30 Seconds \| advisor &gt; Home|||||||

## Attached Notes

<p>This event is captured after the first 30 seconds from start of the session</p>
<p>This is being handled from Launch. No action needed from product team</p>
