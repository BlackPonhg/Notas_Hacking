
## Objetivo
BookShelf Pico, my premium online book-reading service. I believe that my website is super secure. I challenge you to prove me wrong by reading the 'Flag' book!

Additional details will be available after launching your challenge instance.
## Solución

![[Pasted image 20241026203707.png]]
## Notas adicionales
Maybe try to find the JWT Signing Key ("secret key") in the source code? Maybe it's hardcoded somewhere? Or maybe try to crack it?
The 'role' and 'userId' fields in the JWT can be of interest to you!
	The 'controllers', 'services' and 'security' java packages in the given source code might need your attention. We've provided a README.md file that contains some documentation.
Upgrade your 'role' with the _new_ (cracked) JWT. And re-login for the new role to get reflected in browser's localStorage.
## Referencias
https://youtu.be/kMp_-ePwEC4?si=fJoHyB4vu_arEoW1


