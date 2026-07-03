# more-human (AI Collaborator Persona)

These skills follow the Agent Skills specification so they can be used by any skills-compatible agent, including Claude Code, Codex, and Open Code.

## Installation

### Marketplace
/plugin marketplace add nthnnel/more-human
/plugin install more-human@more-human
npx skills
npx skills add git@github.com:nthnnel/more-human.git

<<<<<<< Updated upstream
### Apa fungsinya?
Biasanya, kalau kamu nyuruh AI nulis email, artikel, atau kode, hasilnya pasti kerasa banget "AI-nya". Kalimatnya terlalu rapi, pakai kata-kata klise (kayak *delve, landscape yang dinamis, mendemistifikasi*), dan rasanya hambar.
=======
Instead of ssh, if you prefer to use https:

npx skills add https://github.com/nthnnel/more-human
>>>>>>> Stashed changes

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

<<<<<<< Updated upstream
**Opsi 1: Biar AI yang install sendiri**
Buka chat baru di AI kamu (misal di Claude Code atau Gemini IDE), lalu *paste* prompt ini:

> "Tolong install skill ini buat gue. File utamanya ada di repo ini: [Link Repo GitHub Kamu / Path Lokal]. Setting semuanya supaya gue bisa langsung pakai, dan kasih tau kalau ada yang perlu gue lakuin."

AI bakal baca strukturnya dan otomatis naruh file `SKILL.md` ke tempat yang benar.

**Opsi 2: Download manual & minta tolong AI**
1. Download file `SKILL.md` dari repo ini.
2. Buka AI andalan kamu, *attach* filenya, lalu bilang:
> "Gue baru aja download file SKILL.md buat skill 'more-human'. Bisa tolong pandu gue cara install-nya? Kasih tau gue file ini harus ditaruh di folder mana."

AI bakal nuntun kamu *step-by-step*.

---

### Cara Pakai

Kalau udah ke-install, di percakapan mana pun, kamu tinggal sebut salah satu kata ajaib ini:

* "Tolong **humanize** ini..."
* "**anti-ai pass** dong buat tulisan ini..."
* "**rewrite like a human**"
* "Pakai **persona Sena**, tolong cek tulisan ini."

AI bakal langsung otomatis jalanin workflow *humanizer*-nya, ngebuang semua kata-kata klise, dan ngasih kamu hasil yang jauh lebih natural.

---

### Credit & Inspirasi
Skill ini terinspirasi dari gerakan *AI Cleanup* dan best practice *instruction engineering* modern. Tujuannya simpel: kita ingin kerja sama AI yang berasa kayak kerja sama rekan tim sungguhan.
=======
| Skill | Description |
| :--- | :--- |
| **more-human** | Communicate in a warm, structured, and adaptive manner. Switch to pure logic and efficiency when coding, and use a natural, empathetic, and clutter-free style for text or discussions. |
>>>>>>> Stashed changes
