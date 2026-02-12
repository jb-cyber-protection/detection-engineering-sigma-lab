# Ubuntu Detection Lab (UTM)

## Purpose
This Ubuntu VM serves as the detection engineering lab environment.
It is used to generate telemetry, simulate attack behavior, and validate Sigma detections.

## Platform
- Ubuntu Desktop 22.04 LTS (ARM64)
- UTM on Apple Silicon macOS

## Installed Tooling
- auditd / audispd-plugins (process execution telemetry)
- openssh-server (authentication telemetry)
- git, curl, wget, jq
- python3 + pip
- sigma-cli

## Services Enabled
- auditd
- ssh

## Notes
Single-VM setup used for controlled behavior simulation and telemetry generation.
