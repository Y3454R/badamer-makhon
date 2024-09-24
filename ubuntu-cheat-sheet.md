# 📚 Command Line and Vim Cheat Sheet

## 📂 File and Directory Management

### Navigating Directories
- **Change Directory**: 
  ```bash
  cd [directory_name]
  ```
- **Go Up One Level**:
  ```bash
  cd ..
  ```
- **Go Home Directory**:
  ```bash
  cd ~
  ```
- **List Files and Directories**:
  ```bash
  ls
  ```
- **List All Files (including hidden)**:
  ```bash
  ls -a
  ```
### Creating and Removing Directories
- **Create a Directory**:

  ```bash
  mkdir [directory_name]
  ```
- **Remove an Empty Directory**:
  ```bash
  rmdir [directory_name]
  ```
- **Remove a Directory and its Contents**:
  ```bash
  rm -rf [directory_name]
  ```
### File Operations
- **Copy a File**:

  ```bash
  Copy code
  cp [source_file] [destination_file]
  ```

- **Move/Rename a File**:

  ```bash
  mv [source_file] [destination_file]
  ```

- **Delete a File**:
  ```bash
  rm [file_name]
  ```
### Viewing File Contents
- ** View a File with pagination **:
  ```bash
  less [file_name]
  ```
- **View the First Few Lines of a File**:
  ```bash
  head [file_name]
  ```
- **View the Last Few Lines of a File**:
  ```bash
  tail [file_name]
  ```
<!-- Searching for Text
Search for a String in Files:
bash
Copy code
grep [string] [file_name]
🔧 Common Terminal Shortcuts
Text Manipulation
Delete to the Beginning of the Line:
Press Ctrl + U
Delete to the End of the Line:
Press Ctrl + K
Delete Entire Line:
Press Ctrl + A, then Ctrl + K
Process Management
View Running Processes:
bash
Copy code
ps aux
Kill a Process:
bash
Copy code
kill [PID] -->

#### ⚠️ Caution
- Use commands like rm -rf with caution as they can permanently delete files and directories without recovery options.


## 🖥️ Deleting Lines in the Terminal CLI

When working in the terminal on Unix-like systems (such as Ubuntu), you may need to delete lines that you've typed. Here are some quick commands to help you do that:

### For Bash and Zsh Shells

1. **Delete the Current Line**:
   - **Delete to the Beginning**: Press `Ctrl` + `U` to delete everything from the cursor to the beginning of the line.
   - **Delete to the End**: Press `Ctrl` + `K` to delete everything from the cursor to the end of the line.

2. **Delete the Entire Line**:
   - Move to the beginning of the line by pressing `Ctrl` + `A`, then press `Ctrl` + `K` to delete the line.
   - Alternatively, you can press `Ctrl` + `U` directly to delete the entire line.

### Confirming Deletion

After using these shortcuts, if you press `Enter`, the line will not be executed since it has been cleared. These shortcuts are useful for quickly removing text without executing unwanted commands.

Feel free to use these methods to manage your command input efficiently!
