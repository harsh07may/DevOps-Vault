**Nano:** 
GNU nano is a text editor for Unix-like computing systems or operating environments using a command line interface.
It supports syntax highlighting, spell checking, justifying, completion, undo/redo etc.

**Commands:** 
- `nano [filename]`: start editor and edit `filename` 
- `ctrl+k/ctrl+u`: cut/paste
- `ctrl+o`: write out to another file
- `ctrl+x`: exit
- `alt+6`: copy

---
**Vim** 
Vim is a highly configurable text editor built to make creating and changing any kind of text very efficient. It is included as "vi" with most UNIX systems

- vi is in *command mode* by default, allows you to run commands like `:q` and `:w`.
- press `i` to go into *insert mode*, which allows you to edit the file, `esc` to go to command mode.
- press `l` to go to *line mode*, allows you to see current line info. 

**Commands:**
`vi [filename]`: start editor and edit `filename`
`:w` : write to the file(save).
`:w [filename]` : write to `filename`
`:w! [filename]` : overwrite `filename` 
`:x or :wq` :  exit and write to the file
`:q` :  **how to exit vim :)** 
`:q!` : quit without saving
`:n or nG` : move to line `n`
`:$` : move to last line

`0`: move to start of line
`$`: move to end of line
`w`: move to next word 
`ctrl+l`: refresh and center screen
`/pattern or ?pattern`: search forward/backward for pattern

