# Opened Captions service

{% embed data="{\"url\":\"https://www.youtube.com/embed/k1KAFgilz3o\",\"type\":\"video\",\"title\":\"2017 07 19 14 25 02\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/k1KAFgilz3o/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/k1KAFgilz3o?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/k1KAFgilz3o?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

## Notes:

* OpenedCaptions, a personal project made as a Knight-Mozilla fellow at Boston Globe. 
* There's no API for closed captioning?!
* Line21 Decoding device called TextGrabber, very rare

  Node.js server grabs it and distributed to any listening clients

* Dan made this thing that makes text get super drunk and is claiming that there are useful applications for this
* Like maybe a language translation layer to get things into another language quickly
* The value of having a standard \(but this isn't a standard yet, FYI\), is that things can grow out into more than one source, redistribution through a hub, making it push-based \(easy to scale!\)
* Watch live CNN captions: [https://openedcaptions.com](https://openedcaptions.com) \(at the time, it was showing captions for a pharmaceutical commercial\)
* you can set up your own – source and documentation on GitHub: [https://github.com/slifty/opened-captions](https://github.com/slifty/opened-captions)
* Dan is now doing a live demo and it's important for the record to state that his terminal typeface of choice is Comic Sans
* Get things from television \(usually CSPAN\) and write code against it
* Question: What are the copyright considerations? Hope is that content creators see this and like it, and want to provide their own service about it. A lot of CSPAN is public domain.
* Question: How do we know what channel it is on? 
  * Code has been in stasis but now it needs to be more robust, more than one channel may be running, and provide more info. 
  * Not there yet but anyone who wants to develop on it there's a lot of "low hanging fruit things" to make it more useful.  
* \(PLEASE REACH OUT -- @slifty on twitter, or directly at slifty@gmail.com\)

