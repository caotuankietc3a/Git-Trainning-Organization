# BASIC_COMMAND

# Initilize current directory

git init

# Stage changes

git add .

# Commit file changes

git commit -m "Some TEXT"
git commit -am "Some TEXT" # use when files tracked ~ git add <file_name> && git commit -m "Some TEXT"

# Check status files

git status

# Show commits history

git log
git log --oneline --graph --decorate --all

# Config .gitconfig to use alias

git config --global alias.hist = log --oneline --graph --decorate --all (see .gitconfig)
git hist <file_name>

# show all files tracked

git ls-files

# Unstage changes

git restore --staged <file_name>

# Discard changes in working directory

git restore <file_name>

# Rename git files

git mv <file_name> <new_file_name> (in staging changes)
git commit -m "Some TEXT"

# Remove git files

git rm <file_name> (in staging changes)
git commit -m "Some TEXT"

# Changes not staged for commit

## Update all tracked files

git add -u .

## Add changes from all tracked files and untracked files

git add -A .
