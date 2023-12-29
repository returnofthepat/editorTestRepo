# Vim text editor assesment 

this [website][https://www.freecodecamp.org/news/vim-beginners-guide/] 

## Quick install guide for linux 
	
	Open a new terminal window. type apt update, then type sudo apt
	install vim.  Then launch vim from either the terminal or launch
	the installed application itself.

## Basic Keybindings

### Basic Navigation
	
	h: move left
	l: move right
	k: move up
	j: move down
	C-f: page down
	C-b: page up
	
### Modes

	To change mode you must be in Command mode(normal mode).Command mode
	is where you should cut, copy, and paste.

	Insert mode: This is the mode where you enter text and format the files 
	visual appearance.(i)

	Visual mode: This mode is where you should highlight portions of text
	to cut, copy, paste, etc (v).
	
	Visual block mode: As a beginner I would recomend staying away from this
	mode as you have better places to focus your attention. This mode lets 
	you slected text in block shaped sections.
	
### Editing 
	
	Commands are excuted from command mode after typing ":"
	w - save
    q - quit
	wq or x - save and quit 
	q! - quit without saving 
	!- used to override system safety measures
	yy - copy current line 
	p - paste after the cursor 
	P- paste before the cursor
	
### Searching and replacing 

	/:keyword - search for 'keyword'
	n - move to next search result
	N - move to previous serach result
	
### Moving around 

	gg - go to the begining of the file 
	G - go to the end of the file 
	:[num] - go to line number
	
### Multiple files 

	e filename - open file 
	bn - next buffer
	bp - previous buffer
	
## Initial look:

	Use of redo/undo were quite helpful but not astonishing Deleting large
	chunks of code was difficult to do. I tried entering visual mode and
	selecting the chunk of code, then pressing d to delete it but instead
	left visual mode. After trying different variations of this attempt I
	chose to just manually press d to delete the chunk line by
	line. Relatively easy to understand, the mode function is a bit odd
	but for making sure that files are saved and closed properly this
	seems to be more helpful. However when actually coding in the editors
	I found this to slow me down significantly. Switching between modes
	isn't second nature and the mode you’re currently in is only displayed
	at the bottom of the file.  Saving and exiting the editor is slightly
	obscure from what I’m used to as well. I need to make sure I'm in the
	command mode, then save(:w), then exit(:q); this isn't terrible, just
	peculiar.  Retrieving my file after stopping work proved to be
	aggravating. 
	
## Midpoint 

	I started to get the hang of using vim but the keybindings of Vim are
	quite odd in terms of flow to me. So for any future user who maybe
	considering using Vim be warned, the learning curve can be a bit
	steep. 
	
## Productivity curve 

	In terms of writing code it didn't take ages to become productive. I
	do not like the modes, I find them to be a minor inconvience that
	compounds to be quite annoying. However I believe that they can be
	a good safety crutch for beginners. Compiling a program in a
	terminal was a bit odd to me at first but I gradually got used to
	it. Another thing I really enjoyed about Vim was its predesor
	"Vi". It's particularly helpful for small quick edits but Vim has
	more features and should be used for proper editing/debugging. I
	believe that before a begginner commits to using Vim they should
	give Vi a quick try so they can get a taste of what Vim feels like
	to edit in.

## GDB
<!-- reword section on vim & gdb from gdbVim.md file then paste in -->
	To start debugging press ":", then type "!", then input your command;
	in this case I typed "gdb"

## Conlusion

	I believe that Vim is quite a powerful and helpful editor despite it's
	quirks.

