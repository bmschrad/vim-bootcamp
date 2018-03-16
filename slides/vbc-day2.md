%title: Vim Bootcamp - Day 2
%author: Brandon Schrader
%date 2018-03-16

-> # Into the details <-

-> *You're problem with Vim is you don't grok Vi <-

^
* _Day 2 Topics:_
    ^
    - motions
    ^
    - registers (delete/\yank/\put)
    ^
    - substitutions

---

-> # Motions <-

Learning the Language of Vim

* _Great Community_
    - lots of plugins
    ^
    - large support network
    ^
    - free
    ^

* _Portablility_
    - runs on anything anywhere (windows, mac, linux, ssh, embedded, etc)
    ^
    - easy and fast to setup on current or new system, only a 14MB download
    ^
    - setting are all kept in plain text (dotfiles) which makes sharing and version control a breeze
    ^
    - a lot of the commands and actions are also used in a lot of other linux programs
    ^

* _Efficiency_
    - modal operation leads to fast navigation and very powerful editing commands
    ^
    - learning one program for all your editing needs

---

-> # Why Vim? <-

*Levels of Text Editing Efficiencies*

Simple examples of copying an existing line and pasting it to a new line underneath

^
* _Noob time_
    ^
    - 1. take your paw off the keyboard and grab the mouse
    ^
    - 2. slowly and painfuly drag your cursor over the existing line or double click
    ^
    - 3. click the end of the line
    ^
    - 4. hit *Enter*
    ^
    - 5. right-click and select paste
    ^
    - 6. question your life choices
    ^

* _Normal Modeless Text Editor_ (advanced keyboard shortcut commands)
    ^
    - 1. hit *Home* to get to beginning of line
    - 2. hold *Shift+End* to highlight to end of line
    - 3. *Ctrl-c* to copy
    - 4. *End* to de-highlight line
    - 5. *Enter* to insert line directly underneath current line
    - 6. *Ctrl-v* to finally paste in previous line 

^
* _Vim_
    ^
    - 1. *yyp*

---

-> # Modes <-

*The Four Main Modes of Vim*

^
* _Normal Mode_ (the mode you should spend most of your time in)
    ^
    - browsing files
    - finding words and navigating lines
    - modify/\copy/\paste lines, words, characters
    - undo and redo changes
    - all other modes start from normal mode
^

* _Insert Mode_ (a lot like the default mode in a modeless editor)
    ^
    - insert new text
    - many ways to access
        - *o O* insert line below or above current line
        - *i I* start insert before character or start of line
        - *a A* start insert after character or append end of line
^

* _Visual Mode_ (highlight text)
    ^
    - used to hightlight text to perfom actions on
    - can be accessed by *v or V* to select by character or by line
^

* _Command Mode_ (execute commands in vim)
    ^
    - interact with vim variables, functions and plugins
    - *:e :w :q* open files from disk to edit, save file and quit vim
    - *:!* run bash programs from vim
    - can be accessed by typing *:* in normal mode

---

-> # Basic Setting <-

_Visual Change_

cursor          *Edit->Profile Preference->Cursor Shape->[Block, Underline]*
colorscheme     *:set colorscheme*

---

-> # Efficient File Navigation <-

How to move around easier

^
* _General Browsing_
    - *G gg* go to the bottom or top of file
    ^
    - *Ctrl+d Ctrl+u* page down and page up
    ^

* _Targeted Edit_ (get to line or word fast)
    ^
    - */ ?* search in front or behind cursor (use to target words and lines)
    ^
        - *n N* move to next or prev match
    ^
    - *:set incsearch* if you want highlighting help
    ^

* _Word and Character Movements_ (moving within a line)
    - *w b* move forward a word or back a word
    ^
    - *f[char] F[char]* look forward or back from cursor to [char] in line
    ^
        - *;* move to next [char] match
    ^
    - *h j k l*  one character movements use only if you miss the mark or very close

---

-> # End of Day 1 <-

More resources

blog    [Why Vim](http://www.terminally-incoherent.com/blog/2012/03/21/why-vim/)

video   [Vim from novice to professional](http://derekwyatt.org/vim/tutorials/novice/)
