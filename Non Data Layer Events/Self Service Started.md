# Self Service Started

### 

## Variable Definitions

| Attribute Name|Data Source Type|Data Source|Description|
| --- | --- | --- | --- |
|Process Steps|Static|1|Indicates the user encountered a process step|
|Self Service Starts|Static|1|Description not provided|

## Attached Notes

<p>This event is used to capture the self-service start analytics when user starts self-service and interacts with any field on form.</p>
<p>We have 2 types of forms - session and hit based forms. Update the "sessionSettings" attribute with "session" or "hit" to check this.</p>
<p>More deatiled info here - <a href="https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool">https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool</a>?</p>
<p>Example link - <a href="https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/de98cdef0a97cc7ef69b67adb5f2c3161d72ae48/reactjs/src/containers/Advisor/Create/PlanSponsorInfo/Search.tsx#L201">https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/de98cdef0a97cc7ef69b67adb5f2c3161d72ae48/reactjs/src/containers/Advisor/Create/PlanSponsorInfo/Search.tsx#L201</a></p>
<p>Demo Site Link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep</a></p>
<p>&nbsp;</p>