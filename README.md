# Microbit Auto Transfer

A short Python script to automatically transfer a Micro:bit hex file to a Micro:bit as soon as it has downloaded. Designed to run in the background on a Raspberry Pi using Python 2. 

# Usage

This program was designed to make using a Micro:bit and the ['Let's Code'](https://makecode.microbit.org/) block based web interface much easier for students! Instead of having to drag and drop the file every time they download it, it will automatically move itself across. 

DISCLAIMER: I am very much an amateur and I've written this for exactly what I use it for. It's probably not the best nor most efficient method to this, but it works for me.

# Set Up

The script uses mostly standard Python libraries and one additional one, 'Watchdog' 

Watchdog needs to be installed for Python 2, so DON'T use `sudo apt-get install`, instead use:

`sudo pip install watchdog`

The file also needs to be saved in the 'Downloads' folder on your Pi (or whichever folder you've designated as your downloads folder for your web browser).

Make sure to change the permissions on the file so that it can be excecuted, click on the file and away you go! It'll just run in the background and check for any new .hex files that may appear. 

# Additional Things

For my set up, I've also used a Downloads Manager in Chromium so that the bar on the bottom doesn't appear after a download is initiated. As well as that I've disabled the pop up window that appears when a new drive is connected, as it appears everytime a Micro:Bit has finished writing a finished file to itself, and it's quite annoying! You can do this in the File Explorer preferences, I used this [link](https://askubuntu.com/questions/474607/lubuntu-disable-removable-media-is-inserted-window) as guide. 

I've also got a small button box that our staff use at the end of a workshop to delete the files, mainly so they don't accidentally delete this file. 
