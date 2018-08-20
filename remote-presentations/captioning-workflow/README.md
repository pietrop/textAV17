# Captioning Workflow

{% embed data="{\"url\":\"https://www.youtube.com/embed/62cCMPpgfRU\",\"type\":\"video\",\"title\":\"A Captioning Workflow\",\"description\":\"This video demonstrates a few examples of how to speed up the captioning process.\\n\\nThere are four steps in this workflow: \\n1\) Generating a \\\"Raw Transcript\\\", \\n2\) Editing the Transcript\\n3\) Segmenting and Aligning the Transcript\\n4\) Checking the Accuracy of the Captions File\\n\\nHelp us caption & translate this video!\\n\\nhttp://amara.org/v/8ixU/\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/62cCMPpgfRU/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/62cCMPpgfRU?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/62cCMPpgfRU?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

As presented at the event

{% embed data="{\"url\":\"https://www.youtube.com/embed/ofQyatB0t1I\",\"type\":\"video\",\"title\":\"2017 07 20 12 00 09\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/ofQyatB0t1I/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/ofQyatB0t1I?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/ofQyatB0t1I?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

## Brief description

This captioning workflow is an attempt to eliminate common pain points: generating a transcript, segmenting the transcript, and aligning the transcript with the audio.

We are interested in an open-source, accessible application that can integrate all of the steps in our existing workflow. See our "Needs for A Captioning Tool" document for more specifics.

## Context

Our work is in disability services in Higher Ed \(California Community Colleges and NYU, respectively\). We are required to create captioned videos per section 508 of the Rehabilitiation Act. Many of colleagues are looking for methods to reduce cost and labor in the captioning process.

## Stage of production:

We have created bash scripts that automate common steps in the captioning process. Script \#1 is for getting a "raw transcript" from the YouTube auto-captions track \(we use youtube-dl and Aeneas and Sed\). Script \#2 is for segmenting the edited transcript so that we have "caption-ready" chunks that conform to the DCMP's recommendations of quality captions. In Script \#2, we also align the segmented transcript with the video via Aeneas, a Python library by Alberto Pettarin.

## Roadmap

We plan to dialogue with developers in the hopes of creating an application that includes all the steps in our captioning workflow \(i.e., transcription, editing, segmenting, aligning, fine-tuning\) as we described in our "Needs for a Captioning Tool" document.

This application must be accessible to individuals with disabilities per WCAG 2.0 AA guidelines.

## Vision

The goal is to have a partnership with eager developers who see accessible design as a priority. We also would like to provide substantial documentation that can be easily followed by people without a high level of technical expertise.

On the technical level, we hope to partner with a developer who can integrate Kaldi STT in the application because it is 1\) open source and 2\) amenable to customization \(use of speech models\).

## Any blockers?

Our preferred STT tool at the moment is YouTube, which has limitations: 1\) not every video uploaded will receive an auto-captions track. 2\) foreign language videos may have poorer WER on YouTube compared to English videos. 3\) Our use of scripts is not practical for people in our field who lack command of CLI tools. In addition, our scripts have been used primarily on the macOS and would require installation of UNIX commands on a PC \(we recommend installing Git Bash\).

## Components

We have shared our scripts at our GitHub site and we welcome any feedback. We are not developers and anticipate more efficient and economical ways of achieving the same end.

## Vision

> I wish that the editing step in this workflow were faster. If I had an interface like oTranscribe but with time-codings, that would make the process faster.

## Github repo if available

_Github repo for the project if open source_

[https://github.com/polizoto/segment\_transcript](https://github.com/polizoto/segment_transcript)

[https://github.com/polizoto/auto\_captions\_dl](https://github.com/polizoto/auto_captions_dl)

## Demo Video

[https://youtu.be/62cCMPpgfRU](https://youtu.be/62cCMPpgfRU)

## Website

www.htctu.net

## List of Stack used

Python, Perl, UNIX

## Contributors list

Joseph Polizzotto \(HTCTU\) jpolizzotto@htctu.net

Marshall Sunnes \(NYU\) ms9513@nyu.edu

