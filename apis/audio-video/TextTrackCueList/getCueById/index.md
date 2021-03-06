---
title: 'getCueById'
attributions:
  - 'Microsoft Developer Network: [Windows Internet Explorer API reference Article](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx)'
readiness: 'Ready to Use'
relationships:
  method_of:
    predicate: 'Method of '
    value: apis/audio-video/TextTrackCueList
    href: /apis/audio-video/TextTrackCueList
  return_type:
    predicate: 'Returns an object of type  '
    value: 'DOM Node'
    href: /apis/audio-video/TextTrackCueList
standardization_status: 'W3C Editor''s Draft'
summary: 'Returns the first text track cue object (in text track cue order) with text track cue identifier matching id. Returns null if no cue has the given identifier or if the &quot;id&quot; argument is the empty string.'
tags:
  - API_Object_Methods
  - API
  - Audio
  - Video
uri: apis/audio-video/TextTrackCueList/getCueById

---
## Summary

Returns the first text track cue object (in text track cue order) with text track cue identifier matching id. Returns null if no cue has the given identifier or if the &quot;id&quot; argument is the empty string.

Method of [apis/audio-video/TextTrackCueList](/apis/audio-video/TextTrackCueList)[apis/audio-video/TextTrackCueList](/apis/audio-video/TextTrackCueList)

## Syntax

``` js
var object = TextTrackCueList.getCueById(idString);
```

## Parameters

### idString

 Data-type
:   Blob

**id** for a specific [**TextTrackCue**](/apis/audio-video/TextTrackCue) .

## Return Value

Returns an object of type DOM NodeDOM Node

## Examples

``` js
//. . .
var myTrack = document.getElementById("entrack").track; // get text track from track element
var myCues = myTrack.cues;   // get list of cues
// get a specific TextTrackCue by ID
var myCueObj = myCues.getCueById("CID3");
//. . .
```

## Related specifications

[W3C HTML5 Specification](http://dev.w3.org/html5/spec/single-page.html)
:   W3C Editor's Draft
