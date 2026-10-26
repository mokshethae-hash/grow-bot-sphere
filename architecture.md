# Technical Design: Grow Bot Sphere

## Current prototype architecture
```text
Open index.html in browser
        |
        v
JavaScript generates simulated readings
        |
        +--> Dashboard cards
        +--> Cautious observation messages
        +--> Recent-reading table
        +--> CSV download
```

## Current fields
| Field | Meaning | Status |
|---|---|---|
| Soil moisture | Example percentage | Simulated |
| N, P, K | Arbitrary example values | Simulated, not nutrient units |
| Light | Example ambient illuminance in lux | Simulated |
| Leaf colour indicator | Example category | Simulated |
| Data type | Identifies source | Always SIMULATED |

## Planned hardware architecture — not implemented
```text
Soil moisture sensor ----Validated NPK method -----\
BH1750 light sensor --------> ESP32 --> Wi-Fi/API --> Dashboard
Leaf colour sensor --------/
```
Sensor models, calibration, wiring, communication protocol, and backend must be finalised before claiming hardware operation.

## Safeguards
- Keep simulated-data labels until real readings are verified.
- Calibrate sensors and document units before using readings for decisions.
- Do not infer photosynthesis rate from lux or leaf colour alone.
- Do not diagnose disease or prescribe fertiliser from one reading.
