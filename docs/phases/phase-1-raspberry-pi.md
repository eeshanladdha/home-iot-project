# Phase 1: Raspberry Pi Foundation

## Objective
Build a stable Raspberry Pi/Linux foundation for all later phases.

## Current progress (2026-10-15)
- [x] Ordered hardware received (user-confirmed).
- [x] Raspberry Pi OS installed.
- [x] Raspberry Pi Connect used successfully to access the Pi from the user's Mac.
- [x] Record OS release, Pi model/architecture and boot/storage layout from baseline commands.
- [x] Record Raspberry Pi image reference date, storage usage, network address presence, SSH service status, Python and Git versions.
- [ ] Confirm Raspberry Pi OS-specific release details and document installation/storage details.
- [ ] Verify network stability and document connection approach.
- [x] Test SSH connectivity from the Mac.
- [ ] Review SSH authentication/security settings.
- [ ] Review users, permissions, updates and baseline security.
- [x] Create and activate a project-specific Python virtual environment.
- [x] Clone the existing GitHub repository to `~/home-iot-project-repo` and create/activate its `.venv`.
- [ ] Verify Git identity and working-tree/remote status; make a first controlled commit.
- [ ] Evaluate Docker versus native services and record the decision.
- [ ] Establish logging/monitoring baseline.
- [ ] Test backup and recovery.

Raspberry Pi Connect and SSH connectivity from the Mac have both been confirmed by the user. SSH security settings, long-term network stability, backup/recovery and the complete Phase 1 baseline remain to be validated.

## Baseline recorded (2026-10-15)
- OS release file reports Debian GNU/Linux 13 (Trixie), version `13.7`.
- Hardware reports Raspberry Pi 5 Model B, revision 1.1.
- CPU architecture: `aarch64` (64-bit ARM).
- Hostname: `presh-iot`.
- `lsblk` reports `/dev/sda` as a 28.7 GB removable disk; `/dev/sda1` is mounted at `/boot/firmware` and `/dev/sda2` at `/`. The current root filesystem is therefore on `/dev/sda2`, consistent with booting from USB storage.
- `df -h` reports `/dev/sda2` as a 28 GB root filesystem, 6.7 GB used and 20 GB available (26% used); `/dev/sda1` is 505 MB with 417 MB available at `/boot/firmware`.
- `/etc/rpi-issue` reports `Raspberry Pi reference 2026-10-06` and a `pi-gen` build reference.
- `hostname -I` reports private IPv4 address `192.168.10.199` and an IPv6 address. Do not treat these as permanent addresses; DHCP may change them.
- `systemctl is-active ssh` returns `active`; the user subsequently confirmed that SSH login from the Mac succeeds. Authentication/security configuration has not yet been reviewed.
- Python `3.13.5` and Git `2.47.3` are installed.
- User created `~/home-iot-project/.venv`, activated it, and confirmed Python `3.13.5` runs from `/home/eeshan6868/home-iot-project/.venv/bin/python`.
- User reports the existing GitHub repository cloned successfully to `~/home-iot-project-repo` and a virtual environment was created/activated there. Git identity output, `git status`, and `git remote -v` have not been shared yet.

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
- [x] Python environment ready
- [ ] Git workflow tested
- [ ] Docker decision recorded
- [ ] Monitoring baseline established
- [ ] Backup/recovery tested
