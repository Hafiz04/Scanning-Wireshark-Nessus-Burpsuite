# Scanning-Wireshark-Nessus-Burpsuite
Week 7 task

__Question 1: Analyse packet1.pcap and find the flag.__

1st step- Check the ICMP Data Payload, While the other ICMP packets are standard 98-byte pings, this one is 70 bytes and contains a unique data payload.
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/2843c22c5c3a6529a155524fe0b547c8773e4394/pcap1.png)

2nd step- Decode the base64 code
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/c72ad95e89943a8540313afb23fa10b3b65e5255/decode.png)

__Question 2: Analyse packet2.pcap and find the flag.__

1st step- Filter ftp protocol only
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/e1e0da3af360578b775af7dea127ce9ac79902f6/filter%20ftp.png)

2nd step- Looking at the login sequence or by extracting files transferred during the session

In packet 213, the user sends a RETR (Retrieve) command for a file
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/82ad0a139007bf7adad2882cc26edd7007e66da4/packet%20213.png)

3rd step- The actual content of the file global_thermonuclear_war.gamerules.txt is inside packet 216.

Find Packet 216 in your packet list and found out that there is shortened URL
![image alt](https://github.com/Hafiz04/Scanning-Wireshark-Nessus-Burpsuite/blob/a9b4cba4ce3548b24d77a80fa194e6a773e4b6ac/packet%20216.png)
