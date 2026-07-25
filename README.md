# XIAO ESP32S3 Sense Camera Stream

Wireless camera-streaming component for a vision-enabled Digital Twin
for workforce activity monitoring.

## Hardware

- Seeed Studio XIAO ESP32S3 Sense
- OV5640 camera
- External Wi-Fi antenna
- Raspberry Pi 5

## Current functionality

- Captures camera frames using the OV5640
- Connects to a local Wi-Fi network
- Hosts an HTTP camera interface
- Provides an MJPEG stream for processing on Raspberry Pi 5

## Planned pipeline

XIAO ESP32S3 Sense → Wi-Fi video stream → Raspberry Pi 5 →
computer vision model → MQTT → Digital Twin dashboard

## Security

Wi-Fi credentials are stored in `secrets.h`, which is excluded from Git.
Copy `secrets.example.h` to `secrets.h` and enter local credentials.

## Board configuration

- Board: XIAO ESP32S3
- PSRAM: OPI PSRAM
- Flash size: 8 MB
- Partition scheme: Huge APP