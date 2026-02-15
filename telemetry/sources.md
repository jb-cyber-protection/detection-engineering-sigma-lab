# Telemetry Sources – Linux Detection Lab

## 1. auditd (Process Execution)

Purpose:
Capture process execution (execve) events for detection engineering.

Key:
exec

Validation:
sudo ausearch -k exec

---

## 2. Authentication Logs

Source:
/var/log/auth.log

Purpose:
Capture SSH and sudo authentication activity.

Validation:
sudo tail -n 50 /var/log/auth.log
