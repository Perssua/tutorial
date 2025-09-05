# Capture Output Audio on Windows (Third-Party)

## Overview
This guide shows how to capture **system/output audio** (“what you hear”) on Windows using a third-party app. You can either route audio into Perssua (virtual device) or record/analyze it externally and send results back to the app.  
**Important:** always test with a short call or sample playback before going live, and verify local laws/policies about recording audio.

## Prerequisites
- Windows 10 or 11 with admin rights.
- Audio drivers up to date.
- Permission to record audio when required (company/compliance).
- One of the third-party tools below installed:
  - **Option A (Routing):** [VB-Audio Virtual Cable] – creates a virtual output/input pair to route system audio.
  - **Option B (Recording):** **OBS Studio** – captures “WASAPI loopback” (system audio) and can record or monitor it.

---

## Option A — VB-Audio Virtual Cable (route system audio to Perssua)
Use this when you want apps to “see” your system audio as a microphone-like input.

### Steps
1. **Install VB-Audio Virtual Cable** and reboot if prompted.
2. Open **Windows Sound Settings → System → Sound → Output** and set **CABLE Input (VB-Audio Virtual Cable)** as the **default output** (or only switch the app you care about via *App volume and device preferences*).
3. In **Input**, confirm **CABLE Output** exists (this is the virtual “microphone” that carries your system audio).
4. In **Perssua → Settings → Audio**, choose **CABLE Output** as the **input device** to feed system audio into the app.
5. *(Optional monitoring)* If you need to hear the sound while routing:
   - Open **Control Panel → Sound → Recording** tab.
   - Double-click **CABLE Output** → **Listen** tab → enable **Listen to this device** and choose your real speakers/headset.
6. Play a test video or music and verify the input meter moves in Perssua.

### Notes
- Keep volume moderate to avoid clipping.
- If you only need to route a single app (e.g., browser), use **Advanced sound options** to select output device per-app instead of changing the system default.

---

## Option B — OBS Studio (WASAPI Loopback recording/monitoring)
Use this when you prefer a recorder/monitor for system audio and optionally save files.

### Steps
1. Install **OBS Studio**.
2. In OBS, click **+** under **Sources** → **Audio Output Capture** → choose **Capture audio** → select your **system output device** (or pick **Default**).
3. Alternatively, use **WASAPI (Loopback)** by selecting the exact playback device to capture system audio precisely.
4. To **monitor** what’s captured:  
   - Go to **Edit → Advanced Audio Properties**.  
   - For the output source, set **Audio Monitoring = Monitor and Output** (choose your headphones as Monitoring Device in **Settings → Audio**).
5. To **record**, set the format in **Settings → Output** and press **Start Recording**.
6. If you need to feed this into Perssua, you can pair OBS with a virtual device (e.g., VB-Cable) and route OBS output to the virtual input Perssua listens to.

---

## Verify in Perssua
1. Open **Settings → Audio** and select the intended **Input**:
   - **CABLE Output** (Option A), or your normal microphone if you’re only recording in OBS (Option B).
2. Speak/play audio; check the input meter.
3. Run a short feature test (e.g., transcription or analysis) to confirm.

---

## Shortcuts
- **VB-Audio Virtual Cable:** no native global shortcuts (routing is persistent).  
  - *Tip:* If you need quick toggles, consider creating system-wide hotkeys via **AutoHotkey** (optional).
- **OBS Studio:** configure your own hotkeys in **Settings → Hotkeys** (e.g., *Start/Stop Recording*, *Mute/Unmute*, *Toggle Audio Monitoring*).
---

## Tips
- If audio sounds distorted, lower the source app’s volume and/or reduce Windows output level.
- Keep only one “listen/monitor” path active to avoid echo/feedback.
- On laptops with power saving, disable “audio enhancements” and set **High performance** for consistent capture.

## Troubleshooting
- **No signal in Perssua:** Ensure the correct **Input** is selected (e.g., *CABLE Output*) and that the source app is routed to **CABLE Input**.
- **Echo/feedback:** Disable duplicated monitoring (uncheck *Listen to this device* or set OBS monitoring to *Monitor (Off)*).
- **OBS recording silent:** Verify the correct playback device is chosen for **Audio Output Capture** or use **WASAPI Loopback** of the exact device.
- **Choppy audio:** Close heavy apps, lower OBS recording bitrate, or switch power plan to **High performance**.