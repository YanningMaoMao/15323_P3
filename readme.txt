File : readme.txt
Author : Yanning Mao (yanningm)
Date : Feb 15, 2018
Course : CMU 15-323 S18

--- About the program ---:

This folder contains the code for a real-time program that outputs music using MIDI and generates animation according to the music being played.

The music being played consists of four independent sound tracks, and can be extended to any number of sounds tracks. Although all tracks as a whole are controlled by a universal tempo, each sound track has its own rhythm, own sound effect, and own set of pitches. The rhythm is randomly generated, and the next pitch to be played is randomly selected from the set of pitches.

The canvas displays an animation that corresponds to the music being played. Each sound track is represented by a horizonal line segment. The color of the segment becomes more red when the volume is larger, and the horizontal position of the segment becomes higher when the pitch rises.

--- About the content of the folder ---:

The folder contains the following file:
+ readme.txt
+ main.srp : the main() function
+ canvas.srp : the MusicCanvas class that subclasses Canvas
+ choir.srp : the Choir class that represents the entire music
+ track.srp : the Track class that represents each sound track
+ constants.srp : the constants and libraries used by the program
And the following source files:
+ debug.srp
+ sched.srp
+ wxserpent.srp
+ midi-io.srp
+ prefs.srp
+ mididevice.srp
+ slider.srp
+ prob.srp

--- How to run the program ---:

1. In a terminal, cd into the folder
2. Open output device
3. Run "wxserpent64 main.srp"

--- How to use the GUI ---:

+ The slider labeled "Period" controls the tempo of the music
+ The button labeled "Start All" starts all tracks
+ The button labeled "Stop All" stops all tracks
+ The slider labeled "Sound x Velocity" controls the volume of the sound track (the color of the corresponding segment changes as you adjust this slider)
+ The button labeled "Stop" stops the corresponding track
+ The button labeled "Start" starts the corresponding track
+ The button labeled "Octave Up" raises the pitches of the track by one octave if possible (the level of the segment will jump higher)
+ The button labeled "Octave Down" lowers the pitches of the track by one octave if possible (the level of the segment will jump lower)





