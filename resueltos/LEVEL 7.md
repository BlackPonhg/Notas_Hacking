
## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**

## Datos de acceso al nivel
**Servidor: bandit7@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Solución
bandit7@bandit:~$ wc data.txt
  98567  197133 4184396 data.txt
bandit7@bandit:~$ wc -l data.txt
98567 data.txt
bandit7@bandit:~$ grep millionth data.txt
millionth       dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
## Notas adicionales
**`grep`**: Busca un patrón específico dentro de un archivo o entrada. `grep` recibe como argumento un patrón (una cadena de texto o una expresión regular) y muestra todas las líneas que coincidan con ese patrón.
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


