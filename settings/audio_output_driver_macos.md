# Audio Output Driver (macOS)

## Overview

macOS requires a virtual audio driver (e.g., BlackHole or Soundflower) to capture system audio for transcription or analysis.

## Prerequisites

- Administrator access on macOS
- A virtual audio driver such as BlackHole (2ch)

## Steps

1. Install BlackHole: using Homebrew `brew install blackhole-2ch` or download from the official repository and run the installer.
2. Approve any security prompts under System Settings -> Privacy & Security (System Extensions).
3. Open Audio MIDI Setup and create a Multi-Output Device combining your built-in output and BlackHole.
4. Set the Multi-Output Device as the system output.
5. In the app, choose BlackHole as the audio input.
6. Test by playing audio and verifying that the app receives it.

## Tips

- Create a dedicated Multi-Output Device profile for quick switching.
- Label devices clearly to avoid confusion.

## Troubleshooting

- No audio: ensure sample rates match in Audio MIDI Setup.
- Echo/feedback: avoid routing the app output back into the input device.
- Revert: switch system output back to your speakers and select the normal input in the app.
