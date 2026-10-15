# Phase 1: Raspberry Pi Foundation

## Objective
Build a stable Raspberry Pi/Linux foundation for all later phases.

## Current progress (2026-10-15)
- [x] Ordered hardware received (user-confirmed).
- [x] Raspberry Pi OS installed.
- [x] Raspberry Pi Connect used successfully to access the Pi from the user's Mac.
- [x] Record OS release, Pi model/architecture and boot/storage layout from baseline commands.
- [ ] Confirm Raspberry Pi OS-specific release details and document installation/storage details.
- [ ] Verify network stability and document connection approach.
- [ ] Configure and validate SSH access separately from Raspberry Pi Connect.
- [ ] Review users, permissions, updates and baseline security.
- [ ] Establish Python virtual environment and Git workflow.
- [ ] Evaluate Docker versus native services and record the decision.
- [ ] Establish logging/monitoring baseline.
- [ ] Test backup and recovery.

Raspberry Pi Connect access confirms that remote access works, but it does not by itself validate SSH, long-term network stability, backup/recovery or the complete Phase 1 baseline.

## Baseline recorded (2026-10-15)
- OS release file reports Debian GNU/Linux 13 (Trixie), version `13.7`.
- Hardware reports Raspberry Pi 5 Model B, revision 1.1.
- CPU architecture: `aarch64` (64-bit ARM).
- Hostname: `presh-iot`.
- `lsblk` reports `/dev/sda` as a 28.7 GB removable disk; `/dev/sda1` is mounted at `/boot/firmware` and `/dev/sda2` at `/`. The current root filesystem is therefore on `/dev/sda2`, consistent with booting from USB storage.
- The screenshot does not include `df -h` or `hostname -I`; free space and IP address remain unrecorded.

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
