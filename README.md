# Git 
###### Muista ennen työn tekeminen "git checkout" oikein haaraan
**git log:**  
-n 行数 （多显示行数，自定义）   
--date='2021-06-24'  
-S "字符串" （搜索文件内的字符串）  
-p `<path>/<commit>` 能够显示commit的详细信息，类似于这个commit 对哪些文件进行了更改。。。  

**Branches:**  
* `git checkout -b <branch> <remote branch>`= `git branch <branch> <remote branch>` + `git checkout <remote branch>`  
* `git checkout --track <remote branch>` Creates a new branch from the specified branch. Moves HEAD to the new branch. New branch is set to track remote branch.  

**Submodule:**  
* Adding submodules  
  * `git submodule add <url> <path>`
* Deleting submodules：  
  * 1.Delete submodule from .gitmodules  
  * 2.Delete submodule from .git/config  
  * 3.Remove submodule folder using git rm  
  * 4.Create a commit from the changes  
  
* Cloning a project that contains submodules  
  * `git clone --recursive-submodules <repository>`  
    or 
  * `git clone <repository>`  
  * `cd <repository>` 
  * `git submodule update --init --recursive`  
  
* Updating submodule  
  * `git submodule update --remote <submodule name>`  
  
**回退:**  
* `git reset –-soft`：回退到某个版本，只回退了commit的信息，不会恢复到index file一级。如果还要提交，直接commit即可；   
* `git reset -–hard`：
彻底回退到某个版本，本地的源码也会变为上一个版本的内容，撤销的commit中所包含的更改被冲掉；   
Revert撤销一个提交的同时会创建一个新的提交。这是一个安全的方法，因为它不会重写提交历史。比如，下面的命令会找出倒数第二个提交，然后创建一个新的提交来撤销这些更改，然后把这个提交加入项目中。  
 -相比`git reset`，它不会改变现在的提交历史。因此，`git revert`可以用在公共分支上，`git reset`应该用在私有分支上。  
-可以把`git revert`当作撤销已经提交的更改，而`git reset HEAD`用来撤销没有提交的更改。  

**Ennen aloitus:**  
* `git checkout junyuan`  
* `git fetch origin`  
* `git merge origin/master`  
(tai)  
* `git checkout junyuan`  
* `git pull origin master`  
**Työn teko:**  
&emsp;&emsp;......  
**Muista päivittää oma niminen haara:**  
* `git push origin junyuan`/`git push origin HEAD`  
**Kun työ on tehty, päivitetään etätietovarastoon:**  
* `git push <etätietovaraston nimi> <paikallinen haara>:<etätietovaraston haara>`  
&emsp;&emsp;esim. `git push origin junyuan:master`, paivittaa muutokset junyuan:n haarasta "masteriin"
  
  
**Project2 used codes:**  
* 1. Add a new remote repository for your repository https://course-gitlab.tuni.fi/git-course/intermediate-branches.git  
  * `git remote add  https://course-gitlab.tuni.fi/git-course/intermediate-branches.git`  
* 2. Fetch the history from the remote repository and merge it to yours. You might have to use --allow-unrelated-histories flag  
  * `git fetch Intermediate`  
  * `git merge --allow-unrelated-histories Intermediate/master`  
modify files. delete "<<<<<<<" and "======="

* 3. Create a new branch feature/create-awesome from master branch  
  * `git checkout -b feature/create-awesome master`  
* 4. In branch feature/create-awesome add a following line to file hello_world.py    "print("Hello from feature")"  
* 5. Add and commit changes in feature/create-awesome  
* 6. Push your changes in feature/create-awesome  
  * `git push origin feature/create-awesome:feature/create-awesome`  
    or  
  * ` git push -u origin HEAD`  
    or  
  * `git push --set-upstream origin feature/create-awesome`  
  * `git push origin HEAD`

**Push local directory to remote as a new branch:** 
* 1. `Go to directory files located in`
  2. `rm -rf .git .github`
  3. `git init`
  4. `git remote add origin [link]`
  5. `git checkout -b new_branch_name`
  6. `git add .`
  7. `git commit -m"Innitial commit"`
  8. `git push -u origin [branch name]`
.  
.  
