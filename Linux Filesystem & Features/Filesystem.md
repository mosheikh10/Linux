# Linux Filesystem 🐧

The Linux filesystem is how files and directories are organised. Everything in Linux is treated as a file (even devices and processes).

# 📂 Filesystem Basics
/ → Root directory (the starting point of everything)
/home → Stores user files and folders (/home/momo)
/bin → Basic commands and programs (like ls, cp, mv)
/etc → Configuration files for the system
/var → Variable files (logs, spool, etc.)
/tmp → Temporary files
/usr → User programs and libraries
/dev → Devices (like USB, hard drives)
/proc → Information about running processes

# 📑 Important File Types
Regular file (-) → Normal text, data, or program file
Directory (d) → Folder containing files
Link (l) → Shortcut/alias to another file
Block device (b) → Storage device (e.g., hard drive)
Character device (c) → Devices like keyboard, mouse

# 🔑 Useful Commands
pwd → Show current directory (where you are)
ls → List files in the directory
ls -l → Show detailed info (permissions, owner, size)
ls -a → Show hidden files (start with .)
cd <dir> → Change directory
cd .. → Go back one directory

# 🛠 File Management
touch file.txt → Create a new file
mkdir folder → Create a new folder
cp file1 file2 → Copy file
mv file1 file2 → Move or rename file
rm file.txt → Delete file
rmdir folder → Delete empty folder
rm -r folder → Delete folder and its contents
