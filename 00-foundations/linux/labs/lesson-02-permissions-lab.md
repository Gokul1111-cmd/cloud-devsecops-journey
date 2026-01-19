## Mini-Project: Secure App Directory

### Why we created appuser and appgroup
To isolate the application from root and other users.

### Why /opt/myapp
/opt is used for optional and third-party applications.

### Why chmod 750
- Owner: full control
- Group: limited access
- Others: no access

### Security takeaway
This enforces least privilege and limits blast radius.
