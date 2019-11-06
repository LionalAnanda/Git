# Git Command that will be usefull

Remove a file from git history and rewrite the history
File to be remove in the git repository
  dir1/dir2/sample_file.txt

git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch dir1/dir2/sample_file.txt' --prune-empty --tag-name-filter cat -- --all

git push origin --force --all
git push origin --force --tags

