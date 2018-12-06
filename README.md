This repo is not for setting up vimrc, instead for starting with VIM.
Commands that I have discovered and found quite useful so far through youtube tutorials, vimtutor, awesome vim are all shared here. Commands list will soon go beyond infinity! :rocket:

quit:
* q!
---------
save and quit:
* wq!
---------
Move commands:
* j: down
* h: left
* k: up
* l: right
---------
end of line:
* $
---------
start of line:
* 0
---------
end of file:
* G
---------
start of file:
* gg
---------
set line numbers:
* :set nu
* :set rnu # line numbering relative to current cursor position.
---------
unset line numbers:
* :set nu!
* :set rnu!
---------
search pattern:
* :/[pattern] # then enter
* n # to iterate over next pattern matched.
* N # to iterate over previous pattern matched.
---------
repeat previous task:
* . 
---------
macro: # execute following in same order as given.
* :q[macro alphabet] # starts recording the macro, e.g. `:qa`
* q # stops the current macro.
* @[macro alphabet] # to execute the macro.
---------
delete:
* x  # delete a character
* dd # delete whole line
* d[n]j # delete n number of lines from current position
* di[x] # delete inside x where x can be t for <tag>,   ' for inverted comma
---------
copy:
* y # y stands for yank.
* yy # yank whole line, and similar to delete commands
---------
paste:
* p # p stands for p whatenver being copied or deleted recently.
---------
Undo:
* u
---------
Redo:
* Ctr-R
---------
Indent:
* '>>' # indent right
* '<<' # indent left
---------
append(insert mode):
* a
* A # append from last character of current line.
---------
replace:
* r[x] # where x is the new letter to substitute for current cursor character.
---------
end of word:
* e
---------
start of word:
* w
---------
Delete and enter insert mode:
* c[motion] # `ce` will delete till end of word, and enters insert mode, check `cw`
---------
Cursor-screen Movements:
* H # cursor to top(high) of the screen
* M # move cursor to middle(middle) of the screen
* L # move cursor to bottom(low) of the screen. 
---------
Screen movement, withough affecting cursor: (Shifting screen)
* zt  # current line to top
* zz  # current line to middle
* zb  # current line to bottom.
* [n]Ctr-e  # scroll at a time, without cursor movement, n times optional, e.g. `10Ctr-e`
* [n]Ctr-y  # scroll upward, without cursor movement.
* Ctr-[D/U]  # jump half the screen
* CTR-[F/B]  # jump full screen
---------
Find next word currently cursor at:
* *
* '#'  # previous
---------
Find next character:
* f[x]  # find next first x character
* ;  # find net x
* ,  # find last x
---------
Mark:
* mm  # or m[any register]
* `m  # return to where mark was set.
* 'm  # return to start of line where mark was set.
---------
Special delete/change:
* [d/c]f[x]  # delete/change/replace till first x found and delete x too.
* dt[x]  # delete till first x found, but not delete x!
---------
Delete till next blank line:
* d}
---------
Delete from previous blank line:
* d{
---------
Check enclosing parenthesis:
* %  # put cursor at starting or closing parenthesis, and then write this.
---------
Write from last insert position:
* gi  # write at x pos, do something else, press this command, to resume writing from where you left earlier!
---------
jump sentences:
* ()
---------
jump paragraphs:
* {}
