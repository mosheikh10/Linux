# Level 6 > 7

# Aim
The password for the next level is stored somewhere on the server and has all of the following properties:

`owned by user bandit7` `owned by group bandit6` `33 bytes in size`

# Solution
1. To locate the correct file, use the find command with multiple filters:
 - -type f → ensures only files (not directories) are listed
 - -size 33c → limits the search to files that are exactly 33 bytes in size
 - -user bandit7 → matches files owned by the bandit7 user
 - -group bandit6 → matches files belonging to the bandit6 group

2. find -type f -size 33c -user bandit7 -group bandit6

🔑 : morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
