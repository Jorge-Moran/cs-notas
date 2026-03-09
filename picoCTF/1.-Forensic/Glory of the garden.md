# Glory of the garden
# Descripción
This file contains more than it seems.Get the flag from [garden.jpg](https://challenge-files.picoctf.net/c_fickle_tempest/150b6eaad43200d3dc91f98c390e4c6168620b57d0b95a7e9d04c92910bbbe16/garden.jpg).

# Solución
```
jorge_moran-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_
tempest/150b6eaad43200d3dc91f98c390e4c6168620b57d0b95a7e9d04c92910bbbe16/garden.jp
g
--2026-03-09 14:06:30--  https://challenge-files.picoctf.net/c_fickle_tempest/150b6eaad43200d3dc91f98c390e4c6168620b57d0b95a7e9d04c92910bbbe16/garden.jpg
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.40, 3.160.5.64, 3.160.5.18, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.40|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 2295191 (2.2M) [application/octet-stream]
Saving to: 'garden.jpg'

garden.jpg           100%[====================>]   2.19M  1.83MB/s    in 1.2s    

2026-03-09 14:06:31 (1.83 MB/s) - 'garden.jpg' saved [2295191/2295191]

jorge_moran-picoctf@webshell:~$ strings garden.jpg | grep "picoCTF"
Here is a flag: picoCTF{more_than_m33ts_the_3y3a63b5b27}
```

# Notas Adicionales 
- Sin notas adicionales

# Referencias
- No referencias.