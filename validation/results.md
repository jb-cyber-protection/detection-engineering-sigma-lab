# Validation Results

## Rule 1 — Linux Suspicious curl/wget download to /tmp
- MITRE ATT&CK: T1105 (Ingress Tool Transfer)
- Status: validated (against auditd telemetry)
- Evidence: validation/evidence/test1_exec.txt
- Tuning notes: validation/tuning/rule1-notes.md

## Rule 2 — Linux Base64 decode piped to shell
- MITRE ATT&CK: T1059 (Command and Scripting Interpreter)
- Status: validated (against auditd telemetry)
- Evidence: validation/evidence/test2_exec.txt
- Tuning notes: validation/tuning/rule2-notes.md
