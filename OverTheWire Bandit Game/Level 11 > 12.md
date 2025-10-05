# Level 11 > 12

# Aim
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.

# Solution
1. We use the tr command to translate or substitute characters from one set to another.
2. Since the text is encoded with a ROT13 cipher (each letter shifted 13 positions), we need to “deshift” it back to normal.
3. This is done by mapping A-Za-z to N-ZA-Mn-za-m, effectively reversing the rotation.
4. cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

🔑 : 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
