This repo is being used to practice git commands.  

Initialize a local repository (.git directory) to track our files.
```
# Initialize git
git init
```

We can see what files are untracked or yet to be committed.
```
# Check status
git status
```

Add to stage
Add our work from the working directory to the staging area.

We can add one file at a time:
```
# Add a file to stage
git add README.md
```
We can add all files:
```
# Add all files to stage
git add .
```

### Commit to repo
Commit the files in the staging area to the local repository. 
```
# Commit to local repo
git commit -m "initial commit"
git branch -M main  # rename branch to main (if needed)
```

