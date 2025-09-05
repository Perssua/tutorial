# Prompts & Custom Prompts (Premium)

## Overview
A **prompt** is the instruction set that guides the AI on *what to do*, *how to respond*, and *in which context*. Well-designed prompts generate more useful, consistent, and goal-oriented outputs.  
With the **Custom Prompt (Premium)** feature, you can create reusable templates to standardize analysis, tone of voice, and focus across teams and projects.

## Why prompts matter
- **Clarity → better output:** clear instructions reduce ambiguity.  
- **Right context:** results are more relevant when the AI knows *for whom* and *why*.  
- **Consistency across users:** templates help different users maintain the same quality.  
- **Speed:** less rework and fewer follow-up requests.

### Prompt blueprint (recommended)
Include these blocks in your template:
- **Role:** “You are a pre-sales analyst focused on objection handling.”  
- **Objective:** “Summarize the call in 5 bullets with next steps.”  
- **Context:** audience, product, constraints, examples.  
- **Style & Constraints:** tone, format (Markdown/table), word or token limits.  
- **Inputs:** variables like `{client}`, `{product}`, `{language}`, `{goal}`.

## Prerequisites
- Active Perssua plan.  
- Permission to save settings (Custom Prompt requires **Premium**).  
- (Optional) Input sources: transcripts, screenshots, notes.

---

## Steps — Using a standard prompt
1. Open **Features → Prompts**.  
2. Select a **Prompt** from the list (e.g., *Call Summary*, *Objection Analysis*).  
3. (Optional) Fill in variables (e.g., `{language = en-US}`).  
4. Click **Apply** and send your input (text/audio/screenshot) via chat.  

## Steps — Creating a Custom Prompt (Premium)
1. Go to **Settings → Prompts → New Custom Prompt**.  
2. Add a **Name** and **Description**.  
3. Paste your template content (use the *blueprint* above).  
4. Add **Variables** (e.g., `{client}`, `{goal}`, `{language}`) and set default values.  
5. (Optional) Mark **Set as default** for:  
   - A specific feature (e.g., Whisper / Screenshot Analysis).  
   - A context (e.g., *Demos*, *Support*, *Onboarding*).  
6. Save with **Create**.  
7. In the chat, select your **Custom Prompt** and **Apply** before sending input.  

## Audio Settings (for prompts used with Whisper)
- **Input device:** choose the correct microphone in **Settings → Audio**.  
- **Input level & noise suppression:** adjust to avoid clipping or background noise.  
- **Language:** set your primary language for more accurate transcription.  

---

## Shortcuts
> *There is no default global shortcut to open Prompts.*  
> If available, go to **Settings → Shortcuts** to create a hotkey for “Open Prompts.”  

Helpful related shortcuts:  
- **Ctrl + D** — Record & transcribe audio (Whisper).  
- **Ctrl + E** — Capture a screenshot.  
- **Ctrl + Enter** — Analyze the most recent screenshot.  
- **Ctrl + Up/Down** — Scroll Perssua chat.  
- **Ctrl + B** — Toggle app visibility.  

## Tips
- Use **variables** in templates to reuse prompts across scenarios.  
- Add **example outputs** (few-shot) to guide format and structure.  
- Combine **Ctrl + E** → **Ctrl + Enter** for quick analysis loops with the same prompt.  
- Keep prompts concise, direct, and structured with lists/tables where possible.  

## Troubleshooting
- **Prompt ignored or generic output:** verify the correct prompt is applied before sending.  
- **Too long responses:** add limits (e.g., “max 5 bullets,” “≤120 words”).  
- **Wrong tone or focus:** refine the *Role* and *Objective* sections in your template.  
- **Whisper not sending to AI:** enable “auto-send” or click **Send to AI** after transcription.  
