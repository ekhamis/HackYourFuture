
# Command line 

The command line (cli, shell) is the interface between you (the user) and the operating system which interprets your commands and allows the computer to respond to your command. 

# Filesystem 
Think of the filesystem as a tree starting with a special directory called the root which is the top of the tree - this is referred to as `/`. Every other directory is a child of this directory. 
```
                       /
                       |
 something          users      apps
                       | 
            timir   unmesh  gijs
            /
        projects
        /
    python
```
My `home` directory in this case is `/users/timir` so when I type `cd` (with no arguments)  

# Commands
## Navigating the filesystem 
`ls` - show the contents of the directory. `ls -a` will show all hidden files. 

`pwd` - print the working directory. What directory am I in? 

`cd` - change directory to the one specified. If no directory is specified this will take you to your home directory. Remember that `.` is the current directory and `..` is the parent directory. So `cd .` changes the directory to the current directory (does nothing!). 

`cat` - print the contents of the file - this will print the the WHOLE file. If you want to stop printing after a full screen use the below command 

`more` - show one screen full of the file (spacebar moves forward and <ESC> stops printing)

`head` - show the beginning of a file e.g. `head -3` shows the first 3 lines of the file

`tail` - show the end of a file `tail -4 shows the last 4 lines of the file

`wc` - show the word count of a file (prints lines, words, characters)

`CTRL-c` - stop what is happening on the command line 

`CTRL-z` - hard stop what is happening on the command line 

`mkdir` - create a new directory

`touch` - create an empty file

# vim
vim is an editor (like notepad on windows)
Sometimes it is a little hard to remember all the vim commands so here is a handy cheatsheet: https://www.fprintf.net/vimCheatSheet.html - with practice it will not seem so odd. 

`vim <filename>` will open a file in vim
When you are in vim there are two modes:
1. Insert mode - in this mode you can enter and change text
2. Command mode (also called escape mode) - in this mode you can issue commands to vim

When you are in vim `a` and `i` will put you in insert mode and `esc` will take you our of insert mode. If you get stuck in vim press `esc esc` (yes, twice) and then `:q` and this will take you back to the shell. Some commands we covered: 

`a` = Go to insert mode

`<ESC> :q` = quit file 

`<ESC> :wq` = save file and quit vim

`<ESC> :q!` = exit vim without saving

`<ESC> yy` = copy current line (the line you are on)

`<ESC> p` = paste what you last copied

Many commands can be preceeded by a number to repeat their action. For example, `<ESC> 4yy` copies 4 lines starting from where you entered the command. 
