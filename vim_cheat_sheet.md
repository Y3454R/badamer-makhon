
# Vim Cheat Sheet

## Modes
- `i` : Insert mode - Enter editing mode.
- `Esc` : Normal mode - Return to command mode.
- `v` : Visual mode - Select text.
- `V` : Visual line mode.
- `Ctrl + v` : Visual block mode.
- `:q` : Quit Vim.
- `:w` : Save file.
- `:wq` : Save and quit.
- `:q!` : Quit without saving.

## Cursor Movement
- `h` : Move left.
- `j` : Move down.
- `k` : Move up.
- `l` : Move right.
- `w` : Jump forward to the start of a word.
- `b` : Jump backward to the start of a word.
- `e` : Jump forward to the end of a word.
- `0` : Jump to the beginning of the line.
- `$` : Jump to the end of the line.
- `gg` : Go to the first line of the file.
- `G` : Go to the last line of the file.

## Editing
- `x` : Delete character under the cursor.
- `dd` : Delete current line.
- `dw` : Delete word.
- `yy` : Copy (yank) the current line.
- `p` : Paste after the cursor.
- `P` : Paste before the cursor.
- `u` : Undo last change.
- `Ctrl + r` : Redo last undone change.

## Searching
- `/` : Search for a pattern.
- `n` : Jump to next match.
- `N` : Jump to previous match.
- `:%s/old/new/g` : Replace all occurrences of 'old' with 'new' in the file.

## Miscellaneous
- `.` : Repeat the last command.
- `:%!` : Run shell command.
- `:help <command>` : Get help on a command.
