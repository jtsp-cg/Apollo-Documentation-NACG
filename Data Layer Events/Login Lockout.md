# Login Lockout

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Login Lockout",
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

<p>This event is used to capture the login lockout analytics when user trying to login continuously with incorrect password</p>
<p>This event doesn't have its own beacon call. This has to be attached with "PageLoadCompleted" event.</p>
<p>For<strong> javstack pages </strong>- AEM header will fire the page view call from th header but we want to see login failure events within that page view call.</p>
<p>To resolve this issue - we have approach, product team will set the login failre event in the localstorage "<strong>pushAnalyticsSent</strong>" on DOM ready. AEM header has a logic that will<strong> sanwich</strong> the events from local storage in between page load events.</p>
<p>Reference Link - <a href="https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#28">https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#28</a></p>
<p>Detailed steps with example here - <a href="https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-HowtofireMultistep(Toolevents,SelfServiceEvents,AccountActivityEvent)AnalyticsinJavastackPagesusingsandiwchpattern?">Apollo Analytics Integration</a></p>
