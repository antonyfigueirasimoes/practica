# Practica git

11 - git reset --hard HEAD~1. Porque queriamos eliminar el ultimo commit que habíamos hecho (HEAD~1) incluyendo todo lo que teníamos hecho en el working copy

12 - git reflog para encontrar el # del commit y git reset --hard (# del commit) para eliminar todos los cambios hechos luego de ese commit

13 - No nos da conflicto porque el ultimo commit de styled ya tiene todos los cambios que están en 'main'. 

19 - Si, me ha dado conflicto ya que se le habría modificado las mismas línes de texto en el mismo archivo de las dos ramas. Hay que resolver el conflicto modificando el archivo y decidiendo cual es el contenido que queremos mantener.

21 - No nos da conflicto porque todos los cambios de styled ya estaban incluidos en main.

25 - Usé git log --graph --all

26 - No sería posible realizar un fast-forward merge en este caso ya que la rama title tiene commits adicionales que no están en main

27 - Usamos git reset --soft HEAD~1 para deshacer el ultimo commit y mantener los cambios en el working copy.

28 - Usamos git reset --hard HEAD~1 para eliminar los cambios en el working copy y regresar al estado del commit anterior al merge

29 - Usamos git branch -D title, ya que descartamos previamente el merge con esa rama y no tenemos el commit de title en main

30 - Usamos git reflog para encontrar el # del commit donde realizamos el merge. Luego hacemos un git reset --hard (# commit) para volver a donde estabamos

32 - Usamos git log para encontrar el # del commit donde adicionamos el poema. Hacemos un git reset --hard (# commit) para volver a donde estabamos

33 - Usamos git reflog para encontrar el # del commit donde pusimos titulo al poema. Luego hacemos un git reset --hard (# commit) para volver a donde estabamos

