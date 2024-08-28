
## Objetivo
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once

## Datos de acceso al nivel
Servidor: bandit8@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## Solución
**bandit8@bandit:~$ sort data.txt | uniq -u
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM**
## Notas adicionales
- **`sort`**: Ordena las líneas de `data.txt`.
- **`uniq -u`**: Muestra solo las líneas que no se repiten, después de que hayan sido ordenadas
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


