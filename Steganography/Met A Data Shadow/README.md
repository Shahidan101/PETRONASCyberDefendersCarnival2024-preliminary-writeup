# Met A Data Shadow
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/26850ac2-951d-497f-9f55-2ee29a58a180)

### Solution:
Download `V1g.png`. Start with getting the metadata. I use `exiftool`.

![image](https://github.com/user-attachments/assets/6ebe4d9e-dbe9-4a96-b0b5-50f682010066)

The ChatGPT link doesn't do much. User comment looks to be the flag, but encrypted.

The artist is "Mr Vignere", which references to the [Vigenere Cipher](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher).

Use [CyberChef](https://gchq.github.io/CyberChef/) to decode it.

![image](https://github.com/user-attachments/assets/7ed88e0d-e0cd-499a-b415-122e22a9cead)

We need a key. Looking at the metadata earlier, we see that
>if 1 = 1 then key = ?

key = key. So we use "key" as the key and we get the flag.

The flag is `gcsm2024{4lw4ys_ch3ck_th3_m3t4d4t4}`
