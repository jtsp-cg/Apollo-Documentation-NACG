# Login Complete

### 

## Variable Definitions

| Attribute Name|Data Source Type|Data Source|Description|
| --- | --- | --- | --- |
|Count Sign Ins|Static|1|Description not provided|
|Process Steps|Static|1|Description not provided|

## Attached Notes

<p><strong>For exisiting audiences: ['advisor', 'institutional', 'ria', 'individual' ,'FIT', 'ubs', 'retirement-plan-insights']</strong></p>
<p>This event is used to capture login complete analytics for user successful login.</p>
<p>This will be taken care from adobe launch. Dev team needs to set "loginMethodType" with the login process name on successfull login.</p>
<p>Reference - <a href="https://github.com/cg-cxt/dac-authentication-ui/blob/develop/src/services/login.ts#L51">https://github.com/cg-cxt/dac-authentication-ui/blob/develop/src/services/login.ts#L51</a></p>
<p><strong>For other audiences:&nbsp;</strong></p>
<p>This event is used to capture login complete analytics for user successful login. This event should be sanwiched along with Page Load Completed event to trigger login success event in page view call. (events 9,3 eVar43 and eVar44)</p>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/login">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/login</a></p>
<p>&nbsp;</p>
<p>&nbsp;</p>