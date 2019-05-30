This repo is not for setting up vimrc, instead for starting with  [VIM](https://www.vim.org/).
Commands that I have discovered and found quite useful so far through youtube tutorials, vimtutor, awesome vim are all shared here. Commands list will soon go beyond infinity! :rocket:
<br/>
<br/>

--------
readme instruction format:

**Command for:**
* `command`  # comment
--------

<br/>
<br/>

**quit:**
* q!
---------
**save and quit:**
* wq!
---------
**Move commands:**
* j: down
* h: left
* k: up
* l: right
---------
**end of line:**
* $
* A  # start in insert mode as well
---------
**start of line:**
* 0
* ^
* I  # start in insert mode as well.
---------
**end of file:**
* G
---------
**start of file:**
* gg
---------
**set line numbers:**
* :set nu
* :set rnu # line numbering relative to current cursor position.
---------
**unset line numbers:**
* :set nu!
* :set rnu!
---------
**search pattern:**
* :/[pattern] # then enter
* n # to iterate over next pattern matched.
* N # to iterate over previous pattern matched.
---------
**repeat previous task:**
* . 
---------
**macro: # execute following in same order as given.**
* q[macro alphabet] # starts recording the macro, e.g. `:qa`
* q # stops the current macro.
* @[macro alphabet] # to execute the macro.
* V [n]j :normal @[macro alphabet]  # to execute the macro on the 'n' consecytive lines.
---------
**delete:**
* x  # delete a character
* dd # delete whole line
* d[n]j # delete n number of lines from current position
* di[x] # delete inside x where x can be t for <tag>,   ' for inverted comma
---------
**copy:**
* y # y stands for yank.
* yy # yank whole line, and similar to delete commands
---------
**paste:**
* p # p stands for p whatever being copied or deleted recently.
* P # capital 'P' pastes above the current line.
* viw p # paste the txt in register on a word (by replacing it), by first `visual insert word` command
---------
**Increment a number:**
* ctrl+A
---------
**Undo:**
* u
---------
**Redo:**
* Ctr-R
---------
**Indent:**
* '>>' # indent right
* '<<' # indent left
---------
**append(insert mode):**
* a
* A # append from last character of current line.
* I # insert from beginning of the line.
---------
**replace:**
* r[x] # where x is the new letter to substitute for current cursor character.
---------
**end of word:**
* e
---------
**start of word:**
* w
---------
**Delete and enter insert mode:**
* c[motion] # `ce` will delete till end of word, and enters insert mode, check `cw`
---------
**Cursor-screen Movements:**
* H # cursor to top(high) of the screen
* M # move cursor to middle(middle) of the screen
* L # move cursor to bottom(low) of the screen. 
---------
**Screen movement, withough affecting cursor: (Shifting screen)**
* zt  # current line to top
* zz  # current line to middle
* zb  # current line to bottom.
* [n]Ctr-e  # scroll at a time, without cursor movement, n times optional, e.g. `10Ctr-e`
* [n]Ctr-y  # scroll upward, without cursor movement.
* Ctr-[D/U]  # jump half the screen
* CTR-[F/B]  # jump full screen
---------
**Find next word currently cursor at:**
* *
* '#'  # previous
---------
**Find next character:**
* f[x]  # find next first x character
* ;  # find net x
* ,  # find last x
---------
**Mark:**
* mm  # or m[any register]
* `m  # return to where mark was set.
* 'm  # return to start of line where mark was set.
---------
**Special delete/change:**
* [d/c]f[x]  # delete/change/replace till first x found and delete x too.
* dt[x]  # delete till first x found, but not delete x!
---------
**Delete till next blank line:**
* d}
---------
**Delete from previous blank line:**
* d{
---------
**Check enclosing parenthesis:**
* %  # put cursor at starting or closing parenthesis, and then write this.
---------
**Write from last insert position:**
* gi  # write at x pos, do something else, press this command, to resume writing from where you left earlier!
---------
**jump sentences:**
* ()
---------
**jump paragraphs:**
* {}
---------
**Change:**
* c[a/i]w[[/{]  # changes inside **word**[[/{], change all word (include space next to it), changes will the word end. 
---------
**virtually select all inside:**
* va["/[] or vi["/[]  # and then yank using y or change using c
---------
**Earlier - back to history!**
* :earlier [n][m/s]  # n is number, go back to point of 2minutes/seconds earlier in the file say!
---------
**Store in register:**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* "[a]yy  # 'a' is register name, yy is yank the whole line into the register
* "[a]p  # to paste anywhere the stored value in register a
* Ctrl-R [a]  # **in insert mode**, use ctrl-r to indicate putting register value!
---------
**Last inserted text:**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* Ctrl-a  # **in insert mode.**
---------
**Autocompletion words:(context-aware)**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* Ctrl-p  # in insert mode
* Ctrl-n  # in insert mode
---------
**Autocompletion line:(context-aware)**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* Ctrl-x Ctrl-l  # **works in insert mode only**
---------
**Go to C-Tag:**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* Ctrl-]
* Ctrl-x Ctrl-]  # **in insert mode**, autocomplete the c-tag, instead of using Ctrl-p
--------
**File completion:**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* Ctrl-x  # **in insert mode**, to enter special completion mode
* Ctrl-f  # to complete the file name (current or in the directory)
--------
**Open a new file:**![#f03c15](https://placehold.it/15/f03c15/000000?text=+)
* :e '<file_name>'
--------

**Credits:**

<br/>

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) [Autocompletion mode](http://georgebrock.github.io/talks/vim-completion/)

[vim+tmux - OMG!Code](https://www.youtube.com/watch?v=5r6yzFEXajQ)

[To Read](http://www.yolinux.com/TUTORIALS/LinuxTutorialAdvanced_vi.html)

-------------------------------------------------------------------------

**Vimium chrome Extension:**

Select a text, select that line, yank it and search.
v / [search pattern] ESC shift-0 y p[/P]
