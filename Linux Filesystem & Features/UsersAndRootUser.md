# Root User & Creating Users

Root User
 - Root is the superuser account in Linux.
 - Has full system privileges: install software, manage users, change any file.
 - Running as root is risky — one wrong command can break the system.
 - Run a single command as root:
   - sudo command
 - Start a root shell:
   - sudo -i

Creating a User
 - Create a new user:
   - sudo adduser newuser

 - Check if user exists:
   - cat /etc/passwd | grep newuser

 - Switch to new user:
   - su - newuser

Giving User Root (sudo) Access
Add user to sudo group:
 - sudo usermod -aG sudo newuser

Verify:
 - groups newuser

Deleting a User
- Delete user only:
  - sudo deluser newuser

- Delete user + home directory:
  - sudo deluser --remove-home newuser
