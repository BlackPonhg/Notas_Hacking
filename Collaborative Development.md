
## Objetivo
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

## Solución
```
ricardogarcia-picoctf@webshell:~$                                                                                                                               
ricardogarcia-picoctf@webshell:~/drop-in$ ls
challenge.zip  drop-in
ricardogarcia-picoctf@webshell:~/drop-in$ cd drop-in/     
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ ls
flag.py
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git branch -a
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git checkout 
HEAD             feature/part-2   main 
feature/part-1   feature/part-3   
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ python flag.py 
Printing the flag...
picoCTF{t3@mw0rk_
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ ls
flag.py
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ python flag.py
Printing the flag...
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git branch -a
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ python 
.git/    flag.py  
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ python flag.py 
Printing the flag...
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$ python flag.py 
Printing the flag...
w0rk_7ffa0077}
ricardogarcia-picoctf@webshell:~/drop-in/drop-in$

```

## Notas adicionales
`git branch -a` will let you see available branches

How can file 'diffs' be brought to the main branch? Don't forget to `git config`!

Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


