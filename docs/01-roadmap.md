# Roadmap

## Phase 0: Project Foundation
Goal: establish project control before hardware work.
Deliverables: repository, charter, roadmap, HLD, hardware inventory, experiment/test logs, ADR process and initial backlog.

## Phase 1: Raspberry Pi Foundation
Goal: stable, observable edge-computing base.
Focus: Raspberry Pi OS, network, SSH, users, Python, Git, Docker evaluation, monitoring, backup, service conventions, logging and updates.

## Phase 2: Camera and Vision
Goal: reliable capture and computer vision foundation.
Focus: camera interface, resolution/frame rate, capture, storage, processing location, detection model, event schema, performance and privacy.

## Phase 3: Sensors and Home Monitoring
Goal: common sensor abstraction and meaningful telemetry.
Focus: interfaces, device identity, units, timestamps, event schema, persistence and health.

## Phase 4: Local Automation
Goal: reliable deterministic actions.
Pattern: Event -> Rule -> Action.
Focus: rules, safety, idempotency, failure handling, manual override and audit logging.

## Phase 5: AI and Agent Layer
Goal: useful interpretation, summarization or controlled tool use.
Pattern: Event/Context -> AI/Agent -> Recommendation or controlled tool call -> Rule/Human approval -> Action.

## Phase 6: Integrated Home Platform
Goal: integrate sensing, events, storage, automation, AI and UI.

## Phase 7: Hardening and Showcase
Goal: reproducible, safe and presentable project.
Focus: security, recovery, reliability, documentation, demos and final project record.
