# OpenAI API Key

## Overview
Perssua can connect directly to **OpenAI models** (such as GPT-4 and GPT-4o) using your own API key. This allows you to run analysis, transcription, or chat features backed by OpenAI’s infrastructure.  
This guide explains how to create an **OpenAI API key**, add it to Perssua, and understand its limitations.

---

## Prerequisites
- An **OpenAI account**: <https://platform.openai.com/>
- Perssua installed and active.
- (Optional) Billing enabled in your OpenAI account if you plan to exceed free-trial credits.

> **Security:** API keys are like passwords. Never share them publicly or commit them to code repositories.

---

## Steps — Generate an OpenAI API Key
1. Go to the [OpenAI API Keys page](https://platform.openai.com/api-keys) and log in.  
2. Click **Create new secret key**.  
3. Give it a **name** (e.g., *Perssua Integration*).  
4. Copy the generated key (it begins with `sk-...`).  
   - Important: You will only see it once. Save it securely in a password manager.  
5. Open **Perssua → Settings → Integrations → OpenAI**.  
6. Paste the key into the **API Key** field.  
7. Save changes and test with a simple prompt or screenshot analysis.

---

## Limitations & Notes
- **Free trial:** New OpenAI accounts may include a limited number of free credits. Once expired, billing is required.  
- **Usage charges:** Every request consumes tokens (input + output). Costs depend on the model selected (e.g., GPT-4o is cheaper/faster than GPT-4).  
- **Rate limits:** Your account may have per-minute limits depending on usage and billing status.  
- **Model availability:** Not all OpenAI models are exposed to every account tier. Check [OpenAI’s model list](https://platform.openai.com/docs/models).  
- **Perssua limits:** Using your own key does **not** bypass Perssua’s free-tier restrictions (e.g., max screenshots or chat history).  
- **Security:** Rotate or delete your key if it’s compromised.


---

## Tips
- Use **separate keys** for different projects for easier monitoring.  
- Track usage and costs in your [OpenAI dashboard](https://platform.openai.com/usage).  
- Store keys in a secure password manager.  
- Rotate keys periodically to reduce risk.  

## Troubleshooting
- **“Invalid key” error:** Ensure you copied the key completely and removed extra spaces.  
- **No response / quota exceeded:** Check if you have credits left or enable billing.  
- **Latency / slow responses:** Switch to a faster model (e.g., GPT-4o instead of GPT-4).  
- **Key compromised:** Delete it in the OpenAI dashboard and generate a new one. 
