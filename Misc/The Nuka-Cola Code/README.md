# The Nuka-Cola Code
## 50 points

### Challenge:
<img width="499" height="668" alt="image" src="https://github.com/user-attachments/assets/baa7f4c9-748b-4ad8-bdcd-a18c9b3a31a2" />

### Solution:
Open *STOP_PLEASE.txt*. Looks to be a bunch of text that looks like spam.

I tried lots of things:
* Filtering out only Capital Letters and seeing if it's anything important
* Splitting the entire text by space and converting it all to binary, decimal, hex
* Counting the number of characters for each word, separated by space, then seeing if it's something in decimal, binary, hex
* Running them through CyberChef Magic

Turns out Spam is an encoding in its own. It uses linguistic steganography to hide a message. Instead of encrypting the message, it hides the fact that a secret message exists at all. The technical details of it is in using a mimic function. More can be learned through Google or asking AI.

Use this [website](https://www.spammimic.com/decode.shtml). Paste in the entire text and click "Decode".

<img width="1117" height="903" alt="image" src="https://github.com/user-attachments/assets/4f88ce7e-8c18-4f74-8d7e-cf5daa637661" />

<img width="1130" height="596" alt="image" src="https://github.com/user-attachments/assets/e7d79479-8e60-40da-8c3a-3318bd64a078" />

</br>The flag is `gcsm2024{d0nt_$p4m_m3_P1ea$e}`.
