# Level 10 > 11

# Aim
The password for the next level is stored in the file data.txt, which contains base64 encoded data.

# Solution
1. The file’s contents are encoded in Base64, so we need to decode it to reveal the original text.
 - Note : The base64 command handles encoding and decoding of Base64 data.
2. To decode the file, use the -d flag.
3. base64 -d data.txt

🔑 : dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
