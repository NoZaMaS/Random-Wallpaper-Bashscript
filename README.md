### Random-Wallpaper-Bashscript
Small script done under bash to set a random wallpaper from a given directory and setting a colorscheme from it thanks to pywal

Requires pywal beforhand. Any status bar or wallpaper daemon should do the trick (do make the needed changes)

### Script

`#!/bin/bash

#replace swww with whichever wallpaper daemon you use and its respective arguments
#same goes for waybar
#I mean I'm not your mom, I shouldn't have to tell you that kind of stuff
#don't download random bashscripts from github, you'll catch weird things
#mine is fine though, or it should be, at least :)

randomfile=$(find "set wallpaper directory path" -type f | sort -R | head -1)

swww init
swww img $randomfile
wal -i $randomfile 
killall waybar
waybar`

### Demo
https://youtu.be/rlEPbRJVWPI
