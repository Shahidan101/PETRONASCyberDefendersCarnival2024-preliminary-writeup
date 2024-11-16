# Nuclear Deterrence
## 100 points

### Challenge:
![image](https://github.com/user-attachments/assets/09f32dd3-dc36-4f25-882b-fea8cfe4121d)

### Solution:
Download `size.png`. The file is 1 pixel in size!

Opening the file, you'll get this error.

![image](https://github.com/user-attachments/assets/6eacf83e-0395-48eb-900f-ad73bc688e59)

Looks to be an error relating to the image's CRC value. You can learn more about CRC and its relation with a PNG's size [here](http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html), but essentially, the CRC checks whether the PNG is in the correct dimensions.

Let's say we modify a sample PNG's dimensions using `hexedit`, without correcting the CRC value. We'll get the same error shown earlier.

This challenge looks to have given us an image that has been modified to 1 pixel, when it's original dimensions were different.

To check the CRC value, I use `hexedit`.

![image](https://github.com/user-attachments/assets/e1c77042-62c2-41d9-9417-e7d818fba44f)

The first 8 hexadecimal values of row `00000010` indicate the Width (first 4) and Height (next 4). `80 BF 36 CC` is where the CRC is located.

We can use `pngcheck` in Kali Linux (there should be online tools for non-Kali users) to get the CRC value from the image.

![image](https://github.com/user-attachments/assets/e54401a2-afc4-4d09-920e-02e4250f35fe)

Instead of changing the current CRC value to match the image dimensions, we should change the dimensions to follow the CRC value. But how?

I didn't figure out the mathematics in time, so I used a [python script](https://github.com/Ge0rg3/ctf-png-size-solver/tree/master) online (editor's note: what is a [Script Kiddie](https://en.wikipedia.org/wiki/Script_kiddie?)?).

The tool would get us a corrected PNG file (resized to 400 x 400). Opening it would give us the flag.

The flag is `gcsm2024{m4ke_1t_b1g}`
