# tmux-leader-key

## What is it?

A Vim-like workflow in tmux where a chosen key (leader) in addition to few letters can be mapped to perform an action.

  The below vim configuration maps the key sequences ";ev" to open the vim configuration file and ";sv" loads it.
  - nnoremap ;ev :edit ~/df/init.vim<CR>      " ev - short for edit vimrc
  - nnoremap ;sv :source ~/df/init.vim<CR>    " sv - short for source vimrc  
  The advantages of this workflow is the usage of letters to help remember the action to be performed which is normally in the form of a verb and object.
  
## Trial without installing
  - Have tmux 3.2 or higher (requires display-pop feature) running.
  - curl URL to /tmp/; tmux bind-key 
  - This will bind the ',' key as the leader key. To produce a ',', you will need to press ',' twice.  You have the option of chosing another leader key.
