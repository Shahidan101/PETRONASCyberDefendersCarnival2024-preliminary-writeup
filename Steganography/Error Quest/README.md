# Error Quest
## 150 points

### Challenge:
![image](https://github.com/user-attachments/assets/0ab22d3d-9629-4b97-bb6e-cff5af99bdb4)

### Solution:
Download `error.png`. Looks to be an image with a huge 404 error.

![error](https://github.com/user-attachments/assets/73b3a6f0-4eb0-41e2-aa0d-641c78031159)

A good (some consider cheaty) tool for Steganography is `zsteg`.

![image](https://github.com/user-attachments/assets/c7baf0a1-e68f-4af4-b965-8515d6714fb8)

Looking through the dump, we see some text that have "_" like `hZ7_b_hZs7h`. I tried different ways to decode and couldn't get anything, so I moved on to look for something longer *(heh)*.

Scrolling further, I found `4ihZ57f_t4ibr_K8gh7Z8brsf_r7h7qhsr`. I used [dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier) and got a list of possible ciphers.

![image](https://github.com/user-attachments/assets/d2c886d0-348a-434a-81a9-033c85896ee8)

I tried ASCII85 and got nothing good. When I tried Shift Cipher, I found something suspicious.

![image](https://github.com/user-attachments/assets/16c5a649-fdaf-4b97-a381-42d225165916)

The first one `4utL57r_f4und_W8st7L8nder_d7t7cted` looks like the word "Outlier Found Wastelander Detected". Normally our flags would be in a form of geeky, hacky alphanumerics. So I tried changing the numbers according to that format.
```
4 --> 0
5 --> 1
7 --> 3
8 --> 4
# Do you see the pattern? 4 numbers down!
```

And poof, we got the flag `gcsm2024{0utL13r_f0und_W4st3L4nder_d3t3cted}`
