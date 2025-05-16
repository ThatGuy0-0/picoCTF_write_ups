Title: canyousee
Author: Mubarak Mikail

Description:
-How about some hide and seek? Download this file here. 

Hints:
-How can you view the information about the picture?
-If something isn't in the expected form, maybe it deserves attention?

unzip the file to see the file contents.
-unzip <file>

read the metadata of the picture file.
-run exiftool <file>

Notice how the attribution URL is in base64. Decode this to see the real information.
-run echo "string" | base64 -d

There is the flag. picoCTF{xxx}
