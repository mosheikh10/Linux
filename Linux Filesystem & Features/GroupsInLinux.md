Linux Groups 👥

Groups allow you to manage permissions for multiple users at once. Instead of setting permissions for each user individually, you can give a group permissions and then add users to that group.

🔎 Viewing Groups

View all groups on the system:
cat /etc/group

Each entry shows:

Group name

Password placeholder (usually x)

Group ID (GID)

Members of the group

Example:
sudo group → members have admin (root) privileges.

To give a user sudo rights → add them to the sudo group.

➕ Creating a Group

Create:
sudo groupadd devops

Verify:
cat /etc/group | grep devops

👤 Adding a User to a Group

Add user to a group:
sudo usermod -aG devops newuser

-a → append (don’t remove user from other groups)

-G → specify group

Verify:
groups newuser

❌ Removing a User from a Group

Remove:
sudo gpasswd -d newuser devops

Verify:
su - newuser → then run groups

🗑️ Deleting a Group

Delete:
sudo groupdel devops

Verify:
cat /etc/group | grep devops

No output = group deleted

👥 Adding a User to Multiple Groups

Add:
sudo usermod -aG admin1,admin2 newuser

Verify:
su - newuser → then run groups

Should list both admin1 and admin2
