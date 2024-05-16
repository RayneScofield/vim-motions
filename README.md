# vim-motions
Frequently used vim motions
## Buffers
|commands|descriptions|
| ----------- | ----------- |
|:ls|list all buffers|
|:ball|show all buffer in one window|
|:bn|next buffer|
|:bp|previous buffer|
|:bufferN|switch to buffer n|
|:bdelete n|delete one buffer|
|:bf|switch to first buff|
|:bl|switch to last buff|
|:set hidden|switch to other buffers without save|  
## Windows
Window is a view port of buffer
|commands|descriptions|
| ----------- | ----------- |
|:sp|split buffer horizontally|
|:vs|split buffer vertically|
|Ctrl-w c|close a window|
|Ctrl-w o|maximize a window|  
## Tabs
Tabs are collections of windows layout.
| commands | descriptions |
| ----------- | ----------- |
| :tabnew file | open a file in a tab |
| :tabclose | close a tab |
| :tabnext | next tab |
| 3gt | the third tab |  
## Basic vim motions
| commands | descriptions |
| ----------- | ----------- |
| u                           | undo                                      |
| Ctrl+R                      | redo                                      |
| :set clipboard+=unnamedplus |system clipboard                           |
| g;                          | jump to the last change you made          |
| g,                          | jump back forward through the change list |
| ZZ                          | save the current file and close it        |
| :w !sudo tee %              | save file as root user                    |
| :w !diff % -                | show diff before saving the file          |
## Quickfix commands
```
:copen                Open the quickfix window
:cclose               Close the quickfix window
:cnext     or  ]d     Go to the next error
:cprevious or  [d     Go to the previous error
:colder               Go to the older error list
:cnewer               Go to the newer error list
```
## NetRW Explorer
```
:Explore     Starts netrw on current file
:Sexplore    No kidding. Starts netrw on split top half of the screen
:Vexplore    Starts netrw on split left half of the screen
%    Create a new file
d    Create a new directory
R    Rename a file or directory
D    Delete a file or directory
```
## Vim motion grammar
verb + noun  or operators + motions
| operators / verbs | motions / nouns | description                                                  |
| ----------------- | --------------- | ------------------------------------------------------------ |
| y                 | $               | To yank everything from your current location to the end of the line |
| d                 | 3w              | To delete from your current location to the beginning of the next word |
| c                 | }               | To change from your current location to the end of the current paragraph |
| c                 | 2j              | To change the next two lines                                 |
| yy, dd, cc        |                 | linewise operation                                           |
| d                 | i(              | text objects - w, p, s, (, {, [, <, t, ", ', `               |
| c                 | a(              | text objects                                                 |
| d                 | iw              | delete a word                                                |
| gU                |                 | uppercase                                                    |  

current line search f, t, repeat with ; or ,  

current file search /, ?, repeat with n or N  
## Motions in file
| move type                         | key                                |
| --------------------------------- | ---------------------------------- |
| character navigation              | h,j,k,l,gj,gk                      |
| word navigation                   | w, e, b, ge                        |
| current line navigation           | 0, ^, $, g_                        |
| line search and file search       | f, t, /,?                          |
| sentence and paragraph navigation | (, {                               |
| match navigation                  | %                                  |
| line number navigation            | gg, G, nG, 50%                     |
| window navigation                 | H, M, L, nH, nL                    |
| scrolling                         | zz, zt, zb, ctrl-f, ctrl-d, ctrl-e |
