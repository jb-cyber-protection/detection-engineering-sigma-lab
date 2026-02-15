# Telemetry Verification (Issue #4)

## Verify auditd is running
systemctl status auditd

## Verify rules are loaded
sudo auditctl -l

## Verify exec events are captured
sudo ausearch -k exec | tail

## Verify auth logs exist
sudo tail -n 50 /var/log/auth.log
