# tmux-leader-key

## What is it?

A Vim-like workflow in tmux where a chosen key (leader) in addition to few letters can be mapped to perform an action.

  The below vim configuration maps the key sequences ";ev" to open the vim configuration file and ";sv" loads it.
  - nnoremap ;ev :edit ~/df/init.vim<CR>      " ev - short for edit vimrc
  - nnoremap ;sv :source ~/df/init.vim<CR>    " sv - short for source vimrc
  
The advantages of this workflow is the usage of letters to help remember the action to be performed which is normally in the form of a verb and object.
An extra feature in tmux-leader-key not from vim is after the leader key is pressed, a menu is presented of the mappings.  This helps with mappings that are less often used.
NOTE: If the leader key is a normal key for example a ',' (commma).  You would need to press the ',' a second time to get the ','.
This script include most standard tmux command mappings like:
  - cw: choose windows
  - sp: swap pane
  - sv: split vertically
You can always add more mappings
  
## Trial without installing
  - Have tmux 3.2 or higher (requires display-pop feature) running.
  - curl URL to /tmp/; tmux bind-key 
  - This will bind the ',' key as the leader key. To produce a ',', you will need to press ',' twice.  You have the option of chosing another leader key.
