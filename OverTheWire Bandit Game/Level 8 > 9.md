# Level 8 > 9

# Aim
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once.

# Solution
1. The sort command arranges all the lines in a file alphabetically (A–Z, 0–9).
2. The uniq command then removes consecutive duplicate lines — so it must be used after sorting, since sorting places duplicates next to each other.
3. Adding the -c option to uniq shows how many times each line appears.
4. To find the line that only occurs once, combine the commands like this:
5. sort data.txt | uniq -c | grep ' 1 '
6. This sorts the file, counts occurrences of each line, and filters to display only the one that appears a single time.

7. 🔑 : 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
