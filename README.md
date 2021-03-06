# AudioCue

**AudioCue** is a new Java resource for playing back sound files, 
designed for use with game programming. 

## Why?

Java's **Clip** class (_javax.audio.sampled.Clip_) was not built 
with game programming needs in mind. The class has a tricky, 
non-intuitive syntax and a limited feature set. A _Clip_ cannot
be played concurrently with itself, can only be played at its 
recorded pitch, and the _Control_ class provided for real time
changes such as panning and volume is system-dependent upon
implementation and limited by only allowing changes at buffer 
increments. 

**AudioCue** addresses these issues:

* ### Easy to Use
  * Very light: Download or copy/paste five class files from GitHub directly into your project.
  * Syntax is simpler than Java's _Clip_ class.
  * API and demonstration programs provided.
* ### Powerful
  * Runs directly on Java's _SourceDataLine_.
  * Allows concurrent playback of cues.
  * Allows  playback at varying speeds.
  * Real-time volume, panning and frequency faders.
  * Highly configurable.
  * Messaging system for coordination with graphics.
* ### BSD License (open source, free, donations greatly appreciated)
* ### Now includes *AudioMixer* for consolidating AudioCues into 
a single output line.

## Installation

AudioCue requires five files:
* [AudioCue.java](https://github.com/philfrei/AudioCue/blob/master/com/adonax/audiocue/AudioCue.java)
* [AudioCueInstanceEvent.java](https://github.com/philfrei/AudioCue/blob/master/com/adonax/audiocue/AudioCueInstanceEvent.java)
* [AudioCueListener.java](https://github.com/philfrei/AudioCue/blob/master/com/adonax/audiocue/AudioCueListener.java)
* [AudioMixer.java](https://github.com/philfrei/AudioCue/blob/master/com/adonax/audiocue/AudioMixer.java)
* [AudioMixerTrack.java](https://github.com/philfrei/AudioCue/blob/master/com/adonax/audiocue/AudioMixerTrack.java)

In addition, there are two optional file folders with demo content and resources used by the demo programs:
* [supportpack](https://github.com/philfrei/AudioCue/tree/master/com/adonax/audiocue/supportpack)
* [supportpack.res](https://github.com/philfrei/AudioCue/tree/master/com/adonax/audiocue/supportpack/res)

Installation involves copying and pasting the five files into your 
program.

* Method 1) navigate to, then copy and paste the five files
directly into your program.
* Method 2) download and unzip [audiocue.zip](http://adonax.com/AudioCue/audiocue.zip), which holds
these five files, into your project.
* Method 3) download [audiocue.jar](http://adonax.com/AudioCue/audiocue.jar), 
which includes source code, the "supportpack" and "res" content, 
and import into your IDE.
[NOTE: I'm not clear if the .jar file, which I generated from Eclipse, 
will import into other IDEs.]

