# Fusion Core Crack I
## 150 points

### Challenge:
![image](https://github.com/user-attachments/assets/67eff8a2-a768-4149-bf6e-f2f5c978bbef)

![image](https://github.com/user-attachments/assets/1aa49363-6434-4c9b-b218-8aaf3b2ca9a0)

### Solution:
If you have experience with OT network protocols, you'll know that the flag would be something along the lines of Modbus or `Modbus/TCP` (which is the flag `gcsm2024{Modbus/TCP}`).

Alternatively, download `OT.pcap` and open it in [Wireshark](https://wireshark.org/).

![image](https://github.com/user-attachments/assets/47064434-d3e2-4977-90c7-253048e19b67)

Have a look at the bottom. Normal PCAP files would have protocols like TCP. Modbus/TCP looks to be different and answers the question:
>...identify the OT network protocol used by the...
