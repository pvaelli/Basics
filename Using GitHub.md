##These are notes for connecting Git and the terminal, as well as maintaining version control through GitHub repositories.

Go to GitHub, copy URL for your repository. Paste into terminal:
```
git clone URL
```

Enter username and password on for git account into terminal (unless you've set up SSH keys).


When modifying files on your local machine, you can update between local directories and the GitHub repository using the following:

Is there a change?
```
git status
```

What changed?
```
git diff
```
Add a new commit or modified file
```
git add README.md
```

Git with s short description of changes you made. It is good practice to add descriptions for collaborators to describe changes that are made. 
```
git commit -m "enter description of the change here"
```

Log for reverse chronological order
```
git log
```

Push this repository/changes from my computer onto GitHub
```
git push origin master
```

Can also make changes on the GitHub website with commit descriptions included. However, our computer doesn't know these changes have occurred yet, so we need to update.
```
git log
```
This should say nothing; doesn't know anything has happened yet.


This command tells git to communicate with the remote repository and downloads all of the commits that have happened since then.
It will tell you what changes have occurred (by collaborators, etc.) before you modify your own local files.
```
git fetch origin
```

These commands will pull the commits from GitHub onto your local machine
```
git merge origin/master
```
or
```
git pull origin master
```
The previous command does the `git fetch origin` and `git merge origin/master` combined, but it doesn't give you a chance to review the changes before modifying local files.


## The End.
