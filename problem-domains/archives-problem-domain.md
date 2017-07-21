# The Problem domain with Archives // Dave Rice, CUNY TV / Steven, Villereal University of Virginia Library



Rice: “The archive is often an optional last step for media”
Rice: Discuss challenges of adhering to FCC captioning regulations
Title IX issues, make things accessible to some degree
Must scale up and optimize the workflows
Villereal: Same thing, Section 508 compliance, for university libraries. UVa doesn't have an active broadcast workflow but archival video
If orgs have tape libraries or working with historic tape, they may have captioning information.
Extracting Line 21 data from archival video.
Requires thinking about fair use copyright arguments
Requires thinking broadly about potentials for “recorded information”
CUNY has a microservices open source approach to working with this data
OSS here: https://github.com/mediamicroservices/mm
Probably when there's a mistake at the beginning and everything needs to be re-done -- so they eventually moved to a place where the captions work is asynchronous to the media. They move independently… and at the end they come back together.
Problems with too many captions on one line, bugs causing crashes that eliminate captions for half the content
SCC the broadcast format, basically a hex-dump of the captions. Similar to ASCII except one bit is a checksum (rather than first bit being zero). Then they could see every other letter but then garbage for the others… really needed something in a more human-readable format.
Stephen using Avalon media system and WebVTT 
Stephen: Undersourced for both of these -- needing to kill two birds with one stone, doing archival description and also transcription
AV archives are in a weird place, split between libraries/archives and the broadcast industry. One case being made is that the standards we inherit are things like SMPTE, and don't respect our values. Archives can't afford these standards, they aren't open, they rarely have archivists or people don't that work 
Dave is great for going to IETF to do standardization, because the web is mostly where video gets viewed
Rice: “Steven is always trolling the right people on Twitter”
A single vendor can't be used to do all of this work. CUNY uses  PopUpArchive and another service more common in broadcast, where an audio line to a human captioner does live transcription and sends back a text stream. It's somehow cheaper to get the real time live transcription than if they do it on their own time.
These tools don't do the full work of accessibility. Even though speech to text, there are a lot of things that are not speech that happens and that needs to be communicated too. The whole environment needs to be communicated.
If a show gets played four times a day, they would just end up paying to caption it four times! That’s not a good workflow, should be revised. But maybe will get better with FCC regulations requiring captioning.
UVa also experimenting with PopUp Archives. Who is gonna do that work? Can student workers do that work? What’s the best tool to clean that stuff up? Need a survey of what’s out there right now.
A couple of emerging professional projects (National Digital Stewardship Residency Program: http://www.digitalpreservation.gov/ndsr/) have involved this and other open source techniques.
"Mac Caption"
Timelines matter especially considering accessibility issues
Villereal: Offering the returning of lost Mac Caption dongles as an archival funding source
Extract-CC-Bytestream (https://github.com/IUMDPI/Extract-CC-Bytestream) from Indiana University is a Perl script to do things
Question: What is open source software that needs more work to be better? (v rough paraphrase)
text output from ffmpeg would be great
Dave got a filter called readeia608 in there and you feed in video, finds the line21 capture information (not always on line 21) and translates it to a hex. For old school analog captioning this can help read it out.
