# claude-skills

A collection of personal Claude skills — custom instructions that give Claude specialized behavior for specific workflows.

> **Claude-specific**: These skills are built for [Claude by Anthropic](https://claude.ai) and use Claude's native skill-loading system. They won't work in ChatGPT or Gemini out of the box.

---

## Skills

| Skill | What it does | Trigger |
|-------|-------------|---------|
| [brainstorm-pm](./brainstorm-pm/SKILL.md) | Collaborative project brainstorming + Requirements Gathering Report | `/brainstorm-pm` or describe a project idea |

---

## How to Install a Skill

1. Download the `SKILL.md` file from the skill's folder
2. In Claude, go to **Customize → Skills → +**
3. Upload the `SKILL.md` file
4. The skill is now active — trigger it via slash command or just describe your use case naturally

---

## How to Use

You don't need to type `/skill-name` every message. Just trigger it once at the start of the conversation and it stays active.

You can also stack multiple skills in one chat:
```
/brainstorm-pm let's plan a new project
```

---

## brainstorm-pm

A teammate-style brainstorming skill that helps you think through any project from scratch — then generates a full Requirements Gathering Report (SDLC-style) at the end.

**How a session works:**
1. You describe your project idea
2. Back-and-forth on **features** — you pitch, Claude reacts, challenges, suggests
3. Move to **design** — platform, screens, UX decisions
4. Finish with **tech stack & deployment**
5. Claude generates a `.md` Requirements Gathering Report — detailed enough for any developer or AI agent to start building

**Claude will:**
- Push back if an idea doesn't make sense
- Suggest things you haven't thought of
- Flag when something's too complex for v1
- Conclude each phase mutually before moving on

**Trigger:**
```
/brainstorm-pm I want to build a project from scratch
/brainstorm-pm I want to upgrade my existing app
```
Or just describe a project idea — it auto-triggers.

---

## Contributing

Have a skill to add? PRs welcome. Keep each skill in its own folder:
```
skill-name/
└── SKILL.md
```

---

Made with Claude ✦
