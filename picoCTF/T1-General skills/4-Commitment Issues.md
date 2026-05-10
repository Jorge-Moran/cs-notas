# Commitment Issues
## Descripción


## Solución

```
┌──(jorge㉿kali)-[~/Escritorio]
└─$ wget https://artifacts.picoctf.net/c_titan/139/challenge.zip

┌──(jorge㉿kali)-[~/Escritorio]
└─$ ls
challenge.zip
                                                                             
┌──(jorge㉿kali)-[~/Escritorio]
└─$ unzip challenge.zip

┌──(jorge㉿kali)-[~/Escritorio]
└─$ cd drop-in 

┌──(jorge㉿kali)-[~/Escritorio]
└─$ ls
message.txt

┌──(jorge㉿kali)-[~/Escritorio]
└─$ cat message.txt
TOP SECRET

┌──(jorge㉿kali)-[~/Escritorio/drop-in]
└─$ git show            
commit 144fdc44b09058d7ea7f224121dfa5babadddbb9 (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:06:25 2024 +0000

    remove sensitive info

diff --git a/message.txt b/message.txt
index 3a71673..d552d1e 100644
--- a/message.txt
+++ b/message.txt
@@ -1 +1 @@
-picoCTF{s@n1t1z3_ea83ff2a}
+TOP SECRET
```

picoCTF{s@n1t1z3_ea83ff2a}
## Notas adicionales

Con "git show" muestra el ultimo commit con diferencia al anterior lo que no permite encontrar la flag antes de que cambiara con el commit
## Referencias

https://primer.picoctf.org/#_git_version_control
