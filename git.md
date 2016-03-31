# Git

Master Branch = working code

So when you add, adjust, ... you need to create a new branch. 

To do so:

1. Go to your github account: 
2. Go to:Branch:master
3. write new branch name
4. click create branch:name of new branch


### Searching for differences between files

make sure you go to the folder where the files are in and type: 
**diff -u filename filename**

example: 
<br>
udacity git:(master) ✗ diff -u game_new.js game_old.js

or between two commit id's: 
**git diff commitID commitID**


### Checking out prior commit

- git checkout commitID

### Open Atom from Terminal

- atom .


### Creating new directory 

  - cd ~:
  ** change directories to your home directory** <br>
  - mkdir version-control:
  **make version-control directory**<br>
  - cd version-control:
  **go to version-control directory**
  - mkdir reflections:
  **create reflections directory**
  - cd reflections: 
  **go to reflections directory**
  - atom . lesson_1_reflections.txt:
  **launch sublime with file called lesson_1_reflections.txt**
  
  
### Cloning Repository

- git clone (url repository)


### Getting colored output

- git config --global color.ui auto


### Seeing hidden files

- ls -a


### Creating new Repository

- git init
- git log (see what commits you have) --> Gives "HEAD" message (ERROR)
- git status (Shows what files are changed)


### How to choose what to commit

- git status
- git add FILENAME
- git status (To check)


### Addng Commit message

- git commit (You can type longer messages)
- git commit -m "Commit message" (Short message)

















