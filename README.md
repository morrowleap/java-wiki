# 📚 My Java Learning Wiki

A personal knowledge base for learning Java, maintained by an LLM agent.
Built on the LLM Wiki pattern by Andrej Karpathy.

---

## How to use this wiki

### Starting a session (paste this to Claude Code)
```
Read CLAUDE.md, then read wiki/index.md and wiki/roadmap.md.
Tell me where I left off and what's next.
```

### Adding new material
1. Save an article, note, or paste text into `raw/`
2. Tell Claude Code: `"File raw/[filename] into the wiki"`
3. The agent updates the wiki, index, and log automatically

### Asking questions
Just ask naturally:
- *"Explain how inheritance works based on what's in our wiki"*
- *"What's the difference between an interface and abstract class?"*
- *"I got a NullPointerException — help me understand it and add it to errors/"*

### Running a health check
Tell Claude Code: `"Run a lint pass on the wiki"`

---

## Tools you need
- **Claude Code** — the agent that maintains this wiki
- **Java JDK 21+** — [download here](https://adoptium.net/)
- **IntelliJ IDEA Community** (recommended) — [download here](https://www.jetbrains.com/idea/download/)
- **Obsidian** (optional) — for browsing the wiki visually

---

## Directory structure
```
java-wiki/
  raw/           ← Drop learning material here
  wiki/
    index.md     ← Master page catalog
    log.md       ← Activity history
    roadmap.md   ← Your progress
    concepts/    ← Java concept articles (LLM writes these)
    errors/      ← Bugs you've encountered + fixes
    snippets/    ← Reusable code patterns
  CLAUDE.md      ← Agent instructions & schema
  README.md      ← This file
```
