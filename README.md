PiFMPlay
========
Its an addon for pifm(a program to transmit FM-Radio) for the raspberry pi mini computer.

PiFMPlay makes it easier to play music and control your FM-Broadcast.

PiFM is written by [Icrobotics](http://www.icrobotics.co.uk/wiki/index.php)

PiFMPlay is written by Mikael Jakhelln.
"It's not pretty, but i works."

This is a forked version of Mikaels PiFMPlay with solved bugs and a .deb to make it more noob friendly.

##How to use it:
Step 1 (optional for manual install):
Put pifmplay on your pi (e.g /home/pi).

Step 2 (optional for manual install):
Allow it to be run as a program:
>sudo chmod +x pifmplay

>sudo chmod +x pifm

Step 1 (.deb alternative):
Download pifmplay.deb and run
sudo dpkg -i pifmplay.deb

Step 3:
Install sox and ffmpeg with:
>sudo apt-get install ffmpeg sox libsox-fmt-all 

Attach an antenna to GPIO4 on your raspberry pi.

###Test it:

>sudo pifmplay . 91.3

(88.0 is the default frequency, change it to whatever frequency you want to broadcast on.)

###Play a file with:

>sudo pifmplay "/path/to/file.mp3"

>sudo pifmplay "/path/to/file.m4a"

>sudo pifmplay "/path/to/file.wav"

this will play a file with pifm.

###Play a folder with:

>sudo pifmplay "/path/to/folder" 101.5

(this will play all files in the specified directory with pifm on frequency 101.5)

###How to Pause/Stop broadcast and skip songs:
Open another terminal.

>sudo pifmplay pause

>sudo pifmplay resume

>sudo pifmplay stop

>sudo pifmplay next

To control pifmplay from the same terminal, run pifm in the background:
>sudo pifmplay "/path/to/folder" &
(tho you might want to remove the text output)

####If you get in troube using this, IT'S ON YOU:
The raspberry pi can be made into a powerful fm-transmitter, if you filter and amplify the signal. 
But using a powerful fm-transmitter without a proper licence is illegal in most countries.
So if you break any laws and get fined for it, it's YOUR OWN FAULT!!
But it should be fine as long as you don't attach a big antenna to it.
