# Git 
###### Muista ennen työn tekeminen "git checkout" oikein haaraan
**Ennen aloitus:**  
&emsp;&emsp;- `git checkout junyuan`  
&emsp;&emsp;- `git fetch origin`  
&emsp;&emsp;- `git merge origin/master`  
&emsp;&emsp;(tai)  
&emsp;&emsp;- `git checkout junyuan`  
&emsp;&emsp;- `git pull origin master`  
**Työn teko:**  
&emsp;&emsp;......  
**Muista päivittää oma niminen haara:**  
&emsp;&emsp;-`git push origin junyuan`/`git push origin HEAD`  
**Kun työ on tehty, päivitetään etätietovarastoon:**  
&emsp;&emsp;-`git push <etätietovaraston nimi> <paikallinen haara>:<etätietovaraston haara>`  
&emsp;&emsp;esim. `git push origin junyuan:master`, paivittaa muutokset junyuan:n haarasta "masteriin"


**project2 used codes:**
1.Add a new remote repository for your repository https://course-gitlab.tuni.fi/git-course/intermediate-branches.git
&emsp;&emsp;- `git remote add  https://course-gitlab.tuni.fi/git-course/intermediate-branches.git`
2.Fetch the history from the remote repository and merge it to yours. You might have to use --allow-unrelated-histories flag
&emsp;&emsp;- `git fetch Intermediate`
&emsp;&emsp;- `git merge --allow-unrelated-histories Intermediate/master`
modify files. delete "<<<<<<<" and "======="

3.Create a new branch feature/create-awesome from master branch
&emsp;&emsp;- `git checkout -b feature/create-awesome master`
4.In branch feature/create-awesome add a following line to file hello_world.py    "print("Hello from feature")"
5.Add and commit changes in feature/create-awesome
6.Push your changes in feature/create-awesome
&emsp;&emsp;- `git push origin feature/create-awesome:feature/create-awesome`
or
&emsp;&emsp;- ` git push -u origin HEAD`
or
&emsp;&emsp;- `git push --set-upstream origin feature/create-awesome`
&emsp;&emsp;- `git push origin HEAD`
..
.
.
