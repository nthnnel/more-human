# more-human

**Strip the robot. Keep the brain.**

A persona skill that rewires how your AI coding assistant communicates — from sterile corporate hedging to confident, warm, direct conversation. Works with any agent that supports the [Agent Skills](https://skills.sh) specification.

## What it does

`more-human` is an always-active tone layer. Once installed, every response — code reviews, explanations, emails, discussions — adopts a voice that sounds like a sharp colleague, not a customer service bot.

**It covers:**
- **Voice & structure** — lead with the point, match length to the question, kill the filler
- **Banned AI tells** — a hitlist of robotic words and phrases (`delve`, `tapestry`, `it's important to note...`) in both English and Indonesian
- **The EPOCH framework** — Empathy, Presence, Opinion, Creativity, Hope — with guardrails for when to soften and when to push
- **Coding style** — clean code with meaningful comments, no over-engineering, no fluff inside the code itself
- **Calibrated examples** — five Robotic → Overcorrected → Human rewrites that teach the floor *and* ceiling of the voice

## Before & After

> **Without more-human:**
> *Sure, I can help you with that! It's important to note that managing dependencies can be a complex journey. Let me delve into the various approaches...*

> **With more-human:**
> *Let's get this sorted. Dependency hell is the worst, but we can clean this up in two minutes.*

## Installation

### Claude Code Plugin (Recommended)

Since this repository is a valid Claude Plugin Marketplace, you can install it directly from Claude Code:

```bash
/plugin marketplace add https://github.com/nthnnel/more-human
/plugin install more-human
```

### Using the Skills CLI

```bash
npx skills add nthnnel/more-human
```

Or via HTTPS:

```bash
npx skills add https://github.com/nthnnel/more-human
```

### Gemini (Google AI)

Copy `SKILL.md` into your workspace's `.agents/skills/more-human/` directory:

```
your-project/
└── .agents/
    └── skills/
        └── more-human/
            └── SKILL.md
```

Or add it globally at `~/.gemini/config/skills/more-human/SKILL.md` to apply across all workspaces.

### Claude Code (Manual)

If you prefer not to use the plugin marketplace, you can manually add the skill:
Copy `SKILL.md` to a `/.claude/skills/more-human/` folder in the root of your workspace. See the [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code) for details.

### Codex

Copy the skill file into your Codex skills path:

```bash
mkdir -p ~/.codex/skills/more-human
cp SKILL.md ~/.codex/skills/more-human/
```

### OpenCode

Clone the full repo into the OpenCode skills directory:

```bash
git clone https://github.com/nthnnel/more-human.git ~/.opencode/skills/more-human
```

OpenCode auto-discovers all `SKILL.md` files under `~/.opencode/skills/`. No config changes needed — just restart OpenCode.

## Key design decisions

- **Always active** — no trigger phrase needed. The skill applies to every response automatically.
- **Tone layer, not content override** — safety notes, honest uncertainty, and "I don't know" are preserved. The skill changes *how* the AI says things, not *what* it says.
- **Formal context aware** — the casual voice applies to conversation with you, but deliverables (client emails, cover letters, legal text) adopt the register their audience needs.
- **Frustration-aware** — when you're stressed or debugging at 2am, the teasing stops. Just direct help.
- **Bilingual** — includes banned phrases and calibrated examples for both English and Indonesian.

## What's inside

| File/Folder | Purpose |
| :--- | :--- |
| `.claude-plugin/` | Contains the `marketplace.json` and `plugin.json` manifests for Claude Code integration |
| `SKILL.md` | The complete skill — voice rules, banned words, coding preferences, EPOCH framework, and five calibrated examples |
| `LICENSE` | MIT |
| `README.md` | You're reading it |

## Contributing

The skill is intentionally complete and stable. If you find a real-world response where the voice misses — not a hypothetical, an actual miss — open an issue with the prompt and output. That's how Example F gets written.

## License

[MIT](LICENSE) © nathan
