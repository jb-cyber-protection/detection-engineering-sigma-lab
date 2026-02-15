# MITRE ATT&CK Mapping

Each Sigma rule in this repository is mapped to relevant MITRE ATT&CK techniques.

This document summarizes coverage and rationale.

## Rule 1 — Linux Suspicious curl/wget download to /tmp
- Technique: T1105 (Ingress Tool Transfer)
- Rationale: curl/wget used to stage payloads into a temp directory prior to execution

## Rule 2 — Linux Base64 decode piped to shell
- Technique: T1059 (Command and Scripting Interpreter)
- Rationale: base64 decode piped into a shell is a common obfuscation + execution chain

---

# Detection Coverage Summary

| Rule | Technique | Description |
|------|-----------|------------|
| Rule 1 | T1105 | Payload staging via curl/wget |
| Rule 2 | T1059 | Obfuscated execution via base64 decode |
| Rule 3 | T1110 | SSH brute force authentication failures |

This lab demonstrates detection coverage across initial access, execution, and staging behaviors.
