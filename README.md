# tmux-leader-key
  If you're a vi/vim/neovim user, it is possible to map the below key sequences to easily do an action.

  - nnoremap ;ev :edit ~/df/init.vim<CR>      " ev - short for edit vimrc
  - nnoremap ;sv :source ~/df/init.vim<CR>    " sv - short for source vimrc

I prefer these type of mappings because I can avoid using Control and Alt modifies and can recall the letters better if I haven't used them for a while.

tmux-leader-key attemps to creates this workflow when using tmux.

## Installation
  
  To install, download the tmux-leader-key bash script and place it somewhere in your PATH.  Make the script executable: "chmod +x tmux-leader-key"
  
  Add the belowkey binding to your ~/.tmux.conf file
     bind-key  -n ,   popup -h 98% -E  'tmux-leader-key ","'
