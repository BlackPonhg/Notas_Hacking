
## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:

## Datos de acceso al nivel
Servidor: bandit5@bandit.labs.overthewire.org -p 2220
Constraseña del nivel: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## Solución
bandit5@bandit:~/inhere$ find . -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Notas adicionales
ls -r muestra los archivo de manera recursiva 
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


