## Markdown
## Create and delete directories

    For delating from git repository and the fylesystem:
       git rm text.txt
       
    But if you only want to delete it from the repository, use: 
       git rm text.txt --cached
       
    For creating a directory, use: 
       mkdir <folder name>
       mkdir "project algorythms"
       
## Navigate 

    For navigate in git bash, the code is: 
       cd <folder name>
       cd desktop 
       
## Compare 

    First you have to code: 
       git status
    It will sshow you what files have changed and then use:
       git diff 
    And this will show you what changed of the files
       
## Find files, folders and inside files
     
    To find a file or folder type: 
       find . name <name of the file or folder>
  
## create and edit text files
    In Git Bash are different codes to do this, the one that you can use to create and start editing the file is: 
       vim newFile.txt

## Get the state of the computer

## The initial configuation

      git config --global user.email 2009089@upy.edu.mx
    
    En este comandos se dan a entender que este nombre de usuario y correo serán los que se usarán en los repositorios locales
      git config --local user.name Isai Massa
     
## Starting a project from zero or cloning an existing repository

    If you want to create a project from zero, you should create a directory to contain the project and type: 
       git init 
    And if you want to clone a repository, type: 
       git clone <url>
       Example: git clone https://github.com/markdown
## Basic workflow commands to stage and commit 
    For commit a change, type: 
       git commit -m "I add a gitignore"
    If a file has changed, type: 
       git add <files name>
    If you have lots of changed files in your working copy - and want all of them included in the next commit: 
       git commit -a -m "Change tittles and add a gitignore"
       
## Push to a remote repository
   
    Github give you the codes and the first one is: 
       git remote add origin https://github.com/isai2506/hola.git
    And after that the code to push to a remore repository is: 
       git push -u origin main
## Branches: create, delete, save/commit & merge 

    For know what are the branches created, type: 
       git branch
    It will list you all the branches of the project, for create a new branch type: 
       git branch <name of the new branch>    git branch test
    If you want to swith of branch, type: 
       git checkout <name of the branch>     git checkout test
       
    To merge two branches, first you have to switch to the main branch and type: 
       git merge <name of the branch you want to merge>       git merge test
       
    To delete a branch, type: 
       git branch -d <name of the branch you want to delete>     git branch -d test
 
 ## Gitflow 
 
    Para poder realizar un gitflow es necesario hacer lo siguiente: 
       Clonar un repositorio 
          git clone https://github.com/markdown
       
       crear una rama
          git checkout -b develop master 
        
       crear rama develop en el repositorio remoto 
          git push --set-upstream origin develop 
          
       Iniciar gitflow
          git flow init 
