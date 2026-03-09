# Extensions
# Descripción
This is a really weird text file. Can you find the flag?Get the flag from [TXT](https://challenge-files.picoctf.net/c_fickle_tempest/31fe772e6a4c71e867af0b2a93818e06d8f8ebf8af2a9615495d00356ff576da/flag.txt).

# Solución
```
picoCTF{now_you_know_about_extensions}
```

# Notas Adicionales 
- Se tuvo que descargar la imagen, posteriormente se tuvo que convertir a PNG ya que en un principio se descargaba un archivo file.txt
```
jorge_moran-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_tempest/31fe772e6a4c71e867af0b2a93818e06d8f8ebf8af2a9615495d00356ff576da/flag.txt
--2026-03-09 14:28:18--  https://challenge-files.picoctf.net/c_fickle_tempest/31fe772e6a4c71e867af0b2a93818e06d8f8ebf8af2a9615495d00356ff576da/flag.txt
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.40, 3.160.5.64, 3.160.5.18, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.40|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9984 (9.8K) [application/octet-stream]
Saving to: 'flag.txt'

flag.txt             100%[====================>]   9.75K  --.-KB/s    in 0.001s  

2026-03-09 14:28:18 (13.2 MB/s) - 'flag.txt' saved [9984/9984]

jorge_moran-picoctf@webshell:~$ file flag.txt
flag.txt: PNG image data, 1697 x 608, 8-bit/color RGB, non-interlaced
jorge_moran-picoctf@webshell:~$ mv flag.txt flag.png
```

# Referencias
- No referencias.