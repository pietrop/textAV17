# From Spoken Word To Sheet Music // Brian Foo



NYPL Transcript Editor 
http://transcribe.oralhistory.nypl.org/
Open sourced here: https://github.com/NYPL/transcript-editor
"Spoken word into sheet music" Example: https://github.com/beefoo/still-i-rise
Used Kaldi to get data down to the phoneme level of a word 
After that, used Praat, another open source tool for phonetic analysis of speech. It can extract pitch and intensity and what is called "voice pulses."
Lilypond, another OSS tool for "engraving music"
Blog post on Still I Rise project: https://medium.com/@beefoo/still-i-rise-from-spoken-word-to-sheet-music-c8024911771e


FrameTrail // Joscha Jäger, Open Hypervideo [Slides]
Experience, manage, and edit interactive video
"Like an IDE for film" -- "at this point in time, I want this snippet to be executed"
Open source, of course! https://github.com/OpenHypervideo/FrameTrail
Two use cases:
Annotating German Parliamentary debates
Connecting relevant document sets with video recordings
Web annotation data model (JSON LD) file format https://www.w3.org/TR/annotation-model/
To be released at the end of August
Open source web documentary “Field Trip”
Attempt to do all post-production in-browser
Expected release October 2018
Q: What problems have you encountered when using JSON LD?
Some strange decisions in format spec, e.g. timestamps are represented as strings
A lot of repeated information within a single file
