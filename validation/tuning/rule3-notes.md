# Rule 3 Tuning Notes — SSH Brute Force

## Why it matters
Repeated failed SSH authentication attempts are a common brute force technique used for initial access.

## Validation evidence
- validation/evidence/test3_auth.txt

## What matched in telemetry
- Multiple "Failed password" and "Invalid user" events from same source IP

## False positives / tuning ideas
- Increase threshold in noisy environments
- Correlate by source IP
- Exclude internal scanning hosts if necessary
