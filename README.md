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
