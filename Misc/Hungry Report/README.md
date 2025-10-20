# Hungry Report
## 100 points

### Challenge:
<img width="401" height="683" alt="image" src="https://github.com/user-attachments/assets/2209592a-46be-4b1b-a1a6-de0ad108f4c3" />

### Solution:
Download *ImportantFolder.png*. Check the file type.

<img width="1036" height="707" alt="image" src="https://github.com/user-attachments/assets/e9fd266f-6776-419c-af31-7fe1534b202e" />

</br> Appears to be a ZIP file. Unzip the file.

<img width="1537" height="747" alt="image" src="https://github.com/user-attachments/assets/b64da268-e579-47ca-bf1d-5945d7376ac2" />

</br> We get *Research_Report.docx*. Open the file.

<img width="975" height="627" alt="image" src="https://github.com/user-attachments/assets/fdb1c95f-2f8d-4728-ad79-420f743e7edc" />

</br> It asks for a password. Checking the Challenge Statement, there's a Riddle that hints about something:
*What is orange and sounds like a parrot?*

I'm guessing *carrot*. Use that as the password and the file opens.

<img width="1021" height="556" alt="Screenshot 2025-10-20 182055" src="https://github.com/user-attachments/assets/5e9d1f12-40ac-46e9-81be-a62cf71037bc" />

</br>There seems to be some hidden text near the end of the file. Change the font colour to black.

<img width="1114" height="409" alt="Screenshot 2025-10-20 182315" src="https://github.com/user-attachments/assets/5fa88584-a4a4-45d1-91cb-f59b5493c920" />

</br>Looks (obviously) to be a fake flag. Check into the Properties page using any Word editor (I'm using WPS here).

<img width="364" height="483" alt="Screenshot 2025-10-20 182426" src="https://github.com/user-attachments/assets/0e6a7e35-203c-4270-827d-6d00b750276c" />

</br>Looks to be base64 (we can know since there's an "=" at the end). Copy-paste all the text (except the Author) into CyberChef and decode from Base64.

<img width="1536" height="699" alt="Screenshot 2025-10-20 182829" src="https://github.com/user-attachments/assets/f49b776f-1009-4668-b583-0264ae04ba3a" />

</br>The flag is `gcsm2024{w0rds_1s_my_specialty}`
