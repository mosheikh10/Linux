# 💻 Linux Distributions and Virtual Machines
🐧 Distributions
 - A distribution is a specific version of Linux, packaged with its own tools and features.
 - Different distros are designed for different purposes (servers, desktops, security, development).
 - Common distros: Ubuntu, Debian, Fedora, Arch, Red Hat.
 - Ubuntu is especially popular for beginners because of its easy to use (hence why im using it) and strong community support.

👨‍💻 Running Linux with Virtualisation
Ubuntu via UTM (Mac)
 - UTM allows you to install and run Ubuntu inside your Mac without replacing macOS.
 - You can experiment with Linux safely while still keeping your main OS intact.
 - Installation can be done directly through the UTM website.

Renting a VM on AWS
 - Another option is running Linux in the cloud with Amazon EC2.
 - EC2 provides virtual servers that you can connect to from anywhere.

Steps:
 - Create an AWS account and launch an EC2 instance with Ubuntu.
 - Configure access with an SSH key.
 - Connect from your terminal:
    - ssh -i mykey.pem ubuntu@EC2-IP
 - This gives you a cloud-based Linux machine to practice on without needing local installation.
