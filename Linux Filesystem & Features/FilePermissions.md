# 📁 File Permissions in Linux

Basic Structure (ls -l)
 - Example: -rw-r--r-- 1 user user 1234 file.txt
 - Breakdown:
   - → file type (- = file, d = directory, l = link)
   - rw- → owner permissions
   - r-- → group permissions
   - r-- → others permissions
  
     

Permission Types

r → read

w → write

x → execute

Who Can Have Permissions

User (u) → the file’s owner

Group (g) → users in the file’s group

Others (o) → everyone else

Changing Permissions (chmod)

Symbolic method:

chmod u+x file → add execute for owner

chmod g-w file → remove write for group

chmod o=r file → set read only for others

Numeric method:

Each permission has a number:

Read = 4

Write = 2

Execute = 1

Add them up:

7 = rwx

6 = rw-

5 = r-x

4 = r--

Example:

chmod 755 file → rwxr-xr-x

Changing Ownership (chown)

chown user file → change owner

chown user:group file → change owner & group

Check Permissions

ls -l → detailed permissions of files

stat file.txt → more detailed info
