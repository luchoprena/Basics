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




