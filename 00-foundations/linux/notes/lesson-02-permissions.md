# Linux Lesson 2 – Permissions & Ownership

## Why Permissions Exist
Linux is a multi-user system.  
Permissions prevent unauthorized access, accidental damage, and privilege escalation.

They enforce the principle of least privilege.

---

## Permission Model
Each file and directory has:
- Owner (user)
- Group
- Others

Each entity can have:
- Read (r)
- Write (w)
- Execute (x)

Example:
-rwxr-x---

---

## Files vs Directories
For files:
- r → read content
- w → modify content
- x → execute

For directories:
- r → list files
- w → create/delete files
- x → enter directory (cd)

Without x, a directory is inaccessible even if readable.

---

## Ownership vs Permissions
- chown → changes ownership (who owns the file)
- chmod → changes permissions (what actions are allowed)

They are separate security layers.

---

## Why chmod 777 is Dangerous
777 allows anyone to:
- Read
- Modify
- Execute

This removes all security boundaries and enables:
- Code injection
- Data tampering
- Lateral movement

---

## Least Privilege
Only grant the minimum permissions required for a task.  
Anything more increases the blast radius of a compromise.

---

## Why This Matters in DevOps
- Wrong permissions cause outages
- Wrong ownership crashes applications
- Insecure permissions cause breaches
