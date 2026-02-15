# MITRE ATT&CK Mapping

Each Sigma rule in this repository is mapped to relevant MITRE ATT&CK techniques.

This document summarizes coverage and rationale.

## Rule 1 — Linux Suspicious curl/wget download to /tmp
- Technique: T1105 (Ingress Tool Transfer)
- Rationale: curl/wget used to stage payloads into a temp directory prior to execution

## Rule 2 — Linux Base64 decode piped to shell
- Technique: T1059 (Command and Scripting Interpreter)
- Rationale: base64 decode piped into a shell is a common obfuscation + execution chain
