`winput` is a simple python script that aims to emulate the effect of Compiz plugin [Put](http://wiki.compiz.org/Plugins/Put) for a non-compiz windows manager (like `metacity`, i.e. Ubuntu 2D), or `Win-Left`, `Win-Right` behavior in terms of Microsoft Windows 7. It uses `wnck` python package, which can be installed in Ubuntu 12.04 via:

    sudo apt-get install python-wnck

Usage Example:
    
    ./winput left   # put current window to the left half of the screen
    ./winput right  # put current window to the right half of the screen

The script currently does not handle screen margins (like the task bar) very well, and it does not identify multiple screen settings either. It is quite easy to change the script to fit your own use though. If your system uses `compiz`, i.e. Ubuntu 3D, it is recommended to use the Compiz/Put plugin, which handles margins and multi-screens, and is also usually faster. If your system uses `metacity`, i.e. Ubuntu 2D, this script could be a handy helper.

Tip: in Ubuntu, you can bind custom global shortcut keys to commands in "Keyboard->Shortcut" settings.
