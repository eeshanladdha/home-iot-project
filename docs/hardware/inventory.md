# Hardware Inventory

Authoritative project hardware list. Status is tracked separately from purchase state so the inventory stays useful through setup and testing.

## Ordered hardware

| ID | Component | Exact model / part | DigiKey / reference | Phase | Qty | Status | Purpose |
|---|---|---|---|---|---:|---|---|
| HW-001 | Raspberry Pi 5 | SC1432 / Raspberry Pi Pi 5 8GB | 2648-SC1432-ND | 1 | 1 | **Ordered** | Main edge computer |
| HW-002 | Raspberry Pi case | SC1159 | 2648-SC1159-ND | 1 | 1 | **Ordered** | Pi protection/cooling enclosure |
| HW-003 | Raspberry Pi PSU | SC1407, 27W USB-C EU white | 2648-SC1407-ND | 1 | 1 | **Ordered** | Stable Pi power |
| HW-004 | Light sensor | SEN0097 / BH1750 | 1738-1100-ND | 3 | 1 | **Ordered** | Ambient light measurement |
| HW-005 | Jumper wires M-M | Adafruit 1956, 3", 28AWG | 1528-1966-ND | 1-3 | 1 | **Ordered** | Breadboard/prototyping connections |
| HW-006 | Header wires F-M | Adafruit 5018, 10 headers | 1528-5018-ND | 1-3 | 1 | **Ordered** | GPIO/breadboard connections |
| HW-007 | Jumper wires F-F | Adafruit 1951, 3", 28AWG | 1528-1962-ND | 1-3 | 1 | **Ordered** | GPIO/prototyping connections |
| HW-008 | Temperature/humidity/pressure sensor | BME280, I2C/SPI, 3.3V/5V listing | User order | 3 | 1 | **Ordered** | Environmental telemetry |
| HW-009 | Arduino UNO R3 starter kit | Breadboard, LEDs, jumper cables and accessories | User order | 1-3 | 1 | **Ordered** | Electronics learning/prototyping |

## Previously planned / not yet ordered

| ID | Component | Model | Phase | Status | Purpose | Notes |
|---|---|---|---|---|---|---|
| HW-010 | Camera | SC1174 | 2 | Planned | Primary vision camera | Planned for Phase 2 |
| HW-011 | Camera | SC1785 | TBD | **Not required currently** | Optional/specialized vision | Do not purchase unless a concrete Phase 2+ use case requires it |
| HW-012 | Additional storage | TBD | 1 | TBD | OS/data storage if required | Reassess after Pi 5 setup |
| HW-013 | Additional sensors | TBD | 3+ | TBD | Home telemetry | Select based on experiments |

## Current purchase summary

The ordered DigiKey subtotal supplied for items HW-001 to HW-007 is **1,929.51 NOK**. The BME280 and Arduino UNO R3 starter kit were also ordered separately at **220 NOK** and **110 NOK** respectively, giving a supplied combined hardware total of **2,259.51 NOK** before any additional shipping/tax differences.

## Phase mapping

### Phase 1
- Raspberry Pi 5 8GB
- Official 27W EU PSU
- Raspberry Pi case
- Jumper/prototyping accessories
- Arduino starter kit can be used for electronics learning, but it is not required for the Pi foundation.

### Phase 2
- Camera SC1174 remains planned.
- SC1785 is not currently required.

### Phase 3
- BME280
- BH1750
- Breadboard/jumper accessories

## Status rules

- **Planned**: identified but not ordered.
- **Ordered**: purchase placed, parcel not yet confirmed received.
- **Received**: physically received and checked.
- **Installed**: connected and configured.
- **Validated**: tested successfully with evidence.
- **Retired**: no longer part of the active setup.

Update the status as hardware moves through these states. Record exact board/module revisions when received because breakout-board implementations can differ.

## Inventory rules

- Record exact part number where possible.
- Keep optional hardware explicitly TBD.
- Update this file when hardware changes the architecture.
- Do not treat an ordered component as available for implementation until it is physically received and checked.
