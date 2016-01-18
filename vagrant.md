# Vagrant

= Virtual machine inside your computer. 

To use Vagrant, you have to have access to a terminal.<br> iterm is an app that allows you to use the terminal.<br>
The terminal is also known as the **command-line** or the abbreviation **CLI**.

To run the Vagrant Machine you have to be in the directory where the Vagrant Machine is located:

`cd /Users/kaatje/Documents/Development/CuadranteWeb`

`cd` = change directory

**iterm should show now:**

`➜  CuadranteWeb git:(master) ✗`

---

After you are in the directory you follow these steps: 

### To start

`vagrant up`


### To login 

`vagrant ssh`


### To exit

`exit` (or ctrl + d )

### Shut down Vagrant 

`vagrant halt`

---

**1. Once you are logged in type** `ls` 

`➜  ~  ls`
(to see files and folders)

**2. Type **`cd`

`➜  ~  cd repositories` (to change to your folder repositories)

**3. Type** `ls`

`➜  repositories  ls` (gives a list of the content of the current folder)

**4. Type ** (Choice of repository: this case ` ls SVTechsol`)

`➜  repositories  ls SVTechsol`

**5. Type ** `cd SVTechsol`

`➜ repositories  cd SVTechsol`

**6. Type** `git pull`

`➜  SVTechsol git:(master) git pull`

**7. Type** `git checkout initial`

`➜  SVTechsol git:(master) git checkout initial`

**8. Type** `git status`

`➜  SVTechsol git:(initial) git status`

```
On branch initial
Your branch is up-to-date with 'origin/initial'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	index.html  //* WILL SHOW UP IN RED *//

nothing added to commit but untracked files present (use "git add" to track)```

If Index.html = red, that means this is a new file, so you need to add it to git first. 

**9. Type** `git add index.html` or `git add .`(multiple files)

`➜  SVTechsol git:(initial) ✗ git add index.html`

**10. Type** `git status`

`➜  SVTechsol git:(initial) ✗ git status`

```
On branch initial
Your branch is up-to-date with 'origin/initial'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   index.html //*files are green that have been added *//
```
**11. Type** `git commit -m 'message what you did'`

`➜  SVTechsol git:(initial) ✗ git commit -m 'add index.html Hello World'`

```
[initial df87981] add index.html Hello World
 1 file changed, 10 insertions(+)
 create mode 100644 index.html
 ```
