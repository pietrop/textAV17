# Needs for a Captioning Tool

- July 17, 2017
- Joseph Polizzotto (HTCTU), Marshall Sunnes (NYU)

## General Needs

- major goal: offer a faster and simpler process for the creation of quality caption files (e.g., SRT files)
- open source tool
- accessible design ( WCAG 2.0 AA guidelines)
- Mac, PC, and Linux versions
- ability to save work in progress
- documentation and best practices (e.g., clarify that time-chunked items in "raw transcript" do not correspond to eventual caption blocks)

## Transcription (Step 1)

- Produce a "raw transcript" from an audio file (e.g., WAV, MP3, MP4, OGG, M4A, FLAC, RAW, WMA et al.) using Speech to Text (STT) systems.
- The optimal STT integration would include:
	- an open-source tool (e.g., Kaldi) 
	- ability to train models on speech data
	- off-line computation available

## Editing (Step 2)

- Edit the "raw transcript", which is time-coded to the audio, in a text editor window
- NICE TO HAVE: download auto-captions from YouTube
- The optimal text editor screen contains the following:
	- time coding of chunks at > word-level granularity (phrase or ~7 sec intervals)
	- NICE TO HAVE: speaker diarisation (group chunks into sections based on different speakers)
	- shortcuts for Play / Pause, Previous/ Next (chunk), Increase / Decrease speed
	- automatic adjustments to text (capitalization after full-stops, question marks, exclamation marks, ellipsis)
	- quick key for adding brackets around speaker identification and sound information (brackets, parentheses should be used to tell aligner not to consider this text for the purposes of alignment)
	- settings menu for user configuration:
		- playback stops when keyboard is activated (when editing begins)
		- customize keyboard shortcuts
		- adjust the size of segmented chunks; see step #3 (e.g., number of characters per line, number of lines per caption block)
		- add honorifics and abbreviations to ignore for segmentation step; see step #3 
		- adjust (optional) Aeneas parameters (other essential parameters will already be generated, such as input file types); see step #4
			- select output format (e.g., SRT, VTT, TTML, JSON)
			- Audio-head/tail length
			- Ignore non-speech sound minimum duration
			- save out addition HTML file (for fine-tuning syncmap)
			- see Aeneas docs for additional parameters, flags that could be added
	- NICE TO HAVE: RegEx find and replace

## Segmenting (Step 3)

- Segment now-edited transcript into chunks that meet quality captioning standards (http://www.captioningkey.org/quality_captioning.html)
	- e.g.,
		- lines should not exceed 35 characters per line
		- 1-2 lines per caption block
		- end-sentence punctuation always found at the end of a captioning block, not in the middle
- scripting could be done with perl or Natural Language Processing (NLP) libraries (NLTK, spaCy) to complete this step:
	- e.g., 
		- reference a database of honorifics (Mr. Mrs. Fr. etc.) that will be ignored for segmenting purposes
		- place each sentence on its own line
		- break sentences into desirable chunks (see above)
		- add a space between each chunk (for purposes of alignment with Aeneas "subtitle" format; see step #4)
- NICE TO HAVE:
	- review/edit screen for segmented chunks
	- preset segmenting settings based on previous projects
		
## Aligning (Step 4)

- Align the segmented transcript with the audio using forced alignment tool (e.g, Aeneas) and output to desired syncmap format (e.g., SRT, TTML, VTT, SBV etc.)
- Optimal use of the aligner will include:
	- Python C, and CEW extensions are compiled on PC, Linux, and Mac
	
## NICE TO HAVE: Checking/Fine-Tuning (Step 5)
- Review results of syncmap file (e.g., SRT file) and correct for discrepancies in time-stamps and export correct syncmap
- Optimal use of the fine-tuning tool (see https://github.com/ozdefir/finetuneas for example; also comes in "Third Party" directory in Aeneas package) will include:
	- increase/ decrease speed
	- toggle time-stamp display format
	- save in multiple formats
- Note: some audio files with variable bit rate manifest unpredictable behavior in web browsers (consider adding a note on this Fine-Tuning window)

	


	
	