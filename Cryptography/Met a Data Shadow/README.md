# Met A Data Shadow 
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/75c8647b-cfc3-47e0-b5b8-c27b340eb2fa)

### Solution:
Download the image `V1g.png`.

![V1g](https://github.com/user-attachments/assets/aa090972-ea9c-48aa-a905-3876e20fb22f)

Check the metadata of the image. Use `exiftool` on Terminal or use an [online tool](https://exif.tools/).

![image](https://github.com/user-attachments/assets/89bb28fd-2b19-463e-9cfa-9f304ac3eb31)

The ChatGPT link doesn't do much. There is a suspicious string `{4va4wc_gf3mo_rr3_q3r4n4x4}` that looks like a flag (it even comes with the squiggly brackets). Looks to be encrypted.

We notice that the "Artist" in the metadata is "Mr Vignere". The image `V1g.png` is also a portrait of [Blaise de Vigenère](https://en.wikipedia.org/wiki/Blaise_de_Vigen%C3%A8re), who invented the [Vigenère cipher](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher).

Use a decrypter (I used [CyberChef](https://gchq.github.io/CyberChef/)) on the encrypted flag. Vigenère cipher requires a key. If we look at the metadata earlier under "Image Description", we're given a clue:
>if 1 = 1 then key = ?

That would be key = key. So we use `key` as the key for the decryption and get the flag.

![image](https://github.com/user-attachments/assets/fa43db34-2d8b-4f46-9445-8b2d7f07f2fe)

The flag is `gcsm2024{4lw4ys_ch3ck_th3_m3t4d4t4}`
