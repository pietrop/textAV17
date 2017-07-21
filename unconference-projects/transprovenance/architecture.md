# Data pipeline
1. Input: target web URL (the edited video)

2. Processing:

  1. Request metadata from an external source (e.g. Internet Archive)
  2. Data parsing
  
    * source locations (e.g. URLs)
    * time (start and end of source, start and end of target URL)
    * other extra information (filmed by, title etc.)
    * captions metadata

  3. Generate a manifest file - Have an chimera HLS/Dash manifest file (.m3u8 or .mpd) from the data, such that your playlist contains the metadata for segments and the rendering is prioritised. JWPlayer supports embedding manifest files https://support.jwplayer.com/customer/en/portal/articles/1430240-adaptive-streaming
![](https://developer.apple.com/library/content/referencelibrary/GettingStarted/AboutHTTPLiveStreaming/Art/stream_playlists_2x.png)
Example: https://bitdash-a.akamaihd.net/content/sintel/hls/playlist.m3u8
Note: It was pointed out the exact segment difficult to extract out exactly, but this is just a nice-to-have feature so the segments can be matched up with best effort. 
3. Output:
  * Captions
    * Make the captions go the right way... (Top to bottom)
  * Video
    * 

# Data model
Data model will change based on the API endpoint of the database we get our information from. For now we have a 
See .m3u8 / mpd

# Users needs
Not considered