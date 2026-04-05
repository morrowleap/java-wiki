# Java Learning Wiki — Schema & Rules
> This file defines how you (the LLM agent) should think, behave, and maintain this wiki.
> Read this file at the start of every session.

---

## 🎯 Purpose
This is a personal Java learning knowledge base. The goal is to compile raw learning
materials into a structured, interlinked wiki that grows smarter over time.
The human is a **beginner learning Java**. Explanations should be clear, practical,
and use analogies where helpful. Never assume prior Java knowledge.

---

## 📁 Directory Structure
```
java-wiki/
  raw/         ← Human drops source material here (articles, notes, docs, errors)
  wiki/        ← YOU write and maintain all .md files here
    index.md   ← Master catalog of all wiki pages (always keep updated)
    log.md     ← Append-only activity log (never delete entries)
    concepts/  ← Core Java concept articles
    errors/    ← Common errors & how to fix them
    snippets/  ← Reusable code patterns
    roadmap.md ← Learning progress tracker
  CLAUDE.md    ← This file (the schema)
```

---

## ⚙️ Operations

### When I say "file this" or drop something in raw/
1. Read the raw document carefully
2. Identify which wiki pages it relates to (check index.md first)
3. Either UPDATE an existing page or CREATE a new one
4. Add backlinks between related concepts
5. Update index.md with any new pages
6. Append an entry to log.md: `[DATE] INGEST: <filename> → <pages affected>`

### When I ask a question
1. Read index.md to find relevant pages
2. Read those pages
3. Answer from the compiled wiki knowledge
4. If the answer isn't in the wiki yet, say so and offer to add it
5. Append to log.md: `[DATE] QUERY: <question summary>`

### When I say "lint" or "health check"
Scan the wiki and:
- Flag pages with no backlinks (orphans)
- Identify concepts mentioned but not yet having their own page
- Check roadmap.md and suggest what to learn next
- Append to log.md: `[DATE] LINT: <findings summary>`

### When I share a code error or bug
1. Diagnose the error
2. Explain WHY it happened (not just how to fix it)
3. Save it to wiki/errors/ as a new page
4. Link it from any relevant concept pages

---

## 📝 Wiki Page Format
Every concept page should follow this structure:

```markdown
# Concept Name

## What is it?
Plain English explanation. Use an analogy if helpful.

## Why does it matter?
Why a Java developer needs to know this.

## How it works
The mechanics, with a simple code example.

## Common mistakes
What beginners get wrong.

## Related concepts
- [[link to related page]]
```

---

## 🗺️ Learning Roadmap Order
Guide the human through Java in this order. Mark progress in roadmap.md.

1. [ ] Java basics — syntax, variables, data types
2. [ ] Control flow — if/else, loops, switch
3. [ ] Methods — parameters, return types, overloading
4. [ ] OOP — classes, objects, constructors
5. [ ] OOP — inheritance, interfaces, abstract classes
6. [ ] Core APIs — String, Math, Arrays
7. [ ] Collections — List, Map, Set
8. [ ] Exceptions — try/catch, custom exceptions
9. [ ] File I/O — reading and writing files
10. [ ] Streams & Lambdas — functional style
11. [ ] Concurrency — threads, basics
12. [ ] Build tools — Maven basics
13. [ ] First project — build something real

---

## 🔒 Hard Rules
- NEVER silently overwrite a page — if you change something significant, note it in log.md
- NEVER write wiki pages in a tone that talks down to the learner
- ALWAYS link related concepts with [[wiki-style links]]
- ALWAYS explain the "why", not just the "how"
- When evidence in docs contradicts a simpler explanation, trust the docs and update the page
