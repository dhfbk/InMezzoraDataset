# InMezzoraDataset

The corpus includes the transcripts of **56 TV face-to-face interviews for a total of 14 hours, taken from the Italian political talk show [Mezz'ora in più](https://it.wikipedia.org/wiki/%C2%BD_h_in_pi%C3%B9) broadcast from 24 September 2017 to 14 January 2018 on Rai 3 channel**. The show follows a fixed format, with interviews conducted by a journalist, **Lucia Annunziata**, to a guest, typically a prominent figure in the political or cultural scene (such as _Matteo Renzi, Luigi Di Maio, Pierluigi Bersani, Walter Veltroni, Alessandro Di Battista, Angelino Alfano, Matteo Salvini, etc._). The audio signal has been transcribed using a semi-supervised speech-to-text methodology (Google API + manual correction). Annotation has been done using XML as markup language and following the [TEI standard for Speech Transcripts](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/TS.html) in terms of utterances. **The linguistic resource has currently 100,870 tokens.**

For each interview the following information was manually annotated and is included in the XML resource file:

1. `metadata`: these include useful information for the rapid identification of transcriptions, for example the tools used for the transcription, a link to the interview, the owner account, the title of the talk show, the date of airing, the guests, etc.

2. `pause`: this tag is used to mark a pause either between or within utterances. Speakers differ very much in their rhythm and in particular in the amount of time they leave between words, so the following element is provided to mark occasions where the transcriber judges that speech has been paused, irrespective of the actual amount of silence;

3. `vocal`: with this tag we mark any vocalized but not necessarily lexical phenomenon, for example non-lexical expressions (i.e. burp, click, throat, etc.) and semi-lexical expressions (i.e. ah, aha, aw, eh, ehm etc.);

4. `del`: phenomena of speech management include false starts, repetition, and truncated words included in the transcription, but marked - in the TEI Guidelines - as editorially deleted and therefore indicated with the tag del; 

5.  `overlap`: this phenomenon is present when the speaker conveys (in a verbal or non-verbal manner) that he/she is about to finish his/her turn and the co-locutor starts speaking so that there is a slight overlap of utterances. 

## Data

- the folder "`txt-speeches`" contains transcriptions of every single interviews in plain text without tags

- the folder "`xml-complete`" contains annotated trascriprions of single TV show episode 

- the folder "`xml-speeches`" includes transcriptions of single annotated interviews 
