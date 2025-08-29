# Error Message Presented

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Error Message Presented",
    "formFieldError": "<formFieldError>",
    "process": {
        "processStepLabel": "<processStepLabel>",
        "processStepValue": "<processStepValue>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|formFieldError|string|Error text or code describing a form field error.|No Name Entered\|Please Enter Income\|Missing Required Field|||||||
|process.processStepLabel|string|Captures the process step name, e.g. Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|Buy Shares, Edit Investment, Change Address, Update Information, Investment calculator, Retirement Planning Calculator \(Quick Analysis\)|||||||
|process.processStepValue|string|Captures the tool process step number, .e.g., Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|Complete: Investment Calculator - Results, Complete: Create Presentation, Complete: State tax exclusions for U.S. government income worksheet -Â  Results, Complete: Review Portfolio, Complete: Retirement Planning Calculator \(Quick Analysis\) - Results, Complete: State tax exclusions for U.S. government income worksheet -  Results|||||||

## Attached Notes

<p>This event is used to capture the error analytics when user inputs invalid values in the form and clicks on submit.</p>
<p>It captures the inline errors in listVar3 in '|" seperated format.</p>
<p>Example - First Name is required|Last Name is required|Age is required|Email is Invalid</p>
<p>Demo site link - <a href="https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep">https://plat-analytics-web.usw1.digital.aws-dev.capgroup.com/multistep</a></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
