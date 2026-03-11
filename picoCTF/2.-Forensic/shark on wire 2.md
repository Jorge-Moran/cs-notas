# shark on wire 2
# Descripción
We found this [packet capture](https://challenge-files.picoctf.net/c_fickle_tempest/d2051a169bcab758191e43355c6954ae40a96b0791d75ad33737c7e9ca42703b/capture.pcap). Recover the flag.

# Solución
picoCTF{p1LLf3r3d_data_v1a_st3g0}
```
jorge_moran-picoctf@webshell:~$ tshark -r capture.pcap.1 -Y "udp.srcport == 5000" -T fields -e udp.dstport | head -n 20
9999
9999
9999
9999
8888
8888
8888
8888
8888
8888
8888
8888
8888
8990
8990
8990
8990
8990
8990
8990
jorge_moran-picoctf@webshell:~$ tshark -r capture.pcap.1 -Y "udp.dstport == 5000" -T fields -e udp.srcport | head -n 20
jorge_moran-picoctf@webshell:~$ tshark -r capture.pcap.1 -T fields -e udp.srcport | while read p; do python3 -c "n=$p-5000; print(chr(n), end='') if 32<=n<=126 else None" 2>/dev/null; done
paaaaaicoCTF{p1LLf3aaaaar3daa_adaata_v1a_staaa3gaaaa0}aaaaaaaajorge_moran-picoctf@webshell:~$ 
```

# Notas Adicionales 
- Para obtener los puertos en los cuales buscar se utilizo wshark

# Referencias 
- Sin referencias.
