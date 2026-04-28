---
title: "INFRA.md Template"
summary: "Workspace template for INFRA.md"
read_when:
  - Bootstrapping a workspace manually
---

# INFRA.md - Infrastructure

SENSITIVE — apply chmod 600 on your server — never share contents in chat

## VPS / Servers

| Alias | IP | User | Workspace |
|-------|----|------|-----------|
| [alias e.g. main-vps] | [IP address] | [user e.g. root] | [/path/to/workspace/] |

## SSH Access

ssh [user]@[IP address]

## Notes

- Add new servers here as your stack grows
- Reference this file from TOOLS.md — never copy IP or credentials into TOOLS.md
- After filling in real values, run: chmod 600 /root/.openclaw/workspace/INFRA.md
