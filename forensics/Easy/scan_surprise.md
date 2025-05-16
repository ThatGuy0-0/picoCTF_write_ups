Title: scan surprise
Author: Jeffery John

Description:
-I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead? You can download the challenge files here:

    challenge.zip

    The same files are accessible via SSH here: ssh -p 62665 ctf-player@atlas.picoctf.net Using the password 83dcefb7. Accept the fingerprint with yes, and ls once connected to begin. Remember, in a shell, passwords are hidden!

unzip file to analyse the file contents.
-unzip <file>

there are now file directories that have been extracted. Navigate to the file called "flag.png". This is a qr code file and now you must read the qr code.
-run zbarimg <file>

There is the flag. picoCTF{xxx}
