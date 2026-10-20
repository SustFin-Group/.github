# SustFin Group Shared Repository

Shared space for our team's code, scripts, and resources.

For now, we primarily share **agent skills** that are useful in our day-to-day research (proofreading, citation checks, formatting, and more). Feel free to let me know what else we should share in this shared repo!

## 📚 Available skills

| Skill | What it does | Status |
|-------|--------------|--------|
| [academic-proofreader](skills/academic-proofreader/SKILL.md) | Grammar, spelling, tense, academic tone, US/UK consistency | ✅ Ready |
| [citation-checker](skills/citation-checker/SKILL.md) | Matches in-text citations to references, checks style consistency | 🚧 In progress |
| [format-checker](skills/format-checker/SKILL.md) | Section structure, figure/table numbering, abbreviations, terminology | 🚧 In progress |

## 📁 Folder structure

```
├── README.md              ← overview + list of available skills (this file)
├── CONTRIBUTING.md        ← how to add or update a skill
├── templates/
│   └── SKILL_TEMPLATE.md  ← blank starting point for new skills
└── skills/
    ├── academic-proofreader/
    │   ├── SKILL.md       ← required
    │   └── examples/      ← optional: before/after samples
    ├── citation-checker/
    │   └── SKILL.md
    └── format-checker/
        └── SKILL.md
```

- **One skill per folder.** The folder name is lowercase with hyphens (e.g. `citation-checker`) and matches the `name:` field in its `SKILL.md`.
- **Every skill needs a `SKILL.md`.** Optional extras go in subfolders:
  - `examples/` – sample inputs and outputs
  - `references/` – style guides, journal rules
  - `scripts/` – helper code

## 🚀 Getting started

1. Accept the GitHub invite sent to your email.
2. **LET ME KNOW** if you have trouble doing the following.
3. Clone the repo:
   ```bash
   git clone https://github.com/SustFin-Group/[repo-name].git
   ```
4. Create your own branch before making changes:
   ```bash
   git checkout -b your-name/short-description
   ```

## 🧠 How to use a skill

- **Claude.ai:** download the skill folder, zip it, and upload it under *Settings → Capabilities → Skills*.
- **Claude Code:** copy the skill folder into `~/.claude/skills/` (personal use) or `.claude/skills/` inside a project repo.
- **Other agents:** most can read `SKILL.md` as a plain instruction file. Paste it in or point the agent to it.

## 🤝 How to contribute

**Adding a new skill:**
1. Create a folder under `skills/` and copy `templates/SKILL_TEMPLATE.md` into it as `SKILL.md`.
2. Fill in the name, description, instructions, and output format.
3. Test it on a real piece of text at least once.
4. Add it to the **Available skills** table above.
5. Push your branch and open a pull request.

**General rules:**
- Don't push directly to `main`. Open a pull request instead.
- Write clear commit messages (e.g. "Add citation-checker skill").
- Keep each skill focused on one task, and write its `description` clearly. It's how the agent decides when to use the skill.
- Never commit passwords, API keys, personal data, unpublished manuscripts, or confidential data.

## 👥 Contacts

- Repo admin: Lea – [haoliu1@ethz.ch](mailto:haoliu1@ethz.ch) or just WhatsApp me (you know how to contact me)
