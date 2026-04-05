# My Java Learning Wiki

A personal knowledge base for learning Java, maintained by an LLM agent.

---

## How to use this wiki

### Starting a session
```
Read CLAUDE.md, then read wiki/index.md.
```

### Adding a concept page
1. Write the page yourself and save it to `wiki/concepts/your-topic.md`
2. Tell the model: `"index this: wiki/concepts/your-topic.md — one line description"`
3. The model updates index.md and log.md

### Logging a note
- `"log this: finished the OOP chapter"`

---

## Running with a small local model (Ollama) via Claude Code:
```bash
ollama launch claude --model qwen3.5:4b
```

The CLAUDE.md in this repo is written for small models — explicit commands, fill-in templates, no complex reasoning required.

---

## Tools

- **Ollama** — run local models: [ollama.com](https://ollama.com)
- **Claude Code** — CLI agent: [docs.ollama.com/integrations/claude-code](https://docs.ollama.com/integrations/claude-code)
- **Java JDK 21+** — [adoptium.net](https://adoptium.net/)
- **IntelliJ IDEA Community** (recommended) — [jetbrains.com/idea](https://www.jetbrains.com/idea/download/)
- **Obsidian** (optional) — browse the wiki visually with wiki-style links

---

## Directory structure

```
java-wiki/
  wiki/
    index.md     ← Master page catalog
    log.md       ← Activity history
    concepts/    ← Java concept articles (you write these)
    errors/      ← Bugs you've encountered + fixes
    snippets/    ← Reusable code patterns
  CLAUDE.md      ← Agent instructions & schema
  README.md      ← This file
```

References:
https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f#llm-wiki
- **Obsidian Web Clipper** is a browser extension that converts web articles to markdown. Very useful for quickly getting sources into your raw collection.
  
- **Download images locally.** In Obsidian Settings → Files and links, set "Attachment folder path" to a fixed directory (e.g. `raw/assets/`). Then in Settings → Hotkeys, search for "Download" to find "Download attachments for current file" and bind it to a hotkey (e.g. Ctrl+Shift+D). After clipping an article, hit the hotkey and all images get downloaded to local disk. This is optional but useful — it lets the LLM view and reference images directly instead of relying on URLs that may break. Note that LLMs can't natively read markdown with inline images in one pass — the workaround is to have the LLM read the text first, then view some or all of the referenced images separately to gain additional context. It's a bit clunky but works well enough.

https://docs.ollama.com/integrations/claude-code



