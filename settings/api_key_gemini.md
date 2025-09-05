# Gemini API Key

## Overview
Perssua can connect to **Google’s Gemini** models via API. To enable this, you’ll generate a **Gemini API key** in Google **AI Studio** and paste it into Perssua. This guide explains how to create the key, add it to the app, and what limitations to expect.

---

## Prerequisites
- A Google account.
- Access to **Google AI Studio**: <https://aistudio.google.com/>
- Perssua installed and open.

> **Security:** Treat API keys like passwords. Do not share them or commit them to source control.

---

## Steps — Generate a Gemini API Key
1. Open **AI Studio**: <https://aistudio.google.com/>
2. In the left sidebar, click **API Keys** (or **Get API key**).
3. Click **Create API key**.  
4. Copy the generated key (usually starts with `AI…`).  
   - You may only see it once—store it securely in a password manager.
5. In Perssua, go to **Settings → Integrations → Gemini**.
6. Paste the key into **API Key** and **Save**.
7. Test by sending a short prompt in the chat to confirm the integration works.

---

## Limitations & Notes
- **Quotas & Rate Limits:** Free-tier usage is limited (requests per minute/day). Heavy usage may require upgrading your quota or enabling billing on Google’s side.
- **Regional Availability:** Some regions may not be supported. Availability and features can differ by locale.
- **Model Availability:** Not all Gemini model variants (e.g., vision, long context) may be available or supported by your plan/build.
- **Content & Safety:** Safety filters may block certain inputs/outputs. Adjust your prompts to comply with usage policies.
- **Data Handling:** Review Google’s data use and privacy terms for AI Studio. If you need stricter controls, consider a separate key or organization policies.
- **Perssua Plan Limits:** Using your own API key **does not** bypass Perssua’s product limits (e.g., free-tier screenshot caps).

---

## Tips
- Create **separate keys** per environment (dev/staging/prod) to simplify rotation and monitoring.
- Store keys in a **password manager** and rotate them if you suspect exposure.
- If requests fail due to quotas, check AI Studio usage dashboards or enable billing for higher limits.

## Troubleshooting
- **“Invalid API key”**: Remove extra spaces and confirm you copied the full key.
- **No response / Quota errors**: Check AI Studio quotas/usage and network connectivity.
- **Model not supported**: Select a supported Gemini model in Perssua or update your plan/build.
- **Permission / Region issues**: Verify that Gemini API access is available for your account and region.
