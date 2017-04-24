# Práctica de GIT

**¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1`

Para deshacer un *commit* tengo que mover el puntero de rama. *reset* mueve el puntero de rama ("styled"), **_--hard_** indica que tiene que dejar el working copy tal y como estaba en el *commit* al que me muevo y HEAD~1 indica el *commit* padre del *commit* en el que estoy.


**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog`

`git reset --hard 71d7ccf17b9dade6eae9011c23067019e9dd9042`

He usado git reflog para buscar el *commit* que había deshecho.

Para rehacer un *commit* tengo que mover el puntero de rama. *reset* mueve el puntero de rama. Además , al haber hecho en el comando anterior un *reset* **_--hard_**, había perdido los cambios, por tanto, al hacer un *reset* **_--hard_** al *commit* en el que estaba, recupero el trabajo perdido.


**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No causó ningún conflicto. De hecho no causó ningún efecto porque la rama styled ya contenía todo el trabajo de master.


**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?** 

Sí,se produjo un conflicto, porque en ambas ramas se ha modificado el mismo archivo en las mismas líneas.


**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?** 

No se produjo ningún conflicto porque se ha sucedido es que el puntero de la rama master se ha movido al *commit* donde estaba el puntero de la rama styled. Se ha producido un merge fast-forward.


**¿Qué comando o comandos utilizaste en el paso 25?** 

`git log --graph --decorate --pretty=oneline`


**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí, podría ser fast-forward, porque master y title estaban "en línea"


**¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1`

Un merge no fast-forward, en el fondo es un *commit* con los datos de las dos ramas. Por tanto, para deshacer un merge, lo que hay que hacer es deshacer un *commit*, que como he comentado en la primera pregunta, se hace con un *reset*. Además, como se pedía no deshacer los cambios, el *reset* no ha sido hard.


**¿Qué comando o comandos utilizaste en el paso 28?**

`git checkout git-nuestro.md`


**¿Qué comando o comandos utilizaste en el paso 29?**

 `git branch -d title`
 
 `git branch -D title`
 
 
**¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog`

`git reset --hard ff80934`


**¿Qué comando o comandos usaste en el paso 32?**

`git log`

`git checkout fd7a75a8edfb80c39e207ce639058204d7e37ff3`


**¿Qué comando o comandos usaste en el punto 33?**

`git log --graph --decorate --pretty=oneline`

`git checkout 5dd9ae777327701bbc83806f50bc0daf0e3fd4dd`
