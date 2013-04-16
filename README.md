`winput` is a simple python script that aims to provide the basic functions of 
Compiz plugin [Put](http://wiki.compiz.org/Plugins/Put) for a 
non-compiz windows manager (like `metacity`, i.e. Ubuntu 2D), 
The Compiz/Put plugin enables the user to position and resize the currently active window to
several preset positions, like the left or right half of the current screen. The effect is very similar to
the behavior of pressing `Win-Left`, `Win-Right` keys in Microsoft Windows 7. 

The script requires `wnck` python package, which can be installed in Ubuntu 12.04 via:

    sudo apt-get install python-wnck

Usage Example:
    
    ./winput left   # put current window to the left half of the screen
    ./winput right  # put current window to the right half of the screen

The script currently does not handle screen margins (like the task bar) very well, 
and it does not identify multiple screen settings either. 
It is quite easy to change the script to fit your own use though. 
If your system uses `compiz`, i.e. Ubuntu 3D, it is recommended to use the Compiz/Put plugin instead, 
which handles margins and multi-screens, and is also usually faster. You can find that in `ccsm`,
which can be installed by `sudo apt-get install compizconfig-settings-manager`.
However, if your system uses `metacity`, i.e. Ubuntu 2D, this script could be a handy helper.

Tip: in Ubuntu, you can bind custom global shortcut keys to arbitary commands in "Keyboard->Shortcut" settings.
