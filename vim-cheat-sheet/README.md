
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

## 📖 Working with Text in Vim

### Selecting Text

In Vim, you can select text using visual mode:

1. **Enter Visual Mode**:
   - Press `v` for **character-wise** selection.
   - Press `V` for **line-wise** selection.
   - Press `Ctrl` + `v` for **block** selection.
   - `ggVG` for select all.

2. **Select Text**:
   - Move the cursor using arrow keys or `h`, `j`, `k`, `l` to expand your selection.
   - You can also use movement commands like `w` (word), `b` (back), or `G` (to the end of the file).

3. **Perform Actions on Selected Text**:
   - **Yank (Copy)**: Press `y` to copy the selected text.
   - **Cut (Delete)**: Press `d` to delete the selected text.
   - **Change**: Press `c` to change the selected text (deletes and enters insert mode).

4. **Exit Visual Mode**:
   - Press `Esc` to return to normal mode.

### Copying to Clipboard

To copy selected text to the system clipboard:

1. **Select Text** as described above.
2. **Yank to Clipboard**: After selecting, press `"+y`:
   - `"` indicates a register.
   - `+` refers to the system clipboard.
   - `y` is the yank command.

### Pasting from Clipboard

To paste from the system clipboard back into Vim:

- Press `"+p` to paste the yanked text.

### Note

Ensure your version of Vim has clipboard support by running `vim --version` and looking for `+clipboard`. If it shows `-clipboard`, consider installing a version of Vim with clipboard support (like `vim-gtk` or `vim-gnome`).

