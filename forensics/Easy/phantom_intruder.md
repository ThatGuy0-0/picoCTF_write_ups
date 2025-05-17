Title: Phantom Intruder
Author: Prince Niyonshuti N.

Description:
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻
Your mission is to uncover how this phantom intruder infiltrated my system and recover the hidden flag.

The attacker has left behind traces of their actions in a packet capture (PCAP) file — but nothing is obvious at first glance. The trail is subtle, time-sensitive, and intentionally obfuscated. It's up to you to uncover the hidden message buried within.

Download the PCAP file from the following link: Network Traffic PCAP File
Use your forensic skills to extract and decode the clues!

Hints:

Timing is key. The packets were sent in a well-structured sequence.

Think simple: sometimes you don’t need fancy tools.

Look inside the file for readable strings and decode them.

Approach:
Instead of analyzing the PCAP file with Wireshark, we can take a more efficient command-line approach using basic tools like strings and base64. Follow these steps:

Extract readable strings from the PCAP file:


strings traffic.pcap | grep "=="

There are some base64 strings which can be decoded.

Decode each base64 string:


echo "base64_string" | base64 -d.

You should be able to piece the strings into the flag format:


picoCTF{your_flag_here}

Goal:
Analyze the provided network traffic using string extraction and Base64 decoding to uncover the hidden flag. Show off your forensic skills and reveal the secrets left behind by the phantom intruder!
