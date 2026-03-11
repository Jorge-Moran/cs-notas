# WhitePages
# Descripción
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://challenge-files.picoctf.net/c_fickle_tempest/ab5453de03105a8aab9c68b0b46e66a4fe0a781c3915ab519f7fab31b3ce6894/whitepages.txt) is all blank!

# Solución
```
jorge_moran-picoctf@webshell:~$ python3 -c "import sys; data = open('whitepages.txt', 'rb').read(); data = data.replace(b'\x20', b'0').replace(b'\xe2\x80\x83', b'1'); print(''.join(chr(int(data[i:i+8], 2)) for i in range(0, len(data), 8)))"
õ«¹õõ¬ººß¯ª½³¶¼ß­º¼°­»¬ßÙß½¾¼´¸­°ª±»ß­º¯°­«õÊÏÏÏß¹ß¾Óß¯Óß¯¾ßÎÊÍÎÌõ«¹
                                                                         ËÊËÈÊÈÉÌÇÇËÏÏÊÊÍõ
jorge_moran-picoctf@webshell:~$ ^C
jorge_moran-picoctf@webshell:~$ python3 -c "b=open('whitepages.txt','rb').read().replace(b'\xe2\x80\x83',b'0').replace(b'\x20',b'1'); print(''.join(chr(int(b[i:i+8],2)) for i in range(0,len(b)//8*8,8)))"

picoCTF

SEE PUBLIC RECORDS & BACKGROUND REPORT
5000 Forbes Ave, Pittsburgh, PA 15213
picoCTF{not_all_spaces_are_created_equal_bbc4f54c75763bd78dc840f05eb7a752}
```

# Notas Adicionales 
- Los bits estaban invertidos, es por ello que se tuvo que cambiar la linea de codigo para que no entregara los simbolos que se observaban al principio de querer obtener la bandera.

# Referencias 
- Sin referencias
