# Tuni-Git
for git course

Muista ennen työn tekeminen "git checkout" oikein haaraan

Ennen aloitus:
	1.
	-git checkout junyuan
	-git fetch origin
	-git merge origin/master
	2.(tai)
	-git checkout junyuan
	-git pull origin master

Työn teko:
	......

Muista päivittää oma niminen haara:
	-git push origin junyuan/git push origin HEAD 

Kun työ on tehnyt, päivittää etätietovarastoon:
	-git push <etätietovaraston nimi> <paikallinen haara>:<etätietovaraston haara>
	esim. git push origin junyuan:master, paivittaa muutokset junyuan:n haa-	rasta "masteriin"
