
## Objetivo
Let's start off simple, can you overflow the correct buffer? The program is available [here](https://artifacts.picoctf.net/c/174/vuln). You can view source [here](https://artifacts.picoctf.net/c/174/vuln.c).

Additional details will be available after launching your challenge instance.

## Solución

![[Pasted image 20241112232650.png]]
## Notas adicionales
How can you trigger the flag to print?
If you try to do the math by hand, maybe try and add a few more characters. Sometimes there are things you aren't expecting.

Run `man gets` and read the BUGS section. How many characters can the program really read?
## Referencias



