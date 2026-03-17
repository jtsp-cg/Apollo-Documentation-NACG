# Tool Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Tool Started",
    "process": {
        "processStepLabel": "<processStepLabel>",
        "processStepValue": "<processStepValue>",
        "settingUsed": "<settingUsed>"
    },
    "tool": {
        "SessionSettings": "<SessionSettings>",
        "toolId": "<toolId>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|process.processStepLabel|string|Captures the process step name, e.g. Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|||||||
|process.processStepValue|string|Captures the tool process step number, .e.g., Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|||||||
|process.settingUsed|string|Captures the setting used when running an application\/tool, e.g., Select only Mutual Funds, All, AMUSX, Growth-Income Fund, U.S. Government Securities Fund|Select only Mutual Funds, All, AMUSX, Growth-Income Fund, U.S. Government Securities Fund|||||||
|tool.SessionSettings|string|Tool Usage Session Settings as hit or session based|Hit or Session|||||||
|tool.toolId|string|Unique identifier of a site tool|Mortgage Calculator|||||||

## Attached Notes

<p>This event is used to capture tool start analytics when user start the tool and interacts with any tool field</p>
<p>We have 2 types of forms - session and hit based forms. Update the "sessionSettings" attribute with "session" or "hit" to check this.</p>
<p>More deatiled info here -&nbsp;<a href="https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool">https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-Whatneedstobedoneiftheform/toolisaSessionbasedForm/Tool</a></p>
<p>https://confluence.capgroup.com/display/CGDP/Apollo+Analytics+Integration+Guide#ApolloAnalyticsIntegrationGuide-HowtofireMultistep(Toolevents,SelfServiceEvents,AccountActivityEvent)AnalyticsinJavastackPagesusingsandiwchpattern?</p>
<p>Example link -&nbsp;</p>
<p><a href="https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/develop/reactjs/src/containers/Quiz/Options/Option.tsx#L118-L121">https://github.com/cg-cxt/leapfrog-microsite-web-react/blob/develop/reactjs/src/containers/Quiz/Options/Option.tsx#L118-L121</a></p>
<p>Demo Site Link - &nbsp;<a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/tool">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/tool</a></p>
