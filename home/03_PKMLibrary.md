---
type: pkm-library
tags:
  - moc
  - pkm-library
updated:
  "{ date }":
---
# 📚 PKM Library

> [!info] Knowledge Hub
> Structured reference notes, system guides, and evergreen research—organized by topic rather than buried in folders.
> **Back to:** [[01_Homepage|🏠 Homepage]] · **Index:** [[04_MOCList|🗺️ MOC List]]

---

## 🛠️ Tech, Linux & Media Stack
> [!tip] Systems & Self-Hosting
> Guides, configs, and troubleshooting notes for your desktop, servers, and media tools.

* 🖥️ **[[Linux & Desktop Setup]]** — OS tuning, graphics, compositors, and fonts
* 🎬 **[[Media DB & Self-Hosting]]** — Media DB, OMDb/Tenrai, Jellyfin, and Navidrome
* 📡 **[[Streaming & Audio Workflows]]** — OBS Studio, rich presence, and live production
* 🌐 **[[Web, Design & Typography]]** — UI styling, layout systems, and custom fonts

---

## 💼 Business, Operations & Strategy
> [!abstract] Ventures & Execution
> Frameworks, templates, and reference playbooks across your active and planned ventures.

* ⚡ **[[Elasah - IT & Marketing Playbook]]** — Service offers, client onboarding, and SOPs
* 🐕 **[[Bear Country Ranch - Care & Content]]** — Shiba Inu husbandry, content batches, and merch notes
* 🧥 **[[Dogman - Brand & R&D]]** — Aesthetic direction, materials research, and release notes
* 📈 **[[Growth, Distribution & Media]]** — Audience building, distribution models, and ops

---

## 🧠 Research, Deep Dives & Reference
> [!note] Evergreen Notes & Studies
> Long-form notes, empirical breakdowns, and topic studies worth revisiting.

* 📖 **[[Reading & Book Notes]]** — Takeaways, highlights, and summaries
* 🥋 **[[Biomechanics & Kinetic Chain]]** — Movement physics, timing, and mechanics notes
* 📜 **[[Comics, Grading & Collectibles]]** — Evaluation criteria, market notes, and cataloging
* ⚖️ **[[Policy, Law & Civic Reference]]** — Statutes, ordinances, and public records notes

---

## 📥 Inbox & Unsorted Notes
Notes created quickly that still need tags, links, or a clean summary:

```dataview
TABLE WITHOUT ID
  file.link AS "Note",
  file.folder AS "Folder",
  file.cday AS "Created"
FROM ""
WHERE !contains(file.tags, "pkm") AND !contains(file.tags, "moc") AND (contains(file.folder, "Inbox") OR !status)
SORT file.cday DESC
LIMIT 15