# Content Downloads

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Downloads",
    "download": {
        "filelitcode": "<filelitcode>",
        "filename": "<filename>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|download.filelitcode|string|The literature code tied to the document that was clicked on by the user, e.g., Tax Year 2022\_1099-DIV, 350051:cpdf, irgefm-004\_iraben.pdf, AccountBalanceStatement|Tax Year 2022\_1099-DIV, 350051:cpdf, irgefm-004\_iraben.pdf, AccountBalanceStatement|||||||
|download.filename|string|Name of the file downloaded by the User e.g. Tax Year 2022\_1099-DIV, AccountBalanceStatement, 4.3\_ESG\_Global\_Proxy\_Policy\_NACG\_Aug\_2022.pdf, global-study-esg-2022-chapter2\(en\).pdf|Tax Year 2022\_1099-DIV, AccountBalanceStatement, 4.3\_ESG\_Global\_Proxy\_Policy\_NACG\_Aug\_2022.pdf, global-study-esg-2022-chapter2\(en\).pdf|||||||

## Attached Notes

<p>This event is used to capture the content download analytics when user download any content file i.e. literature download, PDF download</p>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/download">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/download</a></p>
<p>&nbsp;</p>
