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
3. Answer from what is in the page. If no match, say: "Not in the wiki yet. Want me to create a stub?"
4. Append to log.md: `[DATE] QUERY: X`

---

## Command: "create stub for X"

Write a new file at wiki/concepts/x.md with this structure:

    # X
    
    ## What is it?
    
    ## Why does it matter?
    
    ## How it works
    
    ## Common mistakes
    
    ## Related concepts

Then index it (follow "index this" steps above).

---

## log.md format

One line per entry:
```
[YYYY-MM-DD] ACTION: details
```

Actions: INDEX, QUERY, NOTE, CREATE, UPDATE, ERROR

Never delete any line from log.md.

---

## Hard Rules

- Do not overwrite a page without appending an UPDATE entry to log.md
- Do not assume Java knowledge — explain everything simply
- Always link related concepts as `[[concept-name]]`
