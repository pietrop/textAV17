# Palestinian Remix

{% embed data="{\"url\":\"https://www.youtube.com/embed/CzAP\_au2ltM\",\"type\":\"video\",\"title\":\"2017 07 20 10 58 45\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/CzAP\_au2ltM/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/CzAP\_au2ltM?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/CzAP\_au2ltM?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

## Notes:

* Project : [http://PalestineRemix.com](http://PalestineRemix.com) 20 documentaries in 4 languages \(English, Arabic, Hebrew, Bosnian\) - Based on Hyperaud.io technology.
* When people say that they have transcripts they may not have them in the format that you need.
* Getting transcripts in a word document… in tables…??? Built a tool with a vertical timeline, each paragraph with tabs for each language.
* Helped by QCRI who use Kaldi and have a very good arabic language model.
* To deal with hardcoded subtitles: Duplicate video and in javascript canvas, frame-by-frame matching looking for changes in the subtitles, and send it to tesseract server-side with English back \(with bad spelling because hard to do\).
* “One night I managed to write something terrifying like this …”

