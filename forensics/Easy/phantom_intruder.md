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


strings traffic.pcap > output.txt
Inspect the output.txt file and look for suspicious Base64-encoded strings. These often consist of random-looking alphanumeric characters, possibly ending with = or ==.

Collect all the Base64 strings, piece them together in the correct order. The structure of the packet timing might help you figure out the sequence if it’s not immediately obvious.

Decode the full Base64 string:


echo "combined_base64_string" | base64 -d
You should now see the flag in the format:


picoCTF{your_flag_here}

Goal:
Analyze the provided network traffic using string extraction and Base64 decoding to uncover the hidden flag. Show off your forensic skills and reveal the secrets left behind by the phantom intruder!
