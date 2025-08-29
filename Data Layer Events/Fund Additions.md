# Fund Additions

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Fund Additions",
    "product": [
        {
            "productInfo": {
                "productID": "<productID>"
            }
        }
    ],
    "tool": {
        "toolId": "<toolId>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|product[n].productInfo.productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants.||||||||
|tool.toolId|string|Unique identifier of a site tool|Mortgage Calculator|||||||

## Attached Notes

<p>This event is used to capture fund addition analytics when user add any funds in filter from self service or tool.</p>
<p>This event doesn't have its own beacon call to fire. This event has to be merged with "PageLoadCompleted" event to see the beacon call in omnibug,</p>
<p>Or We can just use the helper function created by DAE team to track this analytics here -</p>
<p><a href="https://confluence.capgroup.com/pages/viewpage.action?pageId=880073651">https://confluence.capgroup.com/pages/viewpage.action?pageId=880073651</a></p>
<p>Demo site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/funds">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/funds</a></p>
<p>&nbsp;</p>
