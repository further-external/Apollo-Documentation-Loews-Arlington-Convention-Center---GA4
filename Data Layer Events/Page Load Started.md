# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "page_data": {
        "breadcrumb": "<breadcrumb>",
        "country": "<country>",
        "language": "<language>",
        "name": "<name>",
        "page_location": "<page_location>",
        "page_path": "<page_path>",
        "page_query_string": "<page_query_string>",
        "page_title": "<page_title>",
        "pages_viewed_num_visit": "<pages_viewed_num_visit>",
        "platform_version": "<platform_version>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.breadcrumb|string|A delimited list of hierarchical sections that describe the current page's location within the navigation of the site.|Home&gt;Women&gt;Tops&gt;Sweaters, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Checkout &gt; Order Thank You|||||||
|page_data.country|string|The country associated with the current page.|US, CA, FR, UK|||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.|en-us, en-gb, ch-cn, fr-ca, fr-fr|||||||
|page_data.name|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.page_location|string|Use this only if you need to report Page URLs different from those that appear in the address bar of the browser, for example redacting PII, providing page paths when none exist for SPAs, etc. Captures the URL of the page currently being viewed. This value will include the full, unaltered URL of the page\/screen the user is currently viewing, including query parameters, fragments, etc., for example https:\/\/www.example.com\/home?user=true&audience=test\#aboutus.|https:\/\/www.example.com\/home?user=true&audience=test\#aboutus|||||||
|page_data.page_path|string|Captures the path portion of the page URL.||||||||
|page_data.page_query_string|string|The query string portion of the URL.||||||||
|page_data.page_title|string|The title of the page currently being viewed, generally available in &lt;title&gt;.||||||||
|page_data.pages_viewed_num_visit|string|Running total of how many pages or screens a visitor had viewed at the time they took a website or mobile app action. Count re-starts with each visit.||||||||
|page_data.platform_version|string|The platform used to share content||||||||
|page_data.type|string|The type of page currently viewed.|home, pdp, article|||||||




