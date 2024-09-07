
## Objetivo
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not **/bin/bash**, but something else. Find out what it is, how it works and how to break out of it.

## Datos de acceso al nivel
Servidor: bandit9@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

## Solución
bandit25@bandit:~$ cat /etc/passwd | grep bandit26 
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext 
bandit25@bandit:~$ cat /usr/bin/showtext 
bandit25@bandit:~$ exit
logout
Connection to bandit.labs.overthewire.org closed.
## Notas adicionales

## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1 y chatGPT


