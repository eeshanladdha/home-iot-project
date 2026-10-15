# Phase 1: Raspberry Pi Foundation

## Objective
Build a stable Raspberry Pi/Linux foundation for all later phases.

## Current progress (2026-10-15)
- [x] Ordered hardware received (user-confirmed).
- [x] Raspberry Pi OS installed.
- [x] Raspberry Pi Connect used successfully to access the Pi from the user's Mac.
- [ ] Record exact Raspberry Pi OS release/version and installation/storage details.
- [ ] Verify network stability and document connection approach.
- [ ] Configure and validate SSH access separately from Raspberry Pi Connect.
- [ ] Review users, permissions, updates and baseline security.
- [ ] Establish Python virtual environment and Git workflow.
- [ ] Evaluate Docker versus native services and record the decision.
- [ ] Establish logging/monitoring baseline.
- [ ] Test backup and recovery.

Raspberry Pi Connect access confirms that remote access works, but it does not by itself validate SSH, long-term network stability, backup/recovery or the complete Phase 1 baseline.

## Scope
- Raspberry Pi model and OS
- Storage and power
- Network and remote access (Raspberry Pi Connect and SSH)
- Users and permissions
- Python and Git
- Docker evaluation
- Monitoring and backup
- Logging and update strategy

## LLD placeholders
Runtime, network, services, observability and backup design remain TBD until the exact hardware and environment are recorded and tested.

## Evidence to capture
- Raspberry Pi OS version output (for example, `cat /etc/os-release`)
- Storage/boot-medium details (for example, `lsblk`)
- Network details with sensitive information redacted
- Raspberry Pi Connect access confirmed from Mac
- SSH connection and security checks
- Python/Git checks
- Service/logging and backup/recovery test results

Do not commit passwords, private keys, access tokens, full Wi-Fi credentials or other secrets.

## Exit criteria
- [x] OS installed
- [ ] Network stable and documented
- [ ] SSH secured
- [ ] User model established
- [ ] Python environment ready
- [ ] Git workflow tested
- [ ] Docker decision recorded
- [ ] Monitoring baseline established
- [ ] Backup/recovery tested
