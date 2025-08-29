# Page Load Completed

### Page Load Completed is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the last event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Completed"
});
```





## Attached Notes

<p>This event is used to merge with multiple events like Self Service Step/Self service Completed which doesn't fire its own beacon call.</p>
<p>This event specifically fires a page view call.</p>
