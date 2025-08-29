# Multi-Media Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Multi-Media Started",
    "MultiMedia": {
        "MultiMediaName": "<MultiMediaName>",
        "MultiMediaType": "<MultiMediaType>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|MultiMedia.MultiMediaName|string|Captured the name of the Multi Media playing, .e.g., thecapitalgroup\/ODR-22003\_How\_to\_View\_Download\_Statements\_and\_Tax\_forms\_V7\_HQHD\_MED-AVS, thecapitalgroup\/CPG007\_Registration\_Video\_FINAL\_V2-AVS, How much money do I need for retirement?, thecapitalgroup\/Simple\_IRA\_video-AVS|thecapitalgroup\/ODR-22003\_How\_to\_View\_Download\_Statements\_and\_Tax\_forms\_V7\_HQHD\_MED-AVS, thecapitalgroup\/CPG007\_Registration\_Video\_FINAL\_V2-AVS, How much money do I need for retirement?, thecapitalgroup\/Simple\_IRA\_video-AVS|||||||
|MultiMedia.MultiMediaType|string|Captured the type of the Multi Media playing e.g Video , Audio|Video , Audio|||||||

## Attached Notes

<p>This event is used to capture the multi media start analytics when user interact with multi media start button to start video&nbsp;</p>
