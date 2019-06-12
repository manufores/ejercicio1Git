Respuestas:

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
R: git reset --hard HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
R: git reset --hard 41052ee

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
R: No causó ningún conflicto. Creo que no causa ningún conflicto debido a que los textos de los commits en Master y en Styled son iguales,
sólo que en Styled le aplicamos caracteres de markdown.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
R: En este merge si que ha causado un conflicto. Se debe a que los archivos no son iguales.


- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
R: No causó ningún conflicto. Debe ser que como en el merga anterior al resolver el conflicto nos hemos quedado con el contenido de styled,
sucede el mismo caso que para el merge del paso 13.

- ¿Qué comando o comandos utilizaste en el paso 25?
R: git log --graph --pretty=oneline --decorate

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
R: No podría ser Fast Forward ya que al crear el commit con el archivo modificado al cual le añadimos el título,
éste no es alcanzable por master, así que el merge tiene que crear un commit nuevo como enlace entre los dos commits afectados por el merge.

- ¿Qué comando o comandos utilizaste en el paso 27?
R: git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?
R: Este paso no lo entendí muy bien y, siendo así que me lo salté.
Si no estoy mal informado, debería de haber hecho un git checkout -- (el archivo .md).
Pero aún sigo si tenerlo claro del todo.

- ¿Qué comando o comandos utilizaste en el paso 29?
R: git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
R: He usado un git reflog para saber el SHA del commit antes de deshacer el merge y,
he utilizado git reset 08012c8 para volver al commit.

- ¿Qué comando o comandos usaste en el paso 32?
R: He usado un git log para saber cual es el SHA del commit inicial y,
he usado git checkout cbc495a6899d00a4586e1fadc153d8fcd86a8779 para mover el HEAD hasta ese commit.
Al mover sólo el HEAD, he creado un estado de 'detached HEAD'.

- ¿Qué comando o comandos usaste en el punto 33?
R: He usado un git log para saber el SHA del commit al cual queremos ir y,
posteriormente he usado un git checkout 2094481b6fb673d14c4484fe2a526fa5de2c0574.
