# KC_Practica-GitHub
Práctica del curso de GitHub

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

   <git reset --hard HEAD~1>
   Para deshacer el último commit y restaurar el estado inicial.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

   <git reset --hard "ID del commit">
   Para restaurar el repositoria al estado exacto en que estaba en este commit.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

   En este punto no tuve ningún conflicto. Los pasos que seguí fue:
   1. Git branch (para asegurar que estoy en la raman "styled")
   2. Git fetch origin
   3. git checkout main
   4. git pull origin main
   5. git checkout styled
   6. git merge main

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

   Junto estos dos puntos, para dar una explicación más completa:
    En el punto 19 tuve un conflicto, porque había cambios en la misma línea del archivo "git-nuestro.md" en ambas ramas. 
    Y git no puede decidir cual es el correcto. Por lo que dejamos la versión de Styled.
    Una vez cambiado, no tuvimos más conflicto en el paso 21. 

- ¿Qué comando o comandos utilizaste en el paso 25?

   <git log --online --graph --all -- decorate>
   Además hice un comando alias -> <git config alias.graphlog "log --online --graph --all --decorate">
   y después lo hice "global" -> <git config --global alias.graphlog "...">

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

  Diría que no, porque para poder hacer un "fast forward" la relación entre "main" y "title" debería ser lineal, sin commits adicionales entre estos, y este
  no es el caso.

- ¿Qué comando o comandos utilizaste en el paso 27?

   <git reset --merge>
   <git log --oneline> -> Para revisar los commits recientes.

- ¿Qué comando o comandos utilizaste en el paso 28?

   <git reflog> -> para revisar el historial
   <git reset --hard "ID del commit"> -> para restaurar commit antes del reset.

- ¿Qué comando o comandos utilizaste en el paso 29?

  <git push origin --delete title>

- ¿Qué comando o comandos utilizaste en el paso 30?

   Mismo que el punto 28.

- ¿Qué comando o comandos usaste en el paso 32?

   <git reset --hard "ID del commit"

- ¿Qué comando o comandos usaste en el punto 33?

   lo mismo que el punto 32, pero cambiando el "ID del commit"por el del estado final.
