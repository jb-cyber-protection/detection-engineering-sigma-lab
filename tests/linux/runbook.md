# Linux Test Runbook

## Before each test
1. Run the test command(s)
2. Immediately export:
   - auditd exec events: `sudo ausearch -k exec | tail -n 200`
   - auth events (if relevant): `sudo tail -n 200 /var/log/auth.log`

## Evidence naming
- validation/evidence/test1_exec.txt
- validation/evidence/test2_exec.txt
- validation/evidence/test3_exec.txt
