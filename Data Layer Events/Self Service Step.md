# Self Service Step

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Self Service Step",
    "process": {
        "processStepLabel": "<processStepLabel>",
        "processStepValue": "<processStepValue>",
        "settingUsed": "<settingUsed>"
    },
    "selfservice": {
        "ActivityName": "<ActivityName>",
        "SessionSettings": "<SessionSettings>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|process.processStepLabel|string|Captures the process step name, e.g. Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|||||||
|process.processStepValue|string|Captures the tool process step number, .e.g., Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|||||||
|process.settingUsed|string|Captures the setting used when running an application\/tool, e.g., Select only Mutual Funds, All, AMUSX, Growth-Income Fund, U.S. Government Securities Fund|Select only Mutual Funds, All, AMUSX, Growth-Income Fund, U.S. Government Securities Fund|||||||
|selfservice.ActivityName|string|Captures the name of the self-service activity that the user interacts with, e.g., Portfolio, View Transactions, RSA Reset Password, Change Address, Update Information, Calculator|Portfolio, View Transactions, RSA Reset Password, Change Address, Update Information, Calculator|||||||
|selfservice.SessionSettings|string|Self Service Session Settings as hit or session based|Hit or Session|||||||

## Attached Notes

<p>This event is used to capture the self-service step analytics when user interacting with the different steps of form field during self service process.</p>
<p>We have 2 types of forms - session and hit based forms. Update the "sessionSettings" attribute with "session" or "hit" to check this.</p>
<p>More deatiled info here -&nbsp;<a href="https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool">https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool</a>?</p>
<p>Example link -&nbsp;<a href="https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/develop/reactjs/src/containers/Advisor/Create/Review.tsx#L158-L161">https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/develop/reactjs/src/containers/Advisor/Create/Review.tsx#L158-L161</a></p>
<p>&nbsp;</p>
<p>Demo Site Link -&nbsp;<a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep</a></p>
