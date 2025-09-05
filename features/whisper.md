# Whisper

## Overview
Whisper transcribes your voice and can send transcripts to the AI. Use **manual mode** for on-demand capture or **automatic mode** to transcribe and send every _N_ seconds. Always test with a short sample before live use.

## Prerequisites
- Working microphone connected and selected in the app.
- OS permissions granted (Microphone; on Windows/macOS, allow the app to access audio).
- Stable network connection.

## Steps

### Manual (on-demand)
1. Open **Features → Whisper**.
2. Click the **Microphone** icon **or press `Ctrl + D`** to capture speech.
3. Review the transcript and **click _Send to AI_**.
4. Read the response in the chat panel.

### Automatic (every N seconds)
1. Open **Features → Whisper**.
2. Toggle **Auto Transcribe** **On**.
3. Set the **Interval** (e.g., **10s**).
4. Enable **Auto-send to AI** (if available) so each chunk is sent automatically.
5. Monitor transcripts and replies in the chat panel.

## Audio Settings
- **Input device:** Choose the correct microphone in **Settings → Audio**.
- **Input level / gain:** Adjust so normal speaking peaks below clipping.
- **Noise suppression:** Enable to reduce background noise.
- **Echo cancellation (if available):** Useful when using speakers instead of headphones.
- **Language (optional):** Select your primary speaking language for better accuracy.

## Shortcuts
- **`Ctrl + D`** — Record & transcribe audio (manual capture).
- Related (optional workflow):
  - **`Ctrl + E`** — Capture a screenshot.
  - **`Ctrl + Enter`** — Analyze the most recent screenshot.

## Tips
- Continuous transcription may consume credits—use sensible intervals (e.g., 10–20s).
- For best accuracy, speak close to the mic and reduce room noise.
- Use headphones to avoid echo during calls.

## Troubleshooting
- **No input detected:** Select the right microphone and check OS permissions.
- **Low accuracy:** Confirm language setting and reduce background noise.
- **Delays or missed chunks:** Lower the interval, close heavy apps, or improve network quality.
- **Clipping/distortion:** Reduce input gain in **Settings → Audio**.
