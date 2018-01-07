# Distro_Conky
I found this conky and modified it to my linking and need (compute spec.)
I added a google calendar and a clock so this conky folder got 3 ./conkyrc_mint ./conkyrc_mint_agenda ./conkyrc_clock ./conky/clock_ring.lua ./conky/gcal.sh and Mint.png

./conkyrc_mint => main conky script
./conkyrc_mint_agenda => this will need that gcalcli is install in your computer to work (this script launch ./conky/gcal.sh)
./conkyrc_clock => the clock (this script launch ../conky/clock_ring.lua)

To install this conky configuration file extract the archive into your home directory.  No fonts have been provided, but are easy enough to find and install, and chances are most of them are already installed.  Following is a list of fonts used:
Ubuntu
Ubuntu Mono
PizzaDude Bullets
Neuropol

If any of these fonts needed to be installed just copy them to "~/.fonts".  This may require you to update your font cache.  If so, use the following command:
sudo fc-cache -fv

you will nedd to install Google Calendar python script gcalcli (Check your OS distribution for packages.) source: https://github.com/insanum/gcalcli

Included in this archive are several conky files and a folder with script sh, lua etc..  For those who prefer a minimum of setup follow these steps:

1- extract distro_conky folder to home directory ~/.conky
2- create file conky.desktop in ~/.config/autostart folder
3- open terminal and type:	gedit ~/.config/autostart/conky.desktop
4- paste this code into the file and save it

[Desktop Entry]
Type=Application
Exec=$HOME/.conky/distro_conky/.autostart-conky
Hidden=false
NoDisplay=false
X-GNOME-Autostart-enabled=true
Name[en_IN]=Conky
Name=Conky
Comment[en_IN]=start conky script

As with any conky, your mileage may vary and some end-user configuration may be required.  It works for me, and with a little work it can work for you too.  It was designed for for (1080 heigh desktop; but it should work with larger resolutions as well.

You have my permission to use, modify, and distribute this archive as a whole as you see fit.  All I ask is that you give credit where it is due.  Also, I would love to see any modifications so please contact me if you think your changes are better than what I came up with.

I hope you enjoy!

fragargon
https://github.com/fragargon?tab=repositories

# pictures

![Alt Text](https://github.com/fragargon/conky/raw/master/images/conkyrc_mint.png)
![Alt Text](https://github.com/fragargon/conky/raw/master/images/conkyrc_mint_clock.png)
