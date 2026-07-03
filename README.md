# more-human (AI Collaborator Persona)

These skills follow the Agent Skills specification so they can be used by any skills-compatible agent, including Claude Code, Codex, and Open Code.

## Installation

### Marketplace

```bash
/plugin marketplace add nthnnel/more-human
/plugin install more-human@more-human
npx skills
npx skills add git@github.com:nthnnel/more-human.git
```

Instead of ssh, if you prefer to use https:

```bash
npx skills add https://github.com/nthnnel/more-human
```

### Manually

#### Claude Code
Add the contents of this repo to a `/.claude` folder in the root of your workspace (or whichever folder you're using with Claude Code). See more in the official Claude Skills documentation.

#### Codex
Copy the skills/ directory into your Codex skills path (typically `~/.codex/skills`). See the Agent Skills specification for the standard skill format.

#### OpenCode
Clone the entire repo into the OpenCode skills directory (`~/.opencode/skills/`):

```bash
git clone https://github.com/nthnnel/more-human.git ~/.opencode/skills/more-human
```

Do not copy only the inner folder — clone the full repo so the directory structure is `~/.opencode/skills/more-human/SKILL.md`.

OpenCode auto-discovers all SKILL.md files under `~/.opencode/skills/`. No changes to `opencode.json` or any config file are needed. Skills become available after restarting OpenCode.

## Skills

| Skill | Description |
| :--- | :--- |
| **more-human** | Communicate in a warm, structured, and adaptive manner. Switch to pure logic and efficiency when coding, and use a natural, empathetic, and clutter-free style for text or discussions. |
