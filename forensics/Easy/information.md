Title: information
Author: Susie

Description: Files can always be changed in a secret way. Can you find the flag? cat.jpg

Hints:
Look at the details of the file

https://play.picoctf.org/practice/challenge/186?originalEvent=34&page=1&search=format%20

Analyse file
-Run exiftool to look at metadata of the .jpg file
-Notice the license is encrypted, seems like base64

Decode the license
-Run echo "license" | base64 -d

There is the flag.
