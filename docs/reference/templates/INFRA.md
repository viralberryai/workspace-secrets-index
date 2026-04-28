---
title: INFRA.md
summary: "Workspace template for INFRA.md"
read_when:
  - Bootstrapping a workspace manually
---

# INFRA.md - Infrastructure

SENSITIVE — apply chmod 600 on your server — never share contents in chat

## VPS / Servers

| Alias                 | IP           | User             | Workspace             |
| --------------------- | ------------ | ---------------- | --------------------- |
| [alias e.g. main-vps] | [IP address] | [user e.g. root] | [/path/to/workspace/] |

## SSH Access

```bash
ssh [user]@[IP address]
# Example: ssh root@123.45.67.89
```

Add SSH key path if using key auth: `~/.ssh/[keyname]`

## API Key Locations

| Key Name              | .env File Location      | Service          |
| --------------------- | ----------------------- | ---------------- |
| [e.g. OPENAI_API_KEY] | [/path/to/.env]         | [e.g. OpenAI]    |

Note: List location and service only — never paste key values here.

## Ports & Services

| Port  | Service         | Notes                       |
| ----- | --------------- | --------------------------- |
| 22    | SSH             | [restrict to your IP]       |
| [80]  | [e.g. web app]  | [add as needed]             |

## Domains

| Domain              | Points To      | Purpose           |
| ------------------- | -------------- | ----------------- |
| [yourdomain.com]    | [IP/service]   | [e.g. main site]  |

## Notes

- Add new servers here as your stack grows
- Reference this file from TOOLS.md — never copy IP or credentials into TOOLS.md
- After filling in real values, run: chmod 600 /root/.openclaw/workspace/INFRA.md
- This file is registered in MAP.md under Secrets and Infrastructure. Keep both in sync.
