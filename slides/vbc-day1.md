%title: Vim Bootcamp - Day 1
%author: Brandon Schrader
%date 2018-03-11

-> # Welcome to Vim <-

-> *Edit text at the speed of thought* <-

^
* day 1 topics:
    ^
    - why vim
    ^
    - modes
    ^
    - efficient file navigation

^
* why did I start using vim?
    ^
    - needed to quickly and easily modify files in linux docker containers
    ^
    - i've always dabbled but became frustrated on the seemingly random editing commands
    ^
    - watched screencasts of people using it and tearing though code
    ^
    - research further to use it more efficiently and found a whole new way to edit text
    ^
    - now I'm down the rabbit hole looking to preach the gospel

---

-> # Why Vim? <-

*There are many reasons to use vim and no it's not because you can't figure out how to exit it*

* great community
    - lots of plugins
    ^
    - large support network
    ^
    - free
    ^

* portablility
    - runs on anything anywhere (windows, mac, linux, ssh, embedded, etc)
    ^
    - easy and fast to setup on current or new system, only a 14MB download
    ^
    - setting are all kept in plain text (dotfiles) which makes sharing and version control a breeze
    ^
    - a lot of the commands and actions are also used in a lot of other linux programs

* efficiency
    - modal operation leads to fast navigation and very powerful editing commands
    ^
    - learning one program for all your editing needs

---

-> # Why Vim? <-

*levels of text editing efficiencies*

simple examples of copying an existing line and pasting it to a new line underneath

^
* noob time
    ^
    - 1. take your paw off the keyboard and grab the mouse
    ^
    - 2. slowly and painfuly drag your cursor over the existing line or double click
    ^
    - 3. click the end of the line
    ^
    - 4. hit `Enter`
    ^
    - 5. right-click and select paste
    ^
    - 6. question your life choices
    ^

* normal modeless text editor (advanced keyboard shortcut commands)
    ^
    - 1. hit `Home` to get to beginning of line
    - 2. hold `Shift+End` to highlight to end of line
    - 3. `Ctrl+c` to copy
    - 4. `End` to de-highlight line
    - 5. `Enter` to insert line directly underneath current line
    - 6. `Ctrl-v` to finally paste in previous line 

^
* vim
    ^
    - 1. `yyp`

---

-> # Modes <-

*The four main modes of Vim*

^
* normal mode (the mode you should spend most of your time in)
    ^
    - browsing files
    - finding words and navigating lines
    - modify\copy\paste lines, words, characters
    - undo and redo changes
    - all other modes start from normal mode
^
* insert mode (a lot like the default mode in a modeless editor)
    ^
    - insert new text
    - many ways to access
        - `o` `O` insert line below or above current line
        - `i` `I` start insert before character or start of line
        - `a` `A` start insert after character or append end of line
^
* visual mode (highlight text)
    ^
    - used to hightlight text to perfom actions on
    - can be accessed by `v` or `V` to select by character or by line
^
* command mode (execute commands in vim)
    ^
    - perfom commands on file or range in file
    - interact with vim variables, functions and plugins
    - `:!` run bash programs from vim
    - `:e` `:w` `:q` open files from disk to edit, save file and quit vim
    - can be accessed by typing `:` in normal mode
