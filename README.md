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
### Push to remote
```
git remote add origin https://github.com/RustamyF/git-practice.git
git branch -M main
git push -u origin main
```

We first need to create a new remote repository to push our commit to by filling 
out this GitHub form (make sure we're logged into GitHub first). Let's call the 
repository git-tutorial and don't add any of the default files since we already
 have them. Once we're done, we'll see a HTTPS link like above which we can use
  to establish the connection between our local and the remote repositories.
   Now if we go our GitHub repository link, we'll see the files that we pushed.


### Create a branch
When we want to add or change something, such as adding a feature, fixing a 
bug, etc., it's always best practice to create a separate branch before developing.

```
# Create a new branch
git checkout -b new-branch
```
We can see all the branches we've created with the following 
command where the * indicates our current branch.

```
# View branches
git branch
```

We can easily switch between existing branches using:

```
# Switch between branches
git checkout <BRANCH_NAME>
```

Once we're in a branch, we can work on our project and commit those changes.
```
# Add, commit and push
git add .
git commit -m "added the word good"
git push origin good
```

### Merge branches via CLI
```
git push origin new-branch
git checkout main
git merge new-branch
git push origin main
```