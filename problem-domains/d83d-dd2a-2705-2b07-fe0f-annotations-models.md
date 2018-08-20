# 🔪✅⬇️ \(Annotations models\)

{% embed data="{\"url\":\"https://www.youtube.com/embed/Cd56vF3lZ\_Q \",\"type\":\"video\",\"title\":\"2017 07 19 11 26 13\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/Cd56vF3lZ\_Q/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/Cd56vF3lZ\_Q?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/Cd56vF3lZ\_Q?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

## Notes

* Killing Markdown
* GML \(written in1969\), an IBM project to write text into files for computers to display in a better formatted style 
* GML gave birth to SGML, which gave birth to HTML and XML
* “Our tools were based on presumptions that simply were not true anymore”
* "Content is not hierarchical"
* Can we come up with a better mental model for thinking about content?
* We can write code that does this but it's not reproducible.
* Example of manually edited document: The "content" is the printed material and the notes taken over in pen fit in … where?
* JSON, content, annotations: “Contents” distinct from “annotations” in JSON format. 
  * Here’s a simplified version:

```javascript
{
    contents: “Main text document goes here etc etc etc”,
    annotations: [
        { position: 4, text: “Change this” }
        { position: 12, text: “I like this” }
    ]
}
```

* Theoretically possible for transcript/audio data too.

  Not a standard format – ”I’m allergic to standards”

  Even the format Blaine showed on screen is “massively simplified”

