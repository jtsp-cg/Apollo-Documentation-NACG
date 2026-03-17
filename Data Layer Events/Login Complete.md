# Login Complete

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Login Complete",
    "process": {
        "processStepLabel": "<processStepLabel>",
        "processStepValue": "<processStepValue>"
    },
    "userStatus": {
        "loginMethod": "<loginMethod>",
        "siteLoginStatus": "<siteLoginStatus>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|process.processStepLabel|string|Captures the process step name, e.g. Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|||||||
|process.processStepValue|string|Captures the tool process step number, .e.g., Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|||||||
|userStatus.loginMethod|string|Captures if there was a user login to the website via a customized user name, account, or ID|Vision Login, Advisor Site Login, RKD Sponsor Login, Login, Ria Site Login, Institutional Site Login|||||||
|userStatus.siteLoginStatus|string|Capture Site login status where original login happened.|true, false|||||||

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
