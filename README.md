# i3-settings
**i3** is a tiling window manager and one of the better productivity tools for linux.
**i3** has transformed my developer setup and I believe it should be a goto window manager on linux platform for everyone.

Making some of my settings public.

## QuickStart

**Key features :**

1. Locks using $mod+l.

2. Blurred lock screen instead of the normal plane white.

3. Media keys like Volume Up, Volume Down, Brightness control work like normal.

Tested on Lenove ThinkPad L450. 20 April 2016.

**Installation steps :**

Open Terminal (Windows key + Enter )

Type
`crontab -e`

And add this line at the bottom of the file 
`*/1 * * * * /HOMEPATH/.i3batwarn.sh`

Now install following packages using teminal.

```
sudo apt-get install scrot
sudo apt-get install xautolock
sudo apt-get install pulseaudio
sudo apt-get install xbacklight
sudo apt-get install imagemagick
sudo apt-get install blueman
```

*Now we need to move some files.*

Clone the repository using 

`git clone https://github.com/nikhil2kulkarni/i3-settings.git`

Go to the cloned repository using 

`cd i3-settings`

Move fuzzy_lock.sh to appropriate PATH using

`sudo mv fuzzy_lock.sh ~/.local/share/fuzzy_lock.sh`

Move my i3 configuration file to HOME PATH using

`sudo mv config ~/.i3/config`

Move i3batwarn.sh to HOME using

`sudo mv .i3batwarn.sh ~/.i3batwarn.sh`

Allow execution access to fuzzy_lock

`sudo chmod a+x ~/.local/share/fuzzy_lock.sh`

$mod => Windows key by default.

Now, Refresh i3 using $mod+shift+r 

Test using $mod+l.

Also, your Media keys should work (Volume and Brightness)
