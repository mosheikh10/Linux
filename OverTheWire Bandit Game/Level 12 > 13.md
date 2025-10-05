# Level 12 > 13

# Aim
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

# Solution
1. We first create a temporary directory to work in using mktemp -d, which gives us a unique path 
2. Copy data.txt into that directory and move into it using:
3. cp data.txt /tmp/tmp.9OLnrxH0Ro and then cd /tmp/tmp.9OLnrxH0Ro.

4. Running file data.txt shows it’s ASCII text but in hexdump form, so we reverse it:
5. xxd -r data.txt > stage1

6. Checking file stage1 reveals it’s a gzip file. We decompress it:
7. gzip -dc stage1 > stage2

8. file stage2 → bzip2 compressed data
9. bzip2 -dc stage2 > stage3

10. file stage3 → gzip compressed data
11. gzip -dc stage3 > stage4

12. file stage4 → POSIX tar archive
13. tar -xf stage4 → creates data5.bin

14. file data5.bin → another POSIX tar archive
15. tar -xf data5.bin → creates data6.bin

16. file data6.bin → bzip2 file
17. bzip2 -dc data6.bin > stage5

18. file stage5 → POSIX tar archive
19. tar -xf stage5 → generates data8.bin

20. file data8.bin → gzip file
21. gzip -dc data8.bin > stage6
22. file stage6 → ASCII text

🔑 : FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
