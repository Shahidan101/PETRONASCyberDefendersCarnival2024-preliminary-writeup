# Color QR
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/bee7ecbd-d71a-4b7a-a09e-844b8f787375)

### Solution:
Download `QR.png`. If we scan the QR code, we'll get the first part of the flag `_th4_`.

We need to change the colours of the QR to get different parts of the flag. I used [StegSolve](https://github.com/manisashank/stegsolve/blob/master/process%20to%20install%20stegsolve).

![image](https://github.com/user-attachments/assets/96be0832-885d-44a5-b7b0-2a404f1f0e9b)

Cycle through the different colour modes and adjustments until we get a different QR flag.

`Red plane 7` gets us `gcsm2024{c0l0r`

![image](https://github.com/user-attachments/assets/5a4c1c09-90b2-4009-b4f7-749a3d1eefce)

`Blue plane 7` gets us `QR}`

![image](https://github.com/user-attachments/assets/a0f3d261-4b65-4f5c-9915-95c62ed86f1d)

The flag is `gcsm2024{0l0r_th4_QR}`
