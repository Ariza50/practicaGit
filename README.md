# practicaGit

1.- ¿Que comando utilizaste en el paso 11? ¿Por qué?

Para deshacer un commit y además perder los cambios de nuestro working copy (con —hard), este es el comando.
git reset —hard HEAD~1

2.- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
Para ver el hash del commit creado anteriormente.
git reflog
Para llevarme la rama al commit deseado, perdiendo el wc actual
git reset —hard <hash>

3.- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 

No causa ningún conflicto, de hecho no causa ningún cambio puesto que la rama styled ya contenía todos los commits de la rama master. (Already up to date)
git merge master

4.- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Causa conflicto puesto que git-nuestro.md existe en las dos ramas y es diferente

5.- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No crea ningún conflicto puesto que lo que hace es subir la rama hasta la rama styled mediante fast forward. El archivo git-nuestro.md se actualiza a la versión superior que es la de el merge de styled con htmlify.
git merge styled

6.- ¿Qué comando o comandos utilizaste en el paso 25? 
git log —graph

7.- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

El merge podría ser fast forward puesto que title no dispone de ningún nodo más, aparte del que se encuentra, al que no tenga acceso ya la rama master.

8.- ¿Qué comando o comandos utilizaste en el paso 27? 

git reset HEAD~1

9.- ¿Qué comando o comandos utilizaste en el paso 28? 

git checkout — git-nuestro.md

10.- ¿Qué comando o comandos utilizaste en el paso 29? 

git branch -D title

11.- ¿Qué comando o comandos utilizaste en el paso 30? 

git reset —hard b6a149a

12.- ¿Qué comando o comandos usaste en el paso 32? 

git reflog
git reset —hard 609c6ca

13.- ¿Qué comando o comandos usaste en el punto 33? 

git reflog
git reset —hard b6a149a
