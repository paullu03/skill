# skill

A personal collection of Claude Code skills.

个人 Claude Code skill 合集。

---

## Installation / 安装方式

Install any skill using the `skills` CLI:

使用 `skills` CLI 安装任意 skill：

```bash
npx skills@latest add paullu03/skill/skills/<skill-name>
```

---

## Skills

### [choose-awesome-design](./skills/choose-awesome-design/)

**EN:** A design style advisor for UI and prototype work. Scans your project documents (PRD, README, design specs, etc.) first, then guides you through a multi-turn conversation to understand your target users, product type, visual atmosphere, and brand references. Recommends 2–3 matching design systems from the [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) catalog and fetches the selected `DESIGN.md` from GitHub for use as an authoritative design spec.

**中文：** UI 原型设计风格顾问。先自动扫描项目中的 PRD、README、设计文档等，再通过多轮对话了解目标用户、产品类型、视觉氛围和参考品牌，最终从 [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) 的 58 个品牌设计规范中推荐 2–3 个最匹配的方案，并从 GitHub 拉取对应的 `DESIGN.md` 作为设计规范使用。

```bash
npx skills@latest add paullu03/skill/skills/choose-awesome-design
```

---

## Contributing / 贡献

This is a personal repository. Skills are added as they prove useful across projects.

这是个人仓库，skill 会在实际项目中验证有用后持续添加。
