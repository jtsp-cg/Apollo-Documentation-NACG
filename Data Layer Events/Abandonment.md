# Abandonment

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Abandonment",
    "abandonment": {
        "lasttouchfield": "<lasttouchfield>",
        "userinputfields": "<userinputfields>"
    },
    "process": {
        "processStepLabel": "<processStepLabel>",
        "processStepValue": "<processStepValue>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|abandonment.lasttouchfield|string|What was last interacted filed when user left self service, form or tool activity?|loginEmail, role, firstName, company, lastName, subscribe, residency, question, firm|||||||
|abandonment.userinputfields|string|What are last interacted fields when user left self service , form or tool activity?|loginEmail, firstName, emailAddress, lastName, nickName|||||||
|process.processStepLabel|string|Captures the process step name, e.g. Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|||||||
|process.processStepValue|string|Captures the tool process step number, .e.g., Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|||||||

## Attached Notes

<p>This event is used to capture the abandonment analytics when user start any self-service, form and tool activities and abandons without completing it successfully</p>
<p>Helper function has been created to track form abandoned analytics here: &nbsp;<a href="https://confluence.capgroup.com/display/CGDP/Helper+Functions+to+Track+Form+Abandoned+Analytics">https://confluence.capgroup.com/display/CGDP/Helper+Functions+to+Track+Form+Abandoned+Analytics</a></p>
<p>Reference and Example links are attached in the above link.</p>
<p>&nbsp;</p>
