# Set Account Values

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Set Account Values",
    "account": {
        "accountID": "<accountID>",
        "clientID": "<clientID>",
        "documentID": "<documentID>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|account.accountID|string|Set Account ID in account portal flow|23546878|||||||
|account.clientID|string|Set Client ID in account portal flow|324435|||||||
|account.documentID|string|Set Document ID in account portal flow|244|||||||




