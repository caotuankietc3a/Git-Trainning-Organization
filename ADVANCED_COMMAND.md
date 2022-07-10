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

## Delete branch

git branch -d <branch_name>

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

## Annotated tag

git tag -a <tagname> -m "tag commit"

## Lightweight tag

git tag <tagname>

## Delete tag

git tag -d <tagname>

# Stash

## List Stashes

git stash list

## Apply and Drop a stash

git stash pop <stash_name>

## Fetch

git fetch
git fetch -p (Before fetching, remove any remote-tracking references that no longer exist on the remote)
