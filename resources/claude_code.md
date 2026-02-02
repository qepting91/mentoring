# Claude Code (v2.1) | The Agentic Engineer's Reference

*Verified against v2.1 CLI & 2026 Best Practices.*

---

## Block 1: The Golden Rules (Architecture)

### The Constitution (`CLAUDE.md`)

- **Rule:** Every project root *must* have a `CLAUDE.md` file.
- **Purpose:** It is not documentation; it is **Context Injection**.
- **Structure:**
  - **The Map:** Briefly list key directories (e.g., `@src/core`, `@docs/api`).
  - **The Stack:** Explicitly state libraries (e.g., "Use Hono, not Express").
- **Constraint:** Keep it under 150 lines. Use "Progressive Disclosure" (link to `/docs` instead of pasting text).

### The 10-Minute Rule

- **Trigger:** If a task takes >10 minutes or touches >3 files...
- **Action:** You **MUST** enter **Plan Mode**.
- **Why:** Prevents "hallucination loops" where Claude writes valid code for the wrong architecture.

---

## Block 2: Essential CLI Commands

| Command | Action | Use Case |
|---------|--------|----------|
| `claude` | **Start Interactive** | The daily driver. Starts a REPL in the current folder. |
| `claude -c` | **Continue** | Instantly resumes the *most recent* conversation. |
| `claude -p "query"` | **Print Mode** | One-shot command. Great for piping: `cat logs \| claude -p "Fix this"` |
| `claude --resume <id>` | **Time Travel** | Resume a specific past session. Use `claude --from-pr <url>` for PRs. |
| `claude mcp` | **Connect Data** | Launch the wizard to connect GitHub, Linear, or PostgreSQL. |

---

## Block 3: Power User Flags (The Speed Layer)

### `--verbose` (The Matrix)

- **What it does:** Reveals raw "thinking" logs, tool inputs, and full error traces.
- **When to use:** If Claude gets stuck or loops. *Essential for debugging why a specific tool failed.*

### `--dangerously-skip-permissions` (YOLO Mode)

- **What it does:** Bypasses **ALL** "Approve (y/n)" prompts.
- **When to use:** Trusted automation scripts, CI/CD pipelines, or fresh repos.
- **Safety Tip:** Combine with `--tools "Bash,Read"` to restrict *what* it can do while skipping *approval*.

### `--agents` (The Squad)

- **What it does:** Spins up specialized sub-agents with distinct prompts/tools.
- **When to use:** `claude --agents '{"reviewer": {"model": "opus-4.5"}}'` for parallel QA while you code.

### `--model opus-4.5` (The Architect)

- **What it does:** Forces the SOTA reasoning model.
- **When to use:** Complex refactors or "Ultrathink" tasks.

---

## Block 4: Verified Keyboard Shortcuts

| Shortcut | Action | Note |
|----------|--------|------|
| `Shift+Tab` (x1) | **Toggle Auto-Accept** | Speed mode (Green UI) |
| `Shift+Tab` (x2) | **Enter Plan Mode** | Read-only Architect mode (Blue UI) |
| `/plan` | **Force Plan Mode** | *Reliable fallback if Shift+Tab fails (Windows/Linux)* |
| `Ctrl+R` | **Fuzzy Search** | Search command history |
| `Ctrl+S` | **Stash Draft** | Save input without sending |
| `Ctrl+C` | **Interrupt** | Stop the agent immediately |

---

## Block 5: Troubleshooting & Recovery

| Problem | Solution |
|---------|----------|
| **Agent Stuck?** | Run **`/clear`** (Wipes history but reloads `CLAUDE.md`). |
| **Bad Loop?** | Use **`--fork-session`** to branch off the last good point. |
| **Context Rot?** | **Avoid `/compact`**. It degrades quality significantly. Instead, ask Claude to "Update CLAUDE.md with lessons learned," then exit and start fresh. |

---

## Official Documentation Links (2026 Edition)

### Core Documentation

- **Claude Code Overview & Quickstart:**
  [https://code.claude.com/docs/en/overview](https://code.claude.com/docs/en/overview)

- **CLI Reference (Commands & Flags):**
  [https://code.claude.com/docs/en/cli-reference](https://code.claude.com/docs/en/cli-reference)

- **Best Practices Guide:**
  [https://code.claude.com/docs/en/best-practices](https://code.claude.com/docs/en/best-practices)

### Community & Advanced Guides

- **"Writing a Good CLAUDE.md":**
  [https://humanlayer.dev/blog/writing-a-good-claude-md](https://humanlayer.dev/blog/writing-a-good-claude-md)

- **Safety Guide (Dangerously Skip Permissions):**
  [https://promptaa.com/blog/claude-dangerously-skip-permissions](https://promptaa.com/blog/claude-dangerously-skip-permissions)
