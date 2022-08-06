# VIM
Quick vim reference

### Modes
The VIM has few modes,
- Default mode or normal mode, where commands can be entered
- Insert mode , by pressing i
- Command-line mode, by pressing :

### Navigation keys

Move lines, alternate to arrow keys,

> left <kbd>H</kbd>, down<kbd>J</kbd>, up<kbd>k</kbd>, right<kbd>L</kbd>

Move in pages,
> Page down <kbd>Ctrl</kbd>+<kbd>f</kbd> <br/>
> Page up <kbd>Ctrl</kbd>+<kbd>b</kbd>

Move by word
> Forward move (stop at comma,period) <kbd>w</kbd><br/>
> Forward move (only white space) <kbd>W</kbd><br/>
> Backward move (stop at comma,period) <kbd>b</kbd><br/>
> Backward move (only white space) <kbd>B</kbd><br/>

Move to line number
> Go to first line <kbd>g</kbd><kbd>g</kbd><br/>
> Go to last line <kbd>G</kbd><br/>
> Go to line number, num+<kbd>g</kbd><kbd>g</kbd>

Move to start of the line
> Go to start of line - <kbd>^</kbd> or <kbd>0</kbd>

Move to end of the line
> Go to end of line - <kbd>$</kbd>


Displaying information about file, cursor position
> <kbd>Ctrl</kbd>+<kbd>G</kbd>

Open Vim help
> :h or :help <br/>
> :h wq for help on wq

Deleting Text in Vim

> Delete character at cursor - <kbd>x</kbd>  <br/>
> Delete character right before or left - <kbd>X</kbd>

General command format in Vim

  [count]Operation[count]{motion} ==> 3d2w -> runs 3 time d2w

Reposition text in window

> <kbd>z</kbd> + <kbd>Enter</kbd>


### Delete/Cut, Yank and Put
Delete/cut a line of text
> Delete/cut entire line <kbd>d</kbd><kbd>d</kbd> <br/>
> Delete/cut 10 lines 10 +<kbd>d</kbd><kbd>d</kbd> <br/>
> Delete/cut the character after the cursor <kbd>D</kbd> <br/>
> Delete/cut word <kbd>d</kbd><kbd>w</kbd>

Copy a word
> Copy a word <kbd>y</kbd><kbd>w</kbd>

Copy a line
> Copy a line <kbd>y</kbd><kbd>y</kbd> or <kbd>Y</kbd>

Put content
> Put the line or word after cursor, <kbd>p</kbd> <br/>
> Put the line or word before cursor, <kbd>P</kbd> <br/>

### Registers
- Unnamed register "" is used to store Delete and Yank
- The Delete/cut is stored in Unnamed reg and "1 numbered reg
- The Yank/copy is stored in Unnamed reg and "0 numbered reg
- There are 26 named registers, "a - "z
- The upper casing named registers causes to append the string -> "A
- To view registers -> :reg

### Insert data
To insert text at the cursor
> <kbd>i</kbd>

To insert text at the beginning of the line
> <kbd>I</kbd>

To insert text in next line
> <kbd>o</kbd>

To insert text above
> <kbd>O</kbd>

To insert after cursor
> <kbd>a</kbd>

To insert at the end of line
> <kbd>A</kbd>

To toggle case of a character
> <kbd>~</kbd>

---
### Search
Search for a char within lines
> <kbd>f</kbd> + char -- forward <br/>
> <kbd>F</kbd> + char -- backward

Search for characters in doc
> <kbd>/</kbd>+chars - forward search. <kbd>n</kbd> for next occurrence and <kbd>N</kbd> previous occurrence.
> <kbd>?</kbd>+chars - backward search. <kbd>n</kbd> for next occurrence and <kbd>N</kbd> previous occurrence.

Search word under cursor
> <kbd>*</kbd> - forward <br/>
> <kbd>#</kbd> - backward

Simple find and replace
> Use search <kbd>/</kbd>+chars and issue change cmd <kbd>c</kbd> and move to next search <kbd>n</kbd> and issue <kbd>.</kbd>
.........................
Substitution
- :%s/oldVal/newVa/g
- % entire file
- .,$ entire file - same as %

### Text Object
Text objects are those enclosed with in ",',(,{,<> etc...

Pattern:
- {operator}{a}{object}
- {operator}{a}{object}
- daw - delete a word irrespective of cursor position
- ciw - change inter word irrespective of cursor position
- c[i|a]s - ***s*** for action on sentence, sentence ending with .?!
- c[i|a]p - ***p*** for action on paragraph
- c[i|a]t - ***t*** for html tags
- c[i|a]( - ***( or )*** for parenthesis
- c[i|a]{ - ***{ or }*** for parenthesis


Same apply to ",',~
