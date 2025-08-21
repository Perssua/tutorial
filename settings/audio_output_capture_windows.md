# Audio Output Capture (Windows)

## Overview

Windows apps cannot capture system audio directly without a virtual audio cable. Use a driver like VB-Audio Cable to route output audio into the app.

## Prerequisites

- Administrator access on Windows
- VB-Audio Cable (or similar) installed

## Steps

1. Download and install VB-CABLE from the VB-Audio website. Run the installer as Administrator and reboot if required.
2. Open Windows Sound Settings -> Playback and set VB-CABLE as the default output device (temporarily while capturing).
3. In the app, select VB-CABLE as the audio input source.
4. Play the audio you want captured. The app will receive the system output via the virtual cable.
5. When finished, restore your original playback device in Windows Sound Settings.

## Tips

- Consider creating app-specific output assignments with per-app audio routing (Windows 10/11 Sound -> App volume and device preferences).
- Reduce latency by disabling enhancements and exclusive mode where possible.

## Troubleshooting

- No audio: confirm VB-CABLE is the default output and selected as the input in the app.
- Feedback or echo: avoid routing the app output back into the same input device.
