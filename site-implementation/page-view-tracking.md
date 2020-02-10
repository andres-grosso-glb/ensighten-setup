# Page View Tracking

The example on the right-hand side shows all parameters that can be included with a page view call.

* Use **trackAction** array to push your page view calls.
* **previouspage** variable is handled through Adobe _getPreviousValue_ plugin and does not need to be set.

{% hint style="success" %}
**Track Action Array**

The trackAction array is used for all tracking. Tracked events may be pushed into the trackAction array before Ensighten Bootstrap is loaded.
{% endhint %}

#### **Example Page View Tracking:**

```text
turner_metadata.trackAction.push({
  "type" : "pageview",
  "data" : {
    "pageName": "/ve/cn/home/",
    "products": "category;product;quantity;price",
    "productsevent": "prodView or purchase",
    "section": "site section",
    "searchterm": "search term",
    "region": "region",
    "subregion": "subregion",
    "country": "country",
    "brand": "brand of the site",
    "franchise": "franchise of content",
    "subsection": "site section level 2",
    "contenttype": "content type",
    "contenttitle": "content title",
    "contentID": "content ID",
    "adobehashid": "adobe hash ID",
    "authorizedvhl": "authorized",
    "presentationtemplate": "presentation template",
    "featuredcontent": "featured content",
    "registration": "description of registration",
    "logintype": "login type",
    "authstate": "authentication state of user",
    "englishname": "english name",
    "gametitle": "game title",
    "gamelevel": "game level reached",
    "gamemilstone": "game milestone",
    "micrositename": "microsite name",
    "micrositeadv": "microsite advertiser"
  }
});
```

