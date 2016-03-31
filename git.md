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

Type: 
<br>
git checkout commitID




### Open Atom from Terminal

type: 
<br>
atom .


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











