# Linux Disk Management (My Notes)

Disk management is an essential Linux skill for:

- System Administrators  
- DevOps Engineers  
- Cloud Engineers  
- Server Maintenance  

It includes:

✅ Checking disk usage  
✅ Partition management  
✅ Mounting storage  
✅ Monitoring free space  

---

## 🔹 Checking Disk Space

### View disk usage of all filesystems

```bash
df -h

Filesystem           Size  Used Avail Use% Mounted on
/dev/mapper/cs-root   27G  5.7G   21G  22% /
/dev/nvme0n1p2       960M  603M  358M  63% /boot
/dev/nvme0n1p1       599M  7.3M  592M   2% /boot/efi
/dev/nvme0n2p1       2.9G   24K  2.8G   1% /jaat
/dev/sr0              13G   13G     0 100% /run/media/siddhu/CentOS-Stream-9-BaseOS-x86_64
```
### Checking Directory Size
```bash
du -sh /home/siddhu  #Check size of a folder
du -h --max-depth=1  #Check size of all folders inside
```
### Listing Block Devices
```bash
lsblk  #View disks and partitions

NAME        MAJ:MIN RM  SIZE RO TYPE MOUNTPOINTS
sr0          11:0    1 12.3G  0 rom  /run/media/siddhu/CentOS-Stream-9-BaseOS-x86_64
nvme0n1     259:0    0   30G  0 disk 
├─nvme0n1p1 259:1    0  600M  0 part /boot/efi
├─nvme0n1p2 259:2    0    1G  0 part /boot
└─nvme0n1p3 259:3    0 28.4G  0 part 
  ├─cs-root 253:0    0 26.4G  0 lvm  /
  └─cs-swap 253:1    0    2G  0 lvm  [SWAP]
nvme0n2     259:4    0    5G  0 disk 
└─nvme0n2p1 259:5    0    3G  0 part /jaat
```
### Partition Information
```bash
sudo fdisk -l  #Show partition table
```
### Mounting and unmounting a Disk
```bash
sudo mkdir /mnt/data  #Create mount directory
sudo mount /dev/xvdb1 /mnt/data  #Mount partition
df -h  #Verify mount
sudo umount /mnt/data  #Unmounting a Disk
sudo vi /etc/fstab  #Permanent Mount (fstab)
```
