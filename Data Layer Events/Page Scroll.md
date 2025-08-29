# Page Scroll

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Scroll",
    "scroll": {
        "pagePercentage": "<pagePercentage>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|scroll.pagePercentage|string|% of Page Scrolled \(25, 50, 75, 100\) along with Page Name separated by a '\|' , e.g. 25 Percent \| home &gt; Home, 50 Percent \| tax-center &gt; Tax Forms You May Receive, 75 Percent \| individual &gt; Home, 100 Percent \| investments &gt; Exchange-Traded Funds \(ETFs\)|25 Percent \| home &gt; Home, 50 Percent \| tax-center &gt; Tax Forms You May Receive, 75 Percent \| individual &gt; Home, 100 Percent \| investments &gt; Exchange-Traded Funds \(ETFs\)|||||||

## Attached Notes

<p>This event is used to capture the page scroll analytics when user scrolling on any page i.e. 25,50,75,100%</p>
<p>This is handled from Adobe Launch</p>
