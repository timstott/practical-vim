# Practical Vim - Tips and Exercises

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
