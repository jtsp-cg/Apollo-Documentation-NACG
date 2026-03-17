# Fund Additions

### 

## Variable Definitions

| Attribute Name|Data Source Type|Data Source|Description|
| --- | --- | --- | --- |
|Add 'scAdd' to s.events|Static|scAdd|Fund Additions|
|Set category to 'product'|Static|product|Description not provided|

## Attached Notes

<p>This event is used to capture fund addition analytics when user add any funds in filter from self service or tool.</p>
<p>This event doesn't have its own beacon call to fire. This event has to be merged with "PageLoadCompleted" event to see the beacon call in omnibug,</p>
<p>Or We can just use the helper function created by DAE team to track this analytics here -</p>
<p><a href="https://confluence.capgroup.com/pages/viewpage.action?pageId=880073651">https://confluence.capgroup.com/pages/viewpage.action?pageId=880073651</a></p>
<p>Demo site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/funds">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/funds</a></p>
<p>&nbsp;</p>