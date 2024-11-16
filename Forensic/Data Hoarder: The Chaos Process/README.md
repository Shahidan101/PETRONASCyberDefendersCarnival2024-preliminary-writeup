# Data Hoarder: The Chaos Process
## 150 points

### Challenge:
![image](https://github.com/user-attachments/assets/f6d61f97-0400-417f-8bef-b19a7a948e12)

### Solution:
We are given a registry file `persistence.zip` to analyse. Extract the zip and you'll find `persistence.reg`.

PLEASE FOR THE LOVE OF [SNOWDEN](https://en.wikipedia.org/wiki/Edward_Snowden) DON'T OPEN/EXECUTE THE FILE (unless you want a [BSOD](https://en.wikipedia.org/wiki/Blue_screen_of_death).)

Registry files may look intimidating (and rightfully so when executed without knowing what it does), they are essentially text files that run commands.

Open the registry file using a text editor. I recommend [Notepad++](https://notepad-plus-plus.org/). I personally just used `cat` in the Terminal.

![image](https://github.com/user-attachments/assets/e1b6742f-078e-4be5-8a7f-654815e6b370)

The text is huge with different registry entries. Looking at the challenge description, we find that:
>...it burries its secrets in the system's startup registry to ensure it keeps coming back.

We need to find the registry entry that runs during startup. A quick Google search shows this [link](https://devblogs.microsoft.com/powershell/how-to-access-or-modify-startup-items-in-the-window-registry/).

In the registry file, look for `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run]`.

![image](https://github.com/user-attachments/assets/fa572cf6-686e-4896-8b81-627e42dd3d4e)

The flag is `gcsm2024{pers1st3nce_l0cat1on}`
