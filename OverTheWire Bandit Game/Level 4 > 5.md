# Level 4 > 5

# Aim
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

# Solution
1. We use the file command to check the type of data each file contains.
2. file ./* : Lists all files in the current directory and shows what type of data they hold.
3. The file containing ASCII text is human-readable so in this case, it’s ./-file07.
4. cat ./-file07 : Displays the contents of the readable file.

🔑 : 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
