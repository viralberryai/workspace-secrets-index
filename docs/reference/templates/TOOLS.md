---
title: "TOOLS.md Template"
summary: "Workspace template for TOOLS.md"
read_when:
  - Bootstrapping a workspace manually
---

# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → see INFRA.md for IP and connection details

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

### API Keys

Never print key values in chat — see SECURITY.md

```
source /root/.openclaw/workspace/.env 2>/dev/null
# Add additional: source /root/.openclaw/workspace/.env.<service> 2>/dev/null
```

---

Add whatever helps you do your job. This is your cheat sheet.

## INFRA.md

Sensitive infrastructure details (IPs, ports, hostnames, SSH config)
are stored in INFRA.md — not here.
Apply chmod 600 to INFRA.md on your server.
Reference INFRA.md from this file. Never copy values into TOOLS.md.
