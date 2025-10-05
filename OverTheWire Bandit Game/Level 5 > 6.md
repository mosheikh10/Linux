# Level 5 > 6

# Aim
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

`human-readable` `1033 bytes in size` `not executable`

# Solution
1. As there are multiple subdirectories, the find command is used to search and filter files.
2. find . -type f : Lists all files within all subdirectories of the current working directory.
3. Add -size 1033c to filter files that are exactly 1033 bytes in size (c means bytes).
4. Add ! -executable to include only files that are not executable.
5. Add -exec file {} \; to run the file command on each result to check the file type.
6. Pipe the output to grep ASCII to filter for the human-readable file.
7. find . -type f -size 1033c ! -executable -exec file {} ; | grep ASCII

🔑 : HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
