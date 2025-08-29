# Multi-Media Chapter Click

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Multi-Media Chapter Click",
    "MultiMedia": {
        "MultiMediaName": "<MultiMediaName>",
        "MultiMediaType": "<MultiMediaType>",
        "chapterName": "<chapterName>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|MultiMedia.MultiMediaName|string|Captured the name of the Multi Media playing, .e.g., thecapitalgroup\/ODR-22003\_How\_to\_View\_Download\_Statements\_and\_Tax\_forms\_V7\_HQHD\_MED-AVS, thecapitalgroup\/CPG007\_Registration\_Video\_FINAL\_V2-AVS, How much money do I need for retirement?, thecapitalgroup\/Simple\_IRA\_video-AVS|thecapitalgroup\/ODR-22003\_How\_to\_View\_Download\_Statements\_and\_Tax\_forms\_V7\_HQHD\_MED-AVS, thecapitalgroup\/CPG007\_Registration\_Video\_FINAL\_V2-AVS, How much money do I need for retirement?, thecapitalgroup\/Simple\_IRA\_video-AVS|||||||
|MultiMedia.MultiMediaType|string|Captured the type of the Multi Media playing e.g Video , Audio|Video , Audio|||||||
|MultiMedia.chapterName|string|Name of the chapter of the Multi-Media that was clicked|China's growth over 40 years, On-the-ground research, China's reopening has global benefits, Where elections may be headed, The pivot from fossil fuels|||||||




