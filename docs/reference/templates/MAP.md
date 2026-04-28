---
title: "MAP.md Template"
summary: "Workspace template for MAP.md"
read_when:
  - Bootstrapping a workspace manually
---

# MAP.md - Workspace Directory

The index of everything. If it exists, it is listed here.
Last updated: [fill in today's date when you first set this up]

## Workspace Root

/root/.openclaw/workspace/

## Doctrine Files

| File         | Purpose                                |
| ------------ | -------------------------------------- |
| SOUL.md      | Personality and values                 |
| IDENTITY.md  | Name, vibe, emoji, communication style |
| USER.md      | Owner profile and businesses           |
| MEMORY.md    | Long-term curated memory               |
| SECURITY.md  | Access control and ops policy          |
| AGENTS.md    | Operational doctrine                   |
| TOOLS.md     | SSH aliases, key names, cheat sheet    |
| HEARTBEAT.md | Session startup checklist              |
| MAP.md       | This file — workspace index            |
| INFRA.md     | Infrastructure details (chmod 600)     |

## Memory Files

| Path                        | Purpose                    |
| --------------------------- | -------------------------- |
| memory/YYYY-MM-DD.md        | Daily session logs         |
| memory/heartbeat-state.json | Heartbeat check timestamps |

## Projects

| Project                       | Path             | Status               |
| ----------------------------- | ---------------- | -------------------- |
| [Add your first project here] | projects/[name]/ | [active/paused/done] |

## .env Files

| File              | Location          | Purpose                          |
| ----------------- | ----------------- | -------------------------------- |
| [e.g. .env]       | workspace root    | [e.g. main API keys]             |
| [project/.env]    | projects/[name]/  | [e.g. project-specific config]   |

Rule: Never store values here. Store path + purpose only.

## Skills

| Skill           | Path                    | Purpose            |
| --------------- | ----------------------- | ------------------ |
| memory-rotation | skills/memory-rotation/ | MEMORY.md rotation |

## Secrets and Infrastructure

| File     | Location       | Type     | Access    |
| -------- | -------------- | -------- | --------- |
| .env     | workspace root | API keys | chmod 600 |
| INFRA.md | workspace root | Infra    | chmod 600 |

---

Rule: Any new project, file, or key added must be registered
here before the session ends.
