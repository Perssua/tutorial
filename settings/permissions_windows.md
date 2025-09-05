# Windows Permissions

## Overview
Perssua requires certain **Windows permissions** to capture your screen, record audio, and display notifications.  
Without these permissions, features like **Screenshot Capture (Ctrl + E)** or **Whisper (Ctrl + D)** will not work.  

This guide explains **why** we need these permissions and how to grant them step by step.

---

## Why permissions are needed
- **Screen Capture:** Required so Perssua can grab screenshots of your apps/windows for analysis. Windows controls this to protect user privacy.  
- **Microphone:** Required for Whisper and other audio features (Ctrl + D). Without this, Perssua cannot transcribe speech.  
- **Notifications:** Required so Perssua can show system notifications (e.g., analysis completed).  
- **Background Apps (optional):** Allows Perssua to keep listening for shortcuts when minimized.

---

## Steps — Grant Permissions on Windows

### Enable Screen Capture
1. Open **Settings → Privacy & security**.  
2. Scroll to **App permissions → Camera & screen capture** (varies slightly by Windows version).  
3. Ensure **Allow desktop apps to capture your screen** is toggled **On**.  
4. Verify that **Perssua** is listed and enabled.  

### Enable Microphone
1. Go to **Settings → Privacy & security → Microphone**.  
2. Toggle **Microphone access** to **On**.  
3. Under **Let desktop apps access your microphone**, ensure **On**.  
4. Make sure **Perssua** appears in the list with access allowed.  

### Enable Notifications
1. Go to **Settings → System → Notifications**.  
2. Locate **Perssua** in the app list.  
3. Toggle notifications **On**.  
4. Optionally, customize notification style (banner, sound, priority).  

### Allow Background Apps (optional)
1. Open **Settings → Apps → Installed apps**.  
2. Select **Perssua → Advanced options**.  
3. Under **Background apps permissions**, choose **Let this app run in background**.  

---

## Shortcuts to Test After Permissions
- **Ctrl + E** — Capture a screenshot (requires Screen Capture).  
- **Ctrl + Enter** — Analyze the most recent screenshot.  
- **Ctrl + D** — Record & transcribe audio (requires Microphone).  
- **Ctrl + B** — Toggle app visibility (requires background permission for global shortcuts).  
- **Ctrl + Up/Down** — Scroll the Perssua chat.  

---

## Tips
- After changing permissions, restart Perssua to apply changes.  
- If permissions don’t appear in the list, try triggering the feature once (e.g., attempt a screenshot) so Windows prompts you.  
- Use **Windows + I** shortcut to quickly open **Settings**.  

## Troubleshooting
- **Screenshot not captured:** Ensure *Allow desktop apps to capture your screen* is on.  
- **Microphone not working:** Check that the correct input device is selected in **Settings → Audio → Input**.  
- **No notifications:** Verify Focus Assist (Do Not Disturb) is disabled.  
- **Shortcuts not working in background:** Ensure background app permissions are enabled.  

