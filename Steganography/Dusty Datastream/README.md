# Dusty Datastream
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/1e1c69fc-c77e-4e3b-887b-379b9ce7a674)

### Solution:
Download the JPG `ACMESignCo.jpg`. If we open the image, it shows nothing much.

![image](https://github.com/user-attachments/assets/a50b2323-7166-4950-a2e5-c37f38f023df)

Checking the metadata using `exiftool` and we get a lot of mentions of "404".

![image](https://github.com/user-attachments/assets/c652d802-c0af-4054-94d7-9300d832c5b1)

Could be important, like a password. Maybe there's something hidden inside the image. I use [steghide](https://www.kali.org/tools/steghide/).

![image](https://github.com/user-attachments/assets/b8c2d7f7-8b0f-4693-8ae3-60dcc3c5522f)

It asks for a passphrase. I wonder what could it be?

![image](https://github.com/user-attachments/assets/e4a5fe48-eed6-4958-934d-289d49696a1d)

Opening `flag.txt` gives us the flag. Flag is `gcsm2024{som3one_pl3a$e_h3lp_m3}`
