# macOS Permissions

## Overview
Perssua requires certain **macOS permissions** to capture screenshots, transcribe audio, and analyze what’s on your screen.  
Without these permissions, features like **Screenshot Capture (Ctrl + E)** or **Whisper (Ctrl + D)** will not work.  

This guide explains **why** we need the permissions and how to grant them step by step.

---

## Why permissions are needed
- **Screen Recording:** Required so Perssua can capture your screen or window when you press **Ctrl + E** and then analyze it. macOS protects this to prevent unauthorized screen grabs.  
- **Microphone:** Required for Whisper and other audio features (Ctrl + D). macOS blocks microphone access by default for privacy.  
- **Accessibility:** Required so Perssua can respond to global shortcuts (like **Ctrl + B** to toggle visibility) even when the app is not in focus.  
- **Notifications (optional):** Lets Perssua show alerts (e.g., analysis completed).  

---

## Steps — Grant Permissions on macOS
1. Open **System Settings** (macOS Ventura or later) or **System Preferences** (macOS Monterey or earlier).  
2. In the left sidebar, click **Privacy & Security**.  
3. Under **Privacy**, locate and adjust the following categories:

### Screen Recording
- Select **Screen Recording**.  
- Check the box next to **Perssua**.  
- If Perssua is not listed, try capturing a screenshot once (**Ctrl + E**) so macOS prompts you.

### Microphone
- Select **Microphone**.  
- Enable the checkbox for **Perssua**.  
- Speak into the mic and test with Whisper.

### Accessibility
- Select **Accessibility**.  
- Check **Perssua** to allow global shortcut control.  
- This ensures features like **Ctrl + B** (toggle app visibility) work outside the app window.

### Notifications (optional)
- Select **Notifications**.  
- Enable **Allow Notifications** for Perssua if you want system alerts.  

---

## Shortcuts to Test After Permissions
- **Ctrl + E** — Capture a screenshot (requires Screen Recording).  
- **Ctrl + Enter** — Analyze the most recent screenshot (requires Screen Recording).  
- **Ctrl + D** — Record & transcribe audio (requires Microphone).  
- **Ctrl + B** — Toggle app visibility (requires Accessibility).  


---

## Tips
- After enabling a permission, macOS may prompt you to **quit and reopen Perssua**. Do this to apply changes.  
- If permissions don’t appear, try triggering the feature once (e.g., take a screenshot) so macOS prompts you.  
- Keep your macOS updated to avoid bugs in the Privacy & Security panel.  

## Troubleshooting
- **Feature still blocked:** Go back to Privacy & Security → remove Perssua → restart the app → re-enable.  
- **Option grayed out:** Unlock the padlock icon in the bottom left with your admin password.  
- **No prompt appears:** Manually add Perssua by clicking the **+** button and selecting the app in Applications.  

