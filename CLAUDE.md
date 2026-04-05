# Java Wiki — Agent Rules

Read this file at the start of every session.

---

## Purpose

This is a Java learning wiki for a beginner. Keep explanations simple and use analogies.

---

## Directory Structure

```
wiki/
  index.md       — list of all pages
  log.md         — activity log (append only)
  concepts/      — concept pages (user writes these directly)
  errors/        — error pages
  snippets/      — code snippet pages
```

---

## Your Two Jobs

You only ever do two things:

1. **Update index.md** when a new page exists
2. **Append a line to log.md** to record what happened

---

## Command: "index this"

User will say "index this: wiki/concepts/foo.md — short description"

Do exactly this:

**Step 1** — Add a line to the correct section in wiki/index.md:
```
| [Page Title](concepts/foo.md) | short description |
```
Note: encode spaces as `%20` in the path, never use single quotes. Example: `[Title](concepts/foo%20bar.md)`

**Step 2** — Append to wiki/log.md:
```
[DATE] INDEX: concepts/foo.md added to index
```

---

## Command: "log this"

User will say "log this: <message>"

Do exactly this — append one line to wiki/log.md:
```
[DATE] NOTE: <message>
```

---

## Command: "what do I know about X?"

1. Read wiki/index.md
2. Find a matching page and read it
3. Answer from what is in the page. If no match, say: "Not in the wiki yet."
4. Append to log.md: `[DATE] QUERY: X`

---

## log.md format

One line per entry:
```
[YYYY-MM-DD] ACTION: details
```

Actions: INDEX, QUERY, NOTE, CREATE, UPDATE, ERROR

Never delete any line from log.md.
