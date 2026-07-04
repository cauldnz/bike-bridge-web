# Bike Bridge — Web Bluetooth console

A single-page Web Bluetooth app for the nRF52840 "Bike Bridge": a BLE power-meter
repeater-with-correction plus on-board IMU recording for track sessions.

**Use it:** open the GitHub Pages URL in Chrome/Edge (desktop or Android) or Bluefy (iOS),
tap *Connect to bridge*, and pick the device (default name "SB20 Bridge").

- Live power in/out, cadence, balance, and the active correction
- Edit correction (scale/offset), source filter, and broadcast identity over BLE
- Start/stop bounded IMU recording (13–104 Hz) and download it as CSV (CRC-checked)

The GATT contract this consumes is versioned and documented in the firmware repo
(`firmware-nrf/GATT.md`). Plain static HTML/JS — no build step, no external requests.
