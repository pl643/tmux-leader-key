# tmux-leader-key

## What is it?

An attempt to create a Vim-like workflow in tmux where a chosen key (leader) in addition to few letters can be mapped to perform an action.

  - nnoremap ;ev :edit ~/df/init.vim<CR>      " ev - short for edit vimrc
  - nnoremap ;sv :source ~/df/init.vim<CR>    " sv - short for source vimrc
  
  The above vim configuration maps the key sequences ";ev" to open the vim configuration file and ";sv" loads it.
  
  The advantages of this workflow the usage of letters to help remember the action, which are normally in the for of verb + object.
  
## Installation
  
  To install, download the tmux-leader-key bash script and place it somewhere in your PATH.  Make the script executable: "chmod +x tmux-leader-key"
  
  Add the belowkey binding to your ~/.tmux.conf file
     bind-key  -n ,   popup -h 98% -E  'tmux-leader-key ","'
