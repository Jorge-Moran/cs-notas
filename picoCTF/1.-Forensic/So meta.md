# So meta
# Descripción
Find the flag in this [picture](https://challenge-files.picoctf.net/c_fickle_tempest/5a0c9a73ac940fb0369275fcf8600f02af2e8d732dd178e19ed8ea8f223d65db/pico_img.png).

# Solución
```
jorge_moran-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_tempest/5a0c9a73ac940fb0369275fcf8600f02af2e8d732dd178e19ed8ea8f223d65db/pico_img.png
--2026-03-09 14:11:59--  https://challenge-files.picoctf.net/c_fickle_tempest/5a0c9a73ac940fb0369275fcf8600f02af2e8d732dd178e19ed8ea8f223d65db/pico_img.png
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.18, 3.160.5.95, 3.160.5.40, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 108795 (106K) [application/octet-stream]
Saving to: 'pico_img.png'

pico_img.png         100%[====================>] 106.25K  --.-KB/s    in 0.05s   

2026-03-09 14:11:59 (2.10 MB/s) - 'pico_img.png' saved [108795/108795]

jorge_moran-picoctf@webshell:~$ exiftool pico_img.png
ExifTool Version Number         : 12.40
File Name                       : pico_img.png
Directory                       : .
File Size                       : 106 KiB
File Modification Date/Time     : 2025:11:21 19:11:02+00:00
File Access Date/Time           : 2026:03:09 14:11:59+00:00
File Inode Change Date/Time     : 2026:03:09 14:11:59+00:00
File Permissions                : -rw-rw-r--
File Type                       : PNG
File Type Extension             : png
MIME Type                       : image/png
Image Width                     : 600
Image Height                    : 600
Bit Depth                       : 8
Color Type                      : RGB
Compression                     : Deflate/Inflate
Filter                          : Adaptive
Interlace                       : Noninterlaced
Software                        : Adobe ImageReady
XMP Toolkit                     : Adobe XMP Core 5.3-c011 66.145661, 2012/02/06-14:56:27
Creator Tool                    : Adobe Photoshop CS6 (Windows)
Instance ID                     : xmp.iid:A5566E73B2B811E8BC7F9A4303DF1F9B
Document ID                     : xmp.did:A5566E74B2B811E8BC7F9A4303DF1F9B
Derived From Instance ID        : xmp.iid:A5566E71B2B811E8BC7F9A4303DF1F9B
Derived From Document ID        : xmp.did:A5566E72B2B811E8BC7F9A4303DF1F9B
Artist                          : picoCTF{s0_m3ta_ba6c953a}
Image Size                      : 600x600
Megapixels                      : 0.360
jorge_moran-picoctf@webshell:~$ 
```

# Notas Adicionales 
- Sin notas adicionales

# Referencias
- No referencias.