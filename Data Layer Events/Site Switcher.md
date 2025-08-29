# Site Switcher

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Site Switcher",
    "navigation": {
        "siteSwitcherName": "<siteSwitcherName>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|navigation.siteSwitcherName|string|Capture Site name\path at time of site selection from CG Site Switcher.|\/us\/en\/individual\/|||||||

## Attached Notes

<p>This event is triggered when user uses global site switcher to change sites</p>
