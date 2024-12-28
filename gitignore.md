# .gitignore Cheat Sheet

A `.gitignore` file tells Git which files and directories to ignore in a project. Below is a cheat sheet for common use cases.

## General Syntax
- `#`: Lines starting with `#` are comments.
- `!`: Negates the pattern (e.g., `!important-file.txt` will not be ignored).
- `*`: Matches zero or more characters.
- `**`: Matches directories at any level.
- `?`: Matches a single character.
- `[abc]`: Matches any one of the characters inside the brackets.

---

## Common Patterns

### Ignore Specific Files
```
# Ignore a single file
file.txt
```

### Ignore All Files of a Type
```
# Ignore all .log files
*.log
```

### Ignore Files in Specific Folders
```
# Ignore logs in the logs/ directory
logs/*.log
```

### Ignore All Except Specific Files
```
# Ignore everything in a directory except one file
folder/*
!folder/keep-me.txt
```

### Ignore Entire Folders
```
# Ignore a folder
cache/
```

### Ignore Files with Specific Names
```
# Ignore files named secrets.json anywhere
**/secrets.json
```

### Ignore by Patterns
```
# Ignore any file ending in .tmp or .temp
*.{tmp,temp}
```

---

## OS-Specific Files

### macOS
```
.DS_Store
.AppleDouble
```

### Windows
```
Thumbs.db
Desktop.ini
```

---

## IDEs and Text Editors

### Visual Studio Code
```
.vscode/
*.code-workspace
```

### JetBrains IDEs (IntelliJ, PyCharm, etc.)
```
.idea/
*.iml
```

### Vim
```
*.swp
*.swo
```

---

## Programming Languages and Frameworks

### Python
```
__pycache__/
*.pyc
*.pyo
```

### Node.js
```
node_modules/
npm-debug.log
```

### Java
```
*.class
*.jar
*.war
```

### C/C++
```
*.o
*.out
```

---

## Security Best Practices
- **Do not ignore `.gitignore` itself.**
- Add sensitive files (e.g., `.env`, `secrets.json`) to `.gitignore`.
- Use GitHub's [gitignore templates](https://github.com/github/gitignore) for specific languages and frameworks.

---

## What Happens if a File is Tracked Before Adding to `.gitignore`?

If you add a file to Git (stage or commit it) **before adding it to `.gitignore`**, Git will still track that file. Adding the file to `.gitignore` will not automatically remove it from tracking. To stop Git from tracking the file, you need to remove it manually.

### Steps to Stop Tracking a File After Adding It to `.gitignore`:

1. **Add the File to `.gitignore`:**
   ```bash
   echo "file-to-ignore.txt" >> .gitignore
   ```

2. **Remove the File from Tracking (without deleting it locally):**
   Use the `git rm --cached` command:
   ```bash
   git rm --cached file-to-ignore.txt
   ```

3. **Commit the Changes:**
   ```bash
   git commit -m "Stopped tracking file-to-ignore.txt"
   ```

4. **Verify That the File is Ignored:**
   Make sure Git no longer tracks the file by running:
   ```bash
   git status
   ```

   If done correctly, the file will no longer appear as tracked or modified in `git status`.

### Important Notes:
- **Existing versions** of the file in Git history will still be present in past commits.
- If you want to remove sensitive files from the Git history completely, you'll need to use a tool like `git filter-repo` or `BFG Repo-Cleaner`.

---

## Additional Resources
- [Git Documentation: Ignoring Files](https://git-scm.com/docs/gitignore)
- [GitHub gitignore Templates](https://github.com/github/gitignore)
