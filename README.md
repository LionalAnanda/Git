# Git Command

## Remove a file from git history and rewrite the history

File to be removed from the git a repository
  dir1/dir2/sample_file.txt

```
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch dir1/dir2/sample_file.txt' --prune-empty --tag-name-filter cat -- --all

git push origin --force --all
git push origin --force --tags

```

## Overwrite the current branch with master
The following command will update the local branch and the remote branch to the latest master version.

```
git reset --hard master
git push --force

```

