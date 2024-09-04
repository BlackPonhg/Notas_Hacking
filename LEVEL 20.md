
## Objetivo
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

## Datos de acceso al nivel
bandit20
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## Solución
Listening on 0.0.0.0 6666
./suconnect 6666
Connection received on 127.0.0.1 37752
Read: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Password matches, sending next password
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
[1]+  Done                    nc -lvnp 6666 <<< 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
bandit20@bandit:~$
## Notas adicionales

## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1 y chatGPT


