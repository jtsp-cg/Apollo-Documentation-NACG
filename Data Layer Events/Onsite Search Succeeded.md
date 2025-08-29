# Onsite Search Succeeded

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Succeeded",
    "search": {
        "keyword": {
            "searchTerm": "<searchTerm>",
            "searchType": "<searchType>"
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|search.keyword.searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion.|bluth, blue, red lobster|||||||
|search.keyword.searchType|string|Describes the domain of the search.|products, properties, articles, authors, coupons, publications|||||||




