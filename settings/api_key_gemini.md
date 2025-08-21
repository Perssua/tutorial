# API Key: Gemini

## Overview

Create a Gemini API key via Google Cloud Console and configure it in the app.

## Prerequisites

- Google Cloud account
- A project with the Gemini API enabled

## Steps

1. In Google Cloud Console, select your project.
2. Go to APIs & Services -> Enabled APIs and enable Gemini API (if not already enabled).
3. Navigate to APIs & Services -> Credentials.
4. Click Create Credentials -> API key.
5. (Recommended) Click Restrict Key to limit usage to the Gemini API.
6. Copy the key and add it to the app under Settings -> API Keys -> Gemini.

## Tips

- Use key restrictions (API and HTTP referrer/app restrictions) to reduce risk.
- Monitor quota and usage in the Cloud Console.

## Troubleshooting

- Permission denied: ensure the correct project is selected and the API is enabled.
- Quota exceeded: request increases or reduce usage.
