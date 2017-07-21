# Data pipeline
1. Input: target web URL (the edited video)

2. Processing:

  1. Request metadata from an external source (e.g. Internet Archive)
  2. Data parsing
  
    * source locations (e.g. URLs)
    * time (start and end of source, start and end of target URL)
    * other extra information (filmed by, title etc.)
    * captions metadata

  3. Generate manifest file - Have an chimera HLS/Dash manifest file (.m3u8 or .mpd) from the data, such that your playlist contains the metadata for segments and the rendering is prioritised . JWPlayer supports embedding manifest files https://support.jwplayer.com/customer/en/portal/articles/1430240-adaptive-streaming
![](https://developer.apple.com/library/content/referencelibrary/GettingStarted/AboutHTTPLiveStreaming/Art/stream_playlists_2x.png)
3. Output:
  * Captions
  * Video

# Data model

# Users needs
Not considered