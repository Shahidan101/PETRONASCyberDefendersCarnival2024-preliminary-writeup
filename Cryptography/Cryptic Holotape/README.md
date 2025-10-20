# Cryptic Holotape
## 100 points

### Challenge:
<img width="388" height="676" alt="image" src="https://github.com/user-attachments/assets/a09c85b4-5f3c-457f-8c6f-1303e5fe2adb" />

### Solution:
You're given a dump of binary numbers. There's clues in the challenge statement that mentions **rotating**, could indicate a ROT Cipher.

Let's try [dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier). 

<img width="1025" height="573" alt="image" src="https://github.com/user-attachments/assets/f4018767-711e-4cfb-9983-983651c90b28" />

</br>Looks to be **Spoon Language** (which is hinted from the challenge statement about *utensil*). Use dCode again to decode from Spoon.

<img width="993" height="598" alt="image" src="https://github.com/user-attachments/assets/4de54632-a24a-4ade-aae9-fe3db3e89aa0" />

</br>We get `gcsm2024{DA@@?0E96?0C@E0EH:DED0>J03C2:?}`. Let's now try a ROT Cipher decode on [CyberChef](https://gchq.github.io/CyberChef/). You can use dCode Cipher Identifier to check what ROT value it is. The correct one for this case is ROT47.

<img width="1521" height="611" alt="image" src="https://github.com/user-attachments/assets/9d48cfae-ea54-4304-b4db-dcc0b7ba725c" />

</br>The flag is `gcsm2024{spoon_then_rot_twists_my_brain}`.
