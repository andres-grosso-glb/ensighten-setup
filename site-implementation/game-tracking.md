# Game Tracking

The examples on the right-hand side list the standard game tracking calls.

* The **gamersid** variable will send your call to a different Adobe report suite on fly. Omitting the variable will direct the traffic to the default report suite\(s\).

{% hint style="success" %}
 **iFrame Games**  
  
If your game is hosted in an iframe, you must add the following Ensighten Bootstrap on your iframe page `<head>` before adding any tracking calls.  
 `<script> var turner_metadata = { "trackAction" : [] }; </script> <script src="//nexus.ensighten.com/turnerintl/<example-space>/Bootstrap.js"></script>`

 _\*\* The correct Bootstrap.js file will be provided by the analytics team._  
  
Also, to include the page level data, you must ask the site dev team to add the page metadata to your iframe source query string.  
 `<iframe src="https://emea.iframed.cn.dmti.cloud/game/ben-10-omnicode/index.html?pageName=/cn/ben-10-omnicode&cid=123&OnetrustActiveGroups=1,2"></iframe>`  
Common Page Metadata:

* pageName - page name of the parent page \(e.g. /uk/cn/ben-10-omnicode\)
* cid - campaign code \(e.g. 123\)
* OnetrustActiveGroups - OneTrust banner variable \(e.g. 1,2,3,4\)
{% endhint %}

#### Game Launch Event

```text
turner_metadata.trackAction.push({
  "type" : "game",
  "data" : {
    "gamersid" : "", /* string */
    "interaction" : "game launch event",
    "gametitle" : "", /* string */
    "gamecategory" : "", /* string | pipe delimited */
    "gamelaunchevent" : 1
  }
});
```

#### Game Pre-Roll Ad Start

```text
turner_metadata.trackAction.push({
  "type": "game-preroll",
  "data": {
    "ad_id" : "", /* string */
    "ad_duration" : 0, /* integer | ad duration in seconds */
    "ad_event" : "start",
    "gamename" : "", /* string */
    "gamersid" : "", /* string */
    "playerName" : "", /* string | identifies player of pre-roll advertisement */
    "channel" : "", /* string | identifies pre-roll advertisement delivery channel */
    "appVersion" : "", /* string | SDK version of video player */
    "ovp" : "" /* string | online video platform identifier */
  }
});
```

#### Game Pre-Roll Ad Skip

```text
turner_metadata.trackAction.push({
  "type" : "game-preroll",
  "data" : {
    "ad_event" : "skip"
  }
});
```

