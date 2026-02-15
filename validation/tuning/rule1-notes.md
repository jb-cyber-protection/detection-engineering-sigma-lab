# Rule 1 Tuning Notes — curl/wget download to /tmp

## Why it matters
Payload staging commonly uses curl/wget to drop a file into /tmp before execution.

## Validation evidence
- validation/evidence/test1_exec.txt

## What matched in telemetry
- exe="/usr/bin/curl" and cmdline includes "/tmp/..."

## False positives / tuning ideas
- Exclude known maintenance scripts/users that legitimately download to /tmp
- Restrict to external URLs if your pipeline extracts destination host
- Consider also matching downloads into /dev/shm and /var/tmp
