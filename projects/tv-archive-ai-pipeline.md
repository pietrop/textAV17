# Tv Archive AI pipeline // Internet Archive, Dan Schultz

<iframe width="560" height="315" src="https://www.youtube.com/embed/HmuKbnBYk84" frameborder="0" allowfullscreen></iframe>

SLIDES: https://docs.google.com/presentation/d/17s8tvqYY8zb4cGVk0MPi2HeA85af-x0macLn-WijAdc/edit?usp=sharing

Internet Archive! https://archive.org/
Petabytes of data! The TV Archive! The TV News Archive!
Recording TV, cable news, Philadelphia local news, CSPAN (people LOVE it).
There's an API written in Python 
Clip-based metadata storage. "This clip was fact-checked, this clip is a politlcal ad"
Check it out: https://archive.org/details/tv
What is in the data? VIDEO / AUDIO / CAPTIONS / but also information about… PROGRAM / CONTEXT / AUDIENCE
Not all of this data is easy to grab but each have signals where data can be pulled from. 
[ see excellent slide with detailed examples for each ]
How can we use these signals to provide more information?
Speaker diarization / who is talking?
Experimentation at the Internet Archive:
They want to enable experimentation as a library, not necessarily do it (but they do it too)
Example: Political TV Ad Archive (https://politicaladarchive.org)
Frequency analysis, turning sound into a hash and easily searchable. FIngerprinted each political ad and found all other copies with that ad.
Example: Face o matic http://tv-research5.us.archive.org:8000/auth
Recording in real time, 4 hours to convert into mp4 and other things, run through an algorithm that "doesn't take much time at all" 
This is a prototype: What do YOU want to use it for? What format would you like this in?
Example output in #face-o-matic on hyperaudio slack
Example: Chyron Extraction Extracting the "lower thirds" and how do they compare? That will be discussed tomorrow*

The Vision: What's happening on TV? What's all the metadata associated with what's happening? They don't have a great API for these things but want to use Sockets to push things out.
Be able to look historically, last month, etc.
INTERNET ARCHIVE IS A LIBRARY! Dan wants to make sure you know this. ← it’s true.

Question: 
Can you add more data to the archive? How can submitters use all this cool stuff?
"Good question." 
"Reach out to me, basically." → DAN @slifty SCHULTZ 
"We should talk" dan.schultz@archive.org everyone talk to him!