# Level 13 > 14

# Aim
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on.

# Solution
1. Make sure the private key has the correct permissions so SSH accepts it: `chmod 600 sshkey.private`
2. Connect using the key: ssh -i sshkey.private bandit14@localhost -p 2220
  - -i specifies the identity (private key) file.
  - -p 2220 connects to the OverTheWire Port 2220 SSH port.
3. Once logged in, change to the password directory: cd /etc/bandit_pass
4. Display the password file for bandit14: cat bandit14

🔑 : MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS 
