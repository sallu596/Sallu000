# OpenClaw on Android via GitHub Codespaces

This setup keeps the OpenClaw Gateway in a Linux Codespace and lets the Android phone use the browser Control UI. The official Android app is a companion node and does not host the Gateway itself.

## Start

1. Open this repository in GitHub Codespaces.
2. Wait for the container setup to finish.
3. In the Codespace terminal run:

```bash
pnpm exec openclaw onboard
pnpm exec openclaw gateway --port 18789
```

4. Open the forwarded port **18789** from the Codespaces Ports panel.
5. On the Android phone, open that forwarded HTTPS URL in Chrome.

## Important

- Keep the Codespace running while you use OpenClaw.
- Do not expose the Gateway publicly without authentication.
- Do not commit API keys, tokens, passwords, or personal credentials to GitHub.
- This does not make the Android phone itself the Gateway host; the Gateway runs inside the Codespace.

## Check

```bash
pnpm exec openclaw gateway status
```
