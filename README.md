# Git 
###### Muista ennen työn tekeminen "git checkout" oikein haaraan
**Ennen aloitus:**  
		- `git checkout junyuan`  
		- `git fetch origin`  
		- `git merge origin/master`  
		(tai)  
		- `git checkout junyuan`  
		- `git pull origin master`  
**Työn teko:**  
		......  
**Muista päivittää oma niminen haara:** 
		-`git push origin junyuan`/`git push origin HEAD`  
**Kun työ on tehty, päivitetään etätietovarastoon:**  
		-`git push <etätietovaraston nimi> <paikallinen haara>:<etätietovaraston haara>`  
		esim. `git push origin junyuan:master`, paivittaa muutokset junyuan:n haarasta "masteriin" 
