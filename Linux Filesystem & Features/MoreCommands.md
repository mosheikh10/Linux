# Advanced & Essential Commands

sudo
- Run a command as a superuser (root).
- Example: sudo apt update → runs update with admin privileges.
- NOTE: gives full system access.

vim
- A text editor inside the terminal.

- Modes:

- i → insert mode (type text).
- Esc → exit insert mode.
- :w → save.
- :q → quit.
- :wq → save & quit.
- :q! → quit without saving.

man

Shows the manual page for a command.

Example: man ls → explains how ls works.

grep

Searches text using patterns.

Example: grep hello file.txt → finds "hello" in file.txt.

chmod

Changes file permissions.

Example: chmod 755 script.sh → gives read/write/execute to owner, read/execute to others.

chown

Changes file ownership.

Example: chown user:user file.txt → makes user the owner.

ps

Shows running processes.

Example: ps aux → detailed list of all processes.

kill

Ends a process by its ID (PID).

Example: kill 1234 → kills process with PID 1234.

tar

Create or extract compressed archives.

Example: tar -czvf backup.tar.gz folder/ → compress folder.

Example: tar -xzvf backup.tar.gz → extract.

ssh

Connects to another machine remotely.

Example: ssh user@ip_address

scp

Copy files between systems (uses SSH).

Example: scp file.txt user@ip:/home/user/
