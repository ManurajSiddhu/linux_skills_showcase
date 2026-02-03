# Linux File Permissions (My Notes)

Linux permissions are very important for system security and administration.

This file contains my practice notes on:

- Permission types
- chmod usage
- Ownership commands
- Real-world examples

---

## Permission Types

Linux has 3 permission types:

| Permission | Symbol | Meaning |
|-----------|--------|---------|
| Read      | r      | View file content |
| Write     | w      | Modify file |
| Execute   | x      | Run file/script |

---

## Permission Categories

Permissions apply to:

| Category | Symbol |
|----------|--------|
| Owner    | u      |
| Group    | g      |
| Others   | o      |
| All      | a      |

---

## Checking Permissions

```bash
ls -l
-rwxr-xr--  1 siddhu users  1200 Feb 2 script.sh
```
---

## chmod Command

Symbolic Mode
```bash

chmod u+x script.sh     # add execute permission to owner
chmod g-w file.txt      # remove write from group
chmod o+r file.txt      # add read for others
chmod a+x script.sh     # give execute to all
```
Numeric Mode

| Number | Permission |
| ------ | ---------- |
| 7      | rwx        |
| 6      | rw-        |
| 5      | r-x        |
| 4      | r--        |
| 0      | ---        |

chmod 755 script.sh

---
## Ownership Commands

chown
```bash
chown siddhu file.txt
chown siddhu:devops file.txt
```
chgrp
```bash
chgrp devops file.txt
```

