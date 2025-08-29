# CTA Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "CTA Clicked",
    "linkInfo": {
        "customLinkName": "<customLinkName>",
        "linkId": "<linkId>",
        "linkPosition": "<linkPosition>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkInfo.customLinkName|string|Name of the custom link that applies to a given click|MoneyMinutePromo\_Watch,hispanic-landing\_EXPLORE ICANRETIRE,Language Switch hispanic landing\_es-US,MoneyMinutePromo\_money-minute-promo-here.,Product Cards\_Equity,Show\_get-the-facts\_Investing,Site Switcher\_US Financial Professional,CG\_private-markets\_Logo,CG\_institutions\_Logo,list-2\_50 years of flexible growth investing — and counting,Product Cards\_IVE,Product Cards\_AMF,Strategy Cards\_AMCAP open,Strategy Cards\_EuroPacific Growth open,Strategy Cards\_AMCAP open,Strategy Cards\_AMCAP close,Hispanic Landing\_section\_5,Hispanic Landing\_section\_1,JumpLink\_Class A, 529-A and ABLE-A shares,JumpLink\_Exchanges and other details,ContactUs Modal\_Contact Us Modal\_Cancel,ContactUs Modal\_Contact Us Modal\_OpenETF Returns Page Filter\_etf-returns-list\_settings-dropdown collapsed,ETF Returns Page Filter\_etf-returns-list\_settings-dropdown expanded,ETF etf-returns Page Objective Filter\_etf-etf-returns-list-objective\_Growth,Data Filter\_2020\_Gender\_Leadership,Strategy Selector\_Overview Add Asset Class multi-asset,Newsletter\_Submit Confluence - https:\/\/confluence.capgroup.com\/display\/DIGPD\/Custom-Link-Analytics|||||||
|linkInfo.linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkInfo.linkPosition|string|Position of the link clicked|1,2,3|||||||

## Attached Notes

<p>This event is used to track the interactions of users with custom links present on the web page. These interactions encompass various actions such as clicking on text, buttons, tabs, anchor links, and similar elements.</p>
<p>refer new taxonomy documentation and samples here.</p>
<p><a href="https://confluence.capgroup.com/display/DIGPD/Custom-Link-Analytics">https://confluence.capgroup.com/display/DIGPD/Custom-Link-Analytics</a></p>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/cta">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/cta</a></p>
<p>&nbsp;</p>
