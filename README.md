# sway-alt-tab
Alt-tab functionalty. It switches between two containers. You select the container you would like to be able to switch to with Alt-Tab by holding down Alt and navigating to it. Only release the Alt key when you've found your desired container. The only exception is that you can use Alt-Tab directly without releasing the Tab and the second container ID will still be saved. 

# Setup

## 1. Sway Config

Add the following to your sway config file:
```
# For alt-tab functionality
bindsym --no-repeat Alt_R exec exec /script_location/alt-tab save
bindsym --no-repeat Alt_L exec exec /script_location/alt-tab save
bindsym --no-repeat $mod+Tab exec /script_location/alt-tab switch
```
For my system using `Mod1` directly doesn't work for this purpose. That's why I use Alt_R and Alt_L instead.
Change `script_location` to wherever you saved the script.

## 2. Download Script
Download the scrip and make it executable. 
