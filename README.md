# TeamsPlus

**TeamsPlus** is a modern, lightweight teams plugin for Minecraft servers, designed with performance, scalability, and expandability in mind.

It provides a clean team system with roles, shared team storage, optional MySQL support, and built-in team chat — without unnecessary bloat.

---

## ✨ Features

- Team creation and management
- Team roles: **Leader**, **Officer**, **Member**
- Shared **Team Vault Chest** (double chest size)
- Anti-dupe & anti-lag vault design
- Optional **MySQL storage** (YAML fallback supported)
- Team homes
- Built-in team chat (`!t` and toggle mode)
- Optional Vault economy integration (team bank)
- Fully standalone (no required dependencies)

---

## 📦 Team Vault Chest

Teams can access a shared vault:
/team chest
- 54-slot (double chest)
- Multiple members can open at once
- Async load/save (no server lag)
- Saves only after last viewer closes
- Cooldown protection to prevent spam and duplication
- Stored via YAML or MySQL depending on configuration

Command:---

## 💬 Team Chat

- `!t <message>` — Send a team-only message
- `!tchat` — Toggle team chat mode
- `/chat help` — View chat options

---

## 💾 Storage Modes

TeamsPlus supports two storage backends:

### YAML (default)
- Simple, file-based storage
- Ideal for small or private servers

### MySQL (recommended)
- Auto-creates required tables
- Scales to large servers
- Strict mode: plugin disables itself if database fails to load
- Tables are namespaced to avoid conflicts:
  - `tplus_teams`
  - `tplus_members`
  - `tplus_chests`
  - `tplus_bank`
  - `tplus_meta`

So Much More! Join Discord for help or for the open source