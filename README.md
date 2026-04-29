# Scanning-Wireshark-Nessus-Burpsuite
Week 7 task

__Question 1: Analyse packet1.pcap and find the flag.__

1st step- Check the ICMP Data Payload, While the other ICMP packets are standard 98-byte pings, this one is 70 bytes and contains a unique data payload.
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/2843c22c5c3a6529a155524fe0b547c8773e4394/pcap1.png)

2nd step- Decode the base64 code
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/c72ad95e89943a8540313afb23fa10b3b65e5255/decode.png)

__Question 2: Analyse packet2.pcap and find the flag.__
