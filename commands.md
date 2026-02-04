# Linux Basic Commands (My Practice Notes)

This file contains the most common Linux commands that I use while practicing
Linux tasks.

---

## Navigation & Directory Commands

```bash
pwd              # current working directory
ls               # list files
ls -l            # detailed listing
ls -a            # show hidden files
cd /etc          # move into /etc directory
cd ..            # go one step back
mkdir testdir    # create directory
rm -rf testdir   # delete directory forcefully
```
![img](images/img1.png)
---

## File Handling Commands

```bash
touch file.txt           # create empty file
cp file1 file2           # copy file
mv oldname newname       # rename file
rm file.txt              # remove file
cat file.txt             # view file content
less file.txt            # scroll file
head file.txt            # first 10 lines
tail file.txt            # last 10 lines
tail -f /var/log/messages # live log monitoring
```
![img](images/img2.png)
---

## Searching in Linux

```bash
find /home -name "*.sh"     # search scripts
grep "error" logfile.txt    # search word inside file
wc -l file.txt              # count lines
```
![img](images/img3.png)
---

## User and Permission Related

```bash
whoami          # current user
id siddhu       # UID and group info

chmod 755 script.sh    # give execute permission
chown user:user file   # change ownership
```
---

## Process Monitoring

```bash
ps aux          # running processes
top             # live monitoring
kill -9 PID     # force kill a process
uptime          # system running time
```
---

## Disk and Memory Checks

```bash
df -h           # disk usage
du -sh folder/  # folder size
free -m         # memory usage
lsblk           # list disks/partitions
```
![img](images/img4.png)
---

## Networking Commands I Use

```bash
ping google.com       # connectivity check
ip a                  # check IP address
ss -tulnp             # open ports
curl ifconfig.me      # public IP check
```
---

## Service Management (systemctl)

```bash
systemctl status sshd
systemctl start nginx
systemctl stop nginx
systemctl enable nginx
journalctl -xe        # logs for troubleshooting
```
---

## Package Installation (RHEL/CentOS)

```bash
yum install nginx -y
yum remove httpd -y
yum update -y
```
![img](images/img5.png)
---
`
