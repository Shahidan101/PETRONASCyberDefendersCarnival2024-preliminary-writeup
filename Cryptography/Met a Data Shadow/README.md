# Met A Data Shadow 
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/75c8647b-cfc3-47e0-b5b8-c27b340eb2fa)

### Solution:
The given file is 

![V1g](https://github.com/user-attachments/assets/aa090972-ea9c-48aa-a905-3876e20fb22f)

To solve this we would have to take .png file and put into and exiftool to read the metadata. (https://exif.tools/)

![image](https://github.com/user-attachments/assets/89bb28fd-2b19-463e-9cfa-9f304ac3eb31)

The metadata shows {4va4wc_gf3mo_rr3_q3r4n4x4}, you can get hint on what type of cipher from the artist name: Vignere's Cipher or you can use dCOde to identify the cipher.

Vignere's cipher requires a key, the hint in the metadata is 1=1 key=?. key=key.

Using cyberchef: 
![image](https://github.com/user-attachments/assets/fa43db34-2d8b-4f46-9445-8b2d7f07f2fe)

The flag is `gcsm2024{4lw4ys_ch3ck_th3_m3t4d4t4}`

