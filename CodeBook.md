
## obejetivo
Run the Python script `code.py` in the same directory as `codebook.txt`.

- [Download code.py](https://artifacts.picoctf.net/c/2/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/2/codebook.txt)

##solución
──(kali㉿kali)-[~/Documents/Codebook]
└─$ wget https://artifacts.picoctf.net/c/2/codebook.txt
--2024-09-17 19:49:01--  https://artifacts.picoctf.net/c/2/codebook.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 18.154.144.85, 18.154.144.103, 18.154.144.107, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|18.154.144.85|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 27 [application/octet-stream]
Saving to: ‘codebook.txt’

codebook.txt            100%[==============================>]      27  --.-KB/s    in 0s      

2024-09-17 19:49:01 (75.3 MB/s) - ‘codebook.txt’ saved [27/27]

                                                                                               
┌──(kali㉿kali)-[~/Documents/Codebook]
└─$ ls   
codebook.txt  code.py
                                                                                               
┌──(kali㉿kali)-[~/Documents/Codebook]
└─$ python3 code.py 
picoCTF{c0d3b00k_455157_7d102d7a}
                                                                                               
┌──(kali㉿kali)-[~/Documents/Codebook]
└─$ 
                                                                                               
┌──(kali㉿kali)-[~/Documents/Codebook]
└─$ picoCTF{c0d3b00k_455157_7d102d7a}


## Notas adicionales
On the webshell, use `ls` to see if both files are in the directory you are in
The `str_xor` function does not need to be reverse engineered for this challenge.
## Referencias

