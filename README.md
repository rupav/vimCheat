quit:
* q!

save and quit:
* wq!

Move commands:
* j: down
* h: left
* k: up
* l: right

end of line:
* $

start of line:
* 0

end of file:
* G

start of file:
* gg

set line numbers:
* :set nu
* :set rnu # line numbering relative to current cursor position.

unset line numbers:
* :set nu!
* :set rnu!

search pattern:
* :/[pattern] # then enter
* n # to iterate over next pattern matched.
* N # to iterate over previous pattern matched.

repeat previous task:
* . 

macro: # execute following in same order as given.
* :q[macro alphabet] # starts recording the macro, e.g. `:qa`
* q # stops the current macro.
* @[macro alphabet] # to execute the macro.

delete:
* x  # delete a character
* dd # delete whole line
* d[n]j # delete n number of lines from current position
* di[x] # delete inside x where x can be t for <tag>,   ' for inverted comma

copy:
* y # y stands for yank.
* yy # yank whole line, and similar to delete commands

paste:
* p # p stands for p whatenver being copied or deleted recently.

Undo:
* u

Redo:
* Ctr-R

Indent:
* >> # indent right
* << # indent left

append(insert mode):
* a
* A # append from last character of current line.

replace:
* r[x] # where x is the new letter to substitute for current cursor character.

end of word:
* e

start of word:
* w

Delete and enter insert mode:
* c[motion] # `ce` will delete till end of word, and enters insert mode, check `cw`

Cursor-screen Movements:
* H # cursor to top(high) of the screen
* M # move cursor to middle(middle) of the screen
* L # move cursor to bottom(low) of the screen. 

Screen movement, withough affecting cursor: (Shifting screen)
* zt  # current line to top
* zz  # current line to middle
* zb  # current line to bottom.
* [n]Ctr-e  # scroll at a time, without cursor movement, n times optional, e.g. `10Ctr-e`
* [n]Ctr-y  # scroll upward, without cursor movement.
* Ctr-[D/U]  # jump half the screen
* CTR-[F/B]  # jump full screen

