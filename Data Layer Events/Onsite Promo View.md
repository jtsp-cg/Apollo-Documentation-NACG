# Onsite Promo View

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Promo View",
    "product": [
        {
            "productInfo": {
                "productID": "<productID>"
            }
        }
    ],
    "promotion": {
        "promoName": "<promoName>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|product[n].productInfo.productID|string|Data Campaign IDs||||||||
|promotion.promoName|string|Captures the onsite promo that was clicked on by the user, e.g., inv8681887, adv1975462, adv6804511, inv4695528|inv8681887, adv1975462, adv6804511, inv4695528|||||||

## Attached Notes

<p>This event is used to capture the onsite promo view analytics when user views any promotion banner</p>
<p>Implementation Notes -</p>
<ul>
<li>Product team need to add data campaign code on page&nbsp;
<ul>
<li>AEM - through component dialogue</li>
<li>Non AEM- through content fragment or code</li>
</ul>
</li>
<li>Adobe Launch code will internally call Apollo Promo view schema to capture promo impressions</li>
<li>Promo impressions will be captured at view port.</li>
</ul>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/poc">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/poc</a></p>
<p>&nbsp;</p>
