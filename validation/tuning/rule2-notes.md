# Rule 2 Tuning Notes — base64 decode piped to shell

## Why it matters
This is a high-signal pattern for obfuscated execution and payload delivery via one-liners.

## Validation evidence
- validation/evidence/test2_exec.txt

## What matched in telemetry
- Command line includes `base64 -d` and a pipe into `sh`/`bash` (typical one-liner execution chain)

## False positives / tuning ideas
- Exclude known automation accounts/scripts if they legitimately use base64
- Extend coverage to similar patterns (e.g., `openssl enc -d`, `python -c` decode + exec)
- Add detections for long base64 blobs or suspicious parent processes
