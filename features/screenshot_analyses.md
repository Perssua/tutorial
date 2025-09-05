# Screenshot Capture & ASK Context

## Overview
Use screenshots to show the AI exactly what you see on screen and request targeted analysis. You can capture one or multiple screenshots, optionally add an **ASK** (a short instruction or question that provides extra context), and then send everything for analysis.

## Prerequisites
- Screen capture permissions granted by the OS (Windows/macOS).
- Perssua app open and active.
- Stable internet connection.

---

## Steps

### A) Capture screenshots
1. Open the page/app you want to analyze.
2. Press **Ctrl + E** to capture a screenshot.  
   - Repeat **Ctrl + E** to add more screenshots to the same request (batch).
3. (Optional) Remove any unintended capture from the queue (Trash/Remove on the thumbnail).

### B) Add context with **ASK**
4. In the **ASK** field, type a concise instruction or question to guide the model.  
   - Examples:  
     - “Find UI issues and suggest fixes.”  
     - “Summarize key errors in the console and next steps.”  
     - “Where is the pricing button on this page?”  
   - Keep it specific and outcome-oriented.

### C) Analyze
5. Press **Ctrl + Enter** to analyze the latest captured screenshot(s) **or** click **Analyze**.
6. Review the model’s response in the chat panel.
7. If needed, iterate: capture another screenshot (**Ctrl + E**) and refine the **ASK**.

---

## Free tier limits
- **Screenshots per analysis (Free):** up to **X** screenshots in a single request.  
  > Replace **X** with your current free-tier cap (e.g., **3**). Check **Settings → Plan** for the latest limits.  
- Larger batches and higher history limits are available on paid plans.

---

## Shortcuts
- **Ctrl + E** — Capture a screenshot.  
- **Ctrl + Enter** — Analyze the most recent screenshot(s).  
- **Ctrl + Up/Down** — Scroll the Perssua chat up/down. 

---

## Tips
- **Be specific in ASK:** “Highlight inconsistent spacing and propose CSS fixes” is better than “Improve design.”
- **Batch smartly:** Group related screens (e.g., Page → Modal → Error state) in one request to preserve context.
- **Redact sensitive data** before capturing or blur the region if needed.
- **Tight feedback loops:** **Ctrl + E** → **Ctrl + Enter** makes iterate-and-fix cycles fast.

## Troubleshooting
- **Shortcut not working:** Ensure Perssua is focused, or check if another app is intercepting the hotkey.
- **Blank/black images on macOS:** Re-enable **Screen Recording** permission for Perssua and restart the app.
- **Upload failures:** Check connectivity; large/high-DPI captures may take longer—try a smaller region or window.
- **Irrelevant answers:** Refine the **ASK** with clearer intent (what to check, constraints, desired format).