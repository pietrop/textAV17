# Captioning workflow system/app


Captioning workflow system based on the [Captioning workflow](/remote-presentations/captioning-workflow.md) presentation by Joseph and [notes](/remote-presentations/captioning-workflow/needs-for-captioning-tool.md). 

## R&D approach 

Thought it be good to give a quick high level overview of the methodology we used to quickly prototype this. 

We followed an R&D approach to size and explore the problem. 

First step is to identify, learn, and understand a possible workflow. This was an unusual project in that a lot of the ground work of this was already done by Joseph's [Captioning workflow](/remote-presentations/captioning-workflow.md)

But once you have the workflow figured out, then divide the it into parts. Of those parts identify the granularity of what are the components that make up that part.

For those components are find out  which once you have available and to what degree you are familiar with their workings.  

As well as which once you don't know.

Priority  is given  to the once you don't know to verify how they work and whether they make the whole possible.

Once you have all the components you look at the interfaces and the communication between that, do you need to do any conversion or adjustment eg to get the output of one as input of the other etc..  This also helps you to think about data models representations that are most suited for the overall system.


This allows to work on parts and components in isolation and then combined them. 
Don't leave the combining and integration experiments too late tho because sometimes they are just as important as the building blocks.

Threat everything as an hypothesis and prioritise which one to test first.

## Sections


![Captioning workflow](/assets/captioning_workflow.png)



<img src="https://docs.google.com/drawings/d/e/2PACX-1vTI-q9lNWreAGw-piKQ5XdYKH_7g4mp3tITypsW0aNrW2WbNe4M_WhqBSNMNOAlxuoX6YTSwST39COr/pub?w=2039&amp;h=704">

[See same diagram above in google diagrams](https://docs.google.com/drawings/d/1LWD2lEcOM42XbMAQ9bWemyP7bGuKxUWxQp9cfY0ckiU/edit?usp=sharing)


## Notes from Google doc R&D
[Google doc of R&D research of parts, and components](https://docs.google.com/document/d/1yrPSgLnGW4mWBXCHAxR0STzm--lpV_6nglcqhM8EkDc/edit?usp=sharing)





Trello card [https://trello.com/c/2aXrERbm](https://trello.com/c/2aXrERbm)  & [https://trello.com/c/MFpDrzFT](https://trello.com/c/MFpDrzFT) 

Joseph’s scripts 

[https://github.com/polizoto/segment_transcript](https://github.com/polizoto/segment_transcript) 

[https://github.com/polizoto/auto_captions_dl](https://github.com/polizoto/auto_captions_dl) 

Video of current semi automated workflow

[https://youtu.be/62cCMPpgfRU](https://youtu.be/62cCMPpgfRU) 

 

# Setup

Install dependencies with a script, eg Aeneas and its dependencies.

**TODO**: make script that installs Aeneas using brew

[https://github.com/readbeyond/aeneas/blob/master/wiki/INSTALL.md#via-brew](https://github.com/readbeyond/aeneas/blob/master/wiki/INSTALL.md#via-brew) 

# audio/video input

Audio and video files supported by ffmeg 

Ffmpeg supported format list: [https://github.com/pietrop/ffmpeg_formats_list](https://github.com/pietrop/ffmpeg_formats_list) 

# Convert to HTML5 media - audio 

For STT recognition.

→ Audio file need to have constant bitrate to avoid time drifting with word level recognition. - Joseph

Uses node fluent ffmpeg wraper.

**Component: **(from autoEdit) 

[https://github.com/OpenNewsLabs/autoEdit_2/blob/master/lib/interactive_transcription_generator/transcriber/convert_to_audio.js](https://github.com/OpenNewsLabs/autoEdit_2/blob/master/lib/interactive_transcription_generator/transcriber/convert_to_audio.js) 

The specs of the audio component 

**TODO: **Or could change that component convert to mp4, since electron supports that. 

# Convert to HTML5 media - video

For preview in text editor.

HTML5 media: webm, mp4, ogg.

**Component:** (from autoEdit) [https://github.com/OpenNewsLabs/autoEdit_2/tree/master/lib/interactive_transcription_generator/video_to_html5_webm](https://github.com/OpenNewsLabs/autoEdit_2/tree/master/lib/interactive_transcription_generator/video_to_html5_webm) 

# STT

Youtube? Other TBC? Kaldi? Watson? Google? Baidu?

**TODO**: do test with Baidu to see how accuracy ranks in Joseph’s list. 

**TODO**: same test with microsoft Bing Speech APi

# Text editor

Currently oTranscribe. 

→ Wrapping otranscribe electron?

[http://otranscribe.com/opensource/](http://otranscribe.com/opensource/) 

# Realignment - prep

Divide into smaller bits. Perl script. 

# Realignment - srt 

Aeneas get srt file.

**Component**: Metadata reader. 

Aeneas command needs to have the right audio file ending.

→ Aeneas, how to run inside electron?

Example of running 

```bash
aeneas_execute_task "$f".mp4 "$f" "task_language=eng|os_task_file_format=srt|is_text_type=subtitles|is_audio_file_head_length=12.000|is_audio_file_tail_length=6.000|task_adjust_boundary_nonspeech_min=1.000|task_adjust_boundary_nonspeech_string=REMOVE|task_adjust_boundary_algorithm=percent|task_adjust_boundary_percent_value=75|is_text_file_ignore_regex=[*]" "$f".srt --output-html
```


## User-control arguments

* task_language=**eng**

* os_task_file_format=**srt**

* is_audio_file_head_length=**12.000**

* is_audio_file_tail_length=**6.000**

## Constant arguments 

* is_text_type=**subtitles**

**$f **

task_language=**eng: **

**Creates audio file **

task_adjust_boundary_nonspeech_min=**1.000**: identifies areas of no speech. Value is minimum of seconds to include.

User settings menu would control these arguments.

Aeneas subtitles, one or more lines separated by space.

Documentation:

[https://www.readbeyond.it/aeneas/docs/index.html](https://www.readbeyond.it/aeneas/docs/index.html)

**System Requirements**

1. a reasonably recent machine (recommended 4 GB RAM, 2 GHz 64bit CPU)

2. [Python](https://python.org/) 2.7 (Linux, OS X, Windows) or 3.5 or later (Linux, OS X)

3. [FFmpeg](https://www.ffmpeg.org/)

4. [eSpeak](http://espeak.sourceforge.net/)

5. Python packages BeautifulSoup4, lxml, and numpy

6. Python headers to compile the Python C/C++ extensions (optional but strongly recommended)

7. A shell supporting UTF-8 (optional but strongly recommended)

Aeneasweb.org

learning ally

* * *


# Next Step TODO: 

* Installation script

* Pearl prep script rewrite 

* oTranscribe inside electron, and test

* Running Aeneas inside electron, from oTranscribe 

* * *


# Other / similar

[https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html)

[https://github.com/pietrop/electron-video-downloader](https://github.com/pietrop/electron-video-downloader) 

[https://rg3.github.io/youtube-dl/](https://rg3.github.io/youtube-dl/) 

