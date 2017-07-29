# 🔪✅⬇️ \(Annotations models\) // Blaine Cook, Condé Nast

<iframe width="560" height="315" src="https://www.youtube.com/embed/Cd56vF3lZ_Q" frameborder="0" allowfullscreen></iframe>

### Notes
- Killing Markdown
- GML (written in1969), an IBM project to write text into files for computers to display in a better formatted style 
- GML gave birth to SGML, which gave birth to HTML and XML
- “Our tools were based on presumptions that simply were not true anymore”
- "Content is not hierarchical"
- Can we come up with a better mental model for thinking about content?
- We can write code that does this but it's not reproducible.
- Example of manually edited document: The "content" is the printed material and the notes taken over in pen fit in … where?
- JSON, content, annotations: “Contents” distinct from “annotations” in JSON format. 
    - Here’s a simplified version:

```json
{
    contents: “Main text document goes here etc etc etc”,
    annotations: [
        { position: 4, text: “Change this” }
        { position: 12, text: “I like this” }
    ]
}
```

- Theoretically possible for transcript/audio data too.
Not a standard format – ”I’m allergic to standards”
Even the format Blaine showed on screen is “massively simplified”

