# Arne Eigenfeldt's RSynthBOT #

[Mac executable and audio samples](https://www.sfu.ca/musebots/Musebot_Test_Suite/Musebots/Melody_generators/ae_RSynthBOT.zip)

[Win 32 executable and audio samples](https://www.sfu.ca/musebots/Musebot_Test_Suite/Musebots_Win32/Melody_generators/ae_RSynthBOT_w32.zip)

[Win 64 executable and audio samples](https://www.sfu.ca/musebots/Musebot_Test_Suite/Musebots_Win64/Melody_generators/ae_RSynthBOT_w64.zip)

## version ##

06.21.15

## instrumentation ##

A smart synth bot that generates a rhythmic monophonic synth part using a corpus of 50 Breaks tracks.

type:

      @synth
      @melodic

## platform ##

Max standalone, built from Max 6.1.8 on Macintosh.

## behaviour ##

Creates its own form - # of phrases, and whether to play in those phrases. Synth patches will vary with each appearance.

## messages ##

sends:

      @notepool (pitches used by synth in current measure);
      @tala (additive rhythm of 2 & 3);
      @phraselength (# of measures in phrases);
      @exiting - when it finishes its form, it will exit in the next phrase, and send this message.

receives:

      @tala (additive rhythm of 2 & 3);
      @phraselength (will generate its own at load, but incoming value will replace it);
      @phrases (number of phrases in form: will generate its own, but will converge on received phrases);
      @plan/chordDuration (will generate its own, but incoming plan will replace);
      @plan/chords (will generate its own, but incoming plan will replace);
      @exiting (will exit when other bots send this message).

## license ##

Creative Commons Share Alike

## credits ##

arne eigenfeldt (June 2015)