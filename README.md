HTML-Editor is a set of HTML/XHTML mappings (macros) and menus for Vim 6 or later. The mappings will be local to the buffer so they won't interfere if you edit other files in the same vim session.

# Installation #
First you should put `filetype plugin on` in your vimrc. 

## Automatic installation: ##
Using [Vundle](https://github.com/gmarik/vundle), add the following to your `vimrc` then run
  `:PluginInstall`

        Plugin 'yyq123/HTML-Editor'

## Manual installation: ##
Put "HTML.vim" in your `ftplugin/html` subdirectory somewhere in your `runtimepath`, then install the files below that you want. 

### Documentation: ###
- HTML.txt
Place it in the doc subdirectory somewhere in your `runtimepath` (~/.vim/doc for Unix) and run `:helptags <directory>/doc`. Then you'll be able to do `:help HTML.txt`. 

(You can view the documentation [here](https://github.com/yyq123/HTML-Editor/blob/master/doc/HTML.txt).)

### GUI Toolbar Bitmaps: ###
Put files in the bitmaps directory somewhere in your `runtimepath` (~/vim/bitmaps for Unix).

### Browser Launcher (for Unix/Linux): ###

- browser_launcher.vim
Put browser_launcher.vim in one of the toplevel directories in your `runtimepath` (such as ~/.vim for Unix). 

- netscape-remote
This file is used by browser_launcher.vim and is optional—it will fall back to just using netscape/mozilla/firefox instead. To use it just ompile it and put the binary somewhere in your $PATH. 

(This version is slightly tweaked by me. The original can be found at  http://wp.netscape.com/newsref/std/x-remote.html.) 


### Auto-Update Image Tag Size Attributes: ###
- MangleImageTag.vim
If this file is placed in one of the toplevel directories in your `runtimepath` it will cause the ";mi" mapping to be defined. (See the warning under `:help ;mi`.)

### References: ###
- [Character Entity Reference HTML](https://dev.w3.org/html5/html-author/charref)
