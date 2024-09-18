
## Objetivo
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is **bandit.labs.overthewire.org**, on port 2220. The username is **bandit0** and the password is **bandit0**. Once logged in, go to the [Level 1](https://overthewire.org/wargames/bandit/bandit1.html) page to find out how to beat Level 1.


## Solución
```
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ wget https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static
--2024-09-17 22:03:22--  https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 8376 (8.2K) [application/octet-stream]
Saving to: ‘static’

static                      100%[========================================>]   8.18K  --.-KB/s    in 0s      

2024-09-17 22:03:23 (193 MB/s) - ‘static’ saved [8376/8376]

                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ wget https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh
--2024-09-17 22:03:33--  https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 785 [application/octet-stream]
Saving to: ‘ltdis.sh’

ltdis.sh                    100%[========================================>]     785  --.-KB/s    in 0s      

2024-09-17 22:03:34 (46.6 MB/s) - ‘ltdis.sh’ saved [785/785]

                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ ls
ltdis.sh  static
                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ cat static
 HH/lib64/ld-linux-x86-64.so.2GNUGNU��A+�kpl%h��B0m�'= 
                                                       Y h "libc.so.6puts__cxa_finalize__libc_start_mainGLIBC � � � � � � H�H��terTMCloneTable__gmon_start___ITM_registerTMCloneTableu▒i     1�
 H��t��H���5�
 �%�
 @�%�
 h������%�
8#TT 1tt$D���o�NPTL��H�
�� � @ @ �0@)▒  p�▒V``�^y▒�                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ cat ltdis.sh 
#!/bin/bash



echo "Attempting disassembly of $1 ..."


#This usage of "objdump" disassembles all (-D) of the first file given by 
#invoker, but only prints out the ".text" section (-j .text) (only section
#that matters in almost any compiled program...

objdump -Dj .text $1 > $1.ltdis.x86_64.txt


#Check that $1.ltdis.x86_64.txt is non-empty
#Continue if it is, otherwise print error and eject

if [ -s "$1.ltdis.x86_64.txt" ]
then
        echo "Disassembly successful! Available at: $1.ltdis.x86_64.txt"

        echo "Ripping strings from binary with file offsets..."
        strings -a -t x $1 > $1.ltdis.strings.txt
        echo "Any strings found in $1 have been written to $1.ltdis.strings.txt with file offset"



else
        echo "Disassembly failed!"
        echo "Usage: ltdis.sh <program-file>"
        echo "Bye!"
fi
                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ chmod +x ltdis.sh

                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ ./ltdis.sh static

Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
                                                                                                             
┌──(kali㉿kali)-[~/Documents/retos/staticaint]
└─$ grep "picoCTF" static.ltdis.strings.txt

   1020 picoCTF{d15a5m_t34s3r_f6c48608}

```
]]
## Notas adicionales
Al acceder por primera vez se pide agregar el servidor a la lista de hosts conocidos, al ingresar estamos en un servidor de Linux para pruebas

## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


