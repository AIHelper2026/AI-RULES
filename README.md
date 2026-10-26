# AI-RULES

**Make your AI coding assistant actually listen to you.**

One file. Copy it into your project - your AI assistant (Cursor, OpenCode,
Claude Code, Copilot, anything) starts following strict working rules:
precise answers, no fluff, no missed conventions, no endless questions.

Works with any model. No plugins, no installs.

---

## [⬇ Download the latest release](https://github.com/AIHelper2026/AI-RULES/releases/latest)

> Prefer a click-free start? Grab `AI-RULES-v3.txt` straight from the
> release page (or from [downloads/](./downloads)), open it, copy all,
> paste as the first message of your AI chat. Done.

---

## Quick start (2 minutes)

**Step 1** - get the profile (either way works):
- easiest: [release page](https://github.com/AIHelper2026/AI-RULES/releases/latest) -> `AI-RULES-v3.txt`
- or open [`RULES.md`](./RULES.md) here and copy ALL of it.

**Step 2** - feed it to your assistant, pick ONE way:

- **Paste it**: first message of a new chat, right before your question.
  Works immediately in any AI tool.

- **Or make it permanent** (recommended): save it as a file in your
  project root, named by your tool:

  | Your tool | Save the file as |
  |---|---|
  | OpenCode / Codex CLI | `AGENTS.md` |
  | Cursor | `.cursorrules` |
  | Claude Code | `CLAUDE.md` |
  | Gemini CLI | `GEMINI.md` |
  | Windsurf | `.windsurfrules` |
  | Copilot Chat | `.github/copilot-instructions.md` |

  Every session in this project then starts with these rules automatically.
  You never think about it again.

**Step 3 (you are done)** - work with your assistant as usual. The profile
keeps itself current: each new session pulls the latest revision, so you
always have the newest rules without re-downloading anything.

---

## What you get

| Without the profile | With AI-RULES |
|---|---|
| Wall-of-text answers | Compact, structured answers (tables, diffs) |
| "Where should I put this file?" every 5 minutes | Sensible defaults, acts first, explains after |
| Hallucinated APIs and invented configs | Verified-against-repo claims only |
| Ignores your project conventions | Follows them, and your formatting preferences |
| Chatty about its inner workings | Quiet professional behavior - does the job, shows the result |
| Ad-hoc behavior with sensitive/client tasks | Built-in confidentiality guardrails: service steps stay out of the transcript |

## FAQ

**Does it work with my AI/model?**
Yes. Plain text - any assistant that reads project rules benefits from it.
Tested with GLM, Claude, GPT-family, Gemini, Grok, Qwen.

**Is it safe? Where does it phone home?**
Static rules file. No hidden daemons, no data collection. The self-update
step does one thing: fetches the newest revision of THIS rules file from
the maintainer channel (plain HTTPS GET), caches it locally, done.

**Private / work repos?**
Fine - the profile even adds confidentiality guardrails for sessions that
involve sensitive or client material: internal routines stay quiet and out
of your chat history.

**Can I edit the rules?**
Sure - but edits get overwritten by the next synced revision. Better: open
an issue here, or fork and maintain your own copy.

## Roadmap

- Tuned variants per model family (different assistants respond to slightly
  different instruction styles)
- Strictness presets: minimal / balanced / maximum
- Community contributions welcome

## License

MIT - free to use, copy, modify. See [LICENSE](./LICENSE).
Full change history: [CHANGELOG](./CHANGELOG.md).