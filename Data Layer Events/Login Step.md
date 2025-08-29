# Login Step

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Login Step",
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




