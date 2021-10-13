# Git commands

+ Create and checkout branch (from current branch): 

```bash
$ git checkout -b <branch_name>
```

+ Push branch to remote and track: 

```bash
$ git push -u origin <branch_name>
```

+ List branches: 

```bash
// Local only 
$ git branch

// Local and remote
$ git branch -a

// Only remote
$ git branch -r
```

+ Checkout remote branch: 

```bash
$ git checkout -b <branch_name> origin/<branch_name>
or
$ git checkout --track origin/<branch_name>
```

+ Interactive staging (accept or reject changes before staging)

```bash
$ git add -p
// Then y/n t accept/reject changes
```

+ Merge branch (merges <branch> into current HEAD):

```bash
$ git merge --no-ff <branch_name>
```

+ Abort merge

```bash
$ git merge --abort
```

+ Delete branch: 

```bash
// Local
$  git branch -d <branch_name>

// Remote
$  git push origin --delete <branch_name>
```

+ Stash: 

```bash
$ git stash
$ git stash pop // removes from stash and applies
$ git stash apply // keeps in stash and applies
$ git stash list // list all stashes
$ git stash show // see files stashed
```

+ Change name (file or folder, for a folder the full route from where you are): 

```bash
$ git mv <old_filename> <new_filename>
```

+ Create annotated tag: 

```bash
$ git tag -a <tagname> -m '<message>'
```

+ Push tag to remote

```bash
$ git push origin <tagname>
```

+ View tags: 

```bash
$ git tag
```

+ View tags with annotations: 

```bash
$ git tag -n
```

+ View specific tag with annotation: 

```bash
$ git tag -n <tagname>
```

+ Pushing new repo to remote

```bash
// Create repo in GitHub. Copy HTTP address
// Create local repo. Initialise git (git init).
$ git remote add origin <address>
$ git push -u origin master
```

+ Cloning a remote repo to a new local directory

```bash
git clone <repo-url> <directory>
```
