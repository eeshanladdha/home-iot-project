# High-Level Design

## Architecture
Home -> Sensors / Cameras / Devices -> Edge Ingestion -> Event Bus -> Processing / Storage / Automation -> AI / Agents -> User Interface

## Components
### Sensors and Inputs
Physical sensors and external inputs produce measurements/events.

### Edge Devices
Raspberry Pi and related hardware provide capture, local processing and connectivity.

### Event Layer
Normalizes communication between components. Technology is TBD.

### Processing
Transforms raw input into measurements, detections or derived events.

### Storage
Stores only data needed for operation, analysis and learning. Technology and retention are TBD.

### Automation
Deterministic rules evaluate events and execute constrained actions.

### AI / Agents
Interpret context, summarize information or perform explicitly permitted tool calls.

### UI and Monitoring
Provide status, history, configuration, logs, metrics and evidence.

## Deterministic automation vs AI
AI -> Recommendation/Interpretation -> Rule/Human Approval -> Action

AI should not silently replace deterministic safety rules.

## Cross-cutting concerns
Authentication, authorization, network isolation, secrets, logging, metrics, backup/recovery, retention and privacy.
