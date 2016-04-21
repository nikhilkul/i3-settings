# i3-settings

Key features:

1. Locks using $mod+l.

2. Blurred lock screen instead of the normal plane white.

3. Media keys like Volume Up, Volume Down, Brightness control work like normal.

Tested on Lenove ThinkPad L450. 20 April 2016.

Install folllowing requirements before cloning.

```
sudo apt-get install scrot
sudo apt-get install xautolock
sudo apt-get install pulseaudio
sudo apt-get install xbacklight
sudo apt-get install imagemagick
```

Move fuzzy_lock.sh using
`sudo mv fuzzy_lock.sh ~/.local/share/fuzzy_lock.sh`

Move i3 config using
`sudo mv config ~/.i3/config`

Allow execution access to fuzzy_lock
`sudo chmod a+x ~/.local/share/fuzzy_lock.sh`

Now, Refresh i3 using $mod+shift+r 

Test using $mod+l.

Also, your Media keys should work (Volume and Brightness) 


