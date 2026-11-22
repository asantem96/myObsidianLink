---
type: moc
tags:
  - moc
  - templates
updated:
  "{ date }":
---

# {{title}}

> **Parent Hub:** [[00 - Home MOC]]

## Core & Pinned Notes
- [[Key Note 1]] — *Brief context*
- [[Key Note 2]] — *Brief context*

---

## Sub-Topics & Related MOCs
- [[Sub-MOC 1]]
- [[Sub-MOC 2]]

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



---
---

### 3. Two Quick Rules That Keep MOCs Clean * **Upward Link Pattern:** At the top of any regular note, add a single property or line pointing up (e.g., `moc: "[[Anime & Manga MOC]]"` or `Up: [[IT, Linux & Systems MOC]]`). That single link automatically feeds the Dataview table above. * **Native Obsidian Bases Alternative:** If you ever want a filterable table without Dataview code, create one `moc.base` file filtered by `file.hasLink(this.file.name)` and embed `![[moc.base]]` inside any MOC note. [Obsidian People Note System and Template](https://www.youtube.com/watch?v=N8K41HDRI3o) This walkthrough shows how to pair a centralized MOC index page with templated notes and auto-updating lists in Obsidian.