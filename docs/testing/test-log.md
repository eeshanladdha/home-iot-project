# Test Log

| ID | Date | Component | Test | Expected | Actual | Result | Evidence |
|---|---|---|---|---|---|---|---|
| TEST-001 | 2026-10-15 | Raspberry Pi 5 / Raspberry Pi OS | Install OS and connect remotely from Mac using Raspberry Pi Connect | OS boots and Pi is reachable remotely from Mac | User confirmed Raspberry Pi OS installed and Raspberry Pi Connect access from Mac works | **Pass (user-reported)** | Evidence not yet attached; capture OS version and optional screenshot/photo in project records |
| TEST-002 | 2026-10-15 | Raspberry Pi 5 baseline | Inspect OS release, model, architecture, storage layout and hostname | OS/hardware/storage details are recorded accurately | User-provided screenshot shows Debian GNU/Linux 13 (Trixie) 13.7; Raspberry Pi 5 Model B Rev 1.1; `aarch64`; `/dev/sda` 28.7 GB with `/dev/sda2` mounted at `/`; hostname `presh-iot` | **Pass (screenshot evidence reviewed)** | Screenshot shared in conversation; `df -h`, `hostname -I`, and Pi-specific OS release details still pending |
| TEST-003 | TBD | Phase 1 foundation | Validate network stability, SSH, Python/Git, monitoring and recovery | All Phase 1 exit criteria pass | Not run | Pending | TBD |
