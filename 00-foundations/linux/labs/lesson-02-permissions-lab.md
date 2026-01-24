## Mini-Project: Secure App Directory

### Purpose
To isolate an application using Linux users, groups, ownership, and permissions.

---

### Why a Dedicated User and Group
To enforce least privilege and limit damage if the app is compromised.

---

### Why /opt/myapp
/opt is used for optional or third-party applications and keeps custom apps separate from OS and user files.

---

### Why chown appuser:appgroup
Assigns ownership of the directory to the application identity so access control works correctly.

---

### Why chmod 750
- Owner: full control
- Group: limited access
- Others: no access

This prevents unauthorized access and tampering.

---

### Security Takeaway
Linux permissions are the first security boundary in DevSecOps.
