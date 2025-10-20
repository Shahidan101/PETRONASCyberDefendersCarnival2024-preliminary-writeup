# Radioactive Recon
## 100 points

### Challenge:
<img width="359" height="661" alt="image" src="https://github.com/user-attachments/assets/cfc51c0c-97e8-47df-a3fc-9c3158617ad3" />
<img width="358" height="659" alt="image" src="https://github.com/user-attachments/assets/84737d90-9373-43bb-9d8e-661d1a66c346" />

### Solution:
Ignore the chitty-chat-chat. The cipher is `jfvp2024{5huhfw_f@fk3}`.

If you're a psycho that remembers what alphabet corresponds to what number (I know one such psycho), you'll notice that the characters are shifted forward by 3.

Since we know the flag format is `gcsm2024`, that means `jfvp2024` would be decoded to the flag format. If you shift each alphabet of the encrypted text backwards by 3, you get:
```
g --> j
c --> f
s --> v
m --> p
```
and so on.

Of course, we can just not bother and brute-foce ROT on [CyberChef](https://gchq.github.io/CyberChef/).
<img width="1910" height="893" alt="image" src="https://github.com/user-attachments/assets/36a10af4-8ef4-4a06-b132-ca94b884a865" />

</br>The flag is `gcsm2024{5erect_c@ch3}`.
