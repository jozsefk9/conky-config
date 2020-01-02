# conky-config

This my conky config. It is intended to be run on Manjaro and other Arch-based distros that use the pacman package manager.

On the left side, it shows the status of my servers, my disk usage (and IO read/write), and the local IPv4 as well as the current down- and upload usage for each interface (if the interface has a local IP).<br>
The server status will only be displayed if a file exists at `~/.config/conky/show_servers` and if its content is `on`. This means, you can toggle the display of server status as follows:

Turn on:
```shell script
echo on > ~/.config/conky/show_servers
```

Turn off:
```shell script
echo off > ~/.config/conky/show_servers
# Or just delete the file
rm ~/.config/conky/show_servers
```

On the right side, it shows general system details, the battery status (which can be removed if you're using a desktop), CPU details, memory details and how many updates from official repos and the AUR are available.

Requirements:
- **conky** ~~(what? a config for conky need conky? impossible.)~~
- **yay** (optional, for reliable update checking on Manjaro, Arch, and other pacman-using distros. Can be replaced with checkupdates and checkupdates-aur respectively, but I've found these to be quite unreliable on my systems.)

All files are intended to be located at ~/.config/conky/. If you want a different path, you will have to change it in each file.

![screenshot](screenshot.png)
