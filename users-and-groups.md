# Linux Users and Groups (My Notes)

Managing users and groups is a core Linux administration skill.

Linux is a **multi-user operating system**, so controlling:

- User accounts  
- Group access  
- Permissions  
- Security  

is very important for system admins and DevOps engineers.

---

## 🔹 Checking Current User

```bash
whoami
siddhu
```
## Show user ID details
```bash
id
uid=1000(siddhu) gid=1000(siddhu) groups=1000(siddhu),1003(devopsengineer),1008(xyz),1009(gu) context=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023
```
## List logged-in users
```bash
who
siddhu   tty2         2026-02-03 21:43 (local)
```
## Creating a New User
```bash
sudo useradd username  #adduser
sudo useradd devuser   #example
sudo passwd devuser    #Setting Password for User
sudo useradd -m devuser  #Creating User with Home Directory
sudo userdel devuser  #Deleting a User
sudo userdel -r devuser  #example
```
## Groups in Linux
```bash
groups siddhu  #Check groups of a user
sudo groupadd devops  #Creating a Group
sudo usermod -aG devops devuser  #Adding User to Group
sudo gpasswd -d devuser devops  #sudo gpasswd -d devuser devops
```
## Important System Files

| File          | Purpose                  |
| ------------- | ------------------------ |
| `/etc/passwd` | User account information |
| `/etc/shadow` | Encrypted passwords      |
| `/etc/group`  | Group information        |

```bash
cat /etc/passwd
cat /etc/group
```
## Sudo Privileges
```bash
sudo usermod -aG sudo devuser
```
## User Management Practice
Commands to remember:
```bash
useradd
passwd
usermod
userdel
groupadd
groups
id
```
