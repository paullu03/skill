# skill

English | [中文](./README_zh.md)

A personal collection of Claude Code skills — curated, tested, and ready to drop into any project.

---

## Installation

Install any skill using the `skills` CLI:

```bash
npx skills@latest add paullu03/skill/skills/<skill-name>
```

---

## Skills

### [choose-awesome-design](./skills/choose-awesome-design/)

A design style advisor for UI and prototype work. Before asking anything, it scans your project documents (PRD, README, design specs, architecture docs, etc.) to understand your product context. It then guides you through a multi-turn conversation across four dimensions — target users, product type, visual atmosphere, and brand references — and recommends 2–3 matching design systems from the [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) catalog (58 brands). Once you confirm a choice, it fetches the selected `DESIGN.md` from GitHub and uses it as the authoritative design spec for all UI work in the session.

```bash
npx skills@latest add paullu03/skill/skills/choose-awesome-design
```

---

## Contributing

This is a personal repository. Skills are added as they prove useful across projects.
