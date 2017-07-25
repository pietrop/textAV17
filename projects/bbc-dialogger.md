# Text-based audio editing in radio production, BBC Dialogger // Chris Baume, BBC R&D

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ej5WKJ410oU" frameborder="0" allowfullscreen></iframe>

###Links:
* [Slides](http://slides.com/chrisbaume/textav/)
* [Dialogger software](https://github.com/bbc/dialogger)

###Notes:
* 9 stations, 34 million listeners -- BBC is pretty big
* Transcription is rough and manual process (enough for them to understand whats going on -- slow and "waste of their time")
* Producers will pay other people to do it, in Australia which is overnight because of how time zones work, but only if they have the money
* Timed transcripts in 2002, SCANMail, meant for navigating voicemail using text
* Also this program called SILVER
* 2004, SCANMail could edit text
* Then a video editor can do transcripts with different camera angles and it auto edits the video so there are no awkward jump cuts
* (Association of Computing Machinery) ACM is the journal where all these examples are coming from: https://www.acm.org/publications/journals 
* Removing "ums" and other sounds
* 2016: prototype to quickly revise spoken comments
* Chris is now demo'ing some prototypes out of BBC R&D
* HTML5Compositor
* Demonstrates the Magic Pen tool where transcripts can be printed, written on with a specific pen with a camera, and having those edits uploaded back to the document so producers can work at their leisure / on the go / not in the office
* "Speech to text is a lossy process"

###Academic references:
* Whittaker, Steve, et al. "SCANMail: a voicemail interface that makes speech browsable, readable and searchable." Proceedings of the SIGCHI conference on Human factors in computing systems. ACM, 2002. [DOI](http://doi.acm.org/10.1145/503376.503426)
* Casares, Juan, et al. "Simplifying video editing with SILVER." CHI'02 Extended Abstracts on Human Factors in Computing Systems. ACM, 2002. [DOI](http://doi.acm.org/10.1145/778712.778737)
* Whittaker, Steve, and Brian Amento. "Semantic speech editing." Proceedings of the SIGCHI conference on Human factors in computing systems. ACM, 2004. [DOI](http://doi.acm.org/10.1145/985692.985759)
* Berthouzoz, Floraine, Wilmot Li, and Maneesh Agrawala. "Tools for placing cuts and transitions in interview video." ACM Trans. Graph. 31.4 (2012): 67-1. [DOI](http://doi.acm.org/10.1145/2185520.2185563)
* Rubin, Steve, et al. "Content-based tools for editing audio stories." Proceedings of the 26th annual ACM symposium on User interface software and technology. ACM, 2013. [DOI](http://doi.acm.org/10.1145/2501988.2501993)
* Sivaraman, Venkatesh, Dongwook Yoon, and Piotr Mitros. "Simplified Audio Production in Asynchronous Voice-Based Discussions." Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems. ACM, 2016. [DOI](http://doi.acm.org/10.1145/2858036.2858416)
* Shin, Hijung Valentina, Wilmot Li, and Frédo Durand. "Dynamic Authoring of Audio with Linked Scripts." Proceedings of the 29th Annual Symposium on User Interface Software and Technology. ACM, 2016. [DOI](http://doi.acm.org/10.1145/2984511.2984561)

###Ideas for next steps
* Common base UI element for timed transcript editing
* Google Docs style collaborative time transcript editor/player
* Better, meaningful annotations (e.g. rate segments, export >4*)
* Template for EDL file generation
* Embed transcript and annotations in audio file
* Umm detection/removal (STT with umms?)
* Automatic segmentation with tagging and summaries
* Better time compression
* Tools for recording multiple versions of a script
* Digital pen with audio playback, natural annotation and live bidirectional sync
* Smart correction by exposing STT graphs
* Fast clipping of a live audio stream using transcripts
* Bidirectional integration with a proper audio editing system