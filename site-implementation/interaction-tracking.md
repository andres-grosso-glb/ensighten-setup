# Interaction Tracking

The examples on the right-hand side list all global standard interaction calls.

* Use _trackAction_ array to push your interaction calls.

#### Featured Content:

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "featured content event",
    "featuredcontent" : "featured content name",
    "featuredcontentevent" : 1
  }
});
```

#### Interaction and Social Click

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "name of social or button"
  }
});
```

#### Video Recommendation Click

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "video recommendation event"
  }
});
```

#### Registration Process Start Click

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "registration start event"
  }
});
```

#### Successful Registration Complete

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "registration complete event",
    "registrationevent" : 1
  }
});
```

#### Internal Campaign/Banner Click

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "internal campaign event",
    "internalcampaign" : "campaign name",
    "featuredcontentevent" : 1
  }
});
```

#### Login Click

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "login start event"
  }
});
```

#### Successful Login Complete

```text
turner_metadata.trackAction.push({
  "type" : "interaction",
  "data" : {
    "interaction" : "login complete event",
    "loginevent" : 1
  }
});
```

