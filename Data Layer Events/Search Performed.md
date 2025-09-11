# Search Performed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Search Performed",
    "onsiteSearch": {
        "categoryFilterName": "<categoryFilterName>",
        "filterName": "<filterName>"
    },
    "search": {
        "keyword": {
            "searchTerm": "<searchTerm>",
            "searchType": "<searchType>"
        },
        "numResults": "<numResults>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|onsiteSearch.categoryFilterName|string|Name of the Category filter used to narrow down the search results|Market & Economy|||||||
|onsiteSearch.filterName|string|Name of the filter used to narrow down the search results|Insights, Images, Photo, Investments, Tools, Planning, Outlook, Financial Planning|||||||
|search.keyword.searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion.|bluth, blue, red lobster|||||||
|search.keyword.searchType|string|Describes the domain of the search.|products, properties, articles, authors, coupons, publications|||||||
|search.numResults|string|Number of search results|14|||||||

## Attached Notes

<p>This event captures analytics of the site search performed by the user</p>
