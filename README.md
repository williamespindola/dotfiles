My dotfiles

## Install

Install vim via homebrew

```
brew install macvim
```

clone this project at your home directory and run:

```shell
~/dotfiles/bin/dotfiles
```

## Vim

![my vimrc](https://dl.dropboxusercontent.com/u/28988890/vimrc.png)

### Vim key mapping

```vim
" no replace past
xnoremap p pgvy

" avoid mistyping commands
command! W w
command! Wq wq
command! Bd bd

" hotkey to close window
nnoremap q :q<enter>

" Split line (sister to [J]oin lines)
" The normal use of S is covered by cc, so don't worry about shadowing
nnoremap S i<cr><esc><right>

" movement by screen line instead of file line (for text wrap)
nnoremap j gj
nnoremap <down> gj
nnoremap k gk
nnoremap <up> gk

" next and previus tab
nnoremap <C-Tab> :tabn<CR>
nnoremap <C-S-Tab> :tabp<CR>

" automatic esc, really uncommon to type 
noremap 

#>
inoremap 
c>

" Faster scrolling
nnoremap <C-e> 3<C-e>
nnoremap <C-y> 3<C-y>

" Super faster scrolling
nnoremap <C-E> 10<C-e>
nnoremap <C-Y> 10<C-y>

" Bubble single lines, similar to Eclipse (requires unimpaired.vim)
nmap <C-Up> [e
nmap <C-Down> ]e

" Bubble multiple lines, similar to Eclipse (requires unimpaired.vim)
vmap <C-Up> [egv
vmap <C-Down> ]egv

" Duplicate lines, similar to Eclipse
noremap <C-S-Up> YP
noremap <C-S-Down> YP

" Move between splits (windows)
noremap <C-h> <C-w>h
noremap <C-j> <C-w>j
noremap <C-k> <C-w>k
noremap <C-l> <C-w>l

" Make tab in v mode work like I think it should (keep highlighting):
vmap <tab> >gv
vmap <s-tab> <gv
```
