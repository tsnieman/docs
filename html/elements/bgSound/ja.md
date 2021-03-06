---
title: 'bgsound'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: ja
  topic: html
lang: ja
notes:
  - 'Deletion Candidate: It''s deprecated, http://www.w3.org/TR/html5/obsolete.html#non-conforming-features'
overview_table:
  '[DOM Interface](/dom/interface)': '[HTMLBGSoundElement](/dom/HTMLBGSoundElement)'
readiness: 'Not Ready'
standardization_status: Non-Standard
summary: "bgsoundはユーザがそのページにいる間、音楽ファイルを再生させるための要素です。\nこの要素を使用せず、代わりにaudio要素を使用してください。\n"
tags:
  - Pages_using_duplicate_arguments_in_template_calls
  - Markup_Elements
  - HTML
uri: html/elements/bgSound/ja

---
## Summary

bgsoundはユーザがそのページにいる間、音楽ファイルを再生させるための要素です。 この要素を使用せず、代わりにaudio要素を使用してください。

## Overview Table

[DOM Interface](/dom/interface)
:   [HTMLBGSoundElement](/dom/HTMLBGSoundElement)

## Examples

音楽ファイルを再生したい場合、[audio](/html/elements/audio/ja)要素を使用してください。

``` html


<audio autoplay id="bgsound">
 <source src="http://media.w3.org/2010/07/bunny/04-Death_Becomes_Fur.mp4"
         type="audio/mp4">
 <source src="http://media.w3.org/2010/07/bunny/04-Death_Becomes_Fur.oga"
         type="audio/ogg; codecs=vorbis">
 <p>ご利用のブラウザはHTML5のaudio要素に対応していません。</p>
</audio>
<button type="button"
        onclick="document.getElementById('bgsound').pause();">
  Stop background sound
</button>
```

</pre>

## Notes

### 備考

`<bgSound>`要素は文書内のどこにでも記述することができます。 この要素は画面上に表示されません。 この要素は終了タグ(\</bgsound\>)が要りません。 この要素は使用しないでください。 HTML5では、`<bgSound>`は["非適合機能"](http://momdo.github.io/html5/obsolete.html#non-conforming-features)として記述されています。

### 標準情報

There are no standards that apply here.

### HTML information

{

## See also

### Related articles

#### Audio

-   [audio-video](/apis/audio-video)

-   [enabled](/apis/audio-video/AudioTrack/enabled)

-   [language](/apis/audio-video/AudioTrack/language)

-   [Web Audio API](/apis/webaudio)

-   [value](/apis/webaudio/AudioParam/value)

-   [WebRTC](/concepts/Internet_and_Web/webrtc)

-   [bgSound](/html/elements/bgSound)

-   **bgsound**

-   [implementing html5 audio](/tutorials/implementing_html5_audio)

-   [WebRTC Resources](/tutorials/webrtc_resources)
