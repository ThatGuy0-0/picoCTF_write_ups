Title: Phantom intruder
Author: Prince Niyonshuti N.

Description: 
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag. To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder! Find the PCAP file here Network Traffic PCAP file and try to get the flag. 

Hints: 
-Filter your packets to narrow down your search.
-Attacks were done in timely manner.
-Time is essential

We can see that there is a traffic pcap file to download. You can use wireshark to analyse information on packets sent. Notice the difference in packet lengths. Filter out the different packet lengths. Looking at the packets we can see that there is some base64 string in each packet. We can decode this.
-run echo "string" | base64 -d

Piece all the strings together to make the flag. picoCTF{xxx}
