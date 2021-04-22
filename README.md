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
       
    #Hi
      git config --global user.email 2009089@upy.edu.mx
    
    En este comandos se dan a entender que este nombre de usuario y correo serán los que se usarán en los repositorios locales
     git config --local user.name Isai Massa
