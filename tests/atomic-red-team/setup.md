# Atomic-style Tests (Linux)

This project uses repeatable, controlled command sequences ("atomic-style tests")
to generate ground-truth telemetry for Sigma detection validation.

## Capture method
- auditd exec events: `ausearch -k exec`
- auth events: `/var/log/auth.log`

## Evidence storage
All evidence is saved in `validation/evidence/` with one file per test.
