# Vim CheatSheet

## Moving the cursor

`h,j,k,l` - To move the cursor

`h` - moves left

`j` - moves down

`k` - moves up

`l` - moves right

`w` - move cursor to start of the next word

`e` - move cursor to end of the current word

`0` - move cursor to start of the line

`$` - move cursor to end of the line

Typing a number before motion repeat it that many time
For example,

`2w` - moves cursor to start of two words forward

`3e` - moves cursor to end of three words forward

`3$` - moves cursor to end of third line forward

### Page Scroll
`CTRL-b` - Page Up (Back)

`CTRL-f` - Page down (Forward)

`CTRL-u` - Page 1/2 Up (Up)

`CTRL-d` - Page 1/2 Down (Down)

## Vim Mode

`ESC` - Normal Mode

`i`   - Insert Mode

`v`   - Visual Mode

`V`   - Visual Line Mode

`R`   - Replace Mode

## Exit Vim

`q!`  - Discard any changes & exit file

`wq!` - Save & exit file

## Delete

`x`  - Deletes a character

`dw` - Deletes a word. Until start of the next word excluding its first character

`de` - Deletes to the end of the current word including its last character

`d$` - Deletes to the end of the line

`dd` - Deletes whole line

`cw` - Deletes until start of next word and moves to Insert mode

`ce` - Deletes until start of end of the current word and moves to Insert mode

`c$` - Deletes until end of the line and changes to Insert mode

### Deletes using count

`d2w` - Deletes 2 words and move the cursor to next word forward

`d3e` - Deletes 3 words and move the cursor to end of third word forward

`d2$` - Deletes 2 lines from the cursor forward

`4dd` - Deletes 4 lines

`c2w` - Deletes 2 words and changes to Insert mode

## Insert

`i` - Insert

`A` - Append. Moves the cursor to end of line

`a` - Append text after the cursor

`o` - Open a line below cursor and changes to Insert mode

`O` - open a line above cursor and changes to Insert mode

`r <filename>` - Retrieve file and paste after cursor

`r !<cmd>` - Execute the command and paste the result after cursor

## - Editing a file

`wq!` - Save & exit a file

`w`   - Save a file but not exit

`w <filename>` - Save the file with given filename

`u`      - undo

`U`      - undo whole line

`CTRL-R` - redo

`p`  - Put deleted text after the cursor

`rx` - replace the character at the cursor with `x`

`R`  - replace more than one character

## Cut, Copy & Paste

In vim, `d` - delete is used for `cut`

`y` - yank is used for `copy`

`p` - paste after cursor

`P` - paster before cursor  

`yw` - yanks one word. This can be used with number

## Cursor Location

`gg` - Move to start of the file

`G`  - Move to bottom of the file

`G`      - Goto Line `22G` - Goto 22nd line

`CTRL-G` - Show your location in the file

`g + CTRL-G` - Show more information

## Search

`/` - Search forward

`?` - Search backward

`n` - Search same phrase again$

`N` - Search same phrase again in opposite direction

`CTRL-o` - To go back to the line where you came from

`CTRL-I` - Move forward

`%` - Find matching paranthesis ), ], }

## Substitute

`:s/old/new/g` - Substitute 'new' for 'old' globally in the line

`:s/old/new'   - Substitute 'new' for 'old' once in the line

`#,#s/old/new/g` - Substitute 'new' for 'old' between line numbers range {#,#}

`%s/old/new/g`   - Substitute 'new' for 'old' for every occurence in the file

`%s/old/new/gc`  - Substitute but prompt for every occurence

## Execute External command

`:!<cmd>` - To run any external command, followed by ENTER

## Operators

`c` - change operator

`d` - delete operator

`r` - replace operator

## Motions

`w` - move cursor to start of the next word

`e` - move cursor to end of the current word

`0` - move cursor to start of the line

`$` - move cursor to end of the line

## Vim Setting (.vimrc)

`set showcmd`  - Show the command typed

`set number`   - Show line numbers

`set ruler`    - Show line number & column number$

`set list`     - Show blankspace

`set hlsearch` `set hls` - Highlight search

`set incsearch` `set is` - Increment search

`set ignorecase` `set ic` - Ignore case for search

Note: Prepend `no` to turn an option off. For eg, `set nolist`

## References

* vimtutor

* [Vimsheet](http://vimsheet.com/)

* [fprintf - Vim Cheat Sheet](https://www.fprintf.net/vimCheatSheet.html)

