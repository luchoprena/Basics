# Basics of GIT
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


#### Branching

Before creating a new branch, pull the changes from upstream. Your master needs to be up to date.
- git pull

Create the branch on your local machine and switch in this branch :
- git checkout -b [name_of_your_new_branch]
<br>

Push the branch on github :
- git push --set-upstream origin [name_of_your_new_branch]

When you want to commit something in your branch, be sure to be in your branch. Add -u parameter to set-upstream.
<br>
You can see all the branches created by using :
- git branch -a

Which will show :

* approval_messages
  master
  master_clean

Add a new remote for your branch :

- git remote add [name_of_your_remote] [name_of_your_new_branch]

Push changes from your commit into your branch :
- git push [name_of_your_new_remote] [url]

Update your branch when the original branch from official repository has been updated :
- git fetch [name_of_your_remote]

Then you need to apply to merge changes if your branch is derivated from develop you need to do :
- git merge [name_of_your_remote]/develop

Delete a branch on your local filesystem :
- git branch -d [name_of_your_new_branch]

To force the deletion of local branch on your filesystem :
- git branch -D [name_of_your_new_branch]

Delete the branch on github :
- git push origin :[name_of_your_new_branch]


## Clone from repo

cd /c/projects
git clone git@github.com:luchoprena/[project_name].git


## Local repo

- git init --bare
- git remote add origin "git@github.com:luchoprena/[project_name].git"


## Publish to github

- [Github Cheat Sheet](./git-cheat-sheet-education.pdf)
- [Gitlab Cheat Sheet](./git-cheat-sheet.pdf)


# Laravel

### Create project with composer

- Goto C:\projects
- composer create-project laravel/laravel:^7.0 [project_name]
- cd [project_name]

### Generate app key (.env APP_KEY)

- php artisan key:generate

### Create controllers/models/migrations with artisan

- php artisan make:controller [controller_name]
- php artisan make:model [model_name]
- php artisan make:migration [table_migration_name]

### Install packages with composer

- composer require phpmailer/phpmailer (to install PHPMailer)

### Update packages with composer

- composer update

### Refresh tables

- php artisan migrate:refresh (recreate db)
- php artisan migrate:fresh (recreate tables)
- php artisan migrate:fresh --seed (with data)

### Seed tables

- php artisan make:seeder [table_seeder_name]
- php artisan db:seed  
- php artisan db:seed --class=[table_seeder_name] 

### Storage

Create link for public storage files from your storage folder

- php artisan storage:link

#### This will create a path accessible at [host]/storage linked to folder [app_root]/storage/app/public
#### Symlink at [app_root]/public/storage

Create subfolders under storage at path [app_root]/storage/app/public/[folder_name] and access them via [host]/storage/[folder_name]



# React JS

### Update packages after cloning repo

- npm install react-scripts@latest


# Wampserver

### Enable SSL to virtual hosts guide

- [Go to guide](https://www.infyom.com/blog/how-to-enable-localhost-https-ssl-on-wamp-server)



