# My puzzle writeup
The content of the txt contains only numbers and the letters from A to F. This hints at hexadecimal (my first hint was an image of a hexagon, giving away the hex, a better shape would have 16 sides). It can be tested that there are an even number of characters, so the hex contains an integer number of bytes (one byte contains 8 binary digits, or 2 hexadecimal digits). With an integer number of bytes, the hex is probably not representing a huge number, but instead a hexdump of some text or a file, hence my picture of a dumptruck. The length of the hex means it's probably a file, not some huge text. To find the file type, look at the first few bytes of the txt. The txt starts with 5249464680B9060057415645 which decodes with ASCII into RIFF¹WAVE. The file signature for a wav file according to wikipedia is 52 49 46 46 ?? ?? ?? ?? 57 41 56 45 which matches the beginning of the txt, so it's a wav file. This website: https://tomeko.net/online_tools/hex_to_file.php?lang=en easily does the conversion to a file from a hexdump, and the name of the file can be changed to end in .wav instead of .dat. Listening to the wav doesn't reveal anything, but a spectogram gives the text: n3v3r_g0nn@-g1v3_u_up. I will attach an image of the spectogram, and the txt and wav files.
