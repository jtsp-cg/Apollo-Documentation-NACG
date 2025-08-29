# Login Lockout

### 

## Variable Definitions

| Attribute Name|Data Source Type|Data Source|Description|
| --- | --- | --- | --- |
|Count of Login Lockouts|Static|1|Description not provided|
|Process Steps|Static|1|Description not provided|

## Attached Notes

<p>This event is used to capture the login lockout analytics when user trying to login continuously with incorrect password</p>
<p>This event doesn't have its own beacon call. This has to be attached with "PageLoadCompleted" event.</p>
<p>For<strong> javstack pages </strong>- AEM header will fire the page view call from th header but we want to see login failure events within that page view call.</p>
<p>To resolve this issue - we have approach, product team will set the login failre event in the localstorage "<strong>pushAnalyticsSent</strong>" on DOM ready. AEM header has a logic that will<strong> sanwich</strong> the events from local storage in between page load events.</p>
<p>Reference Link - <a href="https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#28">https://bitbucket.capgroup.com/projects/CIAM/repos/cicwebapp/browse/app/src/main/webapp/js/loginEvent.js#28</a></p>
<p>Detailed steps with example here - <a href="https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-HowtofireMultistep(Toolevents,SelfServiceEvents,AccountActivityEvent)AnalyticsinJavastackPagesusingsandiwchpattern?">Apollo Analytics Integration</a></p>