
## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.

## Datos de acceso al nivel
Servidor: bandit9@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## Solución
bandit9@bandit:~$ ls
data.txt
bandit9@bandit:~$ file data.txt
data.txt: data
bandit9@bandit:~$ strings data.txt | grep ==
\a!;========== the
========== passwordf
========== isc
========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
bandit9@bandit:~$
## Notas adicionales
grep
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1 y chatGPT

