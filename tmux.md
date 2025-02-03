# tmux Manual

## Introduction
[tmux](https://github.com/tmux/tmux) is a terminal multiplexer that allows you to manage multiple terminal sessions within a single window.

---

## Installation

### Linux (Debian/Ubuntu)
```sh
sudo apt update && sudo apt install tmux -y
```

### macOS
```sh
brew install tmux
```

### Windows (via WSL or Cygwin)
```sh
sudo apt install tmux -y
```

---

## Basic Commands

### Starting and Exiting tmux
| Command | Description |
|---------|-------------|
| `tmux` | Start a new tmux session |
| `tmux new -s <name>` | Start a new named session |
| `tmux attach -t <name>` | Attach to an existing session |
| `tmux ls` | List active sessions |
| `tmux kill-session -t <name>` | Kill a specific session |
| `tmux detach` | Detach from the session |

---

## Working with Panes
| Command | Description |
|---------|-------------|
| `Ctrl + b %` | Split the window vertically |
| `Ctrl + b "` | Split the window horizontally |
| `Ctrl + b o` | Switch between panes |
| `Ctrl + b x` | Close the current pane |
| `Ctrl + b {` | Move pane left |
| `Ctrl + b }` | Move pane right |
| `Ctrl + b q` | Show pane numbers |
| `Ctrl + b z` | Toggle pane zoom |

---

## Working with Windows
| Command | Description |
|---------|-------------|
| `Ctrl + b c` | Create a new window |
| `Ctrl + b n` | Next window |
| `Ctrl + b p` | Previous window |
| `Ctrl + b w` | List windows |
| `Ctrl + b &` | Close the current window |

---

## Managing Sessions
| Command | Description |
|---------|-------------|
| `tmux new -s <name>` | Create a new session |
| `tmux attach -t <name>` | Attach to a session |
| `tmux kill-session -t <name>` | Kill a session |
| `tmux list-sessions` | List active sessions |

---

## Copy Mode & Scrolling
| Command | Description |
|---------|-------------|
| `Ctrl + b [` | Enter copy mode |
| `Up/Down` | Scroll line-by-line |
| `PgUp/PgDn` | Scroll page-by-page |
| `Space` | Start selection |
| `Enter` | Copy selection |
| `Ctrl + b ]` | Paste copied text |

---

## Customizing tmux
Create a configuration file `~/.tmux.conf` and add custom settings. Example:
```sh
set -g mouse on  # Enable mouse support
setw -g mode-keys vi  # Use vi keybindings
bind r source-file ~/.tmux.conf  # Reload config
```
Reload configuration with:
```sh
Ctrl + b :source-file ~/.tmux.conf
```

---

## Additional Resources
- [tmux Cheat Sheet](https://tmuxcheatsheet.com/)
- [tmux GitHub Repository](https://github.com/tmux/tmux)

Happy multiplexing!

