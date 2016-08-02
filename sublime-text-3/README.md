# Sublime Text 3 Sync

## Platform Note
For Linux:
	copy the whole Sublime Text 3 folder to ~/.configure
	
For Windows:
	only copy the folder "Sublime Text 3/Pakcages/User" to "$USER/appdata/Roaming". As syncing the packages accross different platforms has differnt version. Therefore let package manager to synchrounize the packages and it read the installed packages list from Control.sublime-settings.

## Packages:

### SublimeLinter-contrib-clang:
A C/C++ Lint based on clang.


clang required 
```sh
$ sudo apt install clang
```
	
### SublimeRtags
A tools can navigate symbol reference for c/c++


RTag is required https://github.com/Andersbakken/rtags