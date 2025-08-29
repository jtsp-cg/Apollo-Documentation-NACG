# Article Click

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Article Click",
    "content": {
        "contentAction": "<contentAction>",
        "contentCategory": "<contentCategory>",
        "contentTitle": "<contentTitle>",
        "contentType": "<contentType>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|content.contentAction|string|Captures the type of content interaction was taken by the user after the article click. E.g., read, News click - read, Add to Wallet - wallet, Add to briefcase, Remove from briefcase|read, News click - read, Add to Wallet - wallet, Add to briefcase, Remove from briefcase|||||||
|content.contentCategory|string|Captures the topic\/content category for the content that the user interacted with E.g.,  'Topic\|Source', Industry News \| City Wire, Market Volatility, Bonds, Markets & Economy, Global Equities, ESG|'Topic\|Source', Industry News \| City Wire, Market Volatility, Bonds, Markets & Economy, Global Equities, ESG|||||||
|content.contentTitle|string|Title of a piece of content. |50 ways to use jello, Another look at pandas, Year end giving|||||||
|content.contentType|string|Captures the format\/category for the content the user interacted with e.g., article, events, guides|article, events, guides|||||||

## Attached Notes

<p>This event is used to capture analytics when the user interacts with any article/notes/guides in website.</p>
<p>Demo site - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/article">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/article</a></p>
<p>&nbsp;</p>
