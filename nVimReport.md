# NeoVim editor assesment 


## Install guide
	
	sudo apt update
	sudo apt install neovim 
	nvim --version

## Basic Keybinding guide 
### Basic Navigation
	
	h: move left
	l: move right
	k: move up
	j: move down
	O: move to the begining of the line
	$ or G: move to the end of the line
	gg: move to the beginning of the file 
	C-f: page down
	C-b: page up
	
### Modes
	
	To change mode you must be in Command mode(normal mode).Command
	mode is where you should cut, copy, and paste. 
	
	Insert mode: This is the mode where you enter text and format the
	files visual appearance.(i) 
	
	Visual mode: This mode is where you
	should highlight portions of text to cut, copy, paste, etc (v).
	
	Visual block mode: As a beginner I would recomend staying away from
	this mode as you have better places to focus your attention. This
	mode lets you slected text in block shaped sections.
	
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

## Initial thoughts:
	
	When starting up neoVim I did not notice a difference between it
	and Vim, upon doing some research I found that the main advertized
	usefulness of neoVim is it's adaptability. So I played around with
	debugging in neoVim using gdb and it worked much the same, please
	reference my section on vim using gdb to get a better picture of
	this.

### Resources 
	
	My main issue with neovim is the lack of documentation for
	extensions. Part of the appeal of neovim is the addition
	extensions, these help neovim become even more powerful from the
	out of the box version of the editor.
	
 
## Productivity curve:
	
	neoVim is very similar to vim but at a bried glance it seems all the
	buzz about neoVim has to do with the extensions that are available
	for it. However I didnt want to dive into configuring neoVim right
	away. So I used it at face value and wrote my experience with it.
	I feel that productivity would increase when using the plug-ins,
	but in my use case of it I didn't notice much of a increase in 
	productivity.

## mid-point thoughts:

	After feeling like I was just using Vim with different keybindings
    I decided to explore some extensions in NeoVim, these include CoC,
    COC explorer, and Format on save. Once I used CoC, COC explorer, 
	and Format on save that when I started to notice the biggest 
	"power boost" in neoVim. All the articles i read were absolutely 
	correct the configuration of neoVim and Vim is what makes them 
	such great editors. Compared to emacs the out of the box version 
	leaves quite a lot to be desired but when it is configured and 
	tailored to the user it becomes quite a great editor. Although 
	a lot of the issues with NeoVim seems to stem from the lack of 
	documentation within the community. 
	
	
## Add-ons 

	Below i have listed the install process and use case for different 
	plug-ins for neovim. Please make sure to install a plug-in manager
	like vim-plug before continuing. 
	
### CoC 
	
	Install:
	
	sudo apt update 
	sudo apt install nodejs npm
	
	sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site
	/autoload/plug.vim --create-dirs \https://raw.githubusercontent.com
	/junegunn/vim-plug/master/plug.vim'

	curl -fLo ~/.vim/autoload/plug.vim --create-dirs \https://
	raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

	call plug#begin('~/.vim/plugged')
	Plug 'neoclide/coc.nvim', {'branch': 'release'}
	call plug#end()
	
	:CocInstall coc-python

	Use case:
	
	
	Conclusion:
	beginner friendly

### COC Explorer

	Install:
	
	sudo apt update 
	sudo apt isntall nodejs npm 
	
	sudo apt install neovim or sudo apt update neovim
	
	curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
     https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
	 
	Plug 'neoclide/coc.nvim', {'branch': 'release'}

	:CocInstall coc-explorer

		
	
	Use:
	
	This plug-in can be quite helpful for a beginner as it makes the 
	listsof files and directories easier to read and navigate. When 
	youre first learning functions, classes, and variables can be
	difficult. I believe that the symbol exploration aspect of coc
	explorer can help aid in this learning process. Additionally the
	intergration of git sounds to be quite helpful from what i've
	read. COC explorers ability to show git status can be a very
	useful tool to help beginners keep track of their publishings
	when they are first starting out.
	
	Conclusion:
	Beginner friendly

### Format on Save

	Install:
	
	Plug 'neovim/nvim-lspconfig'  # LSP
	Plug 'mhartington/formatter.nvim'  # Formatter

	configure language server protocol(LSP)
	lua << EOF
	require'lspconfig'.pyright.setup{}
	EOF
	
	Configure formatter
	require('formatter').setup({
		filetype = {
			python = {
				function()
				return {
					exe = "black",
					args = {"-"},
					stdin = true
				}
			end
			}
		}
	})
	
	Set up Autoformat on Save
	
	vim.api.nvim_exec([[
	augroup FormatAutogroup
	autocmd!
	autocmd BufWritePost *.py FormatWrite
	augroup END
	]], true)

	
	Use:
	
		Some advice I would give to someone thinking of using this 
		plug-in would be to only use it after you've spent sometime
		coding beforehand. You shouldn't build your skill and syntax
		knowledge with a large help from a autofill extension. Most 
		of your formatting style, syntax knowledge, etc. should be 
		built on your own. For anyone who is working on a large 
		project this plug-in would be helpful. Trying to keep 
		consistent style and avoid syntax errors on a large program 
		can be difficult so this extension could defiently help in
		this particular use case.
		
	Conclusion:
	not beginner friendly. I would recommend intermediate or greater level
	
<!-- add a basic blurb on gdb in neovim-->
## gdb


## Conclusion:
	
	to be determined 
