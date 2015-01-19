# Practical Vim - Tips and Exercises

## Tip 21 - Visual modes

In visual mode you can switch between visual modes the same way as normal mode.

v | visual char
V | visual line
<C-v> | visual block

## Tip 15 - Past from a register without leaving normal mode

<C-r>{register} paste register content in insert mode (e.i. <C-r>+, paste from
system clipboard)

## Tip 13 - Move in insert mode

<C-h> Delete back one character
<C-w> Delete back one word
<C-u> Delete back to start of line

<C-o> Switch to Insert Normal mode

## Tip 11 - Combine and conquer

Sample of operator commands

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
