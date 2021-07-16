# Basics
Basic git &amp; Laravel instructions page

- Login to github.com
- New repository ([project_name], public/private, gitignore, license, etc). Check main [branch_name]
- Go to git bash
- cd /c/projects
- git init [project_name]
- cd [project_name]
- git remote add origin "git@github.com:luchoprena/[project_name].git"
- git remote -v (to check fetch & push operations)
- git pull origin [branch_name] --allow-unrelated-histories

#### Work in progress...

#### First push

- git add .
- git commit -m "Message"
- git push --set-upstream origin master

#### Next pushes

- git add [file]
- git commit -m "Message"
- git push


## Clone from repo

cd /c/projects
git clone git@github.com:luchoprena/[project_name].git


## Local repo

- git init --bare
- git remote add origin "git@github.com:luchoprena/[project_name].git"


## Publish to github

- [Github Cheat Sheet](./git-cheat-sheet-education.pdf)
- [Gitlab Cheat Sheet](./git-cheat-sheet.pdf)

