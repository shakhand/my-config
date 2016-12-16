# Sublime Text 3 Sync
## How to port this configuration to your OS
**Linux:** copy the whole Sublime Text 3 folder to ~/.configure

	
**Windows:** only copy the folder "Sublime Text 3/Pakcages/User" to "$USER/appdata/Roaming". As syncing the packages accross different platforms has differnt version. Therefore let package manager to synchrounize the packages and it read the installed packages list from Control.sublime-settings.

## Packages:

### [SublimeLinter-contrib-clang](https://github.com/nirm03/SublimeLinter-clang)
A C/C++ Lint based on clang.


plugin [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter3) is required

clang required 
```sh
$ sudo apt install clang
```
	
### [SublimeRtags](https://github.com/rampage644/sublime-rtags)
A tools can navigate symbol reference for c/c++


[RTag](https://github.com/Andersbakken/rtags) is required 

### [EasyClangComplete](https://github.com/niosus/EasyClangComplete)
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

### [SublimeAllAutocomplete](https://github.com/alienhard/SublimeAllAutocomplete)
Extends the default autocomplete to find matches in all open files


### [MarkdownEditing](https://github.com/SublimeText-Markdown/MarkdownEditing)
support Github Markdown and view the markdown file

### [ClangFormat](https://github.com/rosshemsley/)
Clang-format is a tool for re-formatting C++, built on LLVM. This is a package that allows you to run it easily from within Sublime Text.[SublimeClangFormat)

### [DocBlockr](https://github.com/Warin/Sublime/tree/master/DocBlockr)
DocBlockr is a package for Sublime Text 2 & 3 which makes writing documentation a breeze. DocBlockr supports JavaScript (including ES6), PHP, ActionScript, Haxe, CoffeeScript, TypeScript, Java, Apex, Groovy, Objective C, C, C++ and Rust.

### [Open-Include](https://github.com/titoBouzout/Open-Include)
Open include file in c/c++

### [Sublime Function Name Display](https://github.com/akrabat/SublimeFunctionNameDisplay)
Show function name in status bar for c/c++

