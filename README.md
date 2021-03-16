# Git 
###### Muista ennen työn tekeminen "git checkout" oikein haaraan
**Ennen aloitus:**  
&nbsp;- `git checkout junyuan`  
&nbsp;- `git fetch origin`  
&nbsp;- `git merge origin/master`  
&nbsp;(tai)  
&nbsp;- `git checkout junyuan`  
&nbsp;- `git pull origin master`  
**Työn teko:**  
&nbsp;......  
**Muista päivittää oma niminen haara:**  
&nbsp;-`git push origin junyuan`/`git push origin HEAD`  
**Kun työ on tehty, päivitetään etätietovarastoon:**  
&nbsp;-`git push <etätietovaraston nimi> <paikallinen haara>:<etätietovaraston haara>`  
&nbsp;esim. `git push origin junyuan:master`, paivittaa muutokset junyuan:n haarasta "masteriin" 
