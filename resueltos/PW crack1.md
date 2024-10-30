
## Objetivo
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is **bandit.labs.overthewire.org**, on port 2220. The username is **bandit0** and the password is **bandit0**. Once logged in, go to the [Level 1](https://overthewire.org/wargames/bandit/bandit1.html) page to find out how to beat Level 1.


## Solución

```
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ wget https://artifacts.picoctf.net/c/12/level1.py
--2024-09-17 20:24:07--  https://artifacts.picoctf.net/c/12/level1.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.225.62, 3.161.225.60, 3.161.225.3, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.225.62|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 876 [application/octet-stream]
Saving to: ‘level1.py’

level1.py                                                  100%[========================================================================================================================================>]     876  --.-KB/s    in 0s      

2024-09-17 20:24:08 (50.0 MB/s) - ‘level1.py’ saved [876/876]

                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ wget https://artifacts.picoctf.net/c/12/level1.flag.txt.enc
--2024-09-17 20:24:18--  https://artifacts.picoctf.net/c/12/level1.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.225.11, 3.161.225.3, 3.161.225.60, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.225.11|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 30 [application/octet-stream]
Saving to: ‘level1.flag.txt.enc’

level1.flag.txt.enc                                        100%[========================================================================================================================================>]      30  --.-KB/s    in 0s      

2024-09-17 20:24:18 (76.7 MB/s) - ‘level1.flag.txt.enc’ saved [30/30]

                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ ls
level1.flag.txt.enc  level1.py
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ pthon3 level1.
Command 'pthon3' not found, did you mean:
  command 'python3' from deb python3-minimal
Try: sudo apt install <deb name>
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python3 level1.
python3: can't open file '/home/kali/Documents/retos/PWcrack1/level1.': [Errno 2] No such file or directory
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ ls   
level1.flag.txt.enc  level1.py
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python lebel1.py
python: can't open file '/home/kali/Documents/retos/PWcrack1/lebel1.py': [Errno 2] No such file or directory
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python3 level1.py
Please enter correct password for flag: str_xor 
That password is incorrect
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python3 level1.py
Please enter correct password for flag: nano
That password is incorrect
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ nano level1.py
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python3 level1.py
Please enter correct password for flag: 
That password is incorrect
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~/Documents/retos/PWcrack1]
└─$ python3 level1.py
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}

```
## Notas adicionales
Al acceder por primera vez se pide agregar el servidor a la lista de hosts conocidos, al ingresar estamos en un servidor de Linux para pruebas

## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


