# ADVANCED_COMMAND

# Different

git diff

# Branch

## List Branches

git branch

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

(git add and git commit to resolve)
