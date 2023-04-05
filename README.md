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
- Ex: "git add." = The "." means to add everything instead of a single file

git commit -m "MESSAGE1" -m "MESSAGE2" - The staged changes added by the "add" command will be saved and creates a new updated repository. 
The -m "MESSAGE1" is required. This is the same as the first text box below the "Commit changes. This could be a short message on the what and why of the commits being made
The -m "MESSAGE2" is the same as the optional extended description of the commit changes text box.
- Ex: "git commit -m "Added index.html. Updated README.md" -m "Added index.html. Changed README.md to include commands and instructions in using git to commit changes""

git push - After using a "commit" the changes will only be saved locally. To upload the changes to GitHub use "push". Pushes the commits to a remote repository where your work is

 - To actually do use ssh to prove you own the account. To connect a machine to a GitHub account:
   - COMMAND: ssh-keygen -t rsa -b 4096 -C "example@email.com"
     - "ssh-keygen" - generates a ssh key
     - "-t" - specifies the encryption to use
     - "-b" - specifies the strength of the encryption
     - "C" - the email address. This would be the email address used by GitHub
   - This command will return "example" and "example.pub"
     - The example.pub would be my public key
     - The example would be my private key, which proves I'm the one who generated every public key, specifically the one GitHub is using
- To print out the contents of a file, in this case the contentes of my public key
  - COMMAND: cat example.pub
- To copy the contentes of a file, in this case the contents of my public key (I'll also need to know the file path)
  - COMMAND: pbcopy < ~/example.pub