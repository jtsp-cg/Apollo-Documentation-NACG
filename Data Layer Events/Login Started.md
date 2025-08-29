# Login Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Login Started",
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

<p>This event is used to capture the login started analytics when user start login and interact with any field i.e. Username or Password.</p>
<p>This event fires its own beacon call. product team don't need to se any flag to restrict firing multiple login start calls on multiple interaction of the login form. This willl be taken care by DAE team.</p>
<p><a href="https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#25">https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#25</a></p>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/login">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/login</a></p>
<p>&nbsp;</p>
