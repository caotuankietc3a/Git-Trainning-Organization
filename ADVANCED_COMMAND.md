# ADVANCED_COMMAND

# Different

git diff

# Branch

## List Branches

git branch
git branch -a (remote and local)

## Create new branch and switch

git checkout -b <branch_name>

## Switch to new branch

git checkout <branch_name>
git switch <branch_name>

## Create branch

### Create branch from remote to local

1.go to github and create branch
2.git checkout <branch_name>

### Create branch from local to remote

1.git checkout -b <branch_name>
2.git push -u origin <branch_name>

## Delete branch

### Delete branch from remote to local

1.go to github and delete branch

2.git branch -d <branch_name>

3.git fetch -p (Before fetching, remove any remote-tracking references that no longer exist on the remote)

### Delete branch from local to remote

1.git branch -d <branch_name>

2.git push -u origin :<branch_name>

# Merge

git merge <branch_name> -> (merge <branch_name> to current branch)

# Fix conflicts when merging

## Check where conficts were

git log --merge

## Cancel~Abort current merge

git merge --abort

## Fix merging conflicts

git commit -am "Resloved conflicts"

(git add and git commit to resolve conflicts)

# Tag

## List tags

git tag -l

git tag

## Show tags and related info

git show <tag_name>

## Annotated tag

git tag -a <tag_name> -m "tag commit"

git tag -a <tag_name> -m "tag commit" <commit_id>

## Lightweight tag

git tag <tag_name>

git tag <tag_name> <branch_name>

## Delete tag

### Delete tag from remote to local

1.go to github and delete tag

2.git fetch -p

3.git tag -d <tag_name>

### Delete tag from local to remote

1.git tag -d <tag_name>

2.git push origin :<tag_name>

## Push tags to remote branch

git push origin <tag_name>

git push --tags (all rest tags)

## Update tag

### Update tag from local to remote

git tag -f <tag_name> <commit_id>

git push -f origin <tag_name>

# Stash

## List Stashes

git stash list

## Apply and Drop a stash

git stash pop <stash_name>

## Fetch

git fetch

git fetch --all

# Git pull with rebase

(use when git commit some changes in local branch and commit some changes from remote branch)

git pull --rebase (a method of combining your local unpublished changes with the latest published changes on your remote)

git push -u origin main

# Synchronize forked directory

git remote add <remote_name> <forked_url>

git pull <remote_name> <branch_name>

# Attach commit to closed issue

git add <file_name>

git commit -m "commit_message, close #<number_of_closed_issue>"
