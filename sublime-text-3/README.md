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

### EasyClangComplete
complete your code with clang

configure example:
```json
"settings":
{
		"clang_flags": ["-D_GNU_SOURCE -D__STDC_CONSTANT_MACROS -D__STDC_FORMAT_MACROS -D__STDC_LIMIT_MACROS -Wall -Wextra -Wpointer-arith -Wnon-virtual-dtor -fno-rtti -std=c++11 -Wstrict-aliasing=2 -Wcast-qual -fPIC -fstack-protector-all -Wstack-protector -O3 -DNDEBUG"],
		"include_dirs": [
	                "${project_folder}/src",
	                "${project_folder}/src/rct",
	                "${project_folder}/build/src/include/rct",
	                "${project_folder}/build/src/include/",
	                "/usr/lib/llvm-3.8/include"
	            ],
		"search_clang_complete_file": "${project_folder}/"
}
```

### SublimeAllAutocomplete
Extends the default autocomplete to find matches in all open files
https://github.com/alienhard/SublimeAllAutocomplete