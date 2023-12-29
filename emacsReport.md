# Emacs report

<!-- Revise and simplify this section, think of users that are just
begining and what they really need to know -->
## Basic keybinding guide 

	ctrl will be refrenced as "C" alt will be referenced as "M" emacs has a
	great guide that you should work through but this section can be
	thought of as a reference sheet.
	
### Navigation

	C-f: move forward one char
	C-b: move back one char
	C-n: move to the next line 
	C-p: move to the previous line 
	M-f: move forward one word
	M-b: move back one word
	C-a: move to the begining of the line 
	C-e: move to the end of the line 
	M-<: move to the begining of the buffer
	M->: move to the end of the buffer
	
### Editiing text

	C-d: Delete the char after the cursor 
	C-k; Kill(cut) the cursor to the end of the line 
	C-y: Yank(past) the last killed text
	M-d: Kill the next word
	M-DELETE: Kill the previous word
	C-SPACE: Set the mark for text selection 
	C-w: Cut selected text
	M-w: Copy
	
	If you would prefer to stick with familar keybidnings you can enable
	CUA keys in options. This will allow C-z to undo, C-c to copy, and C-v
	to paste.
	
### Buffers and Windows
	
	C-x b: switch buffers
	C-x C-b: list all buffers
	C-x k: close current buffer
	C-x 2: split window horizontally 
	C-x 3: split window veritcally
	C-x 1: close all other windows
	C-x 0: close the current window
<!-- the shortcut above is useful for more screen real estate -->

### Files

	C-x C-f: open a file
	C-x C-s: save the current file
	C-x s: save all buffers
	C-x C-w: save the file with a new name 
	
### Searching 

	C-s: cancel the current command(you can also press esc)
	C-x u: undo
	M-x: execute and extended command
	C-h k: describe a key 
	C-h f: describe a function
	
	
## 	Initial look:

	    Replace/Find Feature works very well/is quite intuitive.  You can
		search the web from inside the editor which is neat but I dont see
		the appeal of this, as reading information on a deciated web
		browser looks better and is second nature to interact with. The
		main issues I ran into was working with the buffers and compiling
		the code. I think after a while I could get used to working with
		buffers and even becoming proficent in my knowledge of their
		use. Additionally the compiling wasn't entirely straight foraward,
		but once I was using gdb to attempt to debug, compiling became
		easier(but still not completly intuitive).

## productivity curve:

         Switching between the keys you use in your day to day
         work/schoolwork tends to be a odd learning
         experience. Initially I had a notion that emacs would be
         quite difficult to code in for extened periods of time, this
         origniated from jumping straight in without going through the
         built in guide. I would highly suggest going throught the
         guide even if it seems boring. After going back and going
         through the guide I found that jumping into coding I was able
         to sink into a nice flow of interacting with the editor,
         being able to use the tools natively was essential to finding
         this flow. After coding a few programs in emacs I belive that
         it is a fantastic code editor, however there are still some
         gaps in my knowledge while using emacs that cause a slowed
         productivity curve while using the editor, I think over time
         this would no longer be the case. The key to intuitivly
         coding is to repeat steps over and over again; but this
         doesn't mean repeat useless and mundane tasks. Instead find a
         task or game that you find fun to learn to gain this
         intution. One of my favorites is Hanoi, which you can play in
         emacs by typing M-x then typing hanoi. Also you can play
         tetris, snake, and even more games(although there is no
         lesson to learn in these pertaining to emacs keybindings). If
         you want to practice in a way that requires less reading
         shrotcutfoo has an emacs section to practice.  Most of all
         never forget to type C-X & C-S every so often so you dont
         loose information written in the file. This editor has become 
		 my favorite to use out of all true text editors I've used. 
		 


## Second look at emacs:

	During this explination I will explain my use and appreciation for
    the editor while providing a technical break down of problems I
    encountered and my solution to them. I belive a second look is
    essential as staring at a problem for hours on end, then
    attempting to access your feelings towards it is biased and
    unfair.
	
## GDB

<!-- reword section on emacs & gdb from emacsVim.md file then paste in -->

	compile by typing gcc file-name.c -o file-name. Debug pressing M-x
	then typing gdb. And would you look at that it has compiled. One
	of my favorite parts of emacs is how simplistic it is to compile
	using gdb.

## Conclusion

	Emacs is quite a powerful editor to use and debug in. I would
	recommend this to beginners who are intuitive and have some time
	to spend working inside the editor.
