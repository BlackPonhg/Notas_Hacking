
## Objetivo
Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/505/big-zip-files.zip)


## Solución

ricardogarcia-picoctf@webshell:~$ unzip big-zip-files.zip 
...
...
...
ricardogarcia-picoctf@webshell:~$ ls
README.txt  big-zip-files  big-zip-files.zip
ricardogarcia-picoctf@webshell:~$ grep -r "pico" big-zip-files
big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode 
## Notas adicionales
Can grep be instructed to look at every file in a directory and its subdirectories?
## Referencias



