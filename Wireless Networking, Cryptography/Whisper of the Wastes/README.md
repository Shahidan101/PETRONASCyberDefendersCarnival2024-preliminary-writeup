# Whisper of the Wastes
## 200 points 

### Challenge:
![image](https://github.com/user-attachments/assets/da3238af-ffa5-460a-9939-ea89375a8a9a)

### Solution:
Download the CAP file `ctfwifi.cap`.

The challenge description is hinting about hacking a Wi-Fi password. It could be possible to analyse the traffic by using [Wireshark](https://www.wireshark.org/) on the CAP file.

Alternatively, if you're using Kali Linux, there are built-in tools to crack Wi-Fi passwords from CAP files. One of such tools is [aircrack-ng](https://www.aircrack-ng.org/).

In a Kali terminal, enter `sudo aircrack-ng -w '/usr/share/wordlists/rockyou.txt' 'ctfwifi.cap'`

> ShahidanExplains:
> - `sudo` is esentially "Run as Administrator" in Linux. It stands for SuperUser Do.
> - `aircrack-ng` is the tool name in command-line.
> - `-w` is the option used to indicate worldlist to be used. Wordlists are text files containing a large collection of words, phrases, passwords, or other data - one per line. The tool will use wordlist and brute-forces the Wi-Fi password.
> - `/usr/share/wordlists/rockyou.txt` is the location of `rockyou.txt` in Kali Linux. It is a well-known wordlist. There are other wordlists in `/usr/share/wordlists`
> - `ctfwifi.cap` is the target CAP file we intend to crack.

After executing the command, you'll see the tool hacking the password like it's straight out of [Mr. Robot](https://www.imdb.com/title/tt4158110/). After a while, the tool successfully cracks the password.

![image](https://github.com/user-attachments/assets/5cbe8358-eb4b-4e2e-b1cb-9580513271c3)

The flag is `gcsm2024{idonotknow}`
