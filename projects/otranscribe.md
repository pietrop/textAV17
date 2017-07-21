# oTranscribe // Elliot Bentley, WSJ



Available → here http://otranscribe.com/
Created out of passion and perceived need by journalists
90,000 monthly users
“Low tech solution to a common problem”
UX is important! OSS software tends to be developer-focused or assume the user wants to engage/learn but tried to strip out as many features as possible from oTranscribe. "Should I add Markdown? No, the average journalist doesn't know what that is."
Does not currently streamline to video subtitles/captioning
Open source, refactoring helped bring in more PRs
22 Languages- Crowdsourced.

WebAv // Alex Norton, BBC News Labs - Slides: https://goo.gl/d78keM 
BBC Kaldi -- open source framework trained on audio using BBC’s extensive archive

“Transcriptor” retrieves transcripts from BBC production system
Automated transcripts don’t need to be perfect to be useful
“Octo” for transcript-based editing
Components:
Transcript model for representing speaker, segment, word https://github.com/bbc/transcript-model/
Transcript editor https://github.com/bbc/transcript-editor
