# Linux Process Management (My Notes)

Process management is one of the most important Linux administration skills.

A **process** is simply a running program in Linux.

Linux admins and engineers must know how to:

- Monitor processes  
- Kill unwanted tasks  
- Manage CPU & memory usage  
- Run background jobs  

---

## 🔹 Viewing Running Processes

### Show all processes

```bash
ps aux
ps aux | head
```
### Real-Time Process Monitoring
```bash
top  #Press q to quit
```
### Finding a Process
```bash
ps aux | grep nginx  #Search by name
pgrep nginx  #another option
```
### Killing a Process
```bash
kill <PID>  #Kill by PID
kill 1234  #example
kill -9 <PID>  #Force kill
pkill nginx  #Kill by name
```
### Checking Resource Usage
```bash
lscpu  #CPU info
free -h  #Memory usage
df -h  #Disk usage
```
### Monitoring System Load
```bash
uptime
Shows:
load average
running time
logged-in users
```
