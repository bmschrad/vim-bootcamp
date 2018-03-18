%title: Vim Bootcamp - Day 3
%author: Brandon Schrader
%date 2018-03-17

-> # Master Multiple File Navigation <-

-> *Stop the Tab Madness* <-

^
* _Day 3 Topics:_
    ^
    - buffers
    ^
    - windows
    ^
    - tabs
    ^
    - plugins

---

-> # Buffers <-

Where your files are initially loaded

^
* _Ways to Load Your Buffer_
    - *vim* [filename(s)] load on startup
    - *:e :Explore* load when in vim
    - load with plugin like NerdTree CtrlP

^
* _View and Navigate and Manage Buffers_
    - *:ls* view current buffer
    - *:bn :bp* go to next buffer or previous buffer
    - *:b[#] :b[filename]* go to specific buffer
    - *:bd[#] :[range]bd* delete buffers

^
Note: buffers are only in represented in memory and not written to disk until *:w*

---

-> # Windows <-

The viewport into your buffer(s)

^
* _Create New Windows_
    - *Ctrl-W s Ctrl-W v* split current buffer horizontal or vertical
    - *:split [filename] :vsplit [filename]* open new file in horizontal or vertical split

^
* _Navigate Windows_
    - *Ctrl-W w* jump between windows
    - *Ctrl-W (h j k l)* targeted jump between windows

^
* _Managing Windows_
    - *Ctrl-W x* swap current window
    - *Ctrl-W c :q* close current window
    - *Ctrl-W o* close all windows except current window

^
Note: notice all window commands are prefixed with *Ctrl-w*

---

-> # Tabs <-

Saved Layouts For Your Windows

^
* _Create New Tab_
    - *:tabnew tabedit[filename]* open new blank tab or a new tab from a file
    - *Ctrl-w T* move current window into its own tab

^
* _Navigate Tabs_
    - *:tabnext :tabprevious* go to next tab or previous tab
    - *:tabnext[#]* go to specific tab

^
* _Manage Tabs_
    - *:tabclose* close current tab
    - *:tabonly* close all tabs except the active one

---

-> # Plugins <-

Sometimes you just have to spice it up

plugin manager  [vim-plug](https://github.com/junegunn/vim-plug)

file management [NerdTree](https://github.com/scrooloose/nerdtree)
                [CtrlP](https://github.com/kien/ctrlp.vim)

visuals         [Powerline](https://powerline.readthedocs.io/en/master/)
                [Incsearch](https://github.com/haya14busa/incsearch.vim)
                [Indent Line](https://github.com/Yggdroot/indentLine)

---

-> # End of Day 3<-

More resources

blog    [Stop the Tab Madness](https://joshldavis.com/2014/04/05/vim-tab-madness-buffers-vs-tabs/)

video   [All episodes of Vimcast.org](http://vimcasts.org/episodes/archive)
