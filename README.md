# Detection Engineering – Sigma Lab

This repository demonstrates practical detection engineering skills through
the creation, validation, and documentation of Sigma detection rules.

## Objectives
- Develop high-signal Sigma detections mapped to MITRE ATT&CK
- Generate real telemetry using a controlled Linux lab
- Validate detections with reproducible attack simulations
- Document tuning considerations and false positives

## Platform
- Ubuntu Linux (UTM on Apple Silicon)
- auditd process and authentication telemetry
- Atomic-style attack simulations

## Contents
- sigma/        Detection rules (Sigma)
- tests/        Attack simulations used for validation
- telemetry/    Log sources and configuration
- validation/   Evidence and tuning notes
- docs/         Methodology and mapping
