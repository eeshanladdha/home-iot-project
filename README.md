# Home IoT Project

A hands-on home IoT and edge-AI project focused on Raspberry Pi, sensors, computer vision, local automation, event-driven architecture, observability and AI/agent integration.

## Goals
- Build a real incremental home IoT platform.
- Learn Raspberry Pi, Linux, networking, electronics, sensors and cameras.
- Apply HLD, LLD, ADRs, event models, security and observability.
- Add AI only after a reliable deterministic foundation exists.
- Keep the system local-first where practical.
- Capture experiments, evidence and lessons learned.

## Roadmap
| Phase | Focus | Status |
|---|---|---|
| 0 | Project foundation | In progress |
| 1 | Raspberry Pi foundation | **In progress: OS installed; Raspberry Pi Connect access from Mac verified** |
| 2 | Camera and vision | Planned |
| 3 | Sensors and monitoring | Planned |
| 4 | Local automation | Planned |
| 5 | AI and agent layer | Planned |
| 6 | Integrated home platform | Planned |
| 7 | Hardening and showcase | Planned |

## Baseline architecture
Sensors/Cameras -> Edge Devices -> Event Layer -> Processing/Storage/Rules/AI -> Dashboard/User

Technology choices such as event transport, storage, camera processing, AI provider, automation platform and network segmentation remain TBD until experiments provide evidence.

## Principles
1. Local-first
2. Modular
3. Event-driven
4. Observable
5. Secure by default
6. Incremental
7. Deterministic automation separated from AI
8. Evidence-driven decisions

## Project control
Backlog -> Selected -> Implement -> Test -> Validate -> Log Results -> Document Decision -> Complete

Completed work should leave evidence: code/commit, test result, logs, documentation and, where relevant, an ADR.

## Current state (2026-10-15)
- Current phase: Phase 1, Raspberry Pi Foundation
- Hardware: user confirms the order has arrived; inventory statuses updated, with part/revision cross-check still pending
- Raspberry Pi OS: installed
- Remote access: Raspberry Pi Connect tested successfully from Mac
- Remaining Phase 1 work: record OS/storage details, verify network stability, configure SSH securely, set up Python/Git, decide Docker vs native, add monitoring/logging and test backup/recovery
- Next focus: finish the Phase 1 baseline before starting camera or sensor implementation

See `docs/00-project-charter.md`, `docs/01-roadmap.md` and `docs/02-hld.md`.

## Safety and privacy
Do not commit credentials, private keys, sensitive camera images, network secrets or personal data. Use environment templates and appropriate secret handling.

## License
TBD
