
## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size
## Datos de acceso al nivel
**Servidor: bandit6@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Solución
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
bandit6@bandit:~$
## Notas adicionales
- `find /` - Le indica al comando `find` que comience a buscar en el directorio raíz `/`, lo cual hace que la búsqueda se realice en todo el sistema de archivos.
    
- `-user bandit7` - Filtra los resultados para mostrar únicamente los archivos que pertenecen al usuario `bandit7`.
    
- `-group bandit6` - Filtra los resultados para que solo se muestren los archivos que pertenezcan al grupo `bandit6`.
    
- `-size 33c` - Filtra los resultados para que solo se muestren los archivos que tengan un tamaño exacto de 33 bytes (`c` indica que se mide en bytes).
    
- `2>/dev/null` - Redirige cualquier mensaje de error generado durante la búsqueda (como los permisos denegados) al dispositivo especial `/dev/null`, que es una especie de "basurero" digital, donde se descartan los datos. Esto evita que los errores se muestren al usuario, manteniendo la salida limpia.
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1 y chatgpt.


