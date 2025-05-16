Title: disko 1
Author: Darkraicg492

Description:
-Can you find the flag in this disk image? Download the disk image here. 

Hints:
-Maybe Strings could help? If only there was a way to do that?

______________________________________________________________________________

unzip .dd file. This allows you to analyse the file contents
-gunzip <file>

use strings to read contents of the file. combine this with grep "" to find a specific string
-strings <file> | grep "pico"

there is the flag. picoCTF{xxx}
