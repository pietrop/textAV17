# "You Say 'Tomato', I say 'Tomato' ", lessons learnt from the Palestinian Remix // Laurian Gridinoc, Hyperaud.io

<iframe width="560" height="315" src="https://www.youtube.com/embed/CzAP_au2ltM" frameborder="0" allowfullscreen></iframe>


Project : http://PalestineRemix.com 20 documentaries in 4 languages (English, Arabic, Hebrew, Bosnian) - Based on Hyperaud.io technology.

When people say that they have transcripts they may not have them in the format that you need.

Getting transcripts in a word document… in tables…???
Built a tool with a vertical timeline, each paragraph with tabs for each language.

Helped by QCRI who use Kaldi and have a very good arabic language model.

To deal with hardcoded subtitles: Duplicate  video and in javascript canvas, frame-by-frame matching looking for changes in the subtitles, and send it to tesseract server-side with English back (with bad spelling because hard to do).

“One night I managed to write something terrifying like this …”
