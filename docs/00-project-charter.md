# Project Charter

## Purpose
Build a modular home IoT platform as a long-term technical hobby and learning project combining physical computing, software architecture, computer vision, automation and AI.

## Objectives
- Establish a reliable Raspberry Pi/Linux foundation.
- Connect and normalize sensors and cameras.
- Build a consistent event model.
- Add deterministic local automation.
- Experiment with AI/agents where they add value.
- Maintain strong documentation and evidence.

## Scope
In scope: Raspberry Pi, sensors, cameras, local networking, event processing, storage, observability, automation, computer vision, AI/agents, dashboards, security and recovery.

Initially out of scope: commercial-grade services, unrestricted autonomous actions, sensitive-data storage without an explicit design, and premature locking of later technology choices.

## Architecture principles
- Local-first where practical
- Explicit component boundaries
- Simple components before unnecessary platforms
- Observable failures
- Deterministic safety rules
- AI as interpretation/recommendation unless explicitly constrained

## Definition of Done
- Implementation complete
- Tests run
- Result recorded
- Code/config committed
- Important decisions documented
- Architecture updated when changed
- Evidence captured
- GitHub task state updated

## Open decisions
- Event transport
- Storage technology
- Camera processing location
- Local vs cloud AI
- Automation platform
- Network segmentation
- Backup/recovery
