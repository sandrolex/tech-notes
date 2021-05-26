* [NEOVIM Cheat Sheet](https://cheatography.com/pthiruna/cheat-sheets/neovim/)
* [NEOVIM Configuration](https://gist.github.com/synasius/5cdc75c1c8171732c817)
* [VIM SPLITS](https://www.sourceallies.com/2009/11/vim-splits-an-introduction/#:~:text=To%20move%20between%20splits%20first,my%20preferred%20home%20row%20method.)

### NERDTree
    :NERDTree
    C-w -> Go to right pane
    C-w <- Go to left pane
    ...


### Nvim conf (~/.config/nvim/init.vim)
    call plug#begin()
      Plug 'davidhalter/jedi-vim'
      Plug 'preservim/nerdtree'
      Plug 'Shougo/deoplete.nvim', { 'do': ':UpdateRemotePlugins' }
      Plug 'vim-airline/vim-airline'
      Plug 'vim-airline/vim-airline-th  emes'
      Plug 'arcticicestudio/nord-vim'
    call plug#end()

    let g:deoplete#enable_at_startup = 1
    colorscheme nord
    syntax enable
    set hidden
    set nowrap
    set encoding=utf-8
    set pumheight=10
    set fileencoding=utf-8
    set ruler
    set cmdheight=2
    set iskeyword+=-
    "set mouse=a
    set splitbelow
    set splitright
    set t_Co=256
    set conceallevel=0
    set tabstop=4
    set shiftwidth=2
    set smarttab
    set expandtab
    set smartindent
    set autoindent
    set laststatus=0
    set number
    set cursorline
    set background=dark
    set showtabline=2
    set noshowmode
    set nobackup
    set nowritebackup
    set updatetime=300
    set timeoutlen=500
    set formatoptions-=cro
    set clipboard=unnamedplus
