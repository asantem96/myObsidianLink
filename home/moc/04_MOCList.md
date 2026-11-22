---
type: moc
tags:
  - moc
  - homepage
updated:
  "{ date }":
---
# 🗺️ MOC List
> [!abstract] Navigation Hub
> Central index of all Maps of Content across **Self**, **Work**, and **Collections**.

---
## 🌱 SELF (Personal & PKM)
- **[[02_Personal|Personal MOC]]** — Daily routines, health, finances, and home life
- **[[03_PKMLibrary|PKM Library MOC]]** — Reference notes, systems, and learning
- **[[Linux & Systems MOC]]** — Desktop config, scripts, self-hosted servers, troubleshooting
- **[[Design & Creative MOC]]** — Typography, graphics, video editing, UI assets

---
## 💼 WORK (Businesses & Projects)
- **[[Elasah MOC]]** — Agency offers, client onboarding, IT & digital marketing SOPs
- **[[Bear Country Ranch MOC]]** — Shiba Inu breeding records, care logs, content pipeline
- **[[Dogman MOC]]** — Brand identity, mood boards, sourcing, R&D notes
- **[[Content & Streaming MOC]]** — OBS setups, YouTube/Twitch workflows, community tools
## Core & Pinned Notes
- [[Key Note 1]] — *Brief context*
- [[Key Note 2]] — *Brief context*

---

## Sub-Topics & Related MOCs
- [[Sub-MOC 1]]
- [[Sub-MOC 2]]

---

### 3. Two Quick Rules That Keep MOCs Clean
* **Upward Link Pattern:** At the top of any regular note, add a single property or line pointing up (e.g., `moc: "[[Anime & Manga MOC]]"` or `Up: [[IT, Linux & Systems MOC]]`). That single link automatically feeds the Dataview table above.
* **Native Obsidian Bases Alternative:** If you ever want a filterable table without Dataview code, create one `moc.base` file filtered by `file.hasLink(this.file.name)` and embed `![[moc.base]]` inside any MOC note.

---
## All Linked Notes (Auto-Updated)
```dataview
TABLE WITHOUT ID
  file.link AS "Note",
  status AS "Status",
  file.mday AS "Last Modified"
FROM [[]]
WHERE file.name != this.file.name
SORT file.mtime DESC