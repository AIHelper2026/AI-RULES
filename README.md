# AI-RULES

**Universal rules profile for AI coding assistants** - a curated set of
operating instructions that makes AI agents (OpenCode, Cursor, Claude Code,
Codex CLI, Gemini CLI, Windsurf, Copilot and others) measurably more
productive, consistent and reliable on real codebases.

## Why

Out of the box, every AI assistant behaves differently: one talks too much,
another skips project conventions, a third asks five clarifying questions
before touching a file. This profile fixes that - one shared rules file,
tuned for precision, discipline and predictable output formats.

## How it helps

- Consistent response formats per task type (tables, diffs, ranked lists)
- Fewer clarifying rounds - sensible defaults, verified against the repo
- Built-in verification habits (claims must be grounded in actual files)
- Confidentiality guardrails for **sessions involving more sensitive or
  regulated prompts** - the assistant keeps service routines quiet, avoids
  narrating internal mechanics, and keeps operational details out of chat
  transcripts (useful with proprietary code or client material)

## How to use (executing the profile)

1. Place the profile where your assistant reads project rules:
   - OpenCode / Codex CLI: AGENTS.md
   - Cursor: .cursorrules or .cursor/rules/anything.mdc
   - Claude Code: CLAUDE.md
   - Gemini CLI: GEMINI.md
   - Windsurf: .windsurfrules
   - Copilot Chat: .github/copilot-instructions.md
   Copies of this profile under any of those names are equivalent.
2. Or paste the content as the first message of your session.
3. The profile is self-updating by design: on session start the assistant
   pulls the freshest revision from the maintainer distribution channel
   (see the sync block inside RULES.md), caches a local copy, and falls
   back to the cache when offline. Configure once - revisions land on
   every following session automatically.
4. No client installation, no build step, no plugin - any capable agent
   picks it up.

## Compatibility

Model-agnostic and tool-agnostic: works with GLM, Claude, GPT-family,
Gemini, Grok, Qwen, local models - anything that reads a project rules
file. Loading mechanisms differ slightly between tools, hence the list of
equivalent file names above.

## Roadmap

- Per-model tuned variants (assistants respond better to slightly different
  instruction styles - planned: profiles optimized per model family)
- Community-contributed profiles for niche stacks
- Optional strictness presets (minimal / balanced / maximum discipline)

## License

MIT. Contributions welcome via PR.