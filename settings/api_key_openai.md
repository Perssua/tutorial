# API Key: OpenAI

## Overview

Create an OpenAI API key and add it to the app settings.

## Prerequisites

- OpenAI account with billing set up if required

## Steps

1. Sign in to your OpenAI account.
2. Open the API Keys page under your user settings.
3. Click Create new secret key and copy it.
4. Store the key in a password manager.
5. In the app, open Settings -> API Keys -> OpenAI and paste the key.

## Tips

- Never commit keys to source control.
- Rotate keys periodically and remove unused ones.

## Troubleshooting

- 401 Unauthorized: verify the key and your account status.
- Rate limits: backoff and retry, or request higher limits.
