# Level 9 > 10

# Aim
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

# Solution
1. The strings command extracts all human-readable text from files that contain mostly binary or non-printable characters.
- note: It’s useful when a file looks unreadable in normal editors or when you suspect hidden text within it.

2. By combining it with grep, you can search for specific patterns in that readable output.
3. strings data.txt | grep "="
4. This extracts the readable text from data.txt and filters it to only show the lines that contain an equals sign (=)

5. 🔑 : FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
