# Practical Vim - Tips and Exercises

## Tip 29 - Duplicate and move lines using `:t` and `:m` commands

Copy the end of the document to below current cursor
:$copy.
:$t.

Copy current line to below line 6
:t6

Move the end of document to below current cursor
:$m.

## Tip X

Exit inset and visual mode with <C-c>

## Tip 28 - Execute a command on one more consecutive lines

Line numbers as address
:2,6p
Echo lines 2 to 6

:{start},{end}

Symbols

       | description
-------|------------
number | line number
.      | current line (where the cursor is placed)
$      | end of file
%      | all lines in current file

Offset from current line
:.,.+3p
Echo current line + 3 lines

## Tip 26 - Append afer a ragged visual block

var hello = 'world';
var ok = true;
var foo = 1;

## Tip 21 - Visual modes

In visual mode you can switch between visual modes the same way as normal mode.

      | description
------|------------
v     | visual char
V     | visual line
<C-v> | visual block

## Tip 15 - Past from a register without leaving normal mode

In insert mode, paste content from register

registers | description
----------|-----------------
 +        | system clipboard
 "        | text of last deleted or yanked line

keys            | description
----------------|-----------------------
<C-r>{register} | paste content from register
<C-r><C-p>{register} | paste from register and fix indent

## Tip 13 - Move in insert mode

        | description
--------|--------------------------
`<C-h>` | Delete back one character
`<C-w>` | Delete back one word
`<C-u>` | Delete back to start of line

`<C-o>` Switch to Insert Normal mode

## Tip 11 - Combine and conquer

Sample of operator commands

   |
---|---------------
c  | change
g~ | swap case
gu | make lowercase
gU | make uppercase

hello HELLO HeLlO

When operator command is invoked twice it acts on the current line (e.g. cc)

Text objects from plugin:

---|-----------
ae | entire file

=ae autoindent entire file
gUae make entire file uppercase

## Tip 10 - Simple math

<C-a> perform addition (enter twice because tmux prefix)
<C-x> perform substraction

100

Add/Substract count with 10<C-a>

110
