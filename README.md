# Grow Bot Sphere — Greens Monitoring Prototype

A beginner-friendly browser dashboard concept for green leafy vegetables such as spinach, amaranth (keerai), and lettuce.

## Important status
This is a **working front-end demonstration using simulated data only**. It is not connected to an ESP32 or physical sensors. N/P/K numbers are arbitrary demo units, not calibrated nutrient concentrations. Do not present these as real field measurements.

## Features
- Example soil moisture, N/P/K, ambient light, and leaf-colour indicator cards.
- Button to generate new simulated readings.
- Recent history table (up to eight readings).
- CSV download.
- Cautious observation messages; no automatic crop or disease diagnosis.
- Visible simulated-data disclaimer.

## Run it
1. Download or clone this repository.
2. Open `index.html` in a modern web browser.
3. Click **Generate new demo readings**.
4. Click **Download readings CSV** to export the current demo history.

No server, API key, or installation is needed.

## Files
- `index.html` — complete dashboard and browser-side logic.
- `sample_data.csv` — example records clearly labelled simulated.
- `architecture.md` — current and planned architecture.
- `test_cases.md` — manual testing checklist.
- `LICENSE` — MIT licence.

## Photosynthesis limitations
A BH1750 measures illuminance in lux; lux is not a direct measure of photosynthetically active radiation or photosynthesis rate. A colour sensor can record colour values but cannot independently diagnose plant disease or nutrient deficiency. Direct assessment of photosynthetic performance generally requires specialised instruments such as a chlorophyll-fluorescence system and a suitable measurement protocol.

## Planned hardware (not connected yet)
Possible future components include ESP32, a calibrated soil-moisture sensor, a validated soil-nutrient measurement method, BH1750 light sensor, and a colour sensor such as TCS34725. These are proposed options, not current hardware connections.

## Create your GitHub repository
1. Sign in at https://github.com/.
2. Create a **Public** repository named `grow-bot-sphere`.
3. Upload all files in this folder.
4. Check that `README.md` is visible on the repository page.
5. Copy the real public repository URL into your competition form.

Do not submit an empty repository or commit passwords, Wi-Fi credentials, API keys, or personal information.

## Competition honesty
Describe this as a **working browser-based software demo with simulated readings** until physical sensors are connected and tested. Do not claim real-time sensing, measured photosynthesis, verified crop recommendations, or field results unless implemented and validated.
