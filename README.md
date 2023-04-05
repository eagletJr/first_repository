# Demo

This is a general description.
(Now I've edited it!!!)

## Subheader

There's a lot of information. I'm afraid I might forget it all.
This will hold commands to remember:

ls -la: Show me all files in a directory, including hidden files

git status - Shows what changes have been made on what files. When a file is modified it becomes "unstaged", unstaged changes won't be included in the next commit command
- Ex: "git status
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html"

git add - Tells Git what files should have their changes switched to "staged", these files will be included in the next commit command
- Ex: "git add index.html; git add README.md"
- EX: "git add." = The "." means to add everything instead of a single file

git commit -m "MESSAGE1" -m "MESSAGE2" - The staged changes added by the "add" command will be saved and creates a new updated repository. 
The -m "MESSAGE1" is required. This is the same as the first text box below the "Commit changes. This could be a short message on the what and why of the commits being made
The -m "MESSAGE2" is the same as the optional extended description of the commit changes text box.